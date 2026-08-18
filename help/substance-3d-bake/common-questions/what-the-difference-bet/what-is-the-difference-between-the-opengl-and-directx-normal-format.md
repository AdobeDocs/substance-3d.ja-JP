---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-questions/what-is-the-difference-between-the-opengl-and-directx-normal-format.html"
breadcrumb-title: ''
description: OpenGL形式とDirectX形式の違いと、各法線マップ形式をいつ使用するかについて説明します。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > What is the difference between the OpenGL and DirectX normal format "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'OpenGLとDirectX標準フォーマットの違いは何ですか？ '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---


# OpenGLとDirectX標準フォーマットの違いは何ですか？

>[!WARNING]
>
> **質問**
> 
> OpenGLとDirectX標準フォーマットの違いは何ですか？

>[!NOTE]
>
> **説明**
> 
> OpenGLとDirectXは、プログラマがGPU(Graphic Processing Unit)との対話にアプリケーションで使用する2つのグラフィックAPI（関数のセット）です。 法線マップに関しては、RGBテクスチャの緑チャンネルの変換方法が異なります。 OpenGLでは、最初のピクセルが一番下にあり、DirectXでは一番上にあるものと想定しています。 このため、さまざまな技術的な議論では、通常マップの緑チャンネルを反転させて、ピクセル値が反転する（最初が最後になる）ときの動作が適切かどうかを確認することをお勧めします。 OpenGLは&#x200B;**Y+** （ボトムアップ）と呼ばれ、DirectXは&#x200B;**Y-** （トップダウン）と呼ばれます。
> 
> 使用する形式を確認するには、テクスチャを使用するターゲットアプリケーションを参照してください。
