---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/bent-normals-from-mesh.html"
breadcrumb-title: ''
description: 高ポリメッシュからの環境光の平均方向を記述するベント法線テクスチャを計算します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Bent Normals from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからのベント法線
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 3%

---


# メッシュからのベント法線

メッシュベイカーのBent Normalsは、環境光の平均方向を表すテクスチャを計算します。 このベイカーは、Mesh](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md) ベイカーの[Ambient Occlusionから派生しています。

**次の場所で利用できます：**

* Painter
* Designer
* Automation Toolkit

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **セカンダリ レイ** | オクルージョンレイの量。 値を大きくすると、ノイズは少なくなりますが、計算に時間がかかります。 |
| **最小オクルーダー距離** | オクルージョンレイが高いポリジオメトリに当たる最小距離**.** |
| **最大オクルーダー距離** | オクルージョンレイが高いポリジオメトリに当たる最大距離。 |
| **バウンディングボックスに対する相対** | 有効にすると、レイ距離の計算は、ローポリメッシュの正規化されたスペース（0 ～ 1）に基づきます。 無効にした場合、レイ距離の計算は、書き出し時にローポリメッシュで指定された単位（メートル、センチメートルなど）に基づきます。 |
| **スプレッド角度** | オクルージョンレイの最大スプレッド角度 デフォルトは180です。 |
| **配布** | オクルージョンレイの角度分布使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Cosine</strong> （既定値）</li><li data-preserve-html="true"><strong>均一</strong></li></ul> |
| **バックフェイスを無視** | オクルージョンレイを有効にすると、バックフェイス上のヒットが無視されます（高いポリゴンの法線が低いポリゴンと反対の方向に向いている場合は、レイが発生する位置からヒットします）。 多くの場合、この設定はアーティファクトを回避するために有効にする必要があります。 |
| **セルフオクルージョン** | オクルージョンレイの名前によるマッチング。 ベイカーがローポリジオメトリとハイポリジオメトリにどのように一致するかを示します。 これは、手動でメッシュを離す（爆発させる）必要なく、ベーキングプロセスをフィルタリングするために使用できます。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定値）：ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong> メッシュ名</strong>: メッシュを名前でフィルタリングして、不要なジオメトリと一致しないようにします。</li></ul>ジオメトリの一致について詳しくは、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **マップの種類** | 出力テクスチャのタイプを定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong> ワールド空間</strong></li><li data-preserve-html="true"><strong>接線空間</strong> （既定値）</li></ul> |
| **通常の向き** | **Mat Type**&#x200B;がTangent Spaceに設定されている場合、出力テクスチャの通常の形式を制御します。使用可能な値は次のとおりです。<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong> <strong> <br/></strong></li><li data-preserve-html="true"><strong>DirectX</strong> （既定値） <strong> <br/></strong></li></ul> |
