---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5.html"
breadcrumb-title: ''
description: アンリアルエンジン 5でマテリアルテンプレートを作成し、使用して、Substance出力ノードをマテリアル入力に接続する方法を定義します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: マテリアルテンプレートの使用方法 – UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# マテリアルテンプレートの使用方法 – UE5

マテリアルテンプレートを使用すると、サブスタンスのベースマテリアルを作成して、それらの出力ノードをマテリアルの入力に接続するためのテンプレートとして使用できます。\
マテリアル入力と同じ名前と種類を共有する出力が自動的に使用されます。 この親マテリアルの例には「baseColor」テクスチャサンプルノードがあります。このノードは、Substanceに「baseColor」という名前のテクスチャ出力がある場合に塗りつぶされます。\
![](../../../../assets/parent-material-sample.png)

Substance出力では、テクスチャ、1つの浮動小数点またはintスカラー値、およびベクトル(2 ～ 4)値の更新がサポートされています。 floatまたはint出力を実行時に使用するには、constantMaterialInstances （エディタで生成されたすべてのマテリアル）が実行時にスカラー値を変更できないように、グラフからdynamicMaterialInstanceを取得する必要があります。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/scalar-value?$png$&jpegSize=100&wid=245)

Substance グラフインスタンスは、作成時に関連するすべての出力値の入力を試みます。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-04-01-at-4-38-31-pm?$png$&jpegSize=200&wid=1076)
