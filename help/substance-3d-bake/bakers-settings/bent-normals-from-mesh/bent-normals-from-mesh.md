---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/bent-normals-from-mesh.html"
breadcrumb-title: ''
description: 高ポリゴンメッシュからの周囲光の平均方向を記述するベント法線テクスチャを計算します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Bent Normals from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからの曲げ法線
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 3%

---


# メッシュからの曲げ法線

メッシュベイカーの曲げ法線は、周囲光の平均方向を表すテクスチャを計算します。 このパン屋は、[Mesh](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)パン屋の環境オクルージョンから派生します。

**使用可能：**

* Painter
* Designer
* Automation Toolkit

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **セカンダリレイ** | オクルージョンの量。 値を大きくするとノイズは少なくなりますが、計算に時間がかかります。 |
| **最小オクルーダー距離** | オクルージョン線が高ポリゴンジオメトリに当たる最小距離&#x200B;**.** |
| **最大オクルーダー距離** | オクルージョン線が高ポリゴンジオメトリに当たる最大距離。 |
| **バウンディングボックスを基準** | 有効な場合、レイ距離の計算はローポリゴンメッシュの正規化されたスペース(0 ～ 1)に基づいて行われます。 無効にすると、レイ距離の計算は、エクスポート時にローポリゴンメッシュで指定された単位（メートル、センチメートルなど）に基づいて行われます。 |
| **広がり角度** | オクルージョンレイの最大スプレッド角度 デフォルトは180です。 |
| **配布** | オクルージョンレイの角度分布有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>コサイン</strong> （既定）</li><li data-preserve-html="true"><strong>均一</strong></li></ul> |
| **裏面を無視** | 有効にすると、オクルージョンレイは背面のヒットを無視します（高ポリゴン法線がレイが発射される低ポリゴンと反対方向を向いている場合）。 ほとんどの場合、この設定を有効にして、斑点を回避する必要があります。 |
| **セルフオクルージョン** | オクルージョンレイの名前で照合します。 ベイカーが低ポリゴンおよび高ポリゴンのジオメトリに一致する方法を示します。 手動でメッシュを分解する必要なく、ベイク処理をフィルタするために使用できます。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定）:ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong>メッシュ名で</strong>：不要なジオメトリと一致しないように、メッシュを名前でフィルタします。</li></ul>一致するジオメトリの詳細については、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **マップの種類** | 出力テクスチャのタイプを定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ワールドスペース</strong></li><li data-preserve-html="true"><strong>接線空間</strong> （既定）</li></ul> |
| **法線の向き** | **マットの種類**&#x200B;が接線空間に設定されている場合に、出力テクスチャの法線の形式を制御します。可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong> <strong> <br/></strong></li><li data-preserve-html="true"><strong>DirectX</strong> （既定）<strong> <br/></strong></li></ul> |
