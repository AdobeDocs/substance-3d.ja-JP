---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/tiling-substance-ue5.html"
breadcrumb-title: ''
description: テクスチャ座標ノードとスカラーパラメータをマテリアルに追加して、Unreal Engine 5のSubstanceテクスチャをタイリングします。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Tiling Substance - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: タイルSubstance- UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '78'
ht-degree: 0%

---


# タイルSubstance- UE5

Substanceテクスチャをタイリングするには、テクスチャ座標ノードを追加し、これをスカラーパラメータで乗算する必要があります。

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/ExpressionReference/Coordinates/#texturecoordinate>

UタイルとVタイルの両方のパラメータを作成するには、 Append Vectorを使用して、これをTexCoordで乗算します。 これにより、UタイルとVタイルの量を個別に設定できます。

![](../../../../assets/tiling-3.png){width="800px"}
