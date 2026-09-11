---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-bump-offset-parallax-ue4.html"
breadcrumb-title: ''
description: アンリアルエンジン 4のSubstanceマテリアルでバンプオフセットマッピングを使用すると、深度の錯覚やサーフェスのディテールを作成できます。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Bump Offset (Parallax) - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: バンプオフセット（パララックス）の操作 – UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# バンプオフセット（パララックス）の操作 – UE4

**バンプオフセット**&#x200B;マッピングを使用すると、UV座標をクリエイティブな方法で変更して、表面に深度があるように見せ、オブジェクトの表面からテクスチャをさらに置き換えることができます。これにより、表面に実際よりも多くのディテールがあるように見せます。 この操作方法の例では、バンプオフセットマテリアルエクスプレッションを見つける方法だけでなく、マテリアルでバンプオフセットノードを使用する方法についても説明します。

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/HowTo/BumpOffset/>

Height出力を使用するには、Substance・ファクトリ・インスタンスの出力をダブルクリックしてHeightを作成する必要があります。 デフォルトでは、Heightは有効になっていません。 次に、このHeight出力をマテリアルにドラッグできます。

![](../../../../assets/height-1.png){width="600px"}

バンプオフセットノードを作成し、Heightの赤チャンネルをHeightにプラグインします。 次に、バンプオフセットの座標入力にTexCoordを入力できます。 最後に、バンプオフセットの出力が、すべてのテクスチャのUV入力に接続されます。

![](../../../../assets/bump.png){width="800px"}
