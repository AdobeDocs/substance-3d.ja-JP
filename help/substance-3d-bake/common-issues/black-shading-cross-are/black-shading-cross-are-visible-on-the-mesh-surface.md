---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/black-shading-cross-are-visible-on-the-mesh-surface.html"
breadcrumb-title: ''
description: 接線空間と法線の計算を修正することで、メッシュ サーフェスに表示される黒いシェーディング アーティファクトを修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Black shading cross are visible on the mesh surface
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 黒いシェーディング クロスがメッシュ サーフェスに表示されます
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# 黒いシェーディング クロスがメッシュ サーフェスに表示されます

黒いシェーディング アーティファクトは、ライトの下にあるメッシュの複数の領域に表示されます。

![](../../assets/black-shading-cross.jpg)


## 説明

黒い網掛けクロスは、通常、メッシュと法線マップが一致しないことを意味します。これは、通常、メッシュジオメトリが変更されたか、ベイカーが実行する計算とは異なる方法で計算されたためです。 例えば、メッシュの三角形化は、ベイカーと、メッシュとその法線マップをレンダリングするビューポートの間で異なります。

## Solution

メッシュとその法線マップを表示するアプリケーションが、テクスチャのベイク処理の方法と同期していることを確認します。 これは次のことを意味します。

* 接線スペースがビューアとベイカーの間で同じであることを確認します。
* ビューとパン屋の間で通常の書式が同じであることを確認します。
* ビューアとベイカーの間で三角形分割が同じであることを確認します。 詳しくは、[このページ &#x200B;](../../guides/triangulating-before-bak/triangulating-before-baking.md)を参照してください。
