---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/blender/physical-size-in-blender.html"
breadcrumb-title: ''
description: 物理サイズ設定を使用して、Blenderの実際の寸法に基づいてSubstanceマテリアルをスケーリングします。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Physical size in Blender
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ブレンダーでの物理サイズ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# ブレンダーでの物理サイズ

Substanceのマテリアルの物理サイズにより、マテリアルは実際のサイズに基づいてスケールできます。 サイズはDesignerなどのSubstanceアプリケーションで設定され、プラグインパネルの「物理サイズ」セクションに表示されます。

![](../../../assets/blender-physical-size.png)

物理サイズが有効になっている場合、マテリアルは実際のサイズ（センチメートル）に基づいてタイルされます。 マテリアルのタイリングは、オブジェクトのスケールに関係なく同じままです。 この機能は、アドオンパネルで物理サイズシェーダに切り替えることによって有効にできます。 オブジェクトのスケールを調整した後、物理サイズテクスチャを正確にタイリングするには、Ctrl/Cmd + Aキーを押してスケールを適用する必要があります。

## 物理サイズの調整

マッピングノードの値を調整して、物理サイズタイリングをアーティスティックに制御できます。 また、空などのオブジェクトをテクスチャ座標入力に使用して、入力オブジェクトのトランスフォームを使用してテクスチャマッピングを制御します（次の例を参照）。

![](../../../assets/blender-physical-szie-empty.gif)
