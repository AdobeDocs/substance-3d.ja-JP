---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/upgrading-projects-known-issues.html"
breadcrumb-title: ''
description: Unityプロジェクトをマテリアルでアップグレードする方法と、マイグレーション中に避けるべき既知の問題について説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Upgrading ProjectsKnown Issues
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: プロジェクトのアップグレードの既知の問題
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---


# プロジェクトのアップグレード/既知の問題

>[!WARNING]
>
> Unity 3.0.0用のSubstance 3Dプラグインは、下位互換性をサポートしていません。 したがって、必ずUnity 2020.3.27x以降を使用してください。
> 
> Unityはデフォルトのビルドアーキテクチャをx86\_64ではなくx86に変更しました。\
> スクリプトがSubstanceを参照している場合、スクリプトは実行されません。 x86\_64に戻さないとビルドは動作しません。

## 既知の問題

* パネルフォルダーのナビゲーション中に「*式でのアサーションに失敗しました」というエラーが発生しました。*
  * これは、UIに変更が加えられた場合にUnity側で発生するエラーです。通常、サムネイルの変更は無害なメッセージである必要があります。
* *画像入力が8ビットにロックされているようです*
  * この問題は、バージョン3.8.0 ～ 3で修正されました。 正しい手順は、テクスチャに対するUnityのデフォルトフォーマットをRGBA64に変更することです。 プラグインは、その情報をSubstance engineに適切に送信します。
