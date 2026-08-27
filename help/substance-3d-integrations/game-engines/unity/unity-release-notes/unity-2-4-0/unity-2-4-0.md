---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-0.html"
breadcrumb-title: ''
description: Unityプラグインバージョン2.4.0のリリースノートを確認して、新機能、改善点、およびバグ修正について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---


# Unity 2.4.0

>[!WARNING]
>
> Unityはデフォルトのビルドアーキテクチャをx86\_64ではなくx86に変更しました。\
> スクリプトがSubstanceを参照している場合、スクリプトは実行されません。 x86\_64に戻さないとビルドは動作しません。

## 新機能：

* HDRPプロジェクトのサポートが追加されました（プレビュー）
* Substanceメニューに環境設定を追加
* デフォルトのSubstance解決の読み込み設定を設定する機能が追加されました
* デフォルトの標準圧縮を設定する機能が追加されました。
* Substanceの読み込みですべての出力を生成する機能が追加されました
* カスタム出力+同じ使用方法を使用する出力のサポート
* プラットフォーム解像度設定を追加
* IL2CPPサポートのバグ修正を追加

### バグ修正：

* Mac OSでSubstance Sourceを開くとLinuxエラーが発生するバグを修正しました
* プラットフォームの切り替えに要する時間を短縮。 モバイルプラットフォームのテクスチャコンバージョンは、ターゲットプラットフォームの切り替え時ではなくビルド時に実行されるようになりました。
* sbsarの読み込み時のアサーション失敗エラー
* .NET 3.5を使用してプロジェクトをアップグレードすると、Substanceのマテリアルが機能しなくなる
* OS XのLinuxダイアログでSubstanceソースがサポートされていない
* グラフ名を変更すると、ForceTextシリアル化モードでプレハブとシーンファイルが破棄される
* 同じ使用方法を使用する複数の出力を持つマテリアルでは、プラグインがsbsarのカスタム出力をサポートしません

### 既知の問題：

* 2017-2018/2019からプロジェクトをアップグレードする場合、Substanceプラグインをインポートした後、プロジェクトを更新するためにUnityを再起動する必要があります。\
  回避策：アセット/プロジェクトのパッケージを作成し、2.4.0プラグインを使用して、そのパッケージを新しいプロジェクトに読み込みます。 Substanceファイルは正しく変換される必要があります。
* Unityはデフォルトのビルドアーキテクチャをx86に変更しました。 現在、Substanceプラグインはx86\_64のみをサポートしています。

**完全サポートされなくなりました：**

* Substanceライブリンクがアセットストアパッケージから削除されました。 （パッケージはSubstance shareからダウンロードできます）
