---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/mesh-parts-bleed-between-each-other.html"
breadcrumb-title: ''
description: 「名前で一致」または「距離を調整」を使用して、焼き込み中にメッシュのパーツが互いにブリードするのを防ぎます。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Mesh parts bleed between each other
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュ パーツが互いにブリードします
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# メッシュ パーツが互いにブリードします

>[!WARNING]
>
> **問題**
> 
> 他のパーツ上のメッシュ ジオメトリ ブリードとアーティファクトの作成
> 
> ![](../../assets/bleed-example.png)

>[!NOTE]
>
> **説明**
> 
> ベイク処理では、ローポリメッシュのサーフェスから光線を送信して、ハイポリメッシュに当たり、一致を作成します。 光線が行き過ぎて間違ったジオメトリに当たり、出血やアーティファクトが発生することがあります。

>[!NOTE]
>
> **解決策**
> 
> この問題を回避するには、いくつかの解決策があります。
> 
> * [名前で一致](../../features/matching-by-name/matching-by-name.md)機能を使用して、メッシュを分離します
> * 光線の距離を制限するには、[&#x200B; ケージ &#x200B;](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html)を使用します。
> * 共通のベイカー設定のデフォルトのレイ距離を低い値に変更します。
