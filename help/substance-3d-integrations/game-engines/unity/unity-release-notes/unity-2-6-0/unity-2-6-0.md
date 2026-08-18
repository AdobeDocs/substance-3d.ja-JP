---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-6-0.html"
breadcrumb-title: ''
description: Unityプラグインバージョン2.6.0のリリースノートを確認して、新機能、改善点、およびバグ修正について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.6.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.6.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Unity 2.6.0

2021年6月7日リリース

更新/追加：

* Substance Sourceにアクセスするための新しいワークフロー Substance SourceアクションはSubstanceランチャー内の「ソース」タブにアクセスし、アセットをUnityに直接送信できるようになりました
* プラグインのバージョン情報をクリップボードにコピー可能
* ターゲット設定から「ロード時に生成」が削除されました

修正：

* HDRPプロジェクトでは、マテリアル設定に変更を加えると、ディスプレイスメントモードがデフォルト値(Tessallation)に戻ります
* 解像度サイズが「インスペクタ」ウィンドウに表示されない
* Unityバージョン2020.2以降にプラグインをインストールできない

既知の問題：

* バージョン2.5.4以前からプラグインをアップデートすると、アクセス拒否エラーやクラッシュが発生する
  * 回避策：プラグインバージョン2.5.4以前のバージョンは、プラグインバージョン2.6.0をインストールする前に、Unityプロジェクトバージョン2020.2以降からアンインストールする必要があります
* Substanceプラグインがインストールされている場合、イメージファイルのテクスチャプレビューはインスペクターに表示されません
  * この問題の原因はUnity内に存在し、2021.2バージョン（現在ベータ版）内でUnityによって修正される予定です
