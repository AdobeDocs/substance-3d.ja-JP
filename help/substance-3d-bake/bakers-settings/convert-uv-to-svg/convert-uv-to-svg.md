---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/convert-uv-to-svg.html"
breadcrumb-title: ''
description: メッシュのUVをベクターグラフィックファイルに変換して、正確なマスクとオーバーレイの作成に使用できます。
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

UVをSVGに変換ベイカーは、ローポリゴンメッシュUVをベクターグラフィックファイルに変換します。 このベクターグラフィックファイルを使用して、マスクを作成できます。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **パディング** | SVGのシェイプに追加する幾何学的パディングの量を制御します。 |
| **カラーモード** | SVGの形状に色を付ける方法を指定します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ランダム：</strong>各UVシェルはランダムな色で色付けされます。</li><li data-preserve-html="true"><strong>色相のシフト:</strong>各UVシェルは、固有の色相値で色付けされます。</li><li data-preserve-html="true"><strong>グレースケール：</strong>各UVシェルは固有のグレースケール値で色付けされます。</li><li data-preserve-html="true"><strong>均一な色：</strong>すべてのUVシェルは50%グレー値で色付けされます。</li><li data-preserve-html="true"><strong>マテリアルIDカラー</strong>: UVシェルは、[シーンビュー]で定義されたマテリアルカラーによって色付けされます。</li></ul> |
