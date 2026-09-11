---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceeditortools-256212996.html"
breadcrumb-title: ''
description: Unityでのマテリアル管理に使用されるSubstanceEditorToolsクラスの参照ドキュメント。
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceEditorTools
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# SubstanceEditorTools

## Adobe.SubstanceEditor.SubstanceEditorToolsクラスリファレンス

ユーザーがエディタースクリプトで使用するツールおよびユーティリティ。

Adobe.SubstanceEditor.SubstanceEditorToolsの継承図：

![](../../../../../assets/image2022-10-14-17-53-23.png)

### 静的パブリック・メンバー関数

```
• static void SetGraphFloatInput (SubstanceGraphSO graph, int inputId, float value)
```


グラフfloat入力を設定します。

```
• static void SetGraphFloat2Input (SubstanceGraphSO graph, int inputId, Vector2 value)
```


グラフfloat2入力を設定します。

```
• static void SetGraphFloat3Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


グラフfloat3入力を設定します。

```
• static void SetGraphFloat4Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


グラフfloat4入力を設定します。

```
• static void SetGraphIntInput (SubstanceGraphSO graph, int inputId, int value)
```


入力にグラフを設定します。

```
• static void SetGraphInt2Input (SubstanceGraphSO graph, int inputId, Vector2Int value)
```


グラフ int2入力をセットします。

```
• static void SetGraphInt3Input (SubstanceGraphSO graph, int inputId, Vector3Int value)
```


グラフ int3入力をセットします。

```
• static void SetGraphInt4Input (SubstanceGraphSO graph, int inputId, int value0, int value1, int value2, int value3)
```


グラフ int4入力を設定します。

```
• static void SetGraphInputString (SubstanceGraphSO graph, int inputId, string value)
```


グラフ文字列の入力を設定します。

```
• static void SetGraphInputTexture (SubstanceGraphSO graph, int inputId, Texture2D value)
```


グラフテクスチャ入力を設定します。

```
• static void RenderGraph (SubstanceGraphSO graph)
```


ターゲットグラフをレンダリングしてそのアセットを更新します。

```
• static string CreatePresetFromCurrentState (SubstanceGraphSO graph)
```


グラフオブジェクトの現在のステートからプリセットXMLを作成します。

```
• static List< SubstanceGraphSO > GetGraphs (this SubstanceFileSO fileSO)
```


SubstanceFileSOに関連付けられたSubstanceGraphSOのリストを返します。
