---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/guides/triangulating-before-baking.html"
breadcrumb-title: ''
description: メッシュの三角形分割がベイク結果に与える影響を理解し、ジオメトリを準備するためのベストプラクティスを学習します。
helpx_creative_field: ""
helpx_description: bakers > Guides > Triangulating before baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ベイク前の三角形化
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# ベイク前の三角形化

3D メッシュは、面ごとに複数の境界エッジを持つポリゴンで定義できます。 通常は四角形（4つのエッジ）を介し、場合によってはより多く(n-gon)。\
ただし、（特にGPU上で）を使用した方が管理と計算が簡単であるため、これらのポリゴンは後で三角形に変形されます。

## 三角形分割はメッシュにどのような影響を与えますか？

![](../../assets/triangulation.jpg)

クアッド/N – ゴーンを三角形に変換するための&#x200B;**標準ソリューション**&#x200B;がありません。 上の画像に示されているように、複数の選択肢が有効です。\
ベイカーは、ゲームエンジンのようなトライアングルのメッシュとは思えません。

## ベイクする前に三角形分割する理由

ベイクプロセスでは、ジオメトリが読み込まれ、情報がテクスチャにエンコードされます。\
これらの情報はUVやメッシュトポロジに基づいているため、ジオメトリをテクスチャを適用するときと同じように読み取らない場合、他のソフトウェアが情報を誤ってデコードする可能性があります。

下の図では、左上にローポリゴンメッシュが表示され、右上にハイポリゴンメッシュが表示されています。\
下部には低ポリゴンがあり、高ポリゴンから法線マップがベイクされています。 左側のメッシュでは、ベイク時にSubstance Painterで使用した三角形分割と同じ三角形分割を使用しています。 右側のメッシュには黒い斑点は表示されず、黒い斑点が表示されている これは、メッシュのベイク方法と法線マップが現在の三角形分割の方法が一致していないためです。 この問題は、**メッシュの更新や再ベイク処理**&#x200B;によって修正できます。

![](../../assets/example-triangulation-artifact.jpg)
