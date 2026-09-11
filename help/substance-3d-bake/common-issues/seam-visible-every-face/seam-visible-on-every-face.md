---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/seam-visible-on-every-face.html"
breadcrumb-title: ''
description: UVのラップ解除、スムージンググループ、およびメッシュトポロジの問題をチェックして、各面に表示されるシームを修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seam visible on every face
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: すべての面に表示されるシーム
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# すべての面に表示されるシーム

>[!WARNING]
>
> **問題**
> 
> シームは、UVシームが存在しない場合でも、ジオメトリのいくつかのエッジに表示されます。
> 
> ![](../../assets/seam-every-face.jpg)

>[!NOTE]
>
> **説明**
> 
> [ケージ](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)を使用しない場合、ベイク処理プロセスでは、ローポリメッシュの頂点法線方向に光線が発射されます。 各頂点法線が分割されている（各面が隣接する面と同じ頂点法線を共有しない）場合、光線はエッジ上の同じ方向に向きません。 これにより、エッジの両側の情報が異なるために分割されます。
> 
> この問題は、[このページ](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)で説明したように、エイリアスによっても悪化します。

>[!NOTE]
>
> **解決策**
> 
> ここで可能な解決策は2つだけです。
> 
> * [ケージ](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)を使用すると、ベイカーにローポリゴンジオメトリからレイ方向を計算させるのではなく、レイ方向を制御できます。
> * ローポリメッシュの頂点法線をマージします（これらをソフトにします/共通のスムージンググループを適用します）。
