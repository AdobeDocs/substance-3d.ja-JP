---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class.html"
breadcrumb-title: ''
description: Unityの実行時グラフ操作に使用されるSubstanceRuntimeGraphクラスのリファレンスドキュメントです。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceRuntimeGraphクラス
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# SubstanceRuntimeGraphクラス

## Adobe.Substance.ランタイム.SubstanceRuntimeGraphクラスリファレンス

Substanceグラフの入力を変更およびレンダリングするランタイム機能を提供するクラスです。このクラスにより、←GraphSOは実行時にアセットを生成できます。

Substance.Substance.Runtime.SubstanceRuntimeGraphのAdobeダイアグラム：

![](../../../../../assets/image2022-10-14-17-53-23-1.png)

### パブリック・メンバー関数

```
• void AttachGraph (SubstanceGraphSO graph)
```


このランタイムハンドラに新しいグラフオブジェクトをアタッチします。

```
• void SetInputFloat (string inputName, float value)
```


Substance浮動小数点入力を更新

```
• float GetInputFloat (string inputName)
```


Substance浮動小数点値を取得する

```
• void SetInputVector2 (string inputName, Vector2 value)
```


Substanceベクトル2入力を更新

```
• Vector2 GetInputVector2 (string inputName)
```


Substanceベクトル2入力を取得

```
• void SetInputVector3 (string inputName, Vector3 value)
```


Substanceベクトル3入力を更新

```
• Vector3 GetInputVector3 (string inputName)
```


Substance Vector3入力を取得します。

```
• void SetInputVector4 (string inputName, Vector4 value)
```


Substanceベクトル4入力を更新

```
• Vector4 GetInputVector4 (string inputName)
```


Substanceベクトル4入力を取得

```
• void SetInputColor (string inputName, Color value)
```


Substanceカラー入力を更新

```
• Color GetInputColor (string inputName)
```


Substanceカラーを取得

```
• void SetInputBool (string inputName, bool value)
```


Substanceのブール値入力を更新

```
• bool GetInputBool (string inputName)
```


Substanceのブール値入力を取得します。

```
• void SetInputInt (string inputName, int value)
```


Substanceの整数入力を更新

```
• int GetInputInt (string inputName)
```


Substanceの整数入力を取得

```
• void SetInputVector2Int (string inputName, Vector2Int value)
```


Substance Vector2Int入力を更新します。

```
• Vector2Int GetInputVector2Int (string inputName)
```


2 intの配列を取得します。

```
• void SetInputVector3Int (string inputName, Vector3Int value)
```


Substance Vector3Int入力を更新します。

```
• Vector3Int GetInputVector3Int (string inputName)
```


3 intの配列（Vector3Intのx、y、z値）を取得します。

```
• void SetInputVector4Int (string inputName, int x, int y, int z, int w)
```


SubstanceのVector4Int入力を更新

```
• int[ ] GetInputVector4Int (string inputName)
```


4intの配列（Vector4Intのx、y、z、w値）を取得します。

```
• void SetInputString (string inputName, string value)
```


Substance文字列入力を更新します。

```
• string GetInputString (string inputName)
```


Substance文字列の入力を取得します。

```
• SubstanceInputDescription GetInputDescription (string inputName)
```


ターゲット入力名の完全な入力説明を返します。

```
• void SetInputTexture (string inputName, Texture2D value)
```


Substanceテクスチャ2D入力を更新します。

```
• Vector2Int GetTexturesResolution ()
```


インスタンステクスチャ出力解像度を返します。

```
• void SetTexturesResolution (Vector2Int size)
```


インスタンステクスチャ出力解像度を設定します。

```
• bool HasInput (string inputName)
```


このsubstanceインスタンスに指定された名前の入力がある場合はtrueを返します。

```
• List< Texture2D > GetGeneratedTextures ()
```


Substanceインスタンスのすべての出力テクスチャを含むリストを返します。

```
•  Texture2D GetOutputTexture (string outputName)
```


指定された出力名の出力テクスチャを返します。

```
• void Render ()
```


Substanceインスタンスを同期的にレンダリングします。

```
• Task RenderAsync ()
```


Substanceインスタンスを非同期でレンダリングします。

```
• void LoadPreset (string presetXML)
```


プリセットXMLを使用して、グラフ入力パラメーターを設定します。

```
• string CreatePresetFromCurrentState ()
```


現在のグラフ状態をプリセットXMLに保存します。

## パブリック属性

```
• SubstanceGraphSO GraphSO
```


ターゲット物質インスタンス。

## 保護されたメンバー関数

```
• void Awake ()
```


On awake SubstanceRuntimeは、サブスタンスにアタッチされたSubstanceGraphSOのインスタンスを作成するために使用されます

SDK。

```
• void Update ()
```


レンダリング結果については、レンダリングのConcurrentQueueを確認してください。

```
• void OnDestroy ()
```


Substance SDKハンドラーを廃棄します。

## プロパティ

```
• Material DefaulMaterial [get]
```


Substanceインスタンスによって生成されるメインマテリアル。
