---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature.html"
breadcrumb-title: ''
description: メッシュから曲率情報を抽出し、ジオメトリの空洞とエッジを強調表示するテクスチャを作成します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 曲率
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 3%

---


# 曲率

Curvature bakerでは、曲率テクスチャを抽出できます。 このテクスチャには、ジオメトリに関連するキャビティとエッジの情報が含まれています。

テクスチャプロパティは次のように定義されます。

* 黒の値は凹状の領域を表します。
* 白の値は凸形の領域を表します。
* グレー値は、中性領域（主に平坦）を表します。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット
* Substance Painter

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **アルゴリズム** | メッシュ上での曲率情報の計算方法を定義します。 |
| **詳細** | 曲率の情報の強さを制御します。 値を大きくすると、ディテールは鮮明になりますが、繊細さは軽減されます。 |
| **縫い目を有効にする** | これを有効にすると、パン屋はUV アイランド間の継ぎ目を減らすために、一方の端からもう一方の端にテキセルをコピーしようとします。 |
| **縫い目** **強度** | **縫い目を有効にする**&#x200B;を有効にした場合、このパラメーターは縫い目の固定の強さを制御します。 |
