---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/live-link-in-ue4.html"
breadcrumb-title: ''
description: Unreal Engine 4のLive Linkを使用すると、PainterとUE4の間でSubstance素材をリアルタイムで同期できます。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Live Link in UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UE4でのライブリンク
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---


# UE4でのライブリンク

>[!WARNING]
>
> Unreal Engineでのライブリンクのサポートは終了しました。 ライブリンクを使用している古いバージョンのプラグインを使用しているユーザーは、引き続きこの機能を使用できます。

>[!WARNING]
>
> ライブリンクはUE4 BSPメッシュでは機能しません。 送信するアセットは、UE4プロジェクトにインポートされたモデルファイルである必要があります

## Substance Painterへのリンクを確立中

1. Substance Painterを開く
1. コンテンツブラウザーで、Painterに送信するアセットを右クリックし、「Painterに送信」を選択します。

   ![](../../../../assets/link1-22.png){width="400px"}
1. メッシュがSubstance Painterに表示され、テクスチャリングを開始できます。 作業を進めると、テクスチャがUE4に送信され、マテリアルに適用されます。 ツールバーのUE4アイコン上の緑色の点は、リンクがライブでテクスチャを送信していることを示します。

   ![](../../../../assets/icon-12.png)

   1. プラグインの「設定」オプションで、データのストリーミングを一時停止できます。 プラグイン/dcc-live-linkに移動し、「設定」を選択します。 「ストリーミングを有効にする」を無効にして、UE4へのデータの送信を一時停止します。

      ![](https://helpx-prod.scene7.com/is/image/HelpxProd/config-6?$png$&jpegSize=100&wid=393)
1. Painterのテクスチャがコンテンツブラウザーに表示され、UE4でマテリアルに適用されます。

   ![](../../../../assets/link3-11.png){width="500px"}
1. Substance Painterプロジェクト(.spp)は、「.sp」というラベルの付いたフォルダーのUE4プロジェクトフォルダーに作成されます

   ![](../../../../assets/link4-5.png)

## Substance Painterへのリンクの再設定

PainterまたはUnityを閉じた後、中断したところから再開できます。

1. Unityプロジェクト>assets>.spフォルダにあるSubstance Painterで、.sppプロジェクトを開きます。
1. [コンテンツブラウザ]でメッシュを右クリックし、[Painterに送信]を選択してリンクを再設定します。

   ![](../../../../assets/link5-3.png){width="600px"}
