---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/getting-started/software-interface/substance-3d-painter.html"
breadcrumb-title: ''
description: Substance 3D Painterのベイキングウィンドウにアクセスして使用し、テクスチャのメッシュマップを生成する方法を説明します。
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Software Interface > Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 2%

---


# Substance 3D Painter

![](../../../assets/sp-baking-button-access.png)

ベーキングウィンドウには、[&#x200B; テクスチャセット設定](https://experienceleague.adobe.com/ja/docs/substance-3d-painter/using/interface/texture-set/texture-set-settings)からアクセスできます。 「**メッシュマップをベイク**」という名前のボタンをクリックして、現在のプロジェクトのベイクウィンドウを開きます。

## 概要

![](../../../assets/sp-ui-overview.png){width="400px"}

ベーキングウィンドウは3つの主要なコンポーネントに分かれています。

### ベイカーリスト

![](https://helpx-prod.scene7.com/is/image/HelpxProd/sp-baking-list?$png$&jpegSize=100&wid=150)

ウィンドウの左上には、いくつかのボタンがあります。

これらのボタンの横にはチェックボックスがあり、チェックを入れると、このベイク処理が有効になります。 名前の横にアイコンが表示されているボタンは、ハイポリメッシュが必要なボタンを示します。 このアイコンは、ハイポリが利用可能になった場合に警告を表示します。

| *ボタン* | *説明* |
| --- | --- |
| **共通** | パラメーター表示を[共通パラメーター](../../../bakers-settings/common-parameters/common-parameters.md)に変更します。 |
| **標準** | パラメーター表示を[標準パラメーター](../../../bakers-settings/normal-map-from-mesh/normal-map-from-mesh.md)に変更します。 |
| **ワールド空間法線** | パラメーター表示を[&#x200B; ワールド空間法線パラメーター](../../../bakers-settings/world-space-normals/world-space-normals.md)に変更します。 |
| **ID** | パラメーター表示を[&#x200B; カラーパラメーター](../../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)に変更します。 |
| **アンビエントオクルージョン** | パラメーター表示を[&#x200B; アンビエントオクルージョンパラメーター](../../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)に変更します。 |
| **曲率** | パラメーター表示を[曲率パラメーター](../../../bakers-settings/curvature/curvature.md)に変更します。 |
| **位置** | パラメーター表示を[位置パラメーター](../../../bakers-settings/position/position.md)に変更します。 |
| **厚さ** | パラメーター表示を[厚みパラメーター](../../../bakers-settings/thickness-map-from-mesh/thickness-map-from-mesh.md)に変更します。 |
| **高さ** | パラメーター表示を[高さパラメーター](../../../bakers-settings/height-map-from-mesh/height-map-from-mesh.md)に変更します。 |
| **ベント法線** | パラメーター表示を[&#x200B; ベント法線パラメーター](../../../bakers-settings/bent-normals-from-mesh/bent-normals-from-mesh.md)に変更します。 |
| **不透明度** | パラメーター表示を[不透明度パラメーター](../../../bakers-settings/opacity-mask-from-mesh/opacity-mask-from-mesh.md)に変更します。 |

### パラメーター

![](../../../assets/sp-baking-params.png)

ウィンドウのこの部分には、様々なベイク設定が表示されます。 その内容は、現在選択されているベイカーまたは共通のパラメーターによって異なる場合があります。

パン屋の設定について詳しくは、[&#x200B; パン屋の設定](../../../bakers-settings/bakers-settings.md)を参照してください。

### ヘルプメッセージ

![](../../../assets/sp-baking-help.png){width="500px"}

ウィンドウのこの部分には、設定に関連するさまざまなツールヒントとヘルプメッセージが表示されます。 設定の上にマウスを移動して、ツールチップをここに読み込みます。
