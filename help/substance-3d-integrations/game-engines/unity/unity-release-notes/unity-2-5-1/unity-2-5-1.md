---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-1.html"
breadcrumb-title: ''
description: Unityプラグインバージョン2.5.1のリリースノートを確認して、新機能、改善点、バグ修正について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.5.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Unity 2.5.1

2020年5月21日リリース

追加日

* ユニバーサルレンダリングパイプラインのサポート：テクスチャは、URPシェーダとマテリアルを自動的に使用します。

固定

* Substance CPU エンジンの最大解像度設定：
  * Substance設定メニューのフィールド名を「テクスチャクランプ\*\*」から「Substance CPUエンジン最大解像度」に更新しました。
  * 設定が変更されると、すべてのSubstanceマテリアルが再読み込みされることを示す警告通知が表示されます
* インストール時に表示された不要なデバッグメッセージ(&quot;TextureClamp = 4096 Unity.Debug:Log(Object)&quot;)が削除されました
* HDRPプロジェクト：標準マテリアルとHDRPマテリアルの両方に含まれるマテリアルプロパティは、Substanceを含むパッケージが読み込まれたときに引き継がれます
* 以前のUnityバージョンにあったSubstanceのパッケージからSubstanceのマテリアルが読み込まれると、リフレクションとHDRPマスクが正常に作成され、機能します
* 複製機能を使用すると、複製されたマテリアルは意図したカラーになり、黄色ではなくなります
* Unityを閉じて再び開くと、Substanceソースが正常にロードされます
* パッケージをHDRPプロジェクトに読み込む際のクラッシュ（断続的に）
* EditorがColor(Grayscale)に設定された公開パラメータを持つSubstanceマテリアルでは、Sliderは想定どおりに動作します
* デフォルトの解像度のないSubstanceグラフで「プリセットをデフォルトにリセット」をクリックするとクラッシュする
* 出力サイズパラメーターが表示されていない場合にSubstanceマテリアルーの出力サイズを変更すると、クラッシュが発生します
* iOSの構築は失敗しません
* Windows Standalone用に構築すると、マテリアルを使用するスクリプトが実行されます
