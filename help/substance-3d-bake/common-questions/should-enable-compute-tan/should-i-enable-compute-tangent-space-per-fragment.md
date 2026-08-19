---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-questions/should-i-enable-compute-tangent-space-per-fragment.html"
breadcrumb-title: ''
description: フラグメントごとに接線空間を計算を有効にするタイミングと、それがベイク処理の結果にどのような影響を与えるかを説明します。
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
> 「フラグメントごとに接線空間を計算」という設定は何を意味し、その使用方法は何ですか？

>[!NOTE]
>
> **説明**
> 
> この設定を有効にすると、頂点シェーダーではなくフラグメントシェーダー（ピクセルシェーダーとも呼ばれます）で接線空間計算を実行するようにパン屋に指示します。 つまり、頂点から頂点に補間されるのではなく、ピクセルごとに計算が行われます。 この設定は、テクスチャのエンコード方法を理解するために、法線マップベイカーで使用されます。 また、シェーダによるテクスチャの読み方を知ることもありました。
> 
> このパラメーターを有効または無効にするには、通常、3D ビューポートやレンダリングエンジン（Irayなど）と同期させるためにテクスチャを焼き直す必要があります。

>[!NOTE]
>
> **解決策**
> 
> テクスチャをレンダリングする対象のソフトウェアまたはゲームエンジンによっては、この設定が無効または有効になっている場合があります。
> 
> | *ソフトウェア* | *フラグメントごとの接線空間を計算* |
> | --- | --- |
> | **Unreal Engine 4** | 有効にする |
> | **Unity** | 無効 |
