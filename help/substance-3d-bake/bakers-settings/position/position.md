---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/position.html"
breadcrumb-title: ''
description: メッシュジオメトリの場所を計算してテクスチャに保存し、ボリュームベースのエフェクトやグラデーションマスクを作成できます。
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

位置ベイカーは、メッシュジオメトリの位置を計算し、テクスチャに保存します。 この位置は、オブジェクトのボリュームの情報を計算したり、グラデーションマスクを作成したりする場合に便利です。

**使用可能：**

* Substance Painter
* Substance Designer
* Substance自動処理ツールキット

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **モード** | 位置テクスチャに計算する情報を制御します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>すべての軸：</strong> X軸、Y軸、Z軸の位置を出力テクスチャのRGBチャンネルにベイク処理します。</li><li data-preserve-html="true"><strong>1つの軸：</strong>単一の軸をグレースケールイメージとして出力テクスチャにベイク処理します。</li></ul> |
| **軸** | **Mode**&#x200B;パラメーターが&#x200B;**One axis**&#x200B;に設定されている場合に計算する軸を定義します。 |
| **正規化の種類** | 軸ごとに位置の値をスケールする方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ボックス：</strong>メッシュの体積（バウンディングボックスの長さ）に従って各軸を正規化します。</li><li data-preserve-html="true"><strong>球：</strong>メッシュ体積の半径（バウンディング球）に従ってすべての軸を正規化します。</li></ul> |
| **正規化スケール** | メッシュに基づいて位置の値をスケーリングする方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>マテリアル単位</strong>：各マテリアル（テクスチャセット）の値は0 ～ 1の範囲でスケールされます。</li><li data-preserve-html="true"><strong>フルシーン</strong> （既定値）:メッシュ全体を考慮に入れて値がスケールされます。 これにより、オブジェクトおよびマテリアル（テクスチャセット）全体で連続的な位置の値が可能になります。</li></ul> |
