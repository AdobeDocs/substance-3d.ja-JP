---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/geometry-cache.html"
breadcrumb-title: ''
description: ジオメトリキャッシュを使用すると、事前に処理されたメッシュデータを保持し、その後のベイク処理処理を大幅に高速化できます。
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

ベイク時には、メッシュは前処理されてクリーンアップされ、ベイクプロセスと互換性のあるフォーマットに変換されます。 ジオメトリキャッシュを使用すると、事前に処理されたこのジオメトリを後で再ロードしないようにすばやく保持できます（ソースメッシュが変わらない場合）。

* **Substance Designer**&#x200B;では、最初のベイクが実行された後にジオメトリキャッシュが作成されます。 キャッシュは、ベイカーウィンドウが閉じられるまでメモリに保持されます。
* **Substance Painter**&#x200B;で、ジオメトリキャッシュは、最初のベイク後にソースファイルの横に拡張子&#x200B;**assbin**&#x200B;の付いたファイルとして保存されます。

ジオメトリキャッシュを再利用すると、特にベイカー設定を微調整して完璧な結果を得る場合に、ベイク処理プロセスが大幅に高速化されます。
