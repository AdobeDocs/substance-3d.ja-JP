---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/world-space-direction.html"
breadcrumb-title: ''
description: ワールド空間内のベクター方向を計算し、それらをテクスチャに保存して、指向性エフェクトとマスクを作成します。
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

ワールド空間方向ベイカーを使用すると、ワールド空間内のベクトル方向をテクスチャに計算できます。

**次の場所で利用可能：**

* Substance Designer
* Substance Automation Toolkit

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **入力方向** | 方向が計算される入力を定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong> テクスチャから</strong>: ベクトル方向は、入力テクスチャによって定義されます。</li><li data-preserve-html="true"><strong>均一ベクトルから</strong> （既定値）: ベクトルの方向は、X、Y、Z スライダーで定義されます。</li></ul> |
| **通常の向き** | 出力テクスチャの通常のフォーマットを定義します。 これにより、書式に応じて緑色のチャンネルが反転されます。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> （既定値）</li></ul> |
| **X Y Z** | **入力方向**&#x200B;が&#x200B;**均一ベクトルから**&#x200B;に設定されている場合、方向ベクトルの3つのコンポーネントを定義するスライダー。 |
| **方向ファイル** | **入力方向**&#x200B;が&#x200B;**テクスチャから**&#x200B;に設定されている場合、方向ベクトルを定義するための入力テクスチャファイルへのパス。 |
