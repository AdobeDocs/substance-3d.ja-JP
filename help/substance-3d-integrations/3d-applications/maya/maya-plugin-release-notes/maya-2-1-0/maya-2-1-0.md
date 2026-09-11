---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-1-0.html"
breadcrumb-title: ''
description: Mayaプラグインバージョン2.1.0のリリースノートを確認し、新機能、改善点、およびバグ修正について学習してください。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.1.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 2.1.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# Maya 2.1.0

Maya 2.1.0の変更ログのSubstance

* Python 3との互換性の確保
* バージョン7.2.9に更新されたSubstance engine
* ワークフローの適用時に競合するグローバルMEL変数名でエラーが発生する問題を修正しました
* Redshiftワークフローでフレネルがメタネスに設定されるようになりました。
* 他のプラグインプログラムやSubstanceランチャーとの相互運用性を処理する新しいSubstanceファイルsubstancelinkが追加されました。
* substancelinkプラグインが読み込まれた場合、Substance Sourceを開くと「ソース」タブのSubstanceランチャーが開きます
* substancelinkプラグインを使用すると、ランチャーはUIが追加されたときに、Substance SourceマテリアルをMaya統合に送ることができます
* 内部ライブラリのバージョンを取得し、ソースページにSubstanceランチャーを開くために追加されたスクリプトコマンド
* Webサイトのリンクが、[allegorithmic.com](http://allegorithmic.com)ではなく[substance3d.com](http://substance3d.com)に開くようになりました
* Webページを開くときに、ドキュメントとソースリンクでユーザーセットのデフォルトブラウザーが開くようになりました
* Windowsでは、インターネットエクスプローラーは現在開かれていません
* シェルフとメニューの新しいリンクがSubstance shareに追加されました
* Substanceリンカーのバージョンとハッシュを照会する新しいコマンドが追加されました
* Maya LTで、バージョンが設定メニューから削除されました
* PySide2やPythonではメニューについて書かれていませんが、Qtを使ったネイティブコードで書かれています。 以前は使用されていなかったMaya LTで使用できるようになりました。
* バージョン情報メニューには、異なる診断情報があります。ソース管理の変更に合わせてgitハッシュが表示されます
* クリップボードへのバージョン情報メニューのコピーにも、このgitハッシュと、プラグインが構築されたMayaのバージョンが含まれるようになりました。
* 「バージョン情報」ウィンドウのライセンスがテキストファイルとして開くようになりました
* Maya 2017のサポートの追加
* ワークフロースクリプトジェネレータは、&#39;ordering&#39;メンバの文字列を出力しなくなりました。 既存のワークフローは適切に処理されます

追加されたスクリプトコマンド：\
substancemaya:\
\* substanceUtilityGetLinkerVersion\
\* substanceUtilityGetLinkerHash\
\* substanceUiOpenAboutWindow\
\* substanceUiOpenSourceWebsite\
\* substanceUiOpenDocumentation\
\* substanceUiOpenShareWebsite

substancelink:\
\* substanceLinkGetLinkVersion\
\* substanceLinkGetPortalCliVersion\
\* substanceLinkOpenLauncher

Windows版Maya 2017、2018、2019、2020では、このバージョンがリリースされています。\
LinuxおよびMacos。 また、Maya LT 2018、2019、2020用に\
WindowsおよびMacOS
