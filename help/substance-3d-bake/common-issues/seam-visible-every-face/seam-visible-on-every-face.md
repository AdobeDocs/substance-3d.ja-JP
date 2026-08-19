---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/seam-visible-on-every-face.html"
breadcrumb-title: ''
description: UVのラップ解除、スムージング グループ、メッシュ トポロジの問題をチェックして、すべての面に表示されるシームを修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seam visible on every face
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: すべての顔にシームが表示されます
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# すべての顔にシームが表示されます

>[!WARNING]
>
> **問題**
> 
> UV シームが存在しない場合でも、ジオメトリの一部のエッジにシームが表示されます。
> 
> ![](../../assets/seam-every-face.jpg)

>[!NOTE]
>
> **説明**
> 
> [&#x200B; ケージ &#x200B;](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)を使用しない場合、ベイク処理は、ローポリメッシュの頂点法線の方向に光線を起動します。 各頂点法線が分割されている場合（つまり、各面が隣接する面と同じ頂点法線を共有していない場合）、光線はエッジ上で同じ方向に送られません。 エッジの両側の情報が異なるため、分割が発生します。
> 
> この問題は、[このページ &#x200B;](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)で説明しているように、エイリアスによって悪化します。

>[!NOTE]
>
> **解決策**
> 
> ここで可能な解決策は2つだけです。
> 
> * ベイカーにローポリジオメトリから計算させるのではなく、[&#x200B; ケージ &#x200B;](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)を使用してレイ方向を制御します。
> * ローポリメッシュの頂点の法線を結合します（それらをソフト化/共通のスムージンググループを適用）。
