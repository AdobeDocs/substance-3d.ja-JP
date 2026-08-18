---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/geometry-cache.html"
breadcrumb-title: ''
description: ジオメトリキャッシュを使用すると、前処理されたメッシュデータを保持し、その後のベイク処理を大幅に高速化できます。
helpx_creative_field: ""
helpx_description: bakers > Features > Geometry Cache
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ジオメトリキャッシュ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# ジオメトリキャッシュ

ベイク処理では、メッシュが前処理されてクリーンアップされ、ベイク処理と互換性のある形式に変換されます。 ジオメトリキャッシュは、（ソースメッシュが変更されない限り）この操作を後で再実行しないようにするために、事前に処理されたこのジオメトリを高速に再ロードする方法です。

* **Substance Designer**&#x200B;では、最初のベイク処理が実行された後にジオメトリキャッシュが作成されます。 その後、キャッシュはベイカーウィンドウが閉じられるまでメモリに保持されます。
* **Substance Painter**&#x200B;で、ジオメトリキャッシュは、最初のベイク処理の後、ソースファイルの横に拡張子&#x200B;**assbin**&#x200B;の付いたファイルとして保存されます。

ジオメトリキャッシュを再利用すると、ベイク処理が大幅に高速化します。特に、ベイカー設定を微調整して完璧な結果を得た場合に便利です。
