---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-2.html"
breadcrumb-title: ''
description: Unityプラグインバージョン2.5.2のリリースノートを確認して、新機能、改善点、バグ修正について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.5.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Unity 2.5.2

2020年7月23日リリース

追加：

* レンダラーがビジー状態か、アイドル（ビジーでない）かを示す「IsProcessing()」関数

修正：

* 2048クランプおよび4096ターゲット設定の設定時にエラーが表示されなくなりました
* 標準からHDRPやURPにアップグレードすると、マテリアルプロパティが引き継がれます。
* モバイルにデプロイする場合、Substanceのマテリアルを変更するスクリプトは想定どおりに動作します
* レッドチャンネルはAlphaにコピーされなくなり、デフォルトのAlphaは白に設定される
* Macでターゲット設定を変更するとクラッシュする
* Unityマテリアルの作成時にNullReferenceExceptionエラーが削除されました
* タイリングプロパティの編集後に再生モードを終了すると、エラーが削除されました
* 「 GPUインスタンス化を有効にする」を有効にできる
* 既存の再生モードで、透明を使用しているマテリアルが消えたり、誤って黒くなったりすることはありません
* プラグインのアップグレード時に、HDRPプロジェクトでSubstanceのマテリアルが破棄されない
