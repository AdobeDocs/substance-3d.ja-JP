---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/world-space-normals.html"
breadcrumb-title: ''
description: メッシュの法線、接線、および従法線を、ワールド空間座標を使用してテクスチャに保存し、高度なワークフローを行います。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > World Space Normals
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ワールド空間法線
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 6%

---


# ワールド空間法線

ワールド空間法線ベイカーを使用すると、メッシュ法線、接線、および従法線をテクスチャに保存できます。

**次の場所で利用可能：**

* Substance Designer
* Substance Automation Toolkit

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **ベーキングタイプ** | ベイカーが実行する計算のタイプを定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>標準</strong> （既定値）</li><li data-preserve-html="true"><strong>正接</strong></li><li data-preserve-html="true"><strong>従法線</strong></li></ul> |
| **法線マップ** | 詳細を追加するために計算中に使用される入力法線テクスチャへのパス。 |
| **通常の向き** | **Baking Type**&#x200B;が&#x200B;**Normal**&#x200B;に設定されている場合、入力テクスチャの通常の形式を定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> （既定値）</li></ul> |
