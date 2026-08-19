---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/guides/triangulating-before-baking.html"
breadcrumb-title: ''
description: メッシュのトライアンギュレーションがベイク処理の結果にどのような影響を与えるかを理解し、ジオメトリを準備するためのベストプラクティスを学びます。
helpx_creative_field: ""
helpx_description: bakers > Guides > Triangulating before baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 焼く前に三角形分割
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# 焼く前に三角形分割

3D メッシュは、1つの面に複数の境界線エッジを持つポリゴンで定義できます。 通常はクワッド（4つのエッジ）、場合によってはそれ以上（n ゴン）を経由します。\
ソフトウェアは、これらのポリゴンを後で三角形に変換します。これは、で管理および計算を実行する方が簡単だからです（特にGPU）。

## トライアンギュレーションはメッシュにどのように影響しますか？

![](../../assets/triangulation.jpg)

クワッド/N ゴンを三角形に変換する標準ソリューションは&#x200B;**ありません**。 上記の画像に示すように、複数の選択肢が有効です。\
特定のアルゴリズムを選択するため、ゲームエンジンのように三角形のメッシュを作成する可能性は低くなります。

## なぜ焼く前に三角形化するのか？

ベイク処理では、ジオメトリを読み取り、情報をテクスチャにエンコードします。\
これらの情報はUVに基づくもので、時にはメッシュトポロジに基づいているため、テクスチャを適用する場合と同じようにジオメトリを読み取らない場合、他のソフトウェアが情報を誤ってデコードする可能性があります。

下の画像では、左上にローポリメッシュ、右上にハイポリメッシュが表示されています。\
下部はローポリで、法線マップはハイポリからベイクされます。 左側のメッシュは、ベーキング時にSubstance Painterで使用されるものと同じ三角形分割を使用します。 右側のメッシュには黒いアーティファクトが表示されません。 これは、法線マップのベイク処理とメッシュの現在の三角形化の間に不一致があるためです。 これは、**メッシュの更新やリベイク**&#x200B;によって修正できます。

![](../../assets/example-triangulation-artifact.jpg)
