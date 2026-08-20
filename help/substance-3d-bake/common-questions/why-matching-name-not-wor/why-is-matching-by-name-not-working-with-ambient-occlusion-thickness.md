---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-questions/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.html"
breadcrumb-title: ''
description: 名前によるマッチングがアンビエントオクルージョンベイカーや厚みベイカーで機能しない理由を理解し、代替案を見つけます。
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


# 名前によるマッチングがAmbient Occlusion/Thicknessで機能しないのはなぜですか？

>[!WARNING]
>
> **質問**
> 
> [共通パラメーター](../../bakers-settings/common-parameters/common-parameters.md)で[名前で一致](../../features/matching-by-name/matching-by-name.md)を有効にして、ローポリメッシュとハイポリメッシュをフィルタリングおよび並べ替えましたが、Ambient Occlusion ベイカーが無視するのはなぜですか？

>[!NOTE]
>
> **説明**
> 
> Ambient Occlusion、Thickness、Bent Normals ベイカーは、テクスチャを計算するときに二次光線を起動します。 これらのレイには、「名前で一致」の設定があります。

>[!NOTE]
>
> **解決策：Substance Painter**
> 
> 解決策：ベーカーパラメーターのセカンダリレイの名前によるマッチングを有効にします。
