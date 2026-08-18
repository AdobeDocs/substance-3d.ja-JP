---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/is-dithering-applied-to-baked-textures.html"
breadcrumb-title: ''
description: ベイクドテクスチャにディザリングを適用するかどうか、およびディザリングがテクスチャ品質にどのように影響するかを理解します。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Is dithering applied to baked textures "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'ベイクドテクスチャに適用されるディザ '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# ベイクドテクスチャにディザを適用しますか？

>[!WARNING]
>
> **質問**
> 
> ベーカーはテクスチャ[ディザ処理](https://en.wikipedia.org/wiki/Dither)をサポートしていますか。サポートしている場合、いつ適用されますか？

>[!NOTE]
>
> **説明**
> 
> ディザ処理は、例えば8ビットの法線マップでバンディングが起こらないように適用されます。
> 
> ![](../../assets/dither.jpg)

>[!NOTE]
>
> **解決策：Substance Designer**
> 
> 次の状況では、ディザリングが自動的に適用されます。
> 
> * ベイカー出力が8ビットテクスチャファイルに保存される場合
> * Baker出力を8ビットに設定されたグラフのビットマップノードで使用する場合。

>[!NOTE]
>
> **解決策：Substance Painter**
> 
> ディザリングは、書き出し処理中に有効または無効にできるオプションです。 これは、通常、ディスプレイスメント、Heightチャンネル用に8ビットファイル形式に書き出す場合にのみ適用されます。

>[!NOTE]
>
> **ソリューション: Substance自動処理ツールキット**
> 
> 現在、ディザリングはサポートされていません。
