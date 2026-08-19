---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/color-map-from-mesh.html"
breadcrumb-title: ''
description: 高ポリメッシュのカラープロパティをテクスチャに投影して、ポリペイントや選択マスクのマテリアル IDをベイク処理します。
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

メッシュベイカーのこのカラーマップは、高精細メッシュのカラープロパティをテクスチャに投影します。 ポリペイントまたはマテリアル IDをベイク処理して選択マスクを作成するのに使用できます。

**次の場所で利用できます：**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **カラーSource** | カラー生成の基準となるハイポリメッシュのプロパティを制御します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>頂点カラー</strong>：頂点カラーを読み取り、テクスチャに保存します。 カラーは頂点から頂点に補間されます。</li><li data-preserve-html="true"><strong>Material Color</strong>: ポリゴン面に割り当てられたマテリアル カラーを読み取ります。</li><li data-preserve-html="true"><strong> メッシュ ID</strong>：見つかったオブジェクトごとにカラーを割り当てます。</li><li data-preserve-html="true"><strong> ポリグループ / サブメッシュ ID</strong>: サブオブジェクトごとにカラーを割り当てます（エレメントとも呼ばれます）。</li></ul> |
| **カラージェネレーター** | **カラーSource**&#x200B;が&#x200B;**メッシュ ID**&#x200B;または&#x200B;**ポリグループ/サブメッシュ ID**&#x200B;に設定されている場合のカラーの生成方法を定義します。使用可能な値は次のとおりです。<ul data-preserve-html="true"><li data-preserve-html="true"><strong> ランダム </strong>：各オブジェクトまたはサブオブジェクトは、ランダムに生成されたカラーで色付けされます。</li><li data-preserve-html="true"><strong>色相シフト </strong>：各オブジェクトまたはサブオブジェクトは、色相に基づいて一意の色で色付けされます。</li><li data-preserve-html="true"><strong> グレースケール </strong>：各オブジェクトまたはサブオブジェクトは、一意のグレースケール値で色付けされます。</li></ul> |
