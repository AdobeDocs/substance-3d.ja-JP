---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/normal-texture-looks-faceted.html"
breadcrumb-title: ''
description: メッシュ法線をスムージングし、スムージンググループ設定を調整することで、通常のテクスチャのファセットの外観を修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal texture looks faceted
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 通常のテクスチャはファセットに見えます
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# 通常のテクスチャはファセットに見えます

>[!WARNING]
>
> **問題**
> 
> 通常のテクスチャはファセットに見えるか、メッシュのすべての面がベイク後に表示されます。
> 
> ![](../../assets/normal-faceted.jpg)

>[!NOTE]
>
> **説明**
> 
> 法線をベイク処理する主な理由は、低いポリメッシュ法線が適切に設定されていないためです。 各面のすべてのエッジはハード エッジで、ハイポリメッシュとのマッチング中にレイ投影がネイボーリング情報を無視し、シームまたは無意識の情報を作成します。 結果はメッシュ上では正常に見えるかもしれませんが、これは後でシェーディングの問題につながる可能性があり、解決する必要があります。

>[!NOTE]
>
> **解決策**
> 
> 主な解決策は、頂点の法線またはローポリメッシュを再構築することです。プロセスの正確な命名は、3D モデリングソフトウェアによって異なります。
> 
> * Maya、Houdiniで&#x200B;**平均法線**&#x200B;を使用します。
> * 3DS Maxで&#x200B;**1つのスムージング グループ**&#x200B;を使用します。
> * Blenderで&#x200B;**滑らかな色合い**&#x200B;を使用します。
> * zBrushから書き出されたメッシュは常にファセットされ、別のソフトウェアでクリーンアップする必要があります。
> 
> これだけでは不十分な場合があります。メッシュの書き出し時に、頂点の法線またはシェーディング情報も設定で保存または生成してください。
