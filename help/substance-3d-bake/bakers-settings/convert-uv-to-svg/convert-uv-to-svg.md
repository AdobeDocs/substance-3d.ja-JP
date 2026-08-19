---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/convert-uv-to-svg.html"
breadcrumb-title: ''
description: メッシュ UVをベクターグラフィックファイルに変換し、正確なマスクとオーバーレイを作成できます。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Convert UV to SVG
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV を SVG に変換
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 6%

---


# UV を SVG に変換

「UVをSVGに変換」ベイカーは、ローポリメッシュ UVをベクターグラフィックファイルに変換します。 このベクターグラフィックファイルは、マスクの作成に使用できます。

**次の場所で利用可能：**

* Substance Designer
* Substance Automation Toolkit

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **パディング** | SVGのシェイプにどれだけの幾何学的パディングを追加するかを制御します。 |
| **カラーモード** | SVG シェイプの色付け方法を定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong> ランダム：</strong>各UV シェルは、ランダムな色で色付けされます。</li><li data-preserve-html="true"><strong>HUE Shift:</strong>各UV シェルは、一意の色相値で色付けされます。</li><li data-preserve-html="true"><strong> グレースケール：</strong>各UV シェルは、一意のグレースケール値で色付けされます。</li><li data-preserve-html="true"><strong>均一なカラー：</strong>すべてのUV シェルは、50%のグレー値で色付けされます。</li><li data-preserve-html="true"><strong> マテリアル ID カラー</strong>:UV シェルは、シーン ビューで定義されたマテリアル カラーでカラー設定されます。</li></ul> |
