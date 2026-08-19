---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature-from-mesh-deprecated.html"
breadcrumb-title: ''
description: Mesh ベイカーから非推奨の曲率を参照します。 代わりに、更新したメッシュベイカーの曲率を使用します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature from Mesh (deprecated)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからの曲率（非推奨）
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---


# メッシュからの曲率（非推奨）

メッシュベイカーからの曲率は、高ポリメッシュからの曲率テクスチャを生成します。 ベース [曲率](../../bakers-settings/curvature/curvature.md) ベイカーよりも遅くなりますが、より正確な結果が得られます。

**次の場所で利用できます：**

* Substance Designer
* Substance Automation Toolkit

>[!NOTE]
>
> Substance Designer 2019.3以降、このベイカーは非推奨（廃止予定）となり、代わりにメッシュ [&#128279;](../../bakers-settings/curvature-from-mesh/curvature-from-mesh.md) ベイカーの新しい曲率を使用することをお勧めします。

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **強度** | 曲率のディテールの強さです。 **ソフト飽和度**&#x200B;が有効になっている場合、このパラメーターは無効になります。 |
| **ソフト** **彩度** | 有効にすると、曲率の詳細がソフトになります。 |
| **範囲を最大化** | 有効にすると、曲率のディテールがテクスチャ範囲の容量の中に収まります。 つまり、非常に強い値は最大値として定義され、他のすべての値はその極端に従って拡大・縮小されます。 |
