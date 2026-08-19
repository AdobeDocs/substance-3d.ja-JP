---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/why-are-there-strange-stretches-in-my-textures-after-baking-or-exporting.html"
breadcrumb-title: ''
description: UV マッピングまたはメッシュの問題によって生じる、ベイク処理されたテクスチャの奇妙な伸縮を特定して修正します。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Why are there strange stretches in my textures after baking or exporting "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: '焼いたり書き出したりした後、テクスチャに奇妙な伸縮が生じるのはなぜですか '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '108'
ht-degree: 0%

---


# 焼いたり書き出したりした後に、テクスチャに奇妙な伸縮が生じるのはなぜですか？

>[!WARNING]
>
> **質問**
> 
> 焼いたり書き出したりした後、UV島の外に奇妙な伸びた線やカラフルなグラデーションがあるのはなぜですか？

>[!NOTE]
>
> **解決策**
> 
> Substance Bakersは、UV島の外側にディフュージョンとディレイションの両方を適用してギャップを埋め、mipmapが生成されるときにゲームエンジンでテクスチャが正常に動作することを確認します。 詳しくは、[ パディング ](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/padding-134643719.html)を参照してください。
