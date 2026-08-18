---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/what-are-assbin-files.html"
breadcrumb-title: ''
description: Assbinファイルとは何か、またベイク処理を高速化するためにジオメトリキャッシュファイルとしてどのように使用されるかについて説明します。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > What are Assbin files "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Assbinファイルとは '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# Assbinファイルとは

>[!WARNING]
>
> **質問**
> 
> Substance Painterでベイク処理を行った後、ハイポリゴンメッシュの横に、ファイル拡張子が「assbin」のファイルが1つまたは複数あるのが見つかりました。これは何ですか？ 安全に削除できますか？

>[!NOTE]
>
> **解決策**
> 
> Assbinファイルは、ベイク処理時に使用される高ポリゴンメッシュの前処理されたバージョンです。 ベイカー設定を繰り返す際に、元のメッシュファイルよりも読み取りが高速になり、再ベイク処理が高速になります。 これらは安全に取り外すことができます。 Substance Painterは必要に応じて再生成します。 ただし、これはベイク処理のパフォーマンスに影響を与える可能性があります。
> 
> Substance Painter[メインの環境設定](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/general-71008262.html)で、「前処理されたシーンファイルを保存」オプションを無効にすると、これらのファイルを生成しないことがあります。
