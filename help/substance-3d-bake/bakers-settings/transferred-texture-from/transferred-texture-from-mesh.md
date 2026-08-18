---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/transferred-texture-from-mesh.html"
breadcrumb-title: ''
description: 法線マップ変換のサポートなど、UVに基づいてメッシュ間でテクスチャを転送します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Transferred Texture from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからの転送されるテクスチャ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 3%

---


# メッシュからの転送されるテクスチャ

メッシュベイカーから転送されたテクスチャを使用すると、それぞれのUVに基づいて、1つのメッシュから別のメッシュにテクスチャを変換できます。 このベイカーは、転送マップまたは通常のマップ（特殊な変換が必要）もサポートしています。 機能させるには、両方のメッシュにUV定義が必要です。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **テクスチャファイル** | 転送される入力テクスチャファイルへのパス。 |
| **UVセット** | 高ポリゴンメッシュで使用するメッシュUVをテクスチャを読み取り、低ポリゴンメッシュに投影します。 |
| **フィルターモード** | テクスチャのピクセル補間方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>最も近い</strong>：補間は行われません。指定された位置で見つかった最も近いピクセルを使用します。 正確ですが、エイリアスを作成できます。</li><li data-preserve-html="true"><strong>バイリニア</strong> （既定）：指定した位置に最も近い4つのピクセルを使用します。 エイリアスはありませんが、ぼかすことができます。</li></ul> |
| **標準マップ** | 有効になっている場合、転送する入力テクスチャが法線マップであることをベイカーに示します。 これは、ベイカーがテクスチャに特別な変換を適用して、ターゲットメッシュとの互換性を確保することを示します。 |
| **マップの種類** | 入力テクスチャが法線マップのタイプを定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ワールドスペース</strong></li><li data-preserve-html="true"><strong>接線空間</strong> （既定）</li></ul> |
| **法線の向き** | **マップの種類**&#x200B;が&#x200B;**接線空間**&#x200B;に設定されている場合、入力テクスチャの標準の形式を定義します。指定できる値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> （既定）</li></ul> |
