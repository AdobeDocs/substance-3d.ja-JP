---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntime-class.html"
breadcrumb-title: ''
description: UnityのランタイムSubstanceのマテリアル操作に使用されるSubstanceRuntimeクラスのリファレンスドキュメントです。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntime Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceRuntimeクラス
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 1%

---


# SubstanceRuntimeクラス

## Adobe.Substance.ランタイム.SubstanceRuntimeクラスリファレンス

Substanceエンジンの初期化を処理し、Substanceインスタンスへのネイティブハンドラーを取得するために使用されるシングルトンクラスです。\
Substance.Inheritance.Runtime.SubstanceRuntimeのSubstance図：

![](../../../../../assets/image2022-6-22-14-35-28.png)

### パブリック・メンバー関数

```
• SubstanceNativeGraph InitializeInstance (SubstanceGraphSO substanceInstance)
```


指定されたSubstanceGraphSOのSubstance SDKハンドルを作成します。

### プロパティ

```
• static SubstanceRuntime Instance [get]
```


シングルトンインスタンス。

### 詳細な説明

Substanceエンジンの初期化を処理し、Substanceインスタンスへのネイティブハンドラーを取得するために使用されるシングルトンクラスです。

### メンバー関数のドキュメント

#### InitializeInstance()

```
SubstanceNativeGraph Adobe.Substance.Runtime.SubstanceRuntime.InitializeInstance  

( SubstanceGraphSO substanceInstance ) [inline]
```


指定されたSubstanceGraphSOのSubstance SDKハンドルを作成します。

**パラメーター**

|  |  |
| --- | --- |
| substanceInstance | Target SubstanceGraphSO |


**戻り値**

Substance SDKと通信するハンドル

### プロパティドキュメント

#### インスタンス

```
SubstanceRuntime Adobe.Substance.Runtime.SubstanceRuntime.Instance [static], [get]
```


シングルトンインスタンス。

グローバルなシングルトンインスタンス。

>[!NOTE]
>
> NativeGraph.InRenderWorkは、ワークフローとの通信のためだけに内部使用を目的としているため、カスタムSubstance engineには使用しないでください。
