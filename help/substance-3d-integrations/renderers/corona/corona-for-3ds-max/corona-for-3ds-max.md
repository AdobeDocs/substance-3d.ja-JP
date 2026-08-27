---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/renderers/corona/corona-for-3ds-max.html"
breadcrumb-title: ''
description: 3ds Maxのコロナレンダラーでは、Specularや光沢度のワークフローと必要なマップを使用してSubstanceマテリアルを使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona > Corona for 3ds Max
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Maxのコロナ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# 3ds Maxのコロナ

## MayaプラグインのSubstance

![](../../../assets/scene-001v03.jpg)

## コロナ1.6 - 6

[3ds Maxプラグイン](../../../3d-applications/3ds-max/3ds-max.md)を使用すると、[Substance]メニューで[コロナ]を選択して、Substanceテクスチャ入力を使用してコロナマテリアルを自動設定できます。

![](../../../assets/corona.png){width="500px"}

## コロナ7 - 9

Coronaレンダー7以降の場合は、Substance2ノードを選択した状態で「Substanceからコロナへ」を選択すると、コロナ物理マテリアルのネットワークが作成されます。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/corona-physical-material?$png$&jpegSize=200&wid=857)

* **LiftGamaGain**&#x200B;は、Base color出力とBase color入力の間に作成されます。 カラー差の補正にはガンマ値0.455が使用されます。
* **CoronaNormal**&#x200B;は、法線の出力とベースバンプ入力の間、およびCoat normalの出力とクリアコートバンプ入力の間に作成されます。 設定は変更されませんが、ここでは通常の変更を行うことができます。
* **CoronaMix**&#x200B;は、光沢カラー出力と光沢カラー入力の間に作成されます。 ベースレイヤーのミックス量には0が設定され、乗数には2が設定されます。 「ミックス量」の値を調整して、光沢を制御できます。
