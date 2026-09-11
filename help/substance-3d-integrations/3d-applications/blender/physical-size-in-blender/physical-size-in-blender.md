---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/blender/physical-size-in-blender.html"
breadcrumb-title: ''
description: 物理サイズ設定を使用して、Blenderの実際の寸法に基づいてSubstanceマテリアルを拡大・縮小します。
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

マテリアルの物理サイズを使用すると、マテリアルを実際のサイズに基づいて拡大・縮小できます。 サイズはDesignerなどのSubstanceアプリケーションで設定され、プラグインパネルの「物理サイズ」セクションに表示されます。

![](../../../assets/blender-physical-size.png)

物理サイズが有効になっている場合、マテリアルは実際のサイズ（センチメートル）に基づいてタイルされます。 タイリングは、オブジェクトの尺度に関係なく同じままです。 この機能は、アドオンパネルのシェーダーに切り替えることによって有効にできます。 オブジェクトの拡大・縮小を調整した後、Ctrl/Cmd+Aキーを押して拡大・縮小を適用し、テクスチャを正確に並べて表示します。

## 物理サイズの調整

マッピングノードの値は、物理サイズのタイリングをアーティスティックにコントロールするために調整できます。 また、空などのオブジェクトをテクスチャ座標入力に使用して、入力オブジェクトの変換を使用してテクスチャマッピングを制御することができます（次の例を参照）。

![](../../../assets/blender-physical-szie-empty.gif)
