---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-2.html"
breadcrumb-title: ''
description: 新機能、改善点、バグ修正について詳しくは、 3ds Maxプラグインバージョン2.3.2のリリースノートを参照してください。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# 3ds Max 2.3.2

2020年4月8日リリース

今日、プラグインの2.3.2バージョンをリリースしました。これは主に2.3.1の上のバグ修正リリースです。

2.3.2リリース：

* Substance engineを7.2.9に更新
* 3ds Max 2018、2019および2020でRedshift/VRayによるレンダリングがクラッシュする問題を修正しました。
* デバッグアサートエラーは表示されなくなります
* Substance2ノードに、iMultipleOutputChannelsWithValuesのスクリプトインターフェイスが正しく追加されました。
* インストールされている場合、Substanceのソースエントリで「ソース」タブのSubstanceランチャーが開くようになりました
* コロナレンダラーの使用時に、Substanceマテリアルが正しく更新されるようになりました
* 「VRay Next」で使用した場合に、Substance出力が一時的に画像に置き換えられることがなくなりました
* レンダリングの互換性ダイアログが自動表示から削除されました。 この設定は、必要に応じて設定ダイアログでも使用できます
* 3ds Max 2021でsubstanceマテリアルを適用した状態でfbxを書き出すと発生する可能性のある問題を修正

既知の問題：

* 3ds Max 2018では、Substanceマテリアルがオブジェクトにアタッチされたfbxの書き出しはfbxmax.dluプラグインでクラッシュします。 現在、Autodeskと話し合い、何か対処すべきことがあるのか、それが旧リリースのfbx統合の制限なのかを確認しています。 以前の回避策は信頼性が低いため、削除されました。 これは3ds Max 2019以降では発生しません。

このバージョンは3ds Max 2018、2019、2020、2021用にリリースされています。
