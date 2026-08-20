---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: パディング、アンチエイリアス、UV レイアウトを調整することで、ベイク処理された通常テクスチャの目に見えるシームを除去します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seams are visible after baking a normal texture
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 通常のテクスチャをベイク処理すると、シームが表示されます
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# 通常のテクスチャをベイク処理すると、シームが表示されます

>[!WARNING]
>
> **問題**
> 
> 法線マップのシームは、クリーン ベイクの後でもメッシュのUV境界に表示されます。

>[!NOTE]
>
> **説明**
> 
> 完璧な焼き付けの後でも、縫い目は依然として見ることができます。 主な理由は、通常の近似表面情報がテクスチャに含まれることです。 テクスチャに精度が欠けている場合や、低いポリゴンと高いポリゴンのジオメトリの間に精度を十分に確保するために補正しすぎている場合があります。 他の状況では、ジオメトリを法線マップでレンダリングする方法は、見た目の良さに影響します。

>[!NOTE]
>
> **解決策**
> 
> いくつかの可能な解決策は、通常のマップでシームの強度を減らすために試すことができます。
> 
> * 多くの場合、UVはピクセルに整列していないため、エイリアシングが発生し、シームが生成されます。 詳しくは、[このページ &#x200B;](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)を参照してください。
>   * テクスチャの解像度を上げることで、この効果を減らすことができます。
>   * UV境界をピクセルに整列させることも、この効果を減らすもう1つの方法です。
> * シェーダー&#x200B;**品質**&#x200B;設定を上げます。 シェーダの品質は、スペキュラ反射の計算方法に影響を与える可能性があります。 一部のUV島が回転していて、このパラメーターが低すぎる場合、目に見える継ぎ目を生成できます。 詳しくは、[このページ &#x200B;](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html)を参照してください。
