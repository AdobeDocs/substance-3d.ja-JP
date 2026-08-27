---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/modo/working-with-emissive.html"
breadcrumb-title: ''
description: MODOのマテリアルのemissiveプロパティを設定し、明るさの値と色の設定を制御します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Emissive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: emissiveの操作
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# emissiveの操作

## emissiveの操作（明度とカラー）

Substanceには、オプションのemissive出力を指定できます。 MODOのLuminous AmountとColorとして使用できます。 emissive出力を有効にすると、「明るさ量」エフェクトに設定されます。 デフォルトでは、このチャンネルは「テクスチャ画像静止画」タブではリニアと解釈されます。\
シェーダーツリーでテクスチャを右クリックし、[複製]を選択します。 次に、複製したテクスチャに「明るいカラー」エフェクトを適用します。 次に、「明度」エフェクトを制御するテクスチャの高い値と低い値を変更して、値をさらに強調します。

>[!NOTE]
>
> テクスチャセットを「明るいカラー」にするには、「静止画」タブで変換を「sRGB」に設定する必要があります。

ブルーム効果を得るには、レンダーパネルでブルームを有効にし、しきい値と半径を設定する必要があります。

![](../../../assets/bloom.png)

UnrealおよびUnity マテリアルの場合、Emissive出力はマテリアルによって処理されます。\
Unreal = Unreal Emissive\
Unity = Unity Emission

Image StillタブでUnreal EmissiveとUnity EmissionのテクスチャをLinearからsRGBに変更する必要があります。
