---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ''
description: 3ds Max用のSubstanceプラグインと、Substanceマテリアルをプロジェクトに読み込んで使用する方法について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds MaxのSubstanceの概要
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# 3ds MaxのSubstanceの概要

## プラグインの概要

## Substanceのオープン

1. スレートエディタを開き、「Substance」を検索し、「Substance2」ノードをビューにドラッグします。
1. Substanceノードをダブルクリックしてプロパティをアクティブにし、[Substanceパッケージブラウザ]でSubstanceをロードします。

   >[!NOTE]
   >
   > また、.sbsarファイルをスレートエディターにドラッグ&amp;ドロップして、ノードを自動的に作成し、スバーを読み込むこともできます。
1. Substanceに複数のグラフが含まれている場合は、マテリアルとして出力するグラフを「選択したグラフ」ドロップダウンメニューで選択できます。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max8?$png$&jpegSize=100&wid=341)

   ![](../../../assets/max1.png)
1. Substanceノードを選択した状態で、「Substance」メニューに移動し、サポートされているレンダラーを選択します。 マテリアルが作成され、オブジェクトに適用できるようになります。 Substanceテクスチャがレンダリングマテリアルにフックされます。

   | サポートされるレンダラー |
   | --- |
   | アーノルド |
   | Vray |
   | コロナ |
   | オクタン |

   ![](../../../assets/max3.png)

## 解像度の変更：

1. Substanceの出力設定で、計算されたSubstanceテクスチャの解像度を設定します。
1. 解像度を最大8Kにするには、[Substance設定](../../../3d-applications/3ds-max/settings-1/substance-settings.md)で設定されているGPUエンジンを使用していることを確認してください。

   ![](../../../assets/max6.png)

## パラメータの変更：

1. Substanceノードをダブルクリックして、パラメータウィンドウにSubstanceパラメータを読み込みます。
1. パラメーターを変更すると、Substanceテクスチャが自動的に更新されます。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## 出力プレビューの設定：

Substanceノードのサムネールにチャンネルを指定できます。

1. 出力プレビュードロップダウンで、ノードサムネールに使用するチャンネルを選択します。

   ![](../../../assets/max7.png)

## タイリングSubstance:

[座標]プロパティを使用すると、Substanceテクスチャを並べて表示したり、マップチャンネルを設定することができます。

![](../../../assets/max10.png)
