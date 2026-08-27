---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/physical-size-ue5.html"
breadcrumb-title: ''
description: アンリアルエンジン 5では、物理サイズマテリアルを使用して、実寸に基づいてSubstanceの設定をスケールします。
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
親の[Substance\_Triplanar\_テンプレート](../../../../game-engines/unreal-engine/unreal-engine-5/material-template-usage/out-the-box-material-tem/out-of-the-box-material-templates.md)マテリアルには、非現実マテリアルのスケールに物理サイズを使用する方法の例が含まれています。



メッシュの拡大の値に関係なく、マテリアルは実際のサイズ（センチメートル）に基づいてタイリングされます。 岩石マテリアル（写真1）の場合、これは各測定単位で1.8m(180cm)です。

![](../../../../assets/rock-material-parameters.png)

物理サイズデータを含むSubstanceマテリアルの値は、physicalsizeという名前の既存のマテリアルベクターパラメーターノードにコピーされます。



UE5のマテリアルにディスプレイスメント値がないので、物理サイズテンプレートは、その値をX、Y、Xとして三平面マップにコピーする。
