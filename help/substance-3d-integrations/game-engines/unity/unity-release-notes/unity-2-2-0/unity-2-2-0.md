---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-2-0.html"
breadcrumb-title: ''
description: Unityプラグインバージョン2.2.0のリリースノートを確認して、新機能、改善点、バグ修正について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.2.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.2.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---


# Unity 2.2.0

## 2.2.0リリースノート

**リリース日： 2019年1月10日**

### コアプラグイン：

* 更新されたSubstance engine
* コードの安定性の向上
* **Unity 2018.3サポート**
* **.NET 4.xサポート**
* 2018.3でのSubstance Sourceのサポート
* Substance Sourceの色付けの問題が修正されました
* グラフと対応するマテリアルのオブジェクト名が同じになりました
* Unity ProスキンGUIの読みやすさの向上を追加
* マテリアルの出力割り当てのサポートが追加されました
* sRGB処理のバグを修正しました
* ユーザーがグラフのすべてのインスタンスを削除できるバグを修正しました
* 実行時にパラメーターを変更しているときにSubstanceーをレンダリングしようとすると、一度に2つしかレンダリングできないバグを修正しました
* 古いSubstanceファイルを含むパッケージをインポートする場合、プラグインは古いSubstanceデータが含まれていることをユーザーに通知し、Unityがパッケージファイルをインポートする際にパッケージファイルを削除します（これにより、壊れていても、すべてを手動で削除する必要がなくなります）
* Substanceプラグイン関連のビルド情報を表示する「Substance」メニューに「バージョン情報」ボタンが追加されました。
* SubstanceGUIにSubstanceパラメーター名を表示するためのマウスオーバーツールチップが追加されました。
* SubstanceGUIのナビゲーションボタンを追加して、Substanceグラフとマテリアルにリンク
* コンテンツブラウザにSubstanceグラフ/マテリアル/テクスチャの新しいアイコンが追加されました
* コンテンツブラウザのSubstanceサムネイルを更新しました
* Substanceマテリアル名の前面から.matを削除
* グラフとマテリアルの名前を変更する機能が追加されました
* グラフの解像度を変更する場合、適用/復帰ポップアップが表示されなくなり、その時点で変更を確定するように求められます
* リフレクションプロセスで、ユーザーが定義した解像度ではなく、デフォルトのSubstance解像度のみが使用されるバグを修正しました
* カラースペースがガンマに設定されているかどうかを通知するマウスオーバー警告がSubstance GUIに追加されました。
* グラフインスタンスの機能の変更：SubstanceグラフGUIで作成された各インスタンスの確認メッセージを表示しなくても、Substanceでグラフインスタンスを作成できるようになりました

### スクリプト：

* スクリプトのサポート対象外の関数を非表示にしました
* スクリプトを使用してグラフインスタンスを複製する関数Duplicate()が追加されました。
* C#を介してプロシージャルの入力情報を照会する関数が追加され、&#39;InputProperties&#39;要素の配列が返されました。 GetInputProperties()
* グラフに入力が存在するかどうかをチェックする関数が追加され、true/falseが返されました。 HasInput(string inputName)
* 表示されている入力が表示されているかどうかを確認する関数が追加され、true/falseが返されました。 IsInputVisible(string inputName)
* レンダリング方法が再設計されました。 そのため、RenderSubstancesAsync()は非推奨となり、これはgraphName.RenderAsync()に変更されました

## 既知の問題：

**コアSubstanceプラグイン**

* iOS用にビルドするには、Xcodeのビルド設定メニューで「ビットコードを有効にする」を無効にする必要があります
* 構築対象をAndroid/iOSに設定すると、コンテンツブラウザーのSubstanceオブジェクトのプレビューが黒で表示される
* Substanceプラグインを読み込んだ後、Substance以外のテクスチャ GUIに「Alpha」ボタンと「Mipマップ」プレビュースライダーが表示されない
* 2の累乗を使用して、スクリプトによるグラフの解決を定義する必要があります
* Unityパッケージを使用してエクスポート/インポートすると、マテリアルが永続的になりません
* Substanceは、アセットバンドルでは動作しません。
* 再インポートすると、Asset BrowserのSubstanceプレビューアイコンがすべてSubstance Sアイコンに変わります
* シーンにマテリアルが含まれているSubstanceグラフの名前を変更すると、そのマテリアルは配置されているオブジェクトから削除されます
* （Macのみ）Macでプラグインをアップデートすると、シーン内のプレハブからSubstanceマテリアルが削除される|

**スクリプト**

* プロジェクトがビルド設定でx86に設定されている場合、実行時にスクリプトが機能しない
* 特定のビルドプラットフォームでil2cppスクリプトバックエンドを使用する際の問題

**Substance Painterライブリンク**

* Substanceライブリンクでペイントした後にプロジェクトを構築すると、ペイントしたメッシュがデフォルトのマテリアルに戻ります
* PainterのライブリンクでAOチャンネルが送信されない
* 複数のマテリアルを含むメッシュがUnity Live Linkで機能しない
* Unity LiveLinkがSimpleJsonを使用する方法は、プロジェクト内のSimpleJsonの他のインスタンスとクラッシュします
