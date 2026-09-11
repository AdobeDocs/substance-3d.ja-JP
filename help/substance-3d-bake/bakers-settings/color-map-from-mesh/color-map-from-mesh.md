---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/color-map-from-mesh.html"
breadcrumb-title: ''
description: カラープロパティをハイポリゴンメッシュからテクスチャに投影し、選択マスクのポリペイントIDまたはマテリアルIDをベイクします。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからのカラーマップ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 5%

---


# メッシュからのカラーマップ

ベイカーのこのカラーマップは、高精細メッシュのカラープロパティをテクスチャに投影します。 このエフェクトを使用してポリペイントIDまたはマテリアル IDをベイクし、セレクションマスクを作成できます。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット
* Substance Painter

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **カラーソース** | カラー生成の基準とする高ポリゴンメッシュのプロパティをコントロールします。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>頂点の色</strong>: 頂点の色を読み取り、テクスチャに保存します。 カラーは頂点から頂点に補間されます。</li><li data-preserve-html="true"><strong>マテリアルの色</strong>:ポリゴン面に割り当てられたマテリアルの色を読み取ります。</li><li data-preserve-html="true"><strong>メッシュ ID</strong>：見つかったオブジェクトごとに色を割り当てます。</li><li data-preserve-html="true"><strong>ポリグループ/サブメッシュID</strong>:サブオブジェクト（要素とも呼ばれる）ごとに色を割り当てます。</li></ul> |
| **カラージェネレーター** | **カラーソース**&#x200B;が&#x200B;**メッシュ ID**&#x200B;または&#x200B;**ポリグループ/サブメッシュID**&#x200B;に設定されている場合に、色がどのように生成されるかを指定します。指定できる値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>ランダム</strong>：各オブジェクトまたはサブオブジェクトは、ランダムに生成された色で色付けされます。</li><li data-preserve-html="true"><strong>色相シフト</strong>：各オブジェクトまたはサブオブジェクトは、色相に基づいて固有の色で色付けされます。</li><li data-preserve-html="true"><strong>グレースケール</strong>：各オブジェクトまたはサブオブジェクトは、一意のグレースケール値によって色付けされます。</li></ul> |
