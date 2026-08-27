---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/common-parameters.html"
breadcrumb-title: ''
description: すべてのベイカーに適用される一般的なパラメーターと、最適なテクスチャ生成ができるように設定する方法について説明します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Common Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 共通のパラメーター
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 1%

---


# 共通のパラメーター

共通パラメーターはすべてのパン屋に適用されます。 これらのパラメータは、通常、ベイカーがどのように動作し、ハイポリメッシュで動作するかを定義しますが、最終的なテクスチャがどのように生成されるかを定義します。 これらのパラメータの一部は、特定のベイカーによってオーバーライドできます。

これらのパラメーターのほとんどは、すべてのソフトウェア（Software Automation Toolkitを含む）で使用できますが、Substanceのワークフローや実装によっては、動作が若干異なる場合や、使用できない場合があります。

## 一般パラメーター

これらのパラメータは、ベイカーがテクスチャを生成する方法に影響します。

| *名前* | *説明* |
| --- | --- |
| **サイズ** （既定のサイズまたは出力サイズ） | ベイク処理の出力テクスチャの解像度（ピクセル単位）を制御します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>32</strong></li><li data-preserve-html="true"><strong>64</strong></li><li data-preserve-html="true"><strong>128</strong></li><li data-preserve-html="true"><strong>256</strong></li><li data-preserve-html="true"><strong>512</strong></li><li data-preserve-html="true"><strong>1024</strong></li><li data-preserve-html="true"><strong>2048</strong> （既定）</li><li data-preserve-html="true"><strong>4096</strong></li><li data-preserve-html="true"><strong>8192</strong></li></ul>非正方形の解像度もサポートされます(例： 2048 x 1024（2:1比）)。 Substance Designerでは、このパラメータはbaker自身で上書きできます。 |
| **形式** | ベイク処理されたテクスチャのファイルフォーマット。*Substance Painterで使用できません。* 参照： [ベイク済みマップのエクスポート方法](../../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)。 |
| **アンチエイリアス** | アンチエイリアスを制御します。これにより、ベイク処理されたテクスチャの品質が向上し、さまざまなジオメトリが接続する部分のエイリアスが減少します。エイリアスの詳細については、[UVシームでのエイリアス](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)および[Wikipediaでのエイリアス](https://en.wikipedia.org/wiki/Aliasing)を参照してください。利用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>なし</strong> （既定）</li><li data-preserve-html="true"><strong>サブサンプリング2x2</strong></li><li data-preserve-html="true"><strong>サブサンプリング4x4</strong></li><li data-preserve-html="true"><strong>サブサンプリング8x8</strong></li></ul>  **注意：**&#x200B;アンチエイリアスを有効にすると、テクスチャの解像度を上げて計算し、選択した元のサイズにダウンスケールするので、ベイク処理にかかる時間が大幅に長くなります。 つまり、2x2サブサンプリングを使用した2Kテクスチャは、実際には4Kテクスチャを計算します。場合によっては、サブサンプルを増やすよりもパン屋の光線数を増やすほうが好ましい場合があります。 あまり長く待つことなく、より良い結果を得ることができます。 |
| **UVセット** | ベイク処理されたテクスチャの計算に使用するローポリメッシュのUVを制御します。*Substance Painterで使用できません。* |
|  |  |
| **膨張(px)** | UVの外側または境界のピクセルを、指定されたピクセルの量だけ拡張または拡張します。 この操作により、境界がテクスチャピクセルに完全に位置合わせされていない場合、またはテクスチャ解像度が低い場合（例：ミップマップ）に、UV境界の継ぎ目を避けることができます。 これは、ベイクプロセスの後に適用されるポストプロセスです。 パディングと呼ばれることもあります。拡張の詳細については、[UVシーム上のエイリアス](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)および[パディング](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/padding-134643719.html)を参照してください。 |
| **誤差拡散法を適用** | 有効にすると、UVの外側は、UV境界に基づく滑らかなグラデーションカラーで塗りつぶされます。 このプロセスにより、テクスチャのサイズを小さくしても安定した状態が保たれ、目に見えすぎる継ぎ目（例： mipmaps）が生じなくなります。 これは、ベイクプロセスの後に適用されるポストプロセスです。 |
| **平均法線** | このオプションが有効な場合、ベイク処理のメッシュマッチング処理中にレイを送信する方向を知るために頂点の平均法線を計算します。 無効にすると、レイはメッシュの元の頂点法線に従います。 |

## High-Polyパラメータ

次のパラメータは、高ポリゴンから低ポリゴンへのメッシュベイク処理（「メッシュベイカーから」）を制御します。

| *名前* | *説明* |
| --- | --- |
| **高解像度メッシュ** | high-polyメッシュを含むファイル（またはSubstanceパッケージリソース）のリスト。 ベイクプロセスが異なるメッシュを計算し、その情報をテクスチャに保存し始めると、ベイカーによってメモリにロードされます。 このリストは、[**低画質の高解像度を使用**]が有効になっている場合は無視されます。 |
| **低解像度を高精細として使用**&#x200B;または&#x200B;**ローポリメッシュをハイポリメッシュとして使用** | 有効にすると、ベイカーに提供される高ポリゴンのメッシュリストは無視され、低ポリゴンのメッシュは代わりにそれ自体にベイクされます。このパラメータは、高ポリゴンのメッシュを直接操作する場合に便利です。 たとえば、この設定を有効にして高ポリゴンの自動車のテクスチャをベイクする場合、光線距離は無視され、ベイカーは完全なベイクを生成します（光線の欠落やジオメトリの不一致はありません）。 |
|  |  |
| **ケージとの距離を設定**&#x200B;または&#x200B;**ケージを使用** | ベイクプロセスで光線距離値の代わりにケージメッシュファイルを使用するかどうかを示します。 ケージは、レイの最大距離と方向をコントロールします。 |
| **ケージファイル** | ケージを含むメッシュファイルへのパス。 |
| **正面方向の値**&#x200B;または&#x200B;**正面方向の最大距離** | 低ポリゴンサーフェスの上で、レイがそのパスに沿って高ポリゴンジオメトリを検出し始める距離をコントロールします。*ケージを使用する場合、この設定は無効です。* |
| **後方の値**&#x200B;または&#x200B;**後方の最大距離** | パスに沿って高ポリゴンジオメトリを検出するためにレイが停止する低ポリゴンサーフェスの下の距離をコントロールします。*ケージを使用する場合、この設定は無効です。* |
| **バウンディングボックスを基準** | 有効にすると、レイディスタンスやその他のサイズに基づく計算は、ローポリゴンメッシュの正規化されたスペースに基づきます。 無効にした場合、レイの距離の計算はエクスポート時にローポリメッシュで指定された単位（メートル、センチメートルなど）に基づきます。この設定を無効にして、オブジェクトが正確に測定されているときにレイの距離を手動で入力すると便利な場合があります。 |
|  |  |
| **一致** | ベイカーが低ポリゴンおよび高ポリゴンのジオメトリに一致する方法を示します。 手動でメッシュを分解する必要なく、ベイク処理をフィルタするために使用できます。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定）:ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong>メッシュ名で</strong>：不要なジオメトリと一致しないように、メッシュを名前でフィルタします。</li></ul>一致するジオメトリの詳細については、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **サフィックスの一致**&#x200B;または&#x200B;**ハイポリメッシュサフィックス** **ローポリメッシュサフィックス** | 「名前による一致」機能を使用する場合に、ジオメトリを識別してグループ化するためのメッシュ名サフィックス。 利用可能なサフィックス：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ローポリメッシュ</strong>: シーン内のローポリメッシュを特定するためのサフィックス</li><li data-preserve-html="true"><strong>ハイポリメッシュ</strong>: シーン内の高ポリゴンのメッシュを特定するためのサフィックス</li><li data-preserve-html="true"><strong>背面を無視</strong>：特定のベイカーが無視する必要があるメッシュを特定するためのサフィックス（[メッシュからのAmbient occlusion](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)など）</li></ul>一致するジオメトリの詳細については、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
|  |  |
| **ゆがみ補正を使用** | 有効にすると、レイ方向は、入力テクスチャに応じて&#x200B;**平均法線**&#x200B;または元のジオメトリ法線から計算されます。 テクスチャ内の黒の値は計算された平均法線を使用し、白の値は元のメッシュ法線を使用します。*Substance Painterで使用できません。* |
| **歪曲マップ** | 光線投影のスキューに使用するテクスチャファイルへのパス。 |
| **ゆがみ補正を反転** | 入力テクスチャの読み取りを反転します（黒は白に、白は黒になります）。 |
