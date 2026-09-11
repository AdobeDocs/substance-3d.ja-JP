---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/world-space-direction.html"
breadcrumb-title: ''
description: ワールド空間でベクトル方向を計算し、それらをテクスチャに保存して、方向効果やマスキングを行います。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > World Space Direction
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ワールド空間方向
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 4%

---


# ワールド空間方向

ベイカーは、テクスチャにワールド空間するベクトル方向を計算できる。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **入力方向** | どの入力から方向を計算するかを定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>テクスチャから</strong>:ベクトル方向は入力テクスチャによって定義されています。</li><li data-preserve-html="true"><strong>均一ベクトルから</strong> （既定）:ベクトルの方向は、X、Y、Zスライダーで定義されます。</li></ul> |
| **法線の向き** | 出力テクスチャの法線フォーマットを定義します。 これにより、形式に応じてグリーンチャンネルが反転します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> （既定）</li></ul> |
| **X Y Z** | **入力方向**&#x200B;が&#x200B;**均一ベクトルから**&#x200B;に設定されている場合、方向ベクトルの3つの要素を定義するスライダー。 |
| **方向ファイル** | **入力テクスチャ**&#x200B;が&#x200B;**テクスチャから**&#x200B;に設定されている場合、方向ベクトルを定義するための入力方向ファイルへのパス。 |
