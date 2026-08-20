---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/thickness-map-from-mesh.html"
breadcrumb-title: ''
description: SSS シェーダやマスクで使用するために、メッシュ サーフェスから内側に向かって光線をキャストして厚みマップを生成します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Thickness Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからの厚みマップ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 5%

---


# メッシュからの厚みマップ

メッシュからの厚みマップは、アンビエントオクルージョンベイカーと非常によく似ていますが、メッシュの表面から内側に光線をキャストします。 このテクスチャは、Sub Surface Scattering （SSS）シェーダで使用することも、テクスチャのマスキングに使用することもできます。

テクスチャのプロパティは次のように定義されます。

* 黒い値は、モデルの薄い部分を表します。
* 白い値は、モデルの太い部分を表します。

**次の場所で利用できます：**

* Substance Painter
* Substance Designer
* Substance Automation Toolkit

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **セカンダリ レイ** | オクルージョンレイの量。 値を大きくすると、ノイズは少なくなりますが、計算に時間がかかります。 デフォルトは64です。 |
| **最小オクルーダー距離** | オクルージョンレイが高いポリジオメトリに当たる最小距離。 デフォルトは0.00001です。 |
| **最大オクルーダー距離** | オクルージョンレイが高いポリジオメトリに当たる最大距離。 デフォルトは0.1です。 |
| **バウンディングボックスに対する相対** | 有効にすると、単位はオブジェクトのバウンディングボックスに対する相対パスになります（1.0はバウンディングボックスの対角線長です）。 無効にした場合、最小オクルーダー距離と最大オクルーダー距離に使用される単位は、メッシュの書き出し時に定義される単位（メートル、センチメートル、または書き出されたシーンの単位）です。 |
| **スプレッド角度** | オクルージョンレイの最大スプレッド角度 デフォルトは180です。 |
| **配布** | オクルージョンレイの角度分布使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Cosine</strong> （既定値）</li><li data-preserve-html="true"><strong>均一</strong></li></ul> |
| **バックフェイスを無視** | オクルージョンレイを有効にすると、バックフェイス上のヒットが無視されます（高いポリゴンの法線が低いポリゴンと反対の方向に向いている場合は、レイが発生する位置からヒットします）。 多くの場合、この設定はアーティファクトを回避するために有効にする必要があります。 |
| **セルフオクルージョン** | オクルージョンレイの名前によるマッチング。 ベイカーがローポリジオメトリとハイポリジオメトリにどのように一致するかを示します。 これは、手動でメッシュを離す（爆発させる）必要なく、ベーキングプロセスをフィルタリングするために使用できます。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定値）：ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong> メッシュ名</strong>: メッシュを名前でフィルタリングして、不要なジオメトリと一致しないようにします。</li></ul>ジオメトリの一致について詳しくは、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **自動正規化** | 出力値を0 ～ 1の範囲に収めるように拡大・縮小する必要があるかどうかを定義します（最も明るい点は純白に設定し、最も暗い点は純黒に設定します）。 |
