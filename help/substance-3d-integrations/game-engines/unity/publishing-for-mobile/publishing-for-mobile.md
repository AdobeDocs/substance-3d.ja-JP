---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/publishing-for-mobile.html"
breadcrumb-title: ''
description: マテリアルとテクスチャ解像度を調整して、Unityのモバイルプラットフォーム向けのSubstance設定を最適化します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Publishing for Mobile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: モバイル用にパブリッシュ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# モバイル用にパブリッシュ

>[!NOTE]
>
> **モバイルデバイスのテクスチャサイズ**
> 
> Unity Editorのテクスチャセットの解像度は、アプリケーションバイナリでパブリッシュされるサイズになります。 Substanceマテリアルの解像度を下げると、ファイルサイズが小さくなるテクスチャが作成されます。

## プラットフォーム

## Apple iOS

1. 対応するUnityバージョンのiOSモジュールがダウンロードされていることを確認します。
1. Unityで、build targetをiOSに変更します。
1. Player Settingsを開き、「Identification - Bundle Identifier」フィールドを他と異なる識別子に変更します。 （例：com.Adobe.iosProject）
1. ゲームをビルドして実行します。
1. Xcodeで、iOSデバイスをクリックし、「Signing - Team」ドロップダウンをデベロッパーチームIDに変更します。
1. iOSデバイスで、「Settings - General - Device Management」に移動し、表示されるDeveloper Team IDの「Trust」をクリックします。
1. 「現在のスキームをビルドして実行」ボタン（再生ボタン）をクリックして、Xcodeビルドを再実行します。
1. ゲームはiOSデバイスで実行されている必要があります。

## Android OS

1. 対応するUnityバージョンのAndroidモジュールがダウンロードされていることを確認してください。
1. Unityで、build targetをAndroidに変更します。
1. Player Settingsを開き、「Identification - Bundle Identifier」フィールドを他と異なる識別子に変更します。 （例：com.Adobe.androidProject）
1. ゲームをビルドして実行します。
1. ゲームはAndroidデバイスで実行されている必要があります。
