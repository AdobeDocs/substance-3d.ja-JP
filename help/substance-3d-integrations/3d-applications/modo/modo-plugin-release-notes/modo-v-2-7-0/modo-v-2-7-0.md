---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/modo/modo-plugin-release-notes/modo-v-2-7-0.html"
breadcrumb-title: ''
description: MODOプラグインバージョン2.7.0のリリースノートを確認し、新機能、改善点、バグの修正について確認してください。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Modo Plugin Release Notes > Modo v. 2.7.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: モードv. 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---


# モードv. 2.7.0

* 多数のクラッシュを修正
* 32ビットfloatのサポート
* CPUエンジンの4KテクスチャおよびGPUエンジンの8Kテクスチャ
* プラグインリリースの新しいLPK形式
* Substanceプラグインの新規キットメニュー
* MODO 12.0に対するglTF / Principledシェーダのサポート
* Substanceファイルの相対パスが追加されました。
* Linuxのサポート
* プリセットの読み込みと保存を行う新しいUI
* 埋め込みプリセットはDesignerから読み込み
* 削除されたGPUメモリの警告ボックス
* 編集されたプリセットの読み込み/保存コマンド

  使用できる新しいコマンドは次のとおりです。

  **substance.getsbsname** substanceオブジェクトのIDを内部名に変換します

  これらはすべて、substance.getsbsnameから取得された適切な内部名を期待します。

  **substance.setpreset** Substanceの現在のプリセットをインデックスに設定&#x200B;**substance.getpresetindex**&#x200B;現在のプリセットインデックスを取得&#x200B;**substance.getpresetat**&#x200B;指定の&#x200B;**インデックスsubstance.getpresetcount**&#x200B;にあるプリセットの文字列名を返しますSubstanceが持つプリセットの数を返します&#x200B;**substance.savepresetfile**&#x200B;指定のファイルパスに現在ののプリセットを保存します&#x200B;**substance.loadprepresetfile&lbrace;111111111ファイル1ファイル**

  UIコマンド：

  **substance.loadpresetui**&#x200B;プリセットを読み込むためのUIコマンド&#x200B;**substance.savepresetui**&#x200B;プリセットを保存するためのUIコマンド&#x200B;**substance.selectpresetui**&#x200B;プリセットを設定するためのUIコマンド
