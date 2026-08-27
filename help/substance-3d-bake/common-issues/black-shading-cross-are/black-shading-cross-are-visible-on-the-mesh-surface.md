---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/black-shading-cross-are-visible-on-the-mesh-surface.html"
breadcrumb-title: ''
description: 接線空間と法線の計算を補正することで、メッシュサーフェスに表示される黒いシェーディングのアーティファクトを修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Black shading cross are visible on the mesh surface
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 黒いシェーディングの十字がメッシュサーフェスに表示される
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# 黒いシェーディングの十字がメッシュサーフェスに表示される

照明を当てると、メッシュの複数の領域に黒いシェーディングの斑点が表示される。

![](../../assets/black-shading-cross.jpg)


## 説明

黒いシェーディングクロスは通常、法線マップがメッシュと一致しないことを意味します。これは通常、メッシュジオメトリが変更されたか、ベイカーが実行する計算とは異なる方法で計算されたためです。 たとえば、メッシュの三角形分割は、メッシュとその法線マップをレンダリングするベイカーとビューポートで異なります。

## 解決策

メッシュとその法線マップを表示するアプリケーションが、テクスチャがベイク処理された方法と同期していることを確認します。 これは、次のことを意味します。

* ビューアとパン屋の間の接線空間が同じであることを確認します。
* ビューとパン屋の間でNormalフォーマットが同一であることを確認します。
* 見る人とパン屋の間で三角形分割が同じであることを確認します。 詳細については、[このページ](../../guides/triangulating-before-bak/triangulating-before-baking.md)を参照してください。
