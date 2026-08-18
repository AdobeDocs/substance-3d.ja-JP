---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/normal-texture-looks-faceted.html"
breadcrumb-title: ''
description: メッシュ法線をスムージングし、スムージンググループ設定を調整することで、法線テクスチャのファセットされた外観を修正します。
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
> 法線テクスチャがファセットのように見えるか、ベイク処理後にメッシュのすべての面が表示されます。
> 
> ![](../../assets/normal-faceted.jpg)

>[!NOTE]
>
> **説明**
> 
> 法線をベイク処理するとこの結果が生成される主な理由は、ローポリゴンメッシュ法線が正しく設定されていないためです。 各面のすべてのエッジはハードエッジであり、高ポリゴンメッシュとのマッチング中にレイプロジェクションが近接情報を無視し、シームまたは無意識の情報を作成します。 結果はメッシュ上では正常に見える場合がありますが、これは後でシェーディングの問題につながる可能性があり、解決する必要があります。

>[!NOTE]
>
> **解決策**
> 
> 主な解決策は、頂点法線またはローポリゴンメッシュを再処理することです。プロセスの正確な名前は、3Dモデリングソフトウェアによって異なります。
> 
> * Maya、Houdiniでは&#x200B;**平均法線**&#x200B;を使用します。
> * 3DS Maxで&#x200B;**1つのスムージンググループ**&#x200B;を使用します。
> * ブレンダーで&#x200B;**スムーズシェード**&#x200B;を使用します。
> * zBrushからエクスポートされたメッシュは常にファセットされ、別のソフトウェアでクリーンアップする必要があります。
> 
> メッシュを書き出す際には、頂点法線またはシェーディング情報も保存/生成してください。
