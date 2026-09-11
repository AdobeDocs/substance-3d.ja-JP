---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/renderers/corona.html"
breadcrumb-title: ''
description: 3ds Maxのコロナレンダラで、Specular/光沢度のワークフローと必要なマップを使用してSubstanceマテリアルを行います。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: コロナ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 1%

---


# コロナ

Coronaを使用したレンダリングでは、Substance PainterまたはSubstanceプラグインから書き出したマップを使用できます。 コロナは、1/IORマップでSpecular/光沢ワークフローを使用しています。 次のマップが必要です。

* ディフューズ
* 反射(Specular)
* グロシネス
* 1/IOR （変換済み）

1/IORマップは、Substance DesignerとSubstance Painterの両方で既定のワークフローであるメタリック/粗さワークフローからのみ変換できます。

1. 「コロナ」プリセットを使用して、Substance Painterからマップを書き出します。
1. カスタムSubstanceの場合は、Vrayプリセットに変換されたbasecolor\_メタリック\_nodeを使用してカスタム出力を作成できます。
1. 3ds MaxとCinema 4Dの場合は、レイヤコロナマテリアルを使用して金属と誘電体のマテリアルを処理し、1/IORマップを変換する必要はありません。

## 目次

* [3ds Maxのコロナ](../../renderers/corona/corona-for-3ds-max/corona-for-3ds-max.md)
* [コロナ – Substance Painter](../../renderers/corona/corona-painter/corona-substance-painter.md)
