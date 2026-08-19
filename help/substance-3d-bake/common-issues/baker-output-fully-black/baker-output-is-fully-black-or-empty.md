---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/baker-output-is-fully-black-or-empty.html"
breadcrumb-title: ''
description: ベイカー出力が完全に黒または空になる理由をトラブルシューティングし、メッシュとUVの問題を修正する方法を説明します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baker output is fully black or empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ベイカー出力が完全に黒または空です
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# ベイカー出力が完全に黒または空です

>[!WARNING]
>
> **問題**
> 
> パン屋の結果は、黒または空のテクスチャです。
> 
> ![](../../assets/black.png)

>[!NOTE]
>
> **説明**
> 
> 黒いテクスチャは、パン屋が結果を出力するために必要な情報を見つけることができなかったことを意味します。 例えば、ベイク処理では、ローポリと一致するハイポリメッシュが見つからず、比較するものが何も見つかりませんでした。

>[!NOTE]
>
> **解決策**
> 
> * ベイカーに必要なハイポリメッシュが正しく読み込まれたかどうかを確認します（エラーについては、ログファイル/ウィンドウを参照）。
> * ローポリメッシュまたはハイポリメッシュが大きすぎる（1 キロメートル以上）または小さすぎる（1 センチメートル未満）ことを確認します。
> * ベイカーがメッシュを読み取り/処理できたかどうかを確認します（エラーについては、ログファイル/ウィンドウを参照してください）。
> * 名前で一致する[機能が正しく設定されていなかったかどうかを確認します（一部のオブジェクトは互いに除外され、重複しない場合があります）。](../../features/matching-by-name/matching-by-name.md)
> * ローポリ UVが0 ～ 1の範囲内にあることを確認します。
