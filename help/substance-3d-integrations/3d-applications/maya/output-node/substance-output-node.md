---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/maya/substance-output-node.html"
breadcrumb-title: ''
description: MayaのSubstance出力ノードを使用して、計算されたテクスチャをシェーダーネットワークに接続する方法について説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance Output Node
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance出力ノード
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Substance出力ノード

Substance出力ノードは、Substance engineから計算されたテクスチャへの参照です。 Substanceノードに接続されています。 Substanceノードに出力が作成されると、Substanceエンジンはテクスチャを計算し、このデータはRAMに保持されます。 GPU エンジンを使用する場合、データはGPUで計算され、Substance GPU ブレンドエンジンを使用してメモリに返されます。 アクティブ化されていないSubstanceノードの出力は計算されません。

![](../../../assets/outputnode.png)

このノードでは、出力の識別子、ラベル、使用状況セットなどの出力Substance Designerが表示されます。 「出力キャッシュ」セクションでテクスチャをディスクにベイクすることもできます。
