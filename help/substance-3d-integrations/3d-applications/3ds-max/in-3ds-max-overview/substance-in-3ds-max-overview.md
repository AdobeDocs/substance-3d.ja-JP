---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ""
description: 3ds MaxのSubstanceプラグインと、Substance マテリアルをプロジェクトに読み込んで使用する方法について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds MaxのSubstanceの概要
user-guide-description: ""
user-guide-title: ""
source-git-commit: a167bcd2c2f0af70b3a4dc37eafc85145c79c590
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%
---

# 3ds MaxのSubstanceの概要

## プラグインの概要

## Substanceのオープン

1. スレートエディタを開き、「Substance」を検索し、「Substance2」ノードをビューにドラッグします。
1. Substanceノードをダブルクリックしてプロパティをアクティブにし、[Substanceパッケージブラウザ]でSubstanceをロードします。

   >[!NOTE]
   >
   > .sbsar ファイルをスレートエディターにドラッグ&amp;ドロップして、ノードを自動作成し、スバーを読み込むこともできます。

1. Substanceに複数のグラフが含まれている場合は、マテリアルとして出力するグラフを「選択したグラフ 」ドロップダウンメニューで選択できます。

   ![](../../../assets/max1.png)

1. Substanceノードを選択した状態で、「Substance」メニューに移動し、サポートされているレンダラーを選択します。 マテリアルが作成され、オブジェクトに適用できるようになります。 テクスチャはレンダリングマテリアルに接続されます。

>[!NOTE]
>
> **«Substance2 »**&#x200B;ノードを選択したら、最初に&#x200B;**[読み込み] Substance...**&#x200B;をクリックしてsbsar ファイルを選択し、上部メニューからサポートされているレンダラーを選択する必要があります（「ArnoldにSubstance」など）。
>
>サポートされるレンダラーには、Arnold、V-Ray、Corona、Octaneなどがあります。 [OpenPBR マテリアルの使用方法については、3DS Maxのワークフローを参照してください。](../using-workflows-3ds-max/using-workflows-in-3ds-max.md)

![](../../../assets/max3.png)

## 解像度の変更

1. Substanceの出力の設定で、計算されたSubstanceテクスチャの解像度を設定します。
1. 解像度を最大8Kにするには、[Substance設定](../../../3d-applications/3ds-max/settings-1/substance-settings.md)で設定されているGPU エンジンを使用していることを確認してください。

   ![](../../../assets/max6.png)

## パラメータの変更

1. Substanceノードをダブルクリックして、パラメータウィンドウにSubstanceパラメータを読み込みます。
1. パラメーターを変更すると、テクスチャが自動的に更新されます。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## 出力プレビューの設定

Substanceノードのサムネールにチャンネルを指定できます。

1. 出力プレビュードロップダウンで、ノードサムネールに使用するチャンネルを選択します。

   ![](../../../assets/max7.png)

## Substance

[座標]プロパティを使用すると、テクスチャを並べて表示したり、マップチャンネルを設定することができます。

![](../../../assets/max10.png)
