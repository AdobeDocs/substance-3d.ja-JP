---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/rendering-color-space.html"
breadcrumb-title: ''
description: Unityのカラースペース設定を行い、物理ベースのシェーダを使用してマテリアルを適切にレンダリングできるようにします。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Rendering Color Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: カラースペースをレンダリング中
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# カラースペースをレンダリング中

テクスチャは、物理ベースのシェーダーで使用するように設計されています。 最良の結果を得るには、Unity Player設定でカラースペースをリニアに設定する必要があります。

1. 編集/プロジェクト設定/プレーヤーに移動
1. レンダリングセクションで、カラースペースをリニアに変更します。 （Unityのデフォルトはガンマ空間です。これは正しくなく、テクスチャのカラーが正しく表示されません）。

   >[!NOTE]
   >
   > **情報**
   > 
   > Unityのカラースペース設定がガンマに設定されている場合、テクスチャのsRGBオプションは無効になります

   ![](../../../assets/rendering-4.png){width="600px"}
