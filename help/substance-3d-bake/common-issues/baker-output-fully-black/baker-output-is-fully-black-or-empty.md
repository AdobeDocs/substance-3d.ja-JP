---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baker-output-is-fully-black-or-empty.html"
breadcrumb-title: ''
description: パン屋の出力が完全に黒または空である理由のトラブルシューティングと、メッシュとUVの問題を修正する方法について説明します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baker output is fully black or empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ベイカーからの出力が完全に黒または空
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# ベイカーからの出力が完全に黒または空

>[!WARNING]
>
> **問題**
> 
> パン屋の結果は、黒または空のテクスチャになります。
> 
> ![](../../assets/black.png)

>[!NOTE]
>
> **説明**
> 
> 黒いテクスチャは、結果を出力するために必要な情報がパン屋によって見つからなかったことを意味します。 たとえば、ベイク処理では、ローポリゴンと一致するハイポリゴンメッシュは見つからず、比較するものはありません。

>[!NOTE]
>
> **解決策**
> 
> * ベイカーに必要な高ポリゴンメッシュが正しくロードされたかどうかを確認します（エラーについては、ログファイルまたはウィンドウを参照してください）。
> * ローポリゴンメッシュまたはハイポリゴンメッシュが大きすぎたり（1キロメートルを超える）、小さすぎたり（1センチメートル未満）していないことを確認します。
> * ベイカーがメッシュを読み取り/処理できたかどうかを確認します（エラーについては、ログファイル/ウィンドウを参照してください）。
> * [名前による一致](../../features/matching-by-name/matching-by-name.md)機能が適切に設定されていないことを確認してください（一部のオブジェクトは、互いを除外し、重なり合わない場合があります）。
> * ローポリUVが0 ～ 1の範囲内にあることを確認します。
