---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/common-parameters.html"
breadcrumb-title: ''
description: すべてのベイカーに適用される一般的なパラメーターと、最適なテクスチャ生成のためにベイカーを設定する方法について説明します。
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

共通のパラメータはすべてのパン屋に適用されます。 これらのパラメーターは通常、ベイカーがどのように動作し、ハイポリメッシュで動作するかを定義しますが、最終的なテクスチャがどのように生成されるかを定義します。 これらのパラメーターの一部は、特定のベイカーで上書きできます。

これらのパラメーターのほとんどは、すべてのソフトウェア（Substance Automation Toolkitを含む）で使用できますが、その動作は若干異なる場合があります。また、ソフトウェアのワークフローや実装によっては使用できない場合もあります。

## 一般パラメーター

これらのパラメーターは、パン屋がテクスチャを生成する方法に影響します。

| *名前* | *説明* |
| --- | --- |
| **サイズ** （デフォルトサイズまたは出力サイズ） | ベイク処理の出力テクスチャ解像度（ピクセル単位）を制御します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>32</strong></li><li data-preserve-html="true"><strong>64</strong></li><li data-preserve-html="true"><strong>128</strong></li><li data-preserve-html="true"><strong>256</strong></li><li data-preserve-html="true"><strong>512</strong></li><li data-preserve-html="true"><strong>1024</strong></li><li data-preserve-html="true"><strong>2048</strong> （既定値）</li><li data-preserve-html="true"><strong>4096</strong></li><li data-preserve-html="true"><strong>8192</strong></li></ul>非正方形の解像度もサポートされています（例：2048 x 1024 （2:1比率））。 Substance Designerでは、このパラメーターをベイカー自体で上書きできます。 |
| **形式** | ベイク処理されたテクスチャのファイル形式。*Substance Painterでは利用できません。* 参照：[&#x200B; ベイクしたマップの書き出し方法](../../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)。 |
| **アンチエイリアス** | 焼き込まれたテクスチャの品質を向上させ、異なるジオメトリが接続する場所でのエイリアスを減らすことができるアンチエイリアスを制御します。エイリアスについて詳しくは、[UV シームのエイリアス &#x200B;](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)および[Wikipedia](https://en.wikipedia.org/wiki/Aliasing)のエイリアスを参照してください。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>なし</strong> （デフォルト）</li><li data-preserve-html="true"><strong> サブサンプリング 2x2</strong></li><li data-preserve-html="true"><strong> サブサンプリング 4x4</strong></li><li data-preserve-html="true"><strong> サブサンプリング 8x8</strong></li></ul>  **注：** アンチエイリアスを有効にすると、テクスチャをより高解像度で計算してから、最初に選択したサイズに縮小してアンチエイリアスを実行できるため、ベイク処理時間が大幅に長くなります。 つまり、2x2 サブサンプリングを持つ2K テクスチャは、実際には4K テクスチャを計算します。サブサンプリングを増やすよりも、ベイカー内の光線の数を増やすことが望ましい場合があります。 待ちすぎることなく、より優れた結果を得ることができます。 |
| **UV セット** | ベイクしたテクスチャの計算に使用するローポリメッシュのUVを制御します。*Substance Painterでは利用できません。* |
|  |  |
| **拡張（px）** | UVの外側または境界線のピクセルを、指定されたピクセル数だけ拡大または拡大します。 この操作を使用すると、これらの境界線がテクスチャのピクセルに完全に整列していない場合や、テクスチャの解像度が低下した場合（例：mipmaps）に、UV境界でのシームを回避できます。 これは、ベーキングプロセスの後に適用されるポストプロセスです。 また、「パディング」と呼ばれることもあります。拡張について詳しくは、[UV シームのエイリアス &#x200B;](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)および[&#x200B; パディング &#x200B;](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/padding-134643719.html)を参照してください。 |
| **拡散を適用** | 有効にすると、UVの外側は、UVの境界線に基づいて滑らかなグラデーションカラーで塗りつぶされます。 このプロセスにより、テクスチャサイズを小さくすると、安定した状態が維持され、見えすぎるシーム（mipmapsなど）が作成されなくなります。 これは、ベーキングプロセスの後に適用されるポストプロセスです。 |
| **平均法線** | 有効にすると、ベイク処理のメッシュマッチングプロセス中に、どの方向に光線を送るかを知るために、頂点の平均法線を計算します。 無効にすると、レイはメッシュの元の頂点法線に従います。 |

## ハイポリパラメーター

次のパラメーターは、ハイポリからローポリのメッシュベイク処理（「メッシュから」ベイカー）を制御します。

| *名前* | *説明* |
| --- | --- |
| **高定義メッシュ** | ハイポリメッシュを含むファイル（またはSubstance パッケージリソース）のリスト。 ベーキングプロセスが異なる情報を計算し、そのメッシュ情報をテクスチャに保存し始めると、それらはベイカーによってメモリに読み込まれます。 「**低い定義を高い定義として使用**」が有効な場合、このリストは無視されます。 |
| **低解像度を高解像度として使用**&#x200B;または&#x200B;**低解像度ポリメッシュを高解像度メッシュとして使用** | 有効にすると、ベイカーに提供されるハイポリメッシュリストは無視され、代わりにローポリメッシュがベイク処理されます。このパラメーターは、ハイポリメッシュを直接操作する場合に便利です。 例えば、この設定を有効にしたハイポリカーのアンビエントオクルージョンテクスチャをベイクする場合、レイ距離は無視され、ベイカーは完璧なベイクを生成します（レイミスやジオメトリの不一致はありません）。 |
|  |  |
| **ケージとの距離を設定**&#x200B;または&#x200B;**ケージを使用** | レイ ディスタンスの値を使用する代わりに、ベイク処理でケージ メッシュ ファイルを使用するかどうかを示します。 ケージは、レイの最大距離と方向を制御します。 |
| **ケージファイル** | ケージを含むメッシュファイルへのパス。 |
| **Frontal Value**&#x200B;または&#x200B;**最大Frontal Distance** | レイがパスに沿って高ポリジオメトリを見つけるために、低ポリサーフェスからどの程度上に位置するかを制御します。*ケージが使用されている場合、この設定は影響しません。* |
| **後方値**&#x200B;または&#x200B;**最大後方距離** | レイが停止する低ポリサーフェスの下の位置を制御して、パスに沿って高ポリジオメトリを見つけます。*ケージが使用されている場合、この設定は影響しません。* |
| **バウンディングボックスに対する相対** | 有効にすると、レイ距離やその他のサイズ ベースの計算は、ローポリメッシュの正規化されたスペースに基づきます。 無効にした場合、レイ距離の計算は、書き出されたローポリメッシュ（メートル、センチメートルなど）で指定された単位に基づきます。オブジェクトに正確な測定値がある場合は、この設定を無効にしてレイ距離を手動で入力すると便利な場合があります。 |
|  |  |
| **一致** | ベイカーがローポリジオメトリとハイポリジオメトリにどのように一致するかを示します。 これは、手動でメッシュを離す（爆発させる）必要なく、ベーキングプロセスをフィルタリングするために使用できます。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定値）：ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong> メッシュ名</strong>: メッシュを名前でフィルタリングして、不要なジオメトリと一致しないようにします。</li></ul>ジオメトリの一致について詳しくは、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **一致するサフィックス**&#x200B;または&#x200B;**高ポリメッシュサフィックス** **低ポリメッシュサフィックス** | 「名前で一致」機能を使用する場合に、ジオメトリを識別してグループ化するためのメッシュ名の接尾辞。 使用可能な接尾辞：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Low Poly Mesh</strong>: シーン内のLow Poly メッシュを識別するためのサフィックス</li><li data-preserve-html="true"><strong>高ポリメッシュ </strong>：シーン内の高ポリメッシュを識別するためのサフィックス</li><li data-preserve-html="true"><strong> バックフェイスを無視</strong>：特定のベイカーが無視するメッシュを識別するサフィックス（[Ambient Occlusion From Mesh](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)など）</li></ul>ジオメトリの一致について詳しくは、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
|  |  |
| **ゆがみ補正を使用** | 有効にすると、入力テクスチャに応じて、**平均法線**&#x200B;または元のジオメトリ法線からレイ方向が計算されます。 テクスチャの黒い値は計算された平均法線を使用し、白い値は元のメッシュ法線を使用します。*Substance Painterでは利用できません。* |
| **ゆがみマップ** | 光線の投影を傾斜させるために使用されるテクスチャファイルへのパス。 |
| **ゆがみ補正を反転** | 入力テクスチャの読み取りを反転します（黒は白になり、白は黒になります）。 |
