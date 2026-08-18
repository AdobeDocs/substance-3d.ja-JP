---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/texture-baked-outside-of-substance-software-looks-incorrect.html"
breadcrumb-title: ''
description: Substanceソフトウェア以外でベイク処理されたテクスチャが正しく表示されない理由のトラブルシューティングと、カラースペースの問題を修正する方法について説明します。
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Texture baked outside of Substance software looks incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substanceソフトウェア以外でベイク処理されたテクスチャが正しく表示されない
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Substanceソフトウェア以外でベイク処理されたテクスチャが正しく表示されない

>[!WARNING]
>
> **質問**
> 
> Substance Bakersではなく、外部アプリケーションでベイク処理したテクスチャが、Substance Painterーで正しく表示されないのはなぜですか？

>[!NOTE]
>
> **解決策**
> 
> 多くの要因がこの問題に寄与する可能性があるため、この問題に対する差し迫った解決策はありません。
> 
> * Substanceソフトウェアと外部アプリケーションの間の通常のフォーマットが同じであることを確認します。 OpenGLは[X+, Y+, Z+]で、DirectXは[X+, Y-, Z+]です
>   * Substance Painterでは、通常の形式は[プロジェクト構成](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/interface/project-configuration)で変更できます。
>   * Substance Designerでは、通常の形式は[プロジェクトの環境設定](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/workspace/preferences/project-settings)で変更できます。
> * ベイク処理してSubstanceソフトウェアに読み込む前に、メッシュが三角化されていることを確認します。 詳細については、[このページ](../../guides/triangulating-before-bak/triangulating-before-baking.md)を参照してください。
