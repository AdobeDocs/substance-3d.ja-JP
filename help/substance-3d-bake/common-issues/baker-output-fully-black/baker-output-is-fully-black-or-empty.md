---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/baker-output-is-fully-black-or-empty.html"
breadcrumb-title: ''
description: ベイカー出力が完全に黒または空になる理由をトラブルシューティングし、メッシュとUVの問題を解決する方法を説明します。
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
> ベイカーの結果は、黒または空のテクスチャになります。
> 
> ![](../../assets/black.png)

>[!NOTE]
>
> **説明**
> 
> 黒いテクスチャは、結果を出力するために必要な情報がベイカーによって見つからなかったことを示します。 例えば、ベイクプロセスでは、high-polyメッシュがlow-polyと一致するようには見つからず、比較するものはありませんでした。

>[!NOTE]
>
> **解決策**
> 
> * ベイカーに必要なhigh-polyメッシュが正しくロードされているかどうかを確認します（エラーについては、ログ・ファイルまたはウィンドウを参照してください）。
> * ローポリまたはハイポリメッシュが大きすぎない（1キロメートルを超える）か、小さすぎない（1センチメートル未満の）ことを確認します。
> * ベイカーがメッシュを読み取り/処理できたかどうかを確認します（エラーについては、ログファイルまたはウィンドウを参照してください）。
> * [名前による一致](../../features/matching-by-name/matching-by-name.md)機能が適切に設定されていないことを確認してください（一部のオブジェクトは、互いを除外し、重なり合わない場合があります）。
> * ローポリUVが0 ～ 1の範囲内にあることを確認します。
