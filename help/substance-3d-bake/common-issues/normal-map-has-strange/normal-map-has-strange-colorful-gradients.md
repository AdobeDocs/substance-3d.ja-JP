---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/normal-map-has-strange-colorful-gradients.html"
breadcrumb-title: ''
description: メッシュ法線、スムージンググループ、およびUVマッピングをチェックして、法線マップの奇妙でカラフルなグラデーションを修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal map has strange colorful gradients
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 法線マップに奇妙なカラフルなグラデーションが含まれている
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# 法線マップに奇妙なカラフルなグラデーションが含まれている

パン屋さんの作品には、非常に力強いカラフルなグラデーションが含まれています。

![](../../assets/color-gradient.png)


## 説明

通常、カラフルなグラデーションが発生するのは、ベイク処理時にハイポリゴンメッシュとローポリゴンメッシュの間に不一致がある場合です。 この不一致は、次の理由により説明できます。

* 高ポリゴンメッシュと低ポリゴンメッシュ<b>が互いに正しくオーバーラップ</b>していません（下図を参照）。
* 高ポリゴンは、低ポリゴンがカバーしようとする<b>ジオメトリがありません</b>。
* 高ポリゴンメッシュまたは低ポリゴンメッシュには、反転した頂点法線があります。

このような場合は、ベイク処理で存在しないジオメトリを一致させようとします。その結果、何も空になります。 パン屋はこの空白の領域を、テクスチャの隣接するピクセルから抽出した色で塗りつぶして、カラフルなグラデーションを作成します（<b>拡散</b>が無効になっていない場合）。

## 解決策

メッシュ間がオーバーラップしない原因となる可能性のあるいくつかの理由を考慮すると、いくつかの解決策を考慮する必要があります。

* メッシュ変換をフリーズ/リセット（X形のリセットなど）して、すべてのメッシュが一貫していることを確認してください
* 3Dモデリングソフトウェアにローポリメッシュとハイポリメッシュの両方をインポートして、それらが正しくオーバーラップしていることを確認します
* [名前による一致](../../features/matching-by-name/matching-by-name.md)機能を使用している場合は、名前付け規則が有効であることを確認してください（メッシュ名を出力するログファイルをベイク処理してから調べることで確認できます）。

### 例

次に、高ポリゴンの球と低ポリゴンの球の例を示します。 左側では、高ポリゴンがシフトされているため、メッシュはオーバーラップしません。

![](../../assets/baking-gradients.jpg)
