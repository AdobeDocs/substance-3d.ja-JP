---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting.html"
breadcrumb-title: ''
description: 実行時にSubstanceパラメーターを更新および変更するスクリプトを記述するには、UnityでSubstance 3D APIを使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D for Unityスクリプティング
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Substance 3D for Unityスクリプティング

このセクションでは、Unity用のSubstance 3Dプラグインを介して提供されるSubstance 3D APIについて詳しく説明します。 SubstanceAPIを使用すると、実行時にSubstanceパラメーターを更新および変更するスクリプトを作成できます。

## APIの概要

プラグインは3つの異なるアセンブリに分かれています。

* Adobe.Substance
* Adobe.Substance.エディタ
* Adobe.Substance.ランタイム

### Adobe.Substance

Substance SDKとのやり取りや、一致するUnityオブジェクトの生成のための共有コンポーネントが含まれています。 また、C#とSubstance SDK C++ API間の通信のためのマーシャリングデータ構造も備えています。

#### Adobe.Substance.エディタ

Unity Substanceオブジェクトに関する情報の表示を処理したり、sbsarファイルがプロジェクトに追加された場合のインポートパイプラインを処理するための、エディタ固有のクラスが含まれます。 SubstanceEditorEngineクラスは、Substance エンジンとそのすべてのマネージドインスタンスの有効期間を処理するシングルトンです。

#### Adobe.Substance.ランタイム

このクラスには、実行時にSubstanceオブジェクトの作成と管理を処理するコンポーネントがあります。 SubstanceRuntimeは、ランタイムのSubstanceEditorEngineクラスに相当します。 Substance エンジンの初期化と、ユーザースクリプトが操作するSubstanceインスタンスのインスタンス化を処理します。

## ランタイムの使用

Substanceインスタンスの入力を実行時に変更するには、SubstanceRuntime←-マテリアルをシーンに追加する必要があります（マテリアルをサブスタンス化するのと同じGameObjectに追加することも理想的です）。 このクラスは、実行時にSubstanceSDKオブジェクトのインスタンス化を管理するAdobe.Substance.Runtime.SubstanceRuntimeシングルトンを使用してマテリアルを設定するヘルパーとして機能します。

## コード例

次の例は、SubstanceRuntimeGraphを使用して、実行時に入力パラメーターを変更する方法を示しています。

### パラメータの変更

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    // panel color 

    mySubstance.SetInputColor("paint_color", new Color(0.237 f, 0.834 f, 0.045 f, 1.0 f)); 

    // panel size 

    mySubstance.SetInputVector2("square_open", new Vector2(0.101 f, 0.209 f)); 

    // wear level 

    mySubstance.SetInputFloat("wear_level", 0.977 f); 

    // Submit async render. 

    mySubstance.RenderAsync(); 

  } 

}
```


また、SubstanceRuntimeGraphを使用して、マテリアルに関する入出力情報にアクセスすることもできます。

#### 入力情報を取得

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```


次の例は、SubstanceEditorToolsを使用して、エディターにカスタムプリセットメニューを作成する方法を示しています。

##### プリセットコントロールの作成。

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```
