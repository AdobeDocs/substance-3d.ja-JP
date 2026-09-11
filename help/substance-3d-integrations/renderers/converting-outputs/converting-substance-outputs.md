---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/renderers/converting-substance-outputs.html"
breadcrumb-title: ''
description: 様々なレンダラー要件やワークフローに合わせてマテリアル出力を変換する方法について説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Converting Substance outputs
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance出力の変換
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---


# Substance出力の変換

## Substance Painter

変換されたマップをSubstance Painterから書き出すことができます。 幅広いレンダリングプリセットがサポートされており、プリセットを選択するだけでマップの種類が変換されます。 （変換は金属/粗いワークフローに基づきます）。

![](../../assets/convertpainter.png){width="800px"}

## Substanceプラグイン

Substanceプラグインは、出力を生成し、特定のワークフロー用のマテリアルを自動的に作成します。 ただし、DCCアプリケーションおよびサードパーティレンダラーでは、メタリック出力/ラフ出力を手動で変換する必要がある場合があります。 次の統合は自動レンダリングワークフローをサポートしており、必要に応じて任意のマップタイプを適切に変換します。

* [MayaのSubstance](../../3d-applications/maya/using-workflows/using-workflows.md)
* [3ds MaxのSubstance](../../3d-applications/3ds-max/3ds-max.md)

## カスタムSubstance

カスタムSubstanceを作成している場合は、VrayやCoronaなどのレンダラーに必要な出力を作成できます。 メタリック/ラフネス変換ノード（ライブラリ/PBRユーティリティ）を使用すると、base color、ラフネス、メタリックマップを特定のレンダラーに簡単に変換できます。

![](../../assets/convert-designer.png){width="600px"}
