---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/home.html"
breadcrumb-title: ''
description: Substance Bakersを使用して、メッシュベースの情報をテクスチャファイルに計算し、テクスチャリングワークフローを強化する方法を説明します。
helpx_creative_field: ""
helpx_description: bakers > Home
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: サブスタンスベーカー
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 13%

---


# サブスタンスベーカー

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

<b>Substance Bakers</b>は、メッシュベースの情報をテクスチャファイルに計算するための高度なアルゴリズムのツールセットです。 これらのテクスチャは、3Dメッシュを使用するアーティストなら誰でも使用でき、高度なテクスチャリング方法を利用できます。 ベイク処理は、<b>個の強力なツール</b>と<b>自動テクスチャリング</b>を提供するための、Substanceソフトウェアワークフローの中核となるプロセスです。

このドキュメントでは、<b>ベーキングの基礎</b>と<b>一般的な問題</b>と、このプロセスを処理する際に発生する可能性がある間違いについて説明します。

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

* [焼き物とは何ですか？](../getting-started/what-is-baking/what-is-baking.md)
* ベイク処理：
  * [Substance 3D Painter](../getting-started/software-interface/3d-painter/substance-3d-painter.md)
  * [Substance 3D Designer](../getting-started/software-interface/3d-designer/substance-3d-designer.md)
  * [Substance 3D Automation Toolkit](../getting-started/software-interface/3d-automation-toolkit/substance-3d-automation-toolkit.md)
* [ソフトウェアごとの可用性](../getting-started/availability-per-software/availability-per-software.md)
* [互換性のある3Dソフトウェア](../getting-started/compatible-3d-software/compatible-3d-software.md)
* [チュートリアル](../getting-started/tutorials/tutorials.md)

</td>
<td style="border: 0;" valign="top">

### パン焼き設定

* [共通のパラメーター](../bakers-settings/common-parameters/common-parameters.md)
* [アンビエントオクルージョン](../bakers-settings/ambient-occlusion/ambient-occlusion.md)
* [メッシュからの環境オクルージョン](../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)
* [メッシュからの曲げ法線](../bakers-settings/bent-normals-from-mesh/bent-normals-from-mesh.md)
* [メッシュからのカラーマップ](../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)
* [UV を SVG に変換](../bakers-settings/convert-uv-to-svg/convert-uv-to-svg.md)
* [曲率](../bakers-settings/curvature/curvature.md)
* [メッシュからの曲率](../bakers-settings/curvature-from-mesh/curvature-from-mesh.md)
* [メッシュからの曲率（非推奨）](../bakers-settings/curvature-from-mesh-dep/curvature-from-mesh-deprecated.md)
* [メッシュからの高さマップ](../bakers-settings/height-map-from-mesh/height-map-from-mesh.md)
* [メッシュからの法線マップ](../bakers-settings/normal-map-from-mesh/normal-map-from-mesh.md)
* [メッシュからの不透明度マスク](../bakers-settings/opacity-mask-from-mesh/opacity-mask-from-mesh.md)
* [位置](../bakers-settings/position/position.md)
* [メッシュからマップを配置](../bakers-settings/position-map-from-mesh/position-map-from-mesh.md)
* [メッシュからの厚みマップ](../bakers-settings/thickness-map-from-mesh/thickness-map-from-mesh.md)
* [メッシュからの転送されるテクスチャ](../bakers-settings/transferred-texture-from/transferred-texture-from-mesh.md)
* [ワールド空間方向](../bakers-settings/world-space-direction/world-space-direction.md)
* [ワールド空間法線](../bakers-settings/world-space-normals/world-space-normals.md)

</td>
<td style="border: 0;" valign="top">

### ガイド

* [エラーメッセージと警告メッセージ](../guides/error-and-warning-mes/error-and-warning-messages.md)
* [パフォーマンスと最適化](../guides/performances-and-opt/performances-and-optimizations.md)
* [焼き付け前に三角形を作成](../guides/triangulating-before-bak/triangulating-before-baking.md)

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### 機能

* [ジオメトリキャッシュ](../features/geometry-cache/geometry-cache.md)
* [GPU レイトレーシング](../features/gpu-raytracing/gpu-raytracing.md)
* [名前による照合](../features/matching-by-name/matching-by-name.md)
* [タンジェントスペース](../features/tangent-space/tangent-space.md)

</td>
<td style="border: 0;" valign="top">

### よくある質問

* [ベイク済みマップを書き出す方法を教えてください。](../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)
* [ベイクドテクスチャにディザを適用しますか？](../common-questions/dithering-applied-baked/is-dithering-applied-to-baked-textures.md)
* [「フラグメントごとに接線空間を計算」を有効にする必要がありますか？](../common-questions/should-enable-compute-tan/should-i-enable-compute-tangent-space-per-fragment.md)
* [Substanceソフトウェア以外でベイク処理されたテクスチャが正しく表示されない](../common-questions/texture-baked-outside-sof/texture-baked-outside-of-substance-software-looks-incorrect.md)
* [Assbinファイルとは](../common-questions/what-are-assbin-files/what-are-assbin-files.md)
* [ベイクドテクスチャのビット深度は何ですか？](../common-questions/what-the-bit-depth-baked/what-is-the-bit-depth-of-baked-textures.md)
* [OpenGLとDirectX標準フォーマットの違いは何ですか？](../common-questions/what-the-difference-bet/what-is-the-difference-between-the-opengl-and-directx-normal-format.md)
* [ベイク処理または書き出し後に、テクスチャが奇妙に引き伸ばされるのはなぜですか？](../common-questions/why-are-there-strange-str/why-are-there-strange-stretches-in-my-textures-after-baking-or-exporting.md)
* [名前による照合が環境オクルージョン/Thicknessで機能しないのはなぜですか？](../common-questions/why-matching-name-not-wor/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.md)
* [焼いた後にメッシュが完全に黒くなるのはなぜですか？](../common-questions/why-mesh-fully-black-aft/why-is-my-mesh-fully-black-after-baking.md)

</td>
<td style="border: 0;" valign="top">

### 一般的な問題

* [UVシーム上のエイリアス](../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)
* [ベイカーからの出力が完全に黒または空](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/baker-output-is-fully-black-159451835.html)
* [メッシュからのカラーマップでベイク処理が失敗しました](../common-issues/baking-failed-with-color/baking-failed-with-color-map-from-mesh.md)
* [黒いシェーディングの十字がメッシュサーフェスに表示される](../common-issues/black-shading-cross-are/black-shading-cross-are-visible-on-the-mesh-surface.md)
* [メッシュパーツ同士のブリード](../common-issues/mesh-parts-bleed-between/mesh-parts-bleed-between-each-other.md)
* [法線マップに奇妙なカラフルなグラデーションが含まれている](../common-issues/normal-map-has-strange/normal-map-has-strange-colorful-gradients.md)
* [通常のテクスチャはファセットされています](../common-issues/normal-texture-looks-fac/normal-texture-looks-faceted.md)
* [通常のテクスチャをベイク処理した後に継ぎ目が表示される](../common-issues/seams-are-visible-after/seams-are-visible-after-baking-a-normal-texture.md)
* [すべての面に表示される継ぎ目](../common-issues/seam-visible-every-face/seam-visible-on-every-face.md)

</td>
</tr>
</table>
