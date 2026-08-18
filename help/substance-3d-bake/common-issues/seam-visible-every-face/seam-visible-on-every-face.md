---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/seam-visible-on-every-face.html"
breadcrumb-title: ''
description: UVのアンラップ、スムージンググループ、メッシュトポロジの問題をチェックして、すべての面に表示される継ぎ目を修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seam visible on every face
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: すべての面に表示される継ぎ目
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# すべての面に表示される継ぎ目

>[!WARNING]
>
> **問題**
> 
> UVシームが存在しない場合でも、ジオメトリのいくつかのエッジにシームが表示されます。
> 
> ![](../../assets/seam-every-face.jpg)

>[!NOTE]
>
> **説明**
> 
> [ケージ](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)を使用しない場合、ベイク処理はローポリゴンメッシュの頂点法線の方向に光線を発射します。 各頂点法線が分割されている場合（つまり、各面が隣接する面と同じ頂点法線を共有していない場合）、光線はエッジ上の同じ方向に送信されません。 これにより、エッジの両側の情報が異なるために分割されます。
> 
> この問題は、[このページ](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)で説明したように、エイリアスによっても悪化します。

>[!NOTE]
>
> **解決策**
> 
> ここで可能な解決策は2つだけです。
> 
> * パン屋に低ポリゴンジオメトリからレイ方向を計算させる代わりに、[ケージ](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)を使用してレイ方向を制御します。
> * ローポリゴンメッシュの頂点法線をマージします（これらをソフトにする/共通のスムージンググループを適用する）。
