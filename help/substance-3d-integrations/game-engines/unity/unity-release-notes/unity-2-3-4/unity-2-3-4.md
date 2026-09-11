---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-4.html"
breadcrumb-title: ''
description: Unityプラグインバージョン2.3.4のリリースノートを確認して、新機能、改善点、およびバグ修正について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.3.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Unity 2.3.4

>[!WARNING]
>
> **Unity 2019.2でプラグインを使用すると、次のエラーが発生します。**
> 
> InspectorSubstanceImporter.OnInspectorGUIは、予期しない動作を避けるためにApplyRevertGUIを呼び出す必要があります。\
> UnityEditor.Experimental.AssetImporters.AssetImporterEditor:OnDisable()\
> Substance.Editor.InspectorSubstanceImporter:OnDisable()
> 
> このエラーはクリアでき、プラグインの機能には影響しません

>[!WARNING]
>
> **以下を読んでください：壊れているマテリアル:**\
> 使用方法が空白のカスタム出力を含むマテリアルは、読み込み時に機能しません。 また、重複する使用状況を含むマテリアルは機能しなくなります。\
> GameTextures.comの古いsbsarファイルは、現在UnityプラグインのSubstanceと互換性がありません。 サポートされていないUsage出力を含むこれらのマテリアルは機能しません。 プラグインを使用する前に、プロジェクトのバックアップを作成してください。

## 新機能：

* Substance engine v7のサポートが追加されました。
* Linuxのサポートを追加

### バグ修正：

* テクスチャマップを使用しないSubstanceの読み込みに関連する問題を解決しました。
* Unity 2019.xでリフレクションプロセスが正しく動作しない問題を修正しました
* マテリアル付きのプレハブを含むパッケージを読み込む際のプレハブの処理に関する問題を修正しました
* リフレクションプロセス後に継承されない固定マテリアル/テクスチャの割り当て
* マテリアルが壊れる原因となるシェーダの変更に関連する問題を修正しました
* ラフネスがメタリックアルファチャンネルにパックされていない問題を修正しました。
* Substanceプラグインがインストールされている場合に、substance以外のテクスチャの読み込み設定を変更すると、特定のオプションが元に戻る問題を修正しました。
* MacでSubstance Sourceが開かない問題を修正しました

## 既知の問題：

**コアSubstanceプラグイン**

* iOS用にビルドするには、Xcodeのビルド設定メニューで「ビットコードを有効にする」を無効にする必要があります
* Substanceは、アセットバンドルでは動作しません。
* 再インポートすると、Asset BrowserのSubstanceプレビューアイコンがすべてSubstance Sアイコンに変わります
* 使用方法が空白に設定された出力があるカスタムマテリアルは、マテリアルを壊します
* 重複使用のあるカスタムSubstanceマテリアルは、マテリアルを壊します
* プラグインをLinuxに読み込んだ後、エディターを再起動する必要があります

**スクリプト**

* プロジェクトがビルド設定でx86に設定されている場合、実行時にスクリプトが機能しない
* 特定のビルドプラットフォームでil2cppスクリプトバックエンドを使用する際の問題

**Substance Painterライブリンク**

* Substanceライブリンクでペイントした後にプロジェクトを構築すると、ペイントしたメッシュがデフォルトのマテリアルに戻ります
* PainterのライブリンクでAOチャンネルが送信されない
* 複数のマテリアルを含むメッシュがUnity Live Linkで機能しない
* Unity LiveLinkがSimpleJsonを使用する方法は、プロジェクト内のSimpleJsonの他のインスタンスとクラッシュします
