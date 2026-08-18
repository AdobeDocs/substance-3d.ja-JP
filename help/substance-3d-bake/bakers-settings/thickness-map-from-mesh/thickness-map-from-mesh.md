---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/thickness-map-from-mesh.html"
breadcrumb-title: ''
description: SSSシェーダとマスキングで使用するために、メッシュサーフェスから内側に向けて光線を投射してThicknessマップを生成します。
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

メッシュからのThicknessマップは周囲のオクルージョンベイカーと非常によく似ていますが、メッシュのサーフェスから内側に光線を照射します。 このテクスチャは、Sub Surface Scattering(SSS)シェーダまたはマスキングテクスチャで使用できます。

テクスチャプロパティは次のように定義されます。

* 黒の値は、モデルの細い部分を表します。
* 白の値は、モデルの太い部分を表します。

**使用可能：**

* Substance Painter
* Substance Designer
* Substance自動処理ツールキット

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **セカンダリレイ** | オクルージョンの量。 値を大きくすると、ノイズは少なくなりますが、計算に時間がかかります。 デフォルトは64です。 |
| **最小オクルーダー距離** | オクルージョン線が高ポリゴンジオメトリに当たる最小距離。 デフォルトは0.00001です。 |
| **最大オクルーダー距離** | オクルージョン線が高ポリゴンジオメトリに当たる最大距離。 デフォルトは0.1です。 |
| **バウンディングボックスを基準** | 有効になっている場合、単位はオブジェクトのバウンディングボックスを基準とします（1.0はバウンディングボックスの対角線の長さです）。 無効にすると、オクルーダの最小距離と最大距離に使用される単位は、メッシュを書き出すときに定義された単位（メートル、センチメートル、または書き出したシーンの任意の単位）になります。 |
| **広がり角度** | オクルージョンレイの最大スプレッド角度 デフォルトは180です。 |
| **配布** | オクルージョンレイの角度分布有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>コサイン</strong> （既定）</li><li data-preserve-html="true"><strong>均一</strong></li></ul> |
| **裏面を無視** | 有効にすると、オクルージョンレイは背面のヒットを無視します（高ポリゴン法線がレイが発射される低ポリゴンと反対方向を向いている場合）。 ほとんどの場合、この設定を有効にして、斑点を回避する必要があります。 |
| **セルフオクルージョン** | オクルージョンレイの名前で照合します。 ベイカーが低ポリゴンおよび高ポリゴンのジオメトリに一致する方法を示します。 手動でメッシュを分解する必要なく、ベイク処理をフィルタするために使用できます。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定）:ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong>メッシュ名で</strong>：不要なジオメトリと一致しないように、メッシュを名前でフィルタします。</li></ul>一致するジオメトリの詳細については、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **自動正規化** | 出力値を0 ～ 1の範囲に収めるようにスケールするかどうかを定義します（最も明るい点は純粋な白に設定され、最も暗い点は純粋な黒に設定されます）。 |
