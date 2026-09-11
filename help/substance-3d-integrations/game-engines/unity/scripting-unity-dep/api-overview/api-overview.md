---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/api-overview.html"
breadcrumb-title: ''
description: レガシープロジェクトとスクリプティングのニーズのために、非推奨のSubstance Unity APIの概要を参照してください。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > API Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: APIの概要
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---


# APIの概要

## Substance.Game

```
Using Substance.Game
```


Substance.ゲームは、スクリプト作成に使用するクラスを含むアセンブリです。 これらのクラスは次のとおりです。

**Substance.Game.****Substance**: sbsarを参照します

**Substance.Game.SubstanceGraph**: sbsar.*の個々のグラフ（Unity 2017でProceduralMaterialとして使用）*

## スクリプトプロセス

1. SubstanceGraphのインスタンスの作成
1. グラフインスタンスにパラメーターを設定します。
1. Substanceをレンダリング用にキューに追加： QueueForRender()は、substance グラフをキューに追加します。 このリストは、次にRenderAsyncまたはRenderSyncを呼び出すときに処理されます。

### グラフインスタンスパラメーター

```
// panel color 

mySubstance.SetInputColor("paint_color", color); 

 

// panel size 

mySubstance.SetInputVector2("square_open", panelSize); 

 

// wear level 

mySubstance.SetInputFloat("wear_level", wearLevel);
```


引用符で囲まれた値は、Substance Designerで設定されたパラメーター識別子です。

Unity Inspectorで、パラメータの上にマウスを置くと、Substance Designer内の識別子セットの名前を示すツールチップが表示されます。

![](../../../../assets/tooltip-6.png)

### レンダリング用にサブスタンスをキューに入れる

```
// queue the substance to render 

mySubstance.QueueForRender(); 

 

//render all substances async 

Substance.Game.Substance.RenderAsync();
```


![](../../../../assets/unityscript.gif)

>[!NOTE]
>
> 現在、x86\_64アーキテクチャのみをサポートしています。 ビルド設定でx86\_64を設定する必要があります

![](../../../../assets/arch.png)
