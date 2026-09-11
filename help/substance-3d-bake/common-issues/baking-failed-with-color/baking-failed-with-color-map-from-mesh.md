---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: メッシュからのカラーマップの色のプロパティとUVのマッピングを確認して、メッシュのベイクエラーを解決します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baking failed with Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからのカラーマップでベイク処理が失敗しました
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# メッシュからのカラーマップでベイク処理が失敗しました

>[!WARNING]
>
> **問題**
> 
> 考えられるエラーメッセージ：
> 
> > > > 
> 
> [ベイク]ベイクに失敗しました(メッシュからのカラーマップ)\
> 頂点カラーが見つかりませんでした

>[!NOTE]
>
> **説明**
> 
> [メッシュからのカラーマップ](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)の既定の設定では、メッシュのUVに基づいて、高ポリゴンのメッシュ頂点の色がテクスチャにベイクされます。 ただし、多くの場合、high-poly メッシュには頂点カラー情報がありません。 したがって、ベイカーは存在しない情報を書き込むことができません。

>[!NOTE]
>
> **解決策**
> 
> このエラーメッセージを回避するには、さまざまな解決策を利用できます。
> 
> * 頂点なカラーを持つハイポリメッシュを使用する
> * ベイカーを設定します
> * 不要な場合は、ベイカーを使用しないでください
