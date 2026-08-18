---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: パディング、アンチエイリアス、UVレイアウトを調整して、ベイク処理された法線テクスチャの目に見える継ぎ目を除去します。
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
> 法線マップの継ぎ目は、クリーンベイク処理した後でもメッシュのUV境界に表示されます。

>[!NOTE]
>
> **説明**
> 
> 完全にベイク処理した後でも、継ぎ目は表示されます。 その主な理由は、法線がサーフェス情報をテクスチャに近似するためです。 テクスチャの精度が不十分であったり、低ポリゴンジオメトリと高ポリゴンジオメトリの間で十分な精度を得るには補正が必要な場合があります。 その他の状況では、ジオメトリが法線マップを使用してレンダリングされる方法によって、ジオメトリの外観が影響を受ける場合があります。

>[!NOTE]
>
> **解決策**
> 
> 法線マップを使用してシームの強度を低減する方法がいくつかあります。
> 
> * 多くの場合、UVはピクセルに位置揃えされず、エイリアスが発生して継ぎ目が生じます。 詳細については、[このページ](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)を参照してください。
>   * テクスチャ解像度を上げると、この効果を減らすことができます。
>   * このエフェクトを減らすには、UV境界をピクセルに揃えることもできます。
> * シェーダー&#x200B;**品質**&#x200B;設定を上げます。 シェーダの質は、Specular反射の計算方法に影響を与える可能性があります。 回転したUV アイランドの値が小さすぎると、継ぎ目が目立つ場合があります。 詳細については、[このページ](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html)を参照してください。
