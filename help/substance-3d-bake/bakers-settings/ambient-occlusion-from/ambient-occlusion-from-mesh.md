---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/ambient-occlusion-from-mesh.html"
breadcrumb-title: ''
description: レイトレーシングのテクニックを使用して、ハイポリメッシュから正確な環境オクルージョンテクスチャをベイク処理し、リアルさを高めます。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからの環境オクルージョン
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 2%

---


# メッシュからの環境オクルージョン

メッシュベイカーの環境オクルージョンを使用すると、高ポリゴンメッシュの環境オクルージョンテクスチャをベイク処理できます。 ベース[周囲オクルージョン](../../bakers-settings/ambient-occlusion/ambient-occlusion.md)ベイカーよりも低速ですが、より正確な結果が得られます。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット
* Substance Painter

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **セカンダリレイ** | オクルージョンの量。 値を大きくすると、ノイズは少なくなりますが、計算に時間がかかります。 デフォルトは64です。 |
| **最小オクルーダー距離** | オクルージョン線が高ポリゴンジオメトリに当たる最小距離。 デフォルトは0.00001です。 |
| **最大オクルーダー距離** | オクルージョン線が高ポリゴンジオメトリに当たる最大距離。 デフォルトは0.1です。 |
| **バウンディングボックスを基準** | 有効になっている場合、単位はオブジェクトのバウンディングボックスを基準とします（1.0はバウンディングボックスの対角線の長さです）。 無効にすると、オクルーダの最小距離と最大距離に使用される単位は、メッシュを書き出すときに定義された単位（メートル、センチメートル、または書き出したシーンの任意の単位）になります。 |
| **広がり角度** | オクルージョンレイの最大スプレッド角度 デフォルトは180です。 |
| **配布** | オクルージョンレイの角度分布 拡散角度の大きさの円錐内に光線が散乱される方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>コサイン</strong> （既定）:リアルですが、非常に薄い閉塞部に白い線が表示されることがあります。 シェーディングと照明に適しています。</li><li data-preserve-html="true"><strong>均一</strong>：線形グラデーションを作成する場合に便利です。 レイヤーマスクやその他のフィルタリングに適しています。</li></ul> |
| **裏面を無視** | このパラメータは、オクルージョン線が背面のヒットを無視するかどうかを定義します（高いポリゴンの法線が低いポリゴンと反対の方向を向いている場合、レイが発射されます）。 ほとんどの場合、この設定を有効にして、斑点を回避する必要があります。 有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ネバー</strong> （既定）：背面は無視されません</li><li data-preserve-html="true"><strong>常に</strong>：背面は常に無視されます</li><li data-preserve-html="true"><strong>メッシュ名による</strong>：背面は、接尾辞キーワードに一致するメッシュに対してのみ無視されます。 [共通パラメーター](../../bakers-settings/common-parameters/common-parameters.md)を参照してください。</li></ul> |
| **セルフオクルージョン** | オクルージョンレイの名前で照合します。 ベイカーが低ポリゴンおよび高ポリゴンのジオメトリに一致する方法を示します。 手動でメッシュを分解する必要なく、ベイク処理をフィルタするために使用できます。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定）:ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong>メッシュ名で</strong>：不要なジオメトリと一致しないように、メッシュを名前でフィルタします。</li></ul>一致するジオメトリの詳細については、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **標準マップ** | 法線テクスチャへのパス（オプション）。 ベーカーの内部計算の置き換えに使用できます。 |
| **ワールドスペース** | 有効にすると、法線テクスチャは接線空間ではなくワールド空間法線として解釈されます。 |
| **法線の向き** | 接線空間の場合の法線テクスチャのフォーマット。指定可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> （既定）</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
| **減衰** | オクルージョンをオクルダ距離で減衰する方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>なし</strong>：減衰なし。</li><li data-preserve-html="true"><strong>線形</strong> （既定） ：漸進的な減衰です。</li><li data-preserve-html="true"><strong>滑らか</strong>：弱い減衰。</li></ul> |
| **グリッド** | 有効な場合は、XZ軸上のメッシュのバウンディングボックスの下にある平面をシミュレートして、セカンダリレイと衝突させます。 これにより、見えない平面図から生じる影をシミュレートします。 |
| **グリッドのオフセット** | プランをメッシュから離して、効果の強度を下げることができます。 この値は絶対値で、メッシュサイズに対する相対値ではありません。 |
