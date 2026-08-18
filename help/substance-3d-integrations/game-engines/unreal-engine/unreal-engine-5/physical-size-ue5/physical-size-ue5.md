---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/physical-size-ue5.html"
breadcrumb-title: ''
description: Unreal Engine 5で実際の寸法に基づいてSubstanceマテリアルをスケールするには、物理サイズ設定を使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Physical Size - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 物理サイズ- UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# 物理サイズ- UE5

Substanceのマテリアルの物理サイズにより、マテリアルは実際のサイズに基づいてスケールできます。 この値はSubstance Designerで設定され、マテリアルテンプレートシステムを通じてUnrealに読み込まれます。\
親の[Substance\_Triplanar\_テンプレート](../../../../game-engines/unreal-engine/unreal-engine-5/material-template-usage/out-the-box-material-tem/out-of-the-box-material-templates.md)マテリアルには、物理サイズを使用して非現実マテリアルをスケールする方法の例が含まれています。



メッシュ上のアップスケール値に関係なく、マテリアルはワールドで占めるサイズ（センチメートル）に基づいてタイリングされます。 岩石（写真1）の場合、1回の測定で1.8m(180cm)となります。

![](../../../../assets/rock-material-parameters.png)

物理サイズデータを含むSubstanceマテリアルの値は、physicalsizeという名前の既存のマテリアルベクトルパラメータノードにコピーされます。



UE5ではマテリアルにディスプレイスメント値が存在しないため、物理サイズテンプレートは値をX、Y、Xとして三平面マップにコピーします。
