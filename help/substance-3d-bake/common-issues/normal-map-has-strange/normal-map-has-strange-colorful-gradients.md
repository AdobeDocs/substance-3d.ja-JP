---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/normal-map-has-strange-colorful-gradients.html"
breadcrumb-title: ''
description: メッシュ法線、スムージンググループ、UV マッピングをチェックして、法線マップの奇妙なカラフルなグラデーションを修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal map has strange colorful gradients
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 法線マップに奇妙な色彩グラデーションがある
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# 法線マップに奇妙な色彩グラデーションがある

ベイカーの出力は、非常に強いカラフルなグラデーションのセットです。

![](../../assets/color-gradient.png)


## 説明

カラフルなグラデーションは、通常、ベイク処理の際にハイポリメッシュとローポリメッシュの間に不一致が生じた場合に発生します。 この不一致は、次の理由で説明できます。

* ハイポリとローポリのメッシュ <b>が互いに適切に重なり合わない</b> （以下の画像を参照）。
* ハイポリは、ローポリがカバーしようとしている<b> ジオメトリが見つかりません</b>。
* ハイポリまたはローポリメッシュが頂点の法線を反転しています。

これが発生すると、ベイク処理は存在しないジオメトリと一致させようとするため、何かが空になります。 ベイカーは、この空の領域を、テクスチャ内の隣接ピクセルから抽出された色で塗りつぶし、カラフルなグラデーションを作成します（<b>拡散</b>が無効でない限り）。

## Solution

メッシュ間の重複が発生しない原因となる可能性のあるいくつかの理由を考えると、いくつかの解決策を考慮する必要があります。

* メッシュの変形をフリーズ/リセットして（x フォームのリセットなど）、すべてのメッシュが一貫していることを確認します
* 3D モデリングソフトウェアにローポリメッシュとハイポリメッシュの両方を読み込んで、それらが適切に重なっていることを確認します
* [名前で一致](../../features/matching-by-name/matching-by-name.md)機能を使用している場合は、命名規則が有効であることを確認してください（メッシュ名を印刷する必要があるログファイルをベイク処理して確認できます）。

### 例

以下は、ハイポリとローポリの球体を使用した例です。 左側では、ハイポリが移動しているため、メッシュが重なりません。

![](../../assets/baking-gradients.jpg)
