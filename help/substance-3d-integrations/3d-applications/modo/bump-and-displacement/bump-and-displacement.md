---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/modo/bump-and-displacement.html"
breadcrumb-title: ''
description: MODOのSubstanceマテリアルのバンプマップとディスプレイスメントマップを使用して、モデルにサーフェスの詳細と深度を加えます。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Bump and Displacement
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: バンプとディスプレイスメント
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---


# バンプとディスプレイスメント

バンプとディスプレイスメントの操作

Substanceには、オプションのHeight出力を指定できます。 これをディスプレイスメントまたはバンプとして使用できます。 Heightを有効にすると、バンプテクスチャ効果に設定されます。 Unityの場合はUnity Bumpに設定され、UnrealはUnreal Bumpになります。 次に、Substance項目のマテリアルを選択し、それに応じてバンプの振幅を設定します。 Heightをディスプレイスメントとして使用する場合は、マテリアルレイヤー効果をサーフェスシェーディング/ディスプレイスメントに変更できます。 次に、[マテリアル参照]で、適切な[ディスプレイスメント距離]を設定します。

![](../../../assets/bump-1.png)

この例では、Unrealマテリアルを使用しましたが、Unreal Bump Layer Effectをディスプレイスメントに変更しました。 次に、Substance項目マテリアルで、ディスプレイスメントの距離を設定し、それに応じてレンダリング再分割レベルを設定します。

![](../../../assets/dis.png)
