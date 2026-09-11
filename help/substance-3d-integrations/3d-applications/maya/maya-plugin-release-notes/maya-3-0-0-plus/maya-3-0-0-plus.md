---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-3-0-0-plus.html"
breadcrumb-title: ''
description: Mayaプラグインバージョン3.0.0以降のリリースノートを参照して、新機能、改善点、およびバグ修正について確認してください。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > Maya 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Maya 3.0.0以降

## Maya 3.0.3

<b>追加/更新：</b>

* 拡張されたMayaプラグインのキャッシュシステムでは、最初のネットワーク作成時に一度だけキャッシュが行われ、手動での再キャッシュが有効になっています。
* Mayaプラグインの「substance」フォルダの場所を変更するオプションが提供されました。
* Mayaプラグインのワークフロー読み込みシステムが更新され、Python 3.12へのAutodeskの更新との互換性が確保されました。
* Substanceプラグインのアイコンを最新のアイコンに更新しました。
* プラグインでコネクターを使用したプリセットの送受信のサポートが追加されました。

<b>修正済み：</b>

* MayaのSubstanceプラグインをロード/アンロードすると、エラー画面とクラッシュが表示される問題を解決しました。
* キャッシュの問題を修正しました。特に.exrファイルが正しく参照されるようにし、大規模なシーンでのキャッシュ関連のフリーズを減らしました。
* MayaプラグインにSbsar ファイルをロードしたときに、サンプルウィンドウにマテリアルプレビューが表示されない問題を解決しました。
* 少なくとも1つのSBSARが既にハイパーシェードにある場合にコネクターがSbsar ファイルを受け取れない問題を解決しました。
