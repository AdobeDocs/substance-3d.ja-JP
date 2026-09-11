---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-1.html"
breadcrumb-title: ''
description: 新機能、改善点、バグ修正については、 3ds Maxプラグインバージョン2.3.1のリリースノートを確認してください。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# 3ds Max 2.3.1

2020年2月13日公開

プラグインは3ds Maxディレクトリの外部からC:\ProgramData\Autodesk\ApplicationPlugins\SubstanceIn3dsMaxにインストールされます。 これで、3ds Maxがプラグインを検索するように指示されているあらゆる場所で動作するようになったため、ネットワークドライブなどにインストールされます。\
アプリケーションプラグインへの切り替えとインストールディレクトリの変更により、2.1.1以前のバージョンからのアップグレードが正しく動作しなくなることに注意してください。 3ds Max 2018および2019では、これらは手動で削除する必要があります。 バージョン2.2.0は正しくアップグレードされるはずです。\
このリリースで解決されていない問題の一部については、これらおよび発生する可能性のあるその他の問題を修正するために、別の問題がまもなく計画されています。

このバージョンは、3ds Max 2018、2019、2020、2021で現在リリースされています。

* sbsarを読み込むと、最初にプロジェクトイメージフォルダーが検索されるようになりました
* レンダラーの互換性ダイアログが、VRay RTおよびVUEファイルレンダラーでのみ表示されるようになりました
* 最大バッチの問題を解決するには、スレートマテリアルエディターを無効にしてドラッグ&amp;ドロップします
* [レンダリング]ダイアログボックスが3ds Maxサイレントモードで表示されなくなりました
* Python 3と互換性のある小さなPythonスクリプト
* Substance Sourceアセットを3ds Maxに送るためのSubstanceランチャーのサポートが追加されました。 これにはランチャーの変更が必要ですが、機能が追加されるとプラグインのサポートが提供されます。
* Redshiftレンダラースクリプトで、Redshift 2.6.24で設定された新しいノード名が使用されるようになりました。
* Substance 2のSubstanceFilePathに空のパスが割り当てられている場合、Maxがクラッシュしなくなりました。
* SubstanceOutputタイプと古いプラグインの名前の競合を削除
* SubstanceOutputクラスの名前がSubstance 2Outputに変更されました
* Substanceメニューマネージャークラスの名前をSubstance 2MenuManagerに変更しました
* シーンを開いたときにパラメトリックブロックIDが強制的にクリアされるようになり、シーンファイル間の競合が解消されました。 これにより、シーン間で交互に読み込まれる場合の無効なパラメータブロックの問題が修正されます。 より複雑な変更が必要となるため、読み込みにはまだ問題がある場合があります
* これで、プラグインは3ds Maxの外部にインストールされました。 すべてのパスは、ロード位置からの相対パスに変更されています。
* プラグインでは、Autodeskアプリケーションプラグインシステムが使用されるようになりました。
