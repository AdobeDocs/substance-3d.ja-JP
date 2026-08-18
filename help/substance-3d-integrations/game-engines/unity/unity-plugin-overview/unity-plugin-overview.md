---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/unity-plugin-overview.html"
breadcrumb-title: ''
description: バージョンのサポート、機能、統合機能を含む、Unity用Substance 3Dプラグインについて説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Plugin Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unityプラグインの概要
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Unityプラグインの概要

## Unityバージョンのサポート

Adobe Substance 3D for Unityプラグインバージョン3.0.0は、現在Unity 2020 LTS以降をサポートしています。

## Substanceパッケージのダウンロード

1. プラグインはUnityアセットストアからダウンロードできます： <https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208>

## Substanceマテリアルを読み込む

1. プロジェクトウィンドウで右クリックし、「アセットを読み込み」を選択するか、読み込むSubstanceマテリアルをプロジェクトビューパネルにドラッグします。
1. 読み込むSubstanceマテリアルを参照します。 Substanceマテリアルのファイル拡張子は「.sbsar」です。
1. Substance素材がUnityプロジェクトに読み込まれます。

   1. sbsarアセットは、メインの読み込みファイルと、出力テクスチャおよび生成されたUnityマテリアルを含むフォルダーを作成します。
1. 次に、[シーンビュー]のメッシュにマテリアルをドラッグアンドドロップし、[インスペクタ]でパラメータを編集します。

   ![](../../../assets/window-overview.png){width="1000px"}

>[!NOTE]
>
> **標準マップの変換**
> 
> UnityプラグインのSubstanceは、DirectXを自動的にOpenGLに変換します。 [Substance Source](https://source.substance3d.com/)のマテリアルを使用する場合、法線の方向をOGLに変更する必要はありません。 Substance Designerで独自のマテリアルを作成する場合は、デフォルトのDirectXシェーダを使用してください。 詳細は、Unityでの法線の操作を参照してください。

## パラメータの変更

パラメータと解像度は、「インスペクタ」ウィンドウで設定できます。 [パラメーターの変更](../../../game-engines/unity/changing-parameters/changing-parameters.md)を参照してください。

[unity\_tweaking\_parameters.mp4](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/download/attachments/186056716/unity-tweaking-parameters.mp4)

## Unityレンダリングパイプラインのサポート

Substance 3DプラグインはHDRPおよびURPをサポートしています。 詳細については、近日中に公開されます。

## チュートリアルを見る
