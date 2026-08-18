---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: メッシュのカラープロパティとUVマッピングをチェックして、メッシュのベイク処理の失敗からカラーマップを解決します。
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
> &#x200B;> > > 
> 
> [ベイク処理]ベイク処理に失敗しました（メッシュからのカラーマップ）\
> 頂点カラーが見つかりませんでした

>[!NOTE]
>
> **説明**
> 
> [メッシュからのカラーマップ](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)のデフォルト設定では、メッシュのUVに基づいて、高ポリゴンメッシュの頂点カラーをテクスチャにベイク処理します。 ただし、多くの場合、高ポリゴンメッシュには頂点カラー情報がありません。 そのため、パン屋は存在しない情報を書き込むことができない。

>[!NOTE]
>
> **解決策**
> 
> このエラーメッセージを回避するには、さまざまな解決策を利用できます。
> 
> * 頂点カラーを持つ高ポリゴンメッシュを使用する
> * 異なる設定を使用して、メッシュのベイカーからカラーマップを設定します
> * 必要がない場合は、Mesh Bakerのカラーマップを使用しないでください
