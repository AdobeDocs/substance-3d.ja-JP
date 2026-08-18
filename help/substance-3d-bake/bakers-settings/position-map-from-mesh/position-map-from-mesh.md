---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/position-map-from-mesh.html"
breadcrumb-title: ''
description: 高ポリゴンメッシュから正確な位置マップを計算して、正確なジオメトリ位置情報をキャプチャします。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Position map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからマップを配置
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# メッシュからマップを配置

メッシュベイカーから位置マップを使用すると、高ポリゴンメッシュジオメトリの位置が計算され、テクスチャに保存されます。 これはベース位置のパン屋に似ていますが、より正確な結果を生成できます。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **モード** | 位置テクスチャに計算する情報を制御します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>すべての軸：</strong> X軸、Y軸、Z軸の位置を出力テクスチャのRGBチャンネルにベイク処理します。</li><li data-preserve-html="true"><strong>1つの軸：</strong>単一の軸をグレースケールイメージとして出力テクスチャにベイク処理します。</li></ul> |
| **軸** | **Mode**&#x200B;パラメーターが&#x200B;**One axis**&#x200B;に設定されている場合に計算する軸を定義します。 |
| **正規化の種類** | 軸ごとに位置の値をスケールする方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ボックス：</strong>メッシュの体積（バウンディングボックスの長さ）に従って各軸を正規化します。</li><li data-preserve-html="true"><strong>球：</strong>メッシュ体積の半径（バウンディング球）に従ってすべての軸を正規化します。</li></ul> |
| **正規化スケール** | メッシュに基づいて位置の値をスケーリングする方法を定義します。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>マテリアル単位</strong>：各マテリアル（テクスチャセット）の値は0 ～ 1の範囲でスケールされます。</li><li data-preserve-html="true"><strong>フルシーン</strong> （既定値）:メッシュ全体を考慮に入れて値がスケールされます。 これにより、オブジェクトおよびマテリアル（テクスチャセット）全体で連続的な位置の値が可能になります。</li></ul> |
