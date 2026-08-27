---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/mesh-parts-bleed-between-each-other.html"
breadcrumb-title: ''
description: 名前による一致を使用するか、距離を調整することで、ベイク処理の際にメッシュパーツが相互にににじむのを防ぎます。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Mesh parts bleed between each other
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュパーツ同士のブリード
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# メッシュパーツ同士のブリード

>[!WARNING]
>
> **問題**
> 
> メッシュジオメトリは他のパーツ上にブリードし、アーティファクトを生み出します。
> 
> ![](../../assets/bleed-example.png)

>[!NOTE]
>
> **説明**
> 
> ベイク処理では、ローポリゴンメッシュサーフェスからレイが送信され、ハイポリゴンメッシュに衝突して一致が作成されます。 光線が大きすぎて間違ったジオメトリに当たり、にじみやアーティファクトが生じることがあります。

>[!NOTE]
>
> **解決策**
> 
> この問題を回避するには、いくつかの解決策があります。
> 
> * [名前による一致](../../features/matching-by-name/matching-by-name.md)機能を使用して、メッシュを分離します
> * [ケージ](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)を使用して、レイの距離を制限します。
> * 一般的なパンの設定で、既定のレイ距離を低い値に変更します。
