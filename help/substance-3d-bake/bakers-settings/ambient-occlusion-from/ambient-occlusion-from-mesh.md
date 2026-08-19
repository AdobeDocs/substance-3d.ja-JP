---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/ambient-occlusion-from-mesh.html"
breadcrumb-title: ''
description: レイトレーシングテクニックを使用して、高ポリメッシュから正確なアンビエントオクルージョンテクスチャをベイクして、リアルさを高めます。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからのアンビエントオクルージョン
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 2%

---


# メッシュからのアンビエントオクルージョン

メッシュベイカーのAmbient Occlusionを使用すると、高いポリメッシュからAmbient Occlusion テクスチャをベイクできます。 ベース [ アンビエントオクルージョン ](../../bakers-settings/ambient-occlusion/ambient-occlusion.md) ベイカーよりも速度が遅くなりますが、より正確な結果が得られます。

**次の場所で利用できます：**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **セカンダリ レイ** | オクルージョンレイの量。 値を大きくすると、ノイズは少なくなりますが、計算に時間がかかります。 デフォルトは64です。 |
| **最小オクルーダー距離** | オクルージョンレイが高いポリジオメトリに当たる最小距離。 デフォルトは0.00001です。 |
| **最大オクルーダー距離** | オクルージョンレイが高いポリジオメトリに当たる最大距離。 デフォルトは0.1です。 |
| **バウンディングボックスに対する相対** | 有効にすると、単位はオブジェクトのバウンディングボックスに対する相対パスになります（1.0はバウンディングボックスの対角線長です）。 無効にした場合、最小オクルーダー距離と最大オクルーダー距離に使用される単位は、メッシュの書き出し時に定義される単位（メートル、センチメートル、または書き出されたシーンの単位）です。 |
| **スプレッド角度** | オクルージョンレイの最大スプレッド角度 デフォルトは180です。 |
| **配布** | オクルージョンレイの角度分布 スプレッド角度のサイズの円錐内で光線がどのように散乱されるかを定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Cosine</strong> （既定値）：現実的ですが、非常に細い隠れ領域で白い線が生じる可能性があります。 シェーディングとライティングに適しています。</li><li data-preserve-html="true"><strong>Uniform</strong>：線形グラデーションの作成に便利です。 レイヤーマスクやその他のフィルタリングに適しています。</li></ul> |
| **バックフェイスを無視** | このパラメーターは、オクルージョンレイがバックフェイス上のヒットを無視するかどうかを定義します（高いポリ法線が、レイが発生する場所から低いポリと逆方向に面する場合）。 多くの場合、この設定はアーティファクトを回避するために有効にする必要があります。 使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nevers</strong> （既定値）: バックフェイスは無視されません</li><li data-preserve-html="true"><strong>常に</strong>: バックフェイスは常に無視されます</li><li data-preserve-html="true"><strong> メッシュ名</strong>: サフィックス キーワードに一致するメッシュに対してのみ、バックフェイスが無視されます。 [共通パラメーター](../../bakers-settings/common-parameters/common-parameters.md)を参照してください。</li></ul> |
| **セルフオクルージョン** | オクルージョンレイの名前によるマッチング。 ベイカーがローポリジオメトリとハイポリジオメトリにどのように一致するかを示します。 これは、手動でメッシュを離す（爆発させる）必要なく、ベーキングプロセスをフィルタリングするために使用できます。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定値）：ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong> メッシュ名</strong>: メッシュを名前でフィルタリングして、不要なジオメトリと一致しないようにします。</li></ul>ジオメトリの一致について詳しくは、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **法線マップ** | 通常のテクスチャへのオプションのパス。 パン屋の内部計算を置き換えるために使用できます。 |
| **ワールド スペース** | 有効にすると、法線テクスチャは接線空間ではなくワールド空間法線として解釈されます。 |
| **通常の向き** | 接線空間の場合の標準テクスチャの形式。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> （既定値）</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
| **減衰** | オクルーダー距離によるオクルージョンの減衰方法を定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>なし</strong>：減衰なし。</li><li data-preserve-html="true"><strong>線形</strong> （デフォルト）：進行減衰。</li><li data-preserve-html="true"><strong> スムーズ </strong>：ソフト減衰。</li></ul> |
| **地表** | 有効にした場合は、XZ軸上のメッシュのバウンディングボックスの下にある平面をシミュレートして、セカンダリレイと衝突させます。 これは、非表示の平面図からのシャドウをシミュレートします。 |
| **地表オフセット** | メッシュからプランを離して、エフェクトの適用度を下げることができます。 この値は絶対であり、メッシュサイズに対して相対的ではありません。 |
