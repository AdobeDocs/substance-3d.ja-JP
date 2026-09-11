---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/renderers/maxwell/maxwell-substance-painter.html"
breadcrumb-title: ''
description: 適切な出力テンプレートとマテリアル設定を使用して、Maxwellレンダラー用のSubstance Painterテクスチャを書き出します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Maxwell > Maxwell - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: マックスウェル – Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# マックスウェル – Substance Painter

Substance Painter 2020.1(6.1.0)では、メタリック/ラフネスおよびSpecular/光沢についてMaxwell [出力テンプレート](https://experienceleague.adobe.com/ja/docs/substance-3d-painter/using/getting-started/export/export)がサポートされています。 Maxwell **を使用して簡単に書き出すことができます。\
Maxwell 5.1.0**はSubstance Painterとの連携により、テクスチャを簡単に読み込んでMaxwellマテリアルを自動設定できます。

## テクスチャの書き出し

Maxwell （メタリックの粗さ）またはMaxwell （Specular光沢）出力テンプレートを選択して、Maxwellでレンダリングするテクスチャを書き出すことができます。

![](../../../assets/maxwell-output.png){width="500px"}

## Maxwellでのテクスチャの適用

MaxwellのSubstance Painterの組み込みを使用して、Substance Painterから書き出されたマップが適用されたマテリアルを自動作成できます。\
まず、マテリアルリストを右クリックし、**新規/Substance Painter**&#x200B;を選択します。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maxwell-painter?$png$&jpegSize=100&wid=413)

Substance Painterテクスチャを書き出した場所を参照し、ベースカラーなどのマップの1つを選択します。 [開く]をクリックすると、マップが割り当てられた新しいMaxwellマテリアルが統合によって作成されます。\
Substance Painterから複数のテクスチャセットを書き出した場合、統合ではテクスチャの命名規則を使用して、一致するテクスチャマップが割り当てられます。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/image-material?$png$&jpegSize=100&wid=620){width="600px"}

その後、シーン内のアセットにマテリアルを割り当てることができます。

![](../../../assets/assigned.png){width="500px"}

Substance Painter統合を使用して適用されたすべてのマテリアル。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/materials-assigned?$pjpeg$&jpegSize=300&wid=1511){width="800px"}
