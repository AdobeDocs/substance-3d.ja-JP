---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/ambient-occlusion.html"
breadcrumb-title: ''
description: ベイカーを使用して、高速なGPUアクセラレーションアルゴリズムにより環境シャドウテクスチャを生成する方法について説明します。
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

ベイカーを使用すると、アンビエントシャドウテクスチャをベイクできます。 このベイカーは、GPUで実行される高速アルゴリズムを使用します。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット

>[!WARNING]
>
> * このベイカーは、古いGPUではサポートされていない場合があります。
> * ローエンド/モバイルGPUで高解像度でベイクすると、クラッシュが発生する可能性があります。

## パラメーター

| *名前* | *説明* |
| --- | --- |
| **標準マップ** | 計算時に考慮されるメッシュのサーフェス上の追加ジオメトリの詳細を提供するために使用できる入力法線マップファイル。 このパラメーターはオプションです。 |
| **ワールドスペース** | 有効な場合は、入力法線マップが（接線空間ではなく）ワールド空間であることを指定します。 入力法線マップーが指定されていない場合、このパラメーターは無視されるか、または無効になります。 |
| **法線を反転** | 法線を反転させてambient occlusionマップを計算します（厚みマップの生成に使用できます）。 |
| **選択されていないメッシュパーツを使用する** | メッシュの選択されていないメッシュ部分を使用して、ambient occlusionマップをベイクします。 |
| **クォリティ** | ambient occlusionマップの質を選択します。 クォリティが高いと、計算に時間がかかります。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>低</strong> （3パス）</li><li data-preserve-html="true"><strong>中</strong> （既定、5パス）</li><li data-preserve-html="true"><strong>高</strong> （10パス）</li><li data-preserve-html="true"><strong>非常に高い</strong> （16パス）</li></ul> |
| **精度バイアス** | ambient occlusionの精度。 値を小さくすると精度は高くなりますが、アーティファクトが大きくなる可能性があります。 |
| **距離フェード** | アンビエントオクルージョンの広がり。 |
