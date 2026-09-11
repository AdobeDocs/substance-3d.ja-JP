---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.html"
breadcrumb-title: ''
description: 「名前で一致」がAmbient occlusionとThicknessのベイカーで機能しない理由を理解し、代替案を見つけてください。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Why is Matching by Name not working with Ambient OcclusionThickness "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: '名前によるマッチングがAmbient OcclusionThicknessで機能しない理由 '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '109'
ht-degree: 0%

---


# 名前で一致がAmbient occlusion/Thicknessで機能しない理由

>[!WARNING]
>
> **質問**
> 
> [共通パラメーター](../../bakers-settings/common-parameters/common-parameters.md)の[名前による一致](../../features/matching-by-name/matching-by-name.md)を有効にして、ローポリゴンとハイポリゴンのメッシューをフィルターして並べ替えましたが、Ambient occlusionベイカーで無視されるのはなぜですか？

>[!NOTE]
>
> **説明**
> 
> ambient occlusion、Thickness、およびBent normalsベイカーは、テクスチャを計算するとセカンダリレイを起動します。 これらのレイには、独自の[名前による一致]設定があります。

>[!NOTE]
>
> **解決策：Substance Painter**
> 
> 解決策：ベイカーパラメーターで、セカンダリレイの名前による一致フィルタリングを有効にします。
