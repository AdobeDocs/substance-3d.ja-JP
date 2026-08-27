---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/is-dithering-applied-to-baked-textures.html"
breadcrumb-title: ''
description: ディザリングがベイクされたテクスチャに適用されるかどうか、およびデータがテクスチャの質にどのような影響を与えるかを理解します。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Is dithering applied to baked textures "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'ベイクされたテクスチャに適用されるディザリング '
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
> ベイカーはテクスチャ [ディザリング](https://en.wikipedia.org/wiki/Dither)をサポートしていますか。サポートしている場合、いつ適用されますか？

>[!NOTE]
>
> **説明**
> 
> ディザリングは、例えば8ビット法線マップでのバンディングを避けるために適用されます。
> 
> ![](../../assets/dither.jpg)

>[!NOTE]
>
> **解決策：Substance Designer**
> 
> ディザリングは、次の状況で自動的に適用されます。
> 
> * ベイカー出力が8ビットテクスチャファイルに保存される場合
> * ベイカー出力が8ビットにセットされたグラフのビットマップノードで使用される場合。

>[!NOTE]
>
> **解決策：Substance Painter**
> 
> ディザリングは、書き出しプロセス中に有効または無効にできるオプションです。 これは、通常、ディスプレイスメント、Heightチャンネル用に8ビットファイル形式に書き出す場合にのみ適用されます。

>[!NOTE]
>
> **ソリューション: Substance自動処理ツールキット**
> 
> ディザリングは現在サポートされていません。
