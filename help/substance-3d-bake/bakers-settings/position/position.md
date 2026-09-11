---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/position.html"
breadcrumb-title: ''
description: メッシュのジオメトリの場所を計算してテクスチャに保存し、ボリュームベースのエフェクトとグラデーションマスクを作成します。
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

位置ベイカーは、メッシュジオメトリの位置を計算し、テクスチャに保管します。 この位置は、オブジェクトのボリュームの情報を計算したり、グラデーションマスクを作成したりする場合に便利です。

**使用可能：**

* Substance Painter
* Substance Designer
* Substance自動処理ツールキット

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **モード** | 位置テクスチャに計算される情報をコントロールします。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>すべての軸:</strong>出力テクスチャのRGBチャンネルにX、Y、Z軸のポジションをベイクします。</li><li data-preserve-html="true"><strong>1つの軸:</strong>は、1つの軸をグレースケールイメージとして出力テクスチャにベイクします。</li></ul> |
| **軸** | **Mode**&#x200B;パラメーターが&#x200B;**One 軸**&#x200B;に設定されている場合に計算される軸を定義します。 |
| **正規化の種類** | 軸単位で位置の値をスケールする方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ボックス：</strong>は、メッシュのボリューム（境界ボックスの長さ）に従って各軸を正規化します。</li><li data-preserve-html="true"><strong>B面：</strong>すべての軸をメッシュの体積の半径（境界球）に従ってノーマライズします。</li></ul> |
| **正規化スケール** | メッシュに基づいて位置の値をスケールする方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>マテリアルごと</strong>：各マテリアル (テクスチャセット)の値は0 ～ 1の範囲で調整されます。</li><li data-preserve-html="true"><strong>完全なシーン</strong> （既定）：値は、メッシュ全体を考慮して調整されます。 これにより、オブジェクトおよびマテリアル（テクスチャセット）全体で連続的な位置の値が可能になります。</li></ul> |
