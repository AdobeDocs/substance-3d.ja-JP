---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/what-is-the-difference-between-the-opengl-and-directx-normal-format.html"
breadcrumb-title: ''
description: OpenGLとDirectX法線マップ形式の違いと、それぞれの形式を使用するタイミングについて説明します。
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > What is the difference between the OpenGL and DirectX normal format "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'OpenGLとDirectX通常の形式の違いは何ですか '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---


# OpenGLとDirectXの通常の形式の違いは何ですか？

>[!WARNING]
>
> **質問**
> 
> OpenGLとDirectXの通常の形式の違いは何ですか？

>[!NOTE]
>
> **説明**
> 
> OpenGLとDirectXは、プログラマーがGPU （Graphic Processing Unit）と対話するアプリケーションで使用する2つのグラフィック API （一連の関数）です。 通常のマップでは、RGB テクスチャのグリーン チャンネルの解釈に違いが生じます。 OpenGLでは、最初のピクセルが一番下にあることが想定され、DirectXでは、最初のピクセルが一番上にあることが想定されます。 このため、様々な技術的な議論では、法線マップの緑のチャンネルを反転して、ピクセル値を反転する（最初に最後になる）際により良い動作をするかどうかを確認することをお勧めします。 OpenGLは&#x200B;**Y+** （ボトムアップ）と呼ぶことができ、DirectXは&#x200B;**Y-** （トップダウン）と呼ばれます。
> 
> 使用する形式については、テクスチャを使用するターゲットアプリケーションを参照してください。
