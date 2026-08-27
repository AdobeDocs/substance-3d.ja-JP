---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: パディング、アンチエイリアス、UVレイアウトを調整して、ベイクした標準テクスチャのシームを表示しないようにすることができます。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seams are visible after baking a normal texture
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 通常のテクスチャをベイク処理した後に継ぎ目が表示される
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 通常のテクスチャをベイク処理した後に継ぎ目が表示される

>[!WARNING]
>
> **問題**
> 
> シームは、メッシュのUV境界に、清潔なベイクをした後でも見ることができます。

>[!NOTE]
>
> **説明**
> 
> 完璧にベイクした後でも、シームは見ることができます。 その主な理由は、通常のサーフェス情報をテクスチャに近似することです。 テクスチャの精度が不十分であったり、低ポリゴンジオメトリと高ポリゴンジオメトリの間で十分に正確になるように補正しすぎたりすることがあります。 他の状況では、ジオメトリが法線マップによってレンダリングされる方法によって、ジオメトリの外観が変わる場合があります。

>[!NOTE]
>
> **解決策**
> 
> 法線マップによるシームの強さを減らすために、いくつかの可能な解決策を試すことができます。
> 
> * 多くの場合、UVはピクセルに位置揃えされず、エイリアスが発生してシームが発生します。 詳細については、[このページ](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)を参照してください。
>   * テクスチャの解像度を上げると、この効果を減らすことができます。
>   * この効果を減らすには、UVの境界線をピクセルに揃えることもできます。
> * シェーダーの&#x200B;**品質**&#x200B;設定を上げます。 シェーダーの質は、Specular反射の計算方法に影響を与える可能性があります。 回転するUV アイランドの数が少なすぎると、シームが見えることがあります。 詳細については、[このページ](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html)を参照してください。
