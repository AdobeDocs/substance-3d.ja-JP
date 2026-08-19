---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature.html"
breadcrumb-title: ''
description: メッシュから曲率情報を抽出して、ジオメトリのキャビティとエッジを強調するテクスチャを作成します。
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

曲率ベイカーでは、曲率テクスチャを抽出できます。 このテクスチャには、ジオメトリに関連するキャビティとエッジ情報が含まれています。

テクスチャのプロパティは次のように定義されます。

* 黒い値は凹部を表します。
* 白い値は凸状の領域を表します。
* グレーの値は、中立領域（主に平坦）を表します。

**次の場所で利用可能：**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **アルゴリズム** | 曲率情報がメッシュ上でどのように計算されるかを定義します。 |
| **詳細** | 曲率の情報の強さを制御します。 値を大きくすると、ディテールは多くなりますが、微妙さが少なくなります。 |
| **シームを有効にする** | このオプションを有効にすると、ベイカーは境界のテッセルを一方から他方にコピーして、UV島間のシームを減らそうとします。 |
| **縫い目** **強度** | **シームを有効にする**&#x200B;が有効になっている場合、このパラメーターはシーム修正の強度を制御します。 |
