---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/normal-texture-looks-faceted.html"
breadcrumb-title: ''
description: 法線テクスチャのファセットの外観を修正するには、メッシュ法線をスムージングし、スムージンググループの設定を調整します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal texture looks faceted
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 通常のテクスチャはファセットされています
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# 通常のテクスチャはファセットされています

>[!WARNING]
>
> **問題**
> 
> 標準テクスチャはファセットのように見えるか、ベイク後にメッシュのすべての面が表示されます。
> 
> ![](../../assets/normal-faceted.jpg)

>[!NOTE]
>
> **説明**
> 
> 法線をベイクするとこの結果が得られる主な理由は、ローポリメッシュ法線が正しく設定されていないためです。 各面の各エッジはハードエッジであり、高ポリゴンメッシュとのマッチング中にレイ投影が近傍情報を無視し、シームまたは無意識情報を生成します。 結果はメッシュ上では問題なく表示される場合がありますが、これは後でシェーディングの問題につながる可能性があり、解決する必要があります。

>[!NOTE]
>
> **解決策**
> 
> 主な解決策は、頂点法線またはローポリメッシュを再処理することです。プロセスの正確な名前は、3Dモデリングソフトウェアによって異なります。
> 
> * Maya、Houdiniでは&#x200B;**平均法線**&#x200B;を使用します。
> * 3DS Maxで&#x200B;**1つのスムージンググループ**&#x200B;を使用します。
> * ブレンダーで&#x200B;**スムーズシェード**&#x200B;を使用します。
> * zBrushから書き出されたメッシュは常にファセットされ、別のソフトウェアでクリーンアップされます。
> 
> メッシュを書き出す際には、頂点の法線またはシェーディング情報も保存/生成してください。
