---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-5.html"
breadcrumb-title: ''
description: Unityプラグインバージョン2.4.5のリリースノートを確認して、新機能、改善点、およびバグ修正について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Unity 2.4.5

2020年4月6日リリース

* 追加： 2019.3 APIを使用したHDRPアセットチェック
* 追加：Substance engine 7.2アップデート – ソースからの一部のSubstance マテリアルが機能しない問題を修正
* 追加：CPUの解像度に合わせてターゲット設定を更新
* 追加：CPUエンジンの最大解像度設定（4Kまたは2K設定）
* 追加：HDRPプロジェクト内のHDRP以外のSubstanceを変換
* 修正：大量のSubstanceを読み込む際のクラッシュ
* 修正：Substanceパラメーターを変更した後、再生モードで「再読み込み」をクリックすると例外が発生する
* 修正：出力(テクスチャ)解像度を検証する（APIでCPU エンジンを2Kに制限）。ユーザー設定でデフォルトを4Kに設定する
* 修正：再生モードでグラフの「Generate Mip Maps」をクリックすると、パラメーターを変更するとハングが無限に発生する
* 修正：HDRPプロジェクトでSubstanceプラグインを使用しているときに、RAW圧縮を使用すると、グレースケールテクスチャがAlpha8に設定される
* 修正：再生モードでGameObjectの選択を解除
* 修正：パラメーターの変更でラフネスマップが更新されません
* 修正：HDRPで一部のSubstanceファイルのマスク出力が正しく生成されない
* 修正：パックされたアルファマップドロップダウンを2つのオプション間で切り替える際のクラッシュ
* 修正：マテリアルから離れた場所をクリックすると、「GPUインスタンス化」チェックボックスが元に戻りました。
* 修正：Duplicate()関数を使用する際に、複製されたグラフが、メタリックのアルファに適切にパックされたSmoothnessを持っていません。
* 修正：ビルドターゲットをAndroidに切り替えると、手動で再読み込みされるまでテクスチャが間違ったフォーマットになる。
* 修正：UnityでSubstanceファイルを削除すると、NullReferenceExceptionが発生します。
* 修正：以前のバージョンでUnity 2019.3 HDRP APIの使用を無効にする

既知の問題：

* エミッションチェックボックスはデフォルトでは有効になっていません。また、Substanceをインポートすると、HDR 値は黒に設定されます。
* 標準のsubstance マテリアルを含むパッケージのマテリアルプロパティは、読み込み時に継承されません。
* 2017-2019/2020からのアップデートがHDRPで機能しない
* ターゲット設定で4096を選択した状態で設定メニューの2048クランプオプションを（適用をクリックせずに）クリックすると、コンソールログにエラーが記録される
