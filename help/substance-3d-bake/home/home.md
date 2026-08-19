---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/home.html"
breadcrumb-title: ''
description: Substance Bakersを使用して、メッシュベースの情報をテクスチャファイルに変換し、テクスチャリングワークフローを強化する方法を説明します。
helpx_creative_field: ""
helpx_description: bakers > Home
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance Bakers
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 13%

---


# Substance Bakers

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

<b>Substance Bakers</b>は、メッシュベースの情報をテクスチャファイルに計算するための高度なアルゴリズムのツールセットです。 高度なテクスチャリング手法を活用するために、3D メッシュを持つ任意のアーティストが使用できます。 ベーキングは、<b>個の強力なツール </b>と<b>自動テクスチャリング </b>を提供するために、Substance ソフトウェアワークフローの中心にあるプロセスです。

このドキュメントでは、ベイク処理の<b>基本</b>と<b>一般的な問題</b>と、このプロセスを扱う際に発生する可能性のある間違いについて説明します。

</td>
<td width="58.30%" style="border: 0;" valign="top">

![](../assets/optim-baker-home.png){width="400px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## はじめに

* [ベーキングとは何ですか？](../getting-started/what-is-baking/what-is-baking.md)
* 次で焼く：
  * [Substance 3D Painter](../getting-started/software-interface/3d-painter/substance-3d-painter.md)
  * [Substance 3D Designer](../getting-started/software-interface/3d-designer/substance-3d-designer.md)
  * [Substance 3D Automation Toolkit](../getting-started/software-interface/3d-automation-toolkit/substance-3d-automation-toolkit.md)
* [ソフトウェアごとの可用性](../getting-started/availability-per-software/availability-per-software.md)
* [互換性のある3D ソフトウェア](../getting-started/compatible-3d-software/compatible-3d-software.md)
* [チュートリアル](../getting-started/tutorials/tutorials.md)

</td>
<td style="border: 0;" valign="top">

### ベイカーの設定

* [共通のパラメーター](../bakers-settings/common-parameters/common-parameters.md)
* [アンビエントオクルージョン](../bakers-settings/ambient-occlusion/ambient-occlusion.md)
* [メッシュからのアンビエントオクルージョン](../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)
* [メッシュからのベント法線](../bakers-settings/bent-normals-from-mesh/bent-normals-from-mesh.md)
* [メッシュからのカラーマップ](../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)
* [UV を SVG に変換](../bakers-settings/convert-uv-to-svg/convert-uv-to-svg.md)
* [曲率](../bakers-settings/curvature/curvature.md)
* [メッシュからの曲率](../bakers-settings/curvature-from-mesh/curvature-from-mesh.md)
* [メッシュからの曲率（非推奨）](../bakers-settings/curvature-from-mesh-dep/curvature-from-mesh-deprecated.md)
* [メッシュからの高さマップ](../bakers-settings/height-map-from-mesh/height-map-from-mesh.md)
* [メッシュからの法線マップ](../bakers-settings/normal-map-from-mesh/normal-map-from-mesh.md)
* [メッシュからの不透明度マスク](../bakers-settings/opacity-mask-from-mesh/opacity-mask-from-mesh.md)
* [位置](../bakers-settings/position/position.md)
* [メッシュからの位置マップ](../bakers-settings/position-map-from-mesh/position-map-from-mesh.md)
* [メッシュからの厚みマップ](../bakers-settings/thickness-map-from-mesh/thickness-map-from-mesh.md)
* [メッシュからの転送されるテクスチャ](../bakers-settings/transferred-texture-from/transferred-texture-from-mesh.md)
* [ワールド空間方向](../bakers-settings/world-space-direction/world-space-direction.md)
* [ワールド空間法線](../bakers-settings/world-space-normals/world-space-normals.md)

</td>
<td style="border: 0;" valign="top">

### ガイド

* [エラーと警告メッセージ](../guides/error-and-warning-mes/error-and-warning-messages.md)
* [パフォーマンスと最適化](../guides/performances-and-opt/performances-and-optimizations.md)
* [焼く前に三角形分割](../guides/triangulating-before-bak/triangulating-before-baking.md)

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### 機能

* [ジオメトリ キャッシュ](../features/geometry-cache/geometry-cache.md)
* [GPU レイトレーシング](../features/gpu-raytracing/gpu-raytracing.md)
* [名前で一致](../features/matching-by-name/matching-by-name.md)
* [タンジェントスペース](../features/tangent-space/tangent-space.md)

</td>
<td style="border: 0;" valign="top">

### よくある質問

* [ベイクしたマップを書き出す方法は？](../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)
* [焼き上げたテクスチャにディザリングを適用しますか？](../common-questions/dithering-applied-baked/is-dithering-applied-to-baked-textures.md)
* [「フラグメントごとに接線空間を計算」を有効にする必要がありますか？](../common-questions/should-enable-compute-tan/should-i-enable-compute-tangent-space-per-fragment.md)
* [Substance ソフトウェアの外部でベイク処理されたテクスチャが正しく表示されない](../common-questions/texture-baked-outside-sof/texture-baked-outside-of-substance-software-looks-incorrect.md)
* [Asbin ファイルとは？](../common-questions/what-are-assbin-files/what-are-assbin-files.md)
* [焼きテクスチャのビット深度は何ですか？](../common-questions/what-the-bit-depth-baked/what-is-the-bit-depth-of-baked-textures.md)
* [OpenGLとDirectXの通常の形式の違いは何ですか？](../common-questions/what-the-difference-bet/what-is-the-difference-between-the-opengl-and-directx-normal-format.md)
* [焼いたり書き出したりした後に、テクスチャに奇妙な伸縮が生じるのはなぜですか？](../common-questions/why-are-there-strange-str/why-are-there-strange-stretches-in-my-textures-after-baking-or-exporting.md)
* [名前によるマッチングがAmbient Occlusion/Thicknessで機能しないのはなぜですか？](../common-questions/why-matching-name-not-wor/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.md)
* [焼き上げた後、メッシュが完全に黒くなるのはなぜですか？](../common-questions/why-mesh-fully-black-aft/why-is-my-mesh-fully-black-after-baking.md)

</td>
<td style="border: 0;" valign="top">

### 一般的な問題

* [UV シームのエイリアス](../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)
* [ベイカー出力が完全に黒または空です](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/baker-output-is-fully-black-159451835.html)
* [メッシュからのカラーマップでベイク処理に失敗しました](../common-issues/baking-failed-with-color/baking-failed-with-color-map-from-mesh.md)
* [黒いシェーディング クロスがメッシュ サーフェスに表示されます](../common-issues/black-shading-cross-are/black-shading-cross-are-visible-on-the-mesh-surface.md)
* [メッシュ パーツが互いにブリードします](../common-issues/mesh-parts-bleed-between/mesh-parts-bleed-between-each-other.md)
* [法線マップに奇妙な色彩グラデーションがある](../common-issues/normal-map-has-strange/normal-map-has-strange-colorful-gradients.md)
* [通常のテクスチャはファセットに見えます](../common-issues/normal-texture-looks-fac/normal-texture-looks-faceted.md)
* [通常のテクスチャをベイク処理すると、シームが表示されます](../common-issues/seams-are-visible-after/seams-are-visible-after-baking-a-normal-texture.md)
* [すべての顔にシームが表示されます](../common-issues/seam-visible-every-face/seam-visible-on-every-face.md)

</td>
</tr>
</table>
