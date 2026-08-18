---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/guides/triangulating-before-baking.html"
breadcrumb-title: ''
description: メッシュの三角形分割がベイク処理の結果に与える影響を理解し、ジオメトリを準備するためのベストプラクティスを学習します。
helpx_creative_field: ""
helpx_description: bakers > Guides > Triangulating before baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 焼き付け前に三角形を作成
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# 焼き付け前に三角形を作成

3Dメッシュは、面ごとに複数の境界エッジを持つポリゴンで定義できます。 通常は四角形（4つのエッジ）を介し、場合によってはより多く(n-gon)。\
ただし、（特にGPU上で）の管理と計算がより簡単であるため、ソフトウェアはこれらのポリゴンを後で三角形に変換します。

## 三角形分割がメッシュに影響を与える仕組み

![](../../assets/triangulation.jpg)

クアッド/N – ゴーンを三角形に変換するための&#x200B;**標準ソリューション**&#x200B;がありません。 上の画像に示されているように、複数の選択肢が有効です。\
ベーカーは、ゲームエンジンが行うように三角メッシュを作成する可能性はほとんどありません。これは、特定のアルゴリズムを他のアルゴリズムよりも優先して選択するためです。

## 焼く前になぜ三角測量するの？

ベイク処理では、ジオメトリが読み込まれ、情報がテクスチャにエンコードされます。\
これらの情報はUVに基づき、場合によってはメッシュトポロジに基づくため、他のソフトウェアでは、テクスチャを適用するときと同じ方法でジオメトリを読み取らないと、情報が正しくデコードされないことがあります。

下のイメージでは、左上に低ポリゴンメッシュ、右上に高ポリゴンメッシュが表示されています。\
下部にはローポリゴンが表示され、高ポリゴンからベイク処理された法線マップが表示されます。 左側のメッシュは、ベイク処理時にSubstance Painterで使用した三角形分割と同じ方法を使用しています。 右側のメッシュは表示されず、黒いアーティファクトが表示されます。 これは、法線マップがベイク処理された方法と、メッシュが現在どのように三角化されているかとの間に不一致があるためです。 この問題は、**メッシュの更新や再ベイク処理**&#x200B;によって修正できます。

![](../../assets/example-triangulation-artifact.jpg)
