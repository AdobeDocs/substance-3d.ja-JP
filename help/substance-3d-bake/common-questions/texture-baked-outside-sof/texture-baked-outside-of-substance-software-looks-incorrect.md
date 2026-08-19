---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/texture-baked-outside-of-substance-software-looks-incorrect.html"
breadcrumb-title: ''
description: Substance ソフトウェアの外でベイク処理されたテクスチャが正しく見えない理由をトラブルシューティングし、カラースペースの問題を修正する方法を説明します。
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Texture baked outside of Substance software looks incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance ソフトウェアの外部でベイク処理されたテクスチャが正しく表示されない
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Substance ソフトウェアの外部でベイク処理されたテクスチャが正しく表示されない

>[!WARNING]
>
> **質問**
> 
> Substance PainterでSubstance Bakersではなく、外部アプリケーションで焼いたテクスチャが正しく表示されないのはなぜですか？

>[!NOTE]
>
> **解決策**
> 
> この問題に多くの要因が寄与する可能性があるため、この問題に対する即時的な解決策はありません。
> 
> * Substance ソフトウェアと外部アプリケーションの間の通常の形式が同じであることを確認します。 OpenGLは[X+, Y+, Z+]で、DirectXは[X+, Y-, Z+]です
>   * Substance Painterでは、[ プロジェクト設定](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/interface/project-configuration)で通常の形式を変更できます。
>   * Substance Designerでは、[ プロジェクトの環境設定](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/workspace/preferences/project-settings)で通常の形式を変更できます。
> * Substance ソフトウェアにベイク処理して読み込む前に、メッシュが三角形になっていることを確認します。 詳しくは、[このページ ](../../guides/triangulating-before-bak/triangulating-before-baking.md)を参照してください。
