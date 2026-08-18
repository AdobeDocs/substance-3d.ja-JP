---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/height-map-from-mesh.html"
breadcrumb-title: ''
description: ハイポリゴンメッシュからHeightマップを作成し、テクスチャリング用にサーフェスのディテールとジオメトリ情報をキャプチャします。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Height Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからの高さマップ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 8%

---


# メッシュからの高さマップ

メッシュベイカーからHeightマップを使用すると、高ポリゴンメッシュからHeightマップを作成できます。**使用可能：**

* Painter
* Designer
* Automation Toolkit

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| ****正規化**** | Heightの値の範囲をテクスチャに保存する方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>レイ距離に対する相対</strong>:</li><li data-preserve-html="true"><strong>ローポリメッシュを基準（UVタイル単位）</strong> （デフォルト）</li><li data-preserve-html="true"><strong>最小/最大を基準（UVタイル単位）</strong></li><li data-preserve-html="true"><strong>マニュアル</strong></li></ul> |
| **縮尺除数** | Heightの値を乗算または除算する量を指定します。**正規化**&#x200B;が&#x200B;**手動**&#x200B;に設定されている場合にのみ使用できます。 |
