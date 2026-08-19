---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/position.html"
breadcrumb-title: ''
description: メッシュジオメトリの位置を計算してテクスチャに保存し、ボリュームベースのエフェクトとグラデーションマスクを作成します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Position
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 位置
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 2%

---


# 位置

位置ベイカーは、メッシュジオメトリの位置を計算し、テクスチャに保存します。 位置は、オブジェクトのボリューム内の情報を計算したり、グラデーションマスクを作成したりするのに便利です。

**次の場所で利用できます：**

* Substance Painter
* Substance Designer
* Substance Automation Toolkit

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **モード** | 位置テクスチャに計算する情報を制御します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>すべての軸：</strong> X、Y、Z軸の位置を出力テクスチャのRGB チャンネルにベイク処理します。</li><li data-preserve-html="true"><strong>1つの軸：</strong>出力テクスチャに1つの軸をグレースケール画像としてベイク処理します。</li></ul> |
| **軸** | **Mode** パラメーターが&#x200B;**One axis**&#x200B;に設定されている場合に計算する軸を定義します。 |
| **正規化タイプ** | 軸ごとに位置値を拡大・縮小する方法を定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong> ボックス：</strong> メッシュのボリューム（バウンディングボックスの長さ）に従って各軸を正規化します。</li><li data-preserve-html="true"><strong>BSphere:</strong> メッシュ ボリュームの半径（バウンディング球体）に従ってすべての軸を正規化します。</li></ul> |
| **正規化スケール** | メッシュに基づいて位置値を拡大・縮小する方法を定義します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong> マテリアルごとに</strong>：値は、各マテリアルに対して0 ～ 1の間にスケールされます（テクスチャセット）。</li><li data-preserve-html="true"><strong> フルシーン </strong> （デフォルト）：メッシュ全体を考慮して値をスケールします。 これにより、オブジェクトとマテリアル（テクスチャセット）全体で連続的な位置値を使用できます。</li></ul> |
