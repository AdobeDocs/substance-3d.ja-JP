---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature-from-mesh-deprecated.html"
breadcrumb-title: ''
description: ベイカーの非推奨曲率のリファレンス。 代わりに、ベイカーの更新された曲率を使用してください。
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

メッシュベイカーの曲率は、ハイポリメッシュから曲率テクスチャを生成します。 ベースの[曲率](../../bakers-settings/curvature/curvature.md)ベイカーよりも低速ですが、より正確な結果が得られます。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット

>[!NOTE]
>
> Substance Designer 2019.3以降、このベイカーは非推奨となり、代わりにメッシュ[&#128279;](../../bakers-settings/curvature-from-mesh/curvature-from-mesh.md) ベイカーの新しい曲率を使用することをお勧めします。

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **適用度** | 曲率のディテールの強度を指定します。 **ソフト彩度**&#x200B;が有効になっている場合、このパラメーターは無効です。 |
| **ソフト** **彩度** | 有効にすると、曲率のディテールがソフトになります。 |
| **範囲を最大化** | 有効にすると、曲率の詳細がテクスチャ範囲のキャパシティ内に収まります。 つまり、非常に強い値が最大値として定義され、その他のすべての値はその最大値に従ってスケールされます。 |
