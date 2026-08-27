---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/should-i-enable-compute-tangent-space-per-fragment.html"
breadcrumb-title: ''
description: フラグメントごとに接線空間を計算を有効にする場合と、ベイク処理の結果に与える影響について説明します。
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Should I enable
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 有効にする必要があります
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 1%

---


# 「フラグメントごとに接線空間を計算」を有効にする必要がありますか？

>[!WARNING]
>
> **質問**
> 
> 「フラグメントあたりの接線空間を計算」設定はどのような意味を持ち、どのような用途を持ちますか？

>[!NOTE]
>
> **説明**
> 
> この設定を有効にすると、ベイカーは頂点シェーダの代わりにフラグメントシェーダ（ピクセルシェーダとも呼ばれる）で接線空間の計算を実行します。 つまり、頂点から頂点に補間されるのではなく、ピクセルごとに計算が行われます。 この設定は、テクスチャをエンコードする方法を知るために法線マップベイカーが使用します。 また、シェーダによるテクスチャの読み取り方法も学習しました。
> 
> このパラメータを有効または無効にするには、通常、テクスチャを再ベイク処理して3Dビューポートやレンダリングエンジン（Irayなど）と同期させる必要があります。

>[!NOTE]
>
> **解決策**
> 
> テクスチャのレンダリング先のソフトウェアまたはゲームエンジンに応じて、この設定は無効または有効になります。
> 
> | *ソフトウェア* | *フラグメントごとの接線空間の計算* |
> | --- | --- |
> | **アンリアルエンジン4** | 有効にする |
> | **Unity** | 無効 |
