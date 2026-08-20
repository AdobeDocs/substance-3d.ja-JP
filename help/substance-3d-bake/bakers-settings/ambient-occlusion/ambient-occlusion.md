---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/ambient-occlusion.html"
breadcrumb-title: ''
description: Ambient Occlusion ベイカーを使用して、高速GPU アクセラレーション アルゴリズムを使用してアンビエント シャドウ テクスチャを生成する方法を説明します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: アンビエントオクルージョン
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 4%

---


# アンビエントオクルージョン

Ambient Occlusion ベイカーを使用すると、アンビエントシャドウテクスチャをベイクできます。 このベイカーは、GPUで実行される高速アルゴリズムを使用します。

**次の場所で利用できます：**

* Substance Designer
* Substance Automation Toolkit

>[!WARNING]
>
> * このベイカーは古いGPUではサポートされていない可能性があります。
> * ローエンド/モバイル GPUで高解像度でベイクすると、クラッシュする可能性があります。

## パラメーター

| *名前* | *説明* |
| --- | --- |
| **法線マップ** | ベイカー計算時に考慮するメッシュのサーフェス上の追加のジオメトリの詳細を提供するために使用できる法線マップファイルを入力します。 このパラメーターはオプションです。 |
| **ワールド スペース** | 有効にした場合は、入力法線マップがワールド空間（接線空間ではなく）内にあることを指定します。 入力法線マップが指定されていない場合、このパラメーターは無視されるか無効になります。 |
| **標準を反転** | 反転した法線を使用してアンビエントオクルージョンマップを計算します（厚みマップを生成するために使用できます）。 |
| **選択されていないメッシュ パーツを使用** | メッシュの選択されていないメッシュ部分を使用して、アンビエントオクルージョンマップをベイクします。 |
| **品質** | アンビエントオクルージョンマップの品質を選択します。 高いクォリティでは計算が遅くなります。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>低</strong> （3 パス）</li><li data-preserve-html="true"><strong>Medium</strong> （デフォルト、5回）</li><li data-preserve-html="true"><strong>高</strong> （10 パス）</li><li data-preserve-html="true"><strong>非常に高い</strong> （16 パス）</li></ul> |
| **精度バイアス** | アンビエントオクルージョンの精度 値を小さくすると精度は高くなりますが、より大きなアーティファクトが生成されます。 |
| **距離フェード** | アンビエントオクルージョンの広がり。 |
