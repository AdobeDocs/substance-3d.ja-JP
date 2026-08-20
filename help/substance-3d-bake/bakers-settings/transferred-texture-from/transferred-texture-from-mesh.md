---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/transferred-texture-from-mesh.html"
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

メッシュ ベイカーから転送されるテクスチャを使用すると、各UVに基づいて、あるメッシュから別のメッシュにテクスチャを変換できます。 このベイカーは、転送または法線マップもサポートしています（特別な変換が必要です）。 動作させるには、両方のメッシュにUV定義が必要です。

**次の場所で利用可能：**

* Substance Designer
* Substance Automation Toolkit

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **テクスチャファイル** | 転送される入力テクスチャファイルへのパス。 |
| **UV セット** | ハイポリメッシュで使用するUVをメッシュしてテクスチャを読み取り、ローポリメッシュに投影します。 |
| **フィルタリングモード** | テクスチャのピクセル補間の実行方法を定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>最も近い</strong>：補間なし。指定した位置に最も近いピクセルを使用します。 正確ですが、エイリアスを作成できます。</li><li data-preserve-html="true"><strong> バイリニア </strong> （デフォルト）：指定した位置に最も近い4つのピクセルを使用します。 エイリアシングはありませんが、ぼやけることがあります。</li></ul> |
| **法線マップ** | 有効にすると、転送する入力テクスチャが法線マップであることをパン屋に示します。 これは、ベイカーがテクスチャに特別な変換を適用して、ターゲットメッシュと互換性を持たせることを示します。 |
| **マップの種類** | 入力テクスチャの法線マップのタイプを定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong> ワールド スペース </strong></li><li data-preserve-html="true"><strong>接線空間</strong> （既定値）</li></ul> |
| **通常の向き** | **マップの種類**&#x200B;が&#x200B;**接線空間**&#x200B;に設定されている場合、入力テクスチャの通常の形式を定義します。使用可能な値は次のとおりです。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> （既定値）</li></ul> |
