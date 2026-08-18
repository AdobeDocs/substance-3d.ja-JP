---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-2.html"
breadcrumb-title: ''
description: Unityプラグインバージョン2.3.2のリリースノートを確認して、新機能、改善点、バグ修正について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Unity 2.3.2

## 新機能：

* 材料のシリアル化
* Reflection：このプラグインでは、パッケージに古いSubstanceファイルを読み込むことができるようになりました（読み込み時に新しいSubstanceデータに自動的に更新されます）
* マテリアルプロパティは、Substanceデータを含むパッケージの読み込みで引き継がれます
  * 注意：これは、2.3.0アップデート以降を使用して作成されたパッケージにのみ適用されます
* Substanceグラフメニューに「テクスチャのベイク」ボタンを追加

### バグ修正：

* ライブラリフォルダーを削除すると、Substanceのマテリアルのタイル表示がリセットされる問題を修正しました
* 再生モードから出る速度が向上しました
* プラグインDLLの使用中にSubstanceをアップデートするとクラッシュする問題を修正しました。
* AllegorithmicフォルダはUnity内で削除できません。
  * 注意： Allegorithmicフォルダーの内容は変更できません。 Unity内で削除すると、複数の問題が発生する可能性があり、Unityを閉じて再び開くと、Allegorithmicフォルダが再び魔法のように表示されます。 UnityをプロジェクトのAssetsフォルダから手動で閉じた状態で削除するようユーザに通知する警告が表示されるようになりました
* 再生モードから出る速度が向上しました
* ライブラリフォルダーを削除したときに、Substanceのマテリアルプロパティがリセットされるバグを修正しました

## 既知の問題：

**コアSubstanceプラグイン**

* iOS用にビルドするには、Xcodeのビルド設定メニューで「ビットコードを有効にする」を無効にする必要があります
* Substanceは、アセットバンドルでは動作しません。
* 再インポートすると、Asset BrowserのSubstanceプレビューアイコンがすべてSubstance Sアイコンに変わります

**スクリプト**

* プロジェクトがビルド設定でx86に設定されている場合、実行時にスクリプトが機能しない
* 特定のビルドプラットフォームでil2cppスクリプトバックエンドを使用する際の問題

**Substance Painterライブリンク**

* Substanceライブリンクでペイントした後にプロジェクトを構築すると、ペイントしたメッシュがデフォルトのマテリアルに戻ります
* PainterのライブリンクでAOチャンネルが送信されない
* 複数のマテリアルを含むメッシュがUnity Live Linkで機能しない
* Unity LiveLinkがSimpleJsonを使用する方法は、プロジェクト内のSimpleJsonの他のインスタンスとクラッシュします
