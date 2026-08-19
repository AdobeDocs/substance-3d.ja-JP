---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/is-dithering-applied-to-baked-textures.html"
breadcrumb-title: ''
description: ベイク処理されたテクスチャにディザリングが適用されるかどうか、およびテクスチャの品質に与える影響を理解します。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Is dithering applied to baked textures "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'ベイク処理されたテクスチャにディザリングを適用する '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# 焼き上げたテクスチャにディザリングを適用しますか？

>[!WARNING]
>
> **質問**
> 
> ベーカーはテクスチャ [&#x200B; ディザリング &#x200B;](https://en.wikipedia.org/wiki/Dither)をサポートしていますか。サポートしている場合は、いつ適用されますか？

>[!NOTE]
>
> **説明**
> 
> ディザリングは、例えば8bit法線マップでバンディングを避けるために適用されます。
> 
> ![](../../assets/dither.jpg)

>[!NOTE]
>
> **解決策：Substance Designer**
> 
> ディザリングは、次の状況で自動的に適用されます。
> 
> * Baker出力が8bit テクスチャファイルに保存される場合
> * Baker出力が8bitに設定されたグラフのビットマップノードで使用される場合。

>[!NOTE]
>
> **解決策：Substance Painter**
> 
> ディザリングは、書き出しプロセス中に有効または無効にできるオプションです。 これは、標準、変位、高さの各チャンネル用の8 ビットファイル形式に書き出す場合にのみ適用されます。

>[!NOTE]
>
> **解決策：Substance Automation Toolkit**
> 
> 現時点では、ディザリングはサポートされていません。
