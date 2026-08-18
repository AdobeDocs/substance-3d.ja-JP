---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/renderers.html"
breadcrumb-title: ''
description: 3Dワークフローで、Arnold、V-Ray、Redshiftなどの主要なレンダラーを使用したSubstanceマテリアルを使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: レンダラー
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 1%

---


# レンダラー

[Substance Source](https://source.substance3d.com/)で提供されるSubstanceマテリアルには、物理ベースのシェーダーの出力が含まれており、[メタリック/粗さ（既定のワークフロー）とSpecular/光沢ワークフロー](https://academy.substance3d.com/courses/pbrguides)の両方がサポートされています。 レンダラーマテリアルがサポートするワークフローを理解することが重要です。 レンダラーによっては、Substanceマテリアル出力を直接使用できる場合や、出力テクスチャを変換する必要がある場合があります。 substance shareからダウンロードしたカスタムSubstanceマテリアルまたはマテリアルには、特定のレンダラーに必要な適切な出力が含まれていない場合があります。

![](../assets/outputs.png){width="200px"}

例えば、ArnoldまたはVray Nextでは、メタリック/ラフネス出力を直接使用できます。 ただし、RendermanのpxrSurfaceでは、ベースカラー/メタリック出力を拡散反射光およびSpecular面の色に変換する必要があります。 レンダラーがサポートされている場合は、Substance統合プラグインによってこれらの変換が自動的に処理されます。

Substance Painterを使用すると、特定のレンダラーに必要な適切なマップの種類を作成する[出力テンプレート](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/export/export-window/export-window)を選択できます。 レンダラーがデフォルトでサポートされていない場合は、カスタム出力テンプレートを作成することもできます。

**出力テンプレート**

![](../assets/output-template.png){width="500px"}

## レンダラーガイド

* [Substance出力の変換](../renderers/converting-outputs/converting-substance-outputs.md)
* [カラーマネジメント](../renderers/color-management/color-management.md)
* [アーノルド](../renderers/arnold/arnold.md)
* [Vray](../renderers/vray/vray.md)
* [Renderman](../renderers/renderman/renderman.md)
* [Redshift](../renderers/redshift/redshift.md)
* [Maxwell](../renderers/maxwell/maxwell.md)
* [コロナ](../renderers/corona/corona.md)
* [オクタン](../renderers/octane/octane.md)
* [Keyshot](../renderers/keyshot/keyshot.md)
* [テア](../renderers/thea/thea.md)
* [マーベリック](../renderers/maverick/maverick.md)
* [Toolbag](../renderers/toolbag/toolbag.md)
* [サイクルとイベント](../renderers/cycles-and-eevee/cycles-and-eevee.md)
