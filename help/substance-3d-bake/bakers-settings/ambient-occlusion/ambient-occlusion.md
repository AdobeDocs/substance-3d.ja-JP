---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/ambient-occlusion.html"
breadcrumb-title: ''
description: アンビエントオクルージョンベイカーを使用して、高速なGPUアクセラレーションアルゴリズムでアンビエントシャドウテクスチャを生成する方法について説明します。
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

アンビエントオクルージョンベイカーを使用すると、アンビエントシャドウテクスチャをベイク処理できます。 このパン屋はGPU上で実行される高速アルゴリズムを使用します。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット

>[!WARNING]
>
> * 古いGPUではこのベイカーがサポートされていない可能性があります。
> * ローエンド/モバイルGPUで高解像度でベイク処理を行うとクラッシュする場合があります。

## パラメーター

| *名前* | *説明* |
| --- | --- |
| **標準マップ** | ベイカー計算時に考慮するメッシュのサーフェス上の追加ジオメトリの詳細を提供するために使用できる法線マップファイルを入力します。 このパラメーターはオプションです。 |
| **ワールドスペース** | 有効な場合は、入力法線マップが（接線空間ではなく）ワールド空間に存在することを指定します。 入力法線マップが指定されていない場合、このパラメータは無視されるか、または無効になります。 |
| **法線を反転** | 法線が反転した環境オクルージョンマップを計算します（Thicknessマップの生成に使用できます）。 |
| **選択されていないメッシュパーツを使用する** | メッシュの選択されていないメッシュパーツを使用して、環境オクルージョンマップをベイク処理します。 |
| **クォリティ** | 環境オクルージョンマップの質を選択します。 クォリティが高いと、計算に時間がかかります。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>低</strong> （3パス）</li><li data-preserve-html="true"><strong>中</strong> （既定、5パス）</li><li data-preserve-html="true"><strong>高</strong> （10パス）</li><li data-preserve-html="true"><strong>非常に高い</strong> （16パス）</li></ul> |
| **精密バイアス** | 環境オクルージョンの精度。 値を小さくすると精度は高くなりますが、アーティファクトが大きくなる可能性があります。 |
| **距離フェード** | アンビエントオクルージョンの広がり。 |
