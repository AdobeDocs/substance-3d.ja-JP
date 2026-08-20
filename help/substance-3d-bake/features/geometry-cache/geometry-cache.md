---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/features/geometry-cache.html"
breadcrumb-title: ''
description: ジオメトリ キャッシュを使用すると、事前に処理されたメッシュ データを保持し、その後のベイク処理を大幅に高速化できます。
helpx_creative_field: ""
helpx_description: bakers > Features > Geometry Cache
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ジオメトリ キャッシュ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# ジオメトリ キャッシュ

ベイク処理では、メッシュをクリーンアップするために事前に処理し、ベイク処理と互換性のある形式で変換します。 ジオメトリ キャッシュは、この前処理済みジオメトリを高速にリロードして、後でこの操作をやり直さないように保持する方法です（ソース メッシュが変更されない限り）。

* **Substance Designer**&#x200B;では、最初のベイク実行後にジオメトリ キャッシュが作成されます。 その後、ベーカーウィンドウが閉じるまで、キャッシュはメモリ内に保持されます。
* **Substance Painter**&#x200B;では、ジオメトリ キャッシュは、最初のベイクの後、ソース ファイルの横に&#x200B;**assbin**&#x200B;という拡張子のファイルとして保存されます。

ジオメトリ キャッシュを再利用すると、特にベイカーの設定を微調整して完璧な結果を得る場合は、ベイク処理が大幅にスピードアップします。
