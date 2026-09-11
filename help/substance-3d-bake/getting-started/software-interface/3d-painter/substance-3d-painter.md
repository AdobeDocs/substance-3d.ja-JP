---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/getting-started/software-interface/substance-3d-painter.html"
breadcrumb-title: ''
description: Substance 3D Painterのベイク処理ウィンドウにアクセスして使用し、テクスチャ用のメッシュマップを生成する方法について説明します。
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

ベイクウィンドウには、[テクスチャセットの設定](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/interface/texture-set/texture-set-settings)からアクセスできます。 「**メッシュマップのベイク**」という名前のボタンをクリックして、現在のプロジェクトのベイクウィンドウを開きます。

## 概要

![](../../../assets/sp-ui-overview.png){width="400px"}

ベイクウィンドウは、3つの主要コンポーネントに分かれています。

### ベイカー一覧

![](https://helpx-prod.scene7.com/is/image/HelpxProd/sp-baking-list?$png$&jpegSize=100&wid=150)

ウィンドウの左上には、いくつかのボタンがあります。

これらのボタンの横にあるチェックボックスをオンにすると、このベイクがベイクプロセスで有効になります。 名前の横にアイコンが付いているボタンは、high-poly メッシュが必要なボタンを示します。 このアイコンは、ハイポリゴンが使用可能になった場合に警告を表示します。

| *ボタン* | *説明* |
| --- | --- |
| **全般** | パラメータービューを[共通パラメーター](../../../bakers-settings/common-parameters/common-parameters.md)に変更します。 |
| **標準** | パラメータービューを[通常のパラメーター](../../../bakers-settings/normal-map-from-mesh/normal-map-from-mesh.md)に変更します。 |
| **ワールド空間標準** | パラメータービューを[ワールド空間法線パラメーター](../../../bakers-settings/world-space-normals/world-space-normals.md)に変更します。 |
| **ID** | パラメータービューを[カラーパラメーター](../../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)に変更します。 |
| **環境オクルージョン** | パラメータービューを[Ambient occlusionパラメーター](../../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)に変更します。 |
| **曲線** | パラメータービューを[曲率パラメーター](../../../bakers-settings/curvature/curvature.md)に変更します。 |
| **位置** | パラメータービューを[位置パラメーター](../../../bakers-settings/position/position.md)に変更します。 |
| **Thickness** | パラメータービューを[Thicknessパラメーター](../../../bakers-settings/thickness-map-from-mesh/thickness-map-from-mesh.md)に変更します。 |
| **Height** | パラメータービューを[Heightパラメーター](../../../bakers-settings/height-map-from-mesh/height-map-from-mesh.md)に変更します。 |
| **Bent normals** | パラメータービューを[Bent normalsパラメーター](../../../bakers-settings/bent-normals-from-mesh/bent-normals-from-mesh.md)に変更します。 |
| **不透明度** | パラメータービューを[不透明度パラメーター](../../../bakers-settings/opacity-mask-from-mesh/opacity-mask-from-mesh.md)に変更します。 |

### パラメーター

![](../../../assets/sp-baking-params.png)

ウィンドウのこの部分には、さまざまなベイク設定が表示されます。 この内容は、現在選択されているベイカーまたは共通パラメーターによって異なる場合があります。

ベイカーの設定の詳細については、[ベイカーの設定](../../../bakers-settings/bakers-settings.md)を参照してください。

### ヘルプメッセージ

![](../../../assets/sp-baking-help.png){width="500px"}

ウィンドウのこの部分には、設定に関連するさまざまなツールチップとヘルプメッセージが表示されます。 設定の上にマウスを移動すると、ここにツールチップが表示されます。
