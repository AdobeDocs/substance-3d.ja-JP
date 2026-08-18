---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/modo/working-with-emissive.html"
breadcrumb-title: ''
description: MODOでSubstanceマテリアルの放射プロパティを設定し、発光量とカラー設定を制御します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Emissive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Emissiveの操作
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# Emissiveの操作

## 放射光を使用した作業（明るさの量とカラー）

Substanceには、オプションの放射出力を指定できます。 MODOのLuminous AmountとColorとして使用できます。 放射出力を有効にすると、「明るさ量」エフェクトに設定されます。 デフォルトでは、このチャンネルはテクスチャイメージ静止タブの下でリニアとして解釈されます。\
シェーダツリーでテクスチャを右クリックし、 duplicateを選択します。 次に、複製した発光テクスチャを「明るいカラー」効果に設定します。 次に、「明度」エフェクトを制御するテクスチャの高い値と低い値を変更して、値をさらに強調します。

>[!NOTE]
>
> テクスチャを「明るいカラー」に設定するには、「静止画イメージ」タブで変換を「sRGB」に設定する必要があります。

ブルーム効果を得るには、レンダーパネルでブルームを有効にし、しきい値と半径を設定する必要があります。

![](../../../assets/bloom.png)

UnrealおよびUnityマテリアルの場合、Emissive出力はマテリアルによって処理されます。\
Unreal = Unreal Emissive\
Unity = Unity Emission

Image Stillタブで、Unreal EmissiveとUnity EmissionのテクスチャをLinearからsRGBに変更する必要があります。
