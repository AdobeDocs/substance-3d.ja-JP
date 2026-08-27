---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-4.html"
breadcrumb-title: ''
description: Unityプラグインバージョン2.4.4のリリースノートを確認して、新機能、改善点、バグ修正について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Unity 2.4.4

2020年2月リリース

* 追加： 2019.3の適切なサポート：Substanceプラグインのスクリプト可能なオブジェクトを壊すUnity APIの変更を修正しました。 2019.3 APIアップデートで動作するようにオブジェクトを修正しました。 修正 – カスタムマテリアルを使用すると、プレイ終了時にマテリアルが黒くなる
* 修正 – スクリプトでDuplicate()関数を使用した後、再生を開始および終了するとクラッシュする。
* 固定 – 2019.3でのマテリアルのタイリング、設定、およびシェーダのリセット
* 固定 – HDRPマテリアルシェーダでパラメータの変更が更新されない
* 修正 – HDRPマスクマップが更新されない
* 固定 – 重複する関数の文字列パラメータを追加します。
* 修正 – 最新のUnity StableでのLinuxのサポートを修正
* 修正 – iOSでビットコードを無効にする必要がある問題の解決

既知の問題：

* HDRPアセットの名前を変更すると、プラグインでマスクマップが生成されなくなります。
* HDRPプロジェクトでSubstanceプラグインを使用しているときに、Raw圧縮を使用すると、グレースケールテクスチャがAlpha8に設定される。
* GameObjectsは再生モードで選択解除されます
* 再生モードでSubstanceグラフの「Generate Mip Maps」をクリックすると、パラメーターを変更した結果、ハングが無限に発生します。
