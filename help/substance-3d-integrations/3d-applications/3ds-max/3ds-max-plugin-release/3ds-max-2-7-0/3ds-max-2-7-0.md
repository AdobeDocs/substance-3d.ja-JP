---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-7-0.html"
breadcrumb-title: ''
description: 新機能、改善点、バグ修正については、 3ds Maxプラグインバージョン2.7.0のリリースノートを確認してください。
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# 3ds Max 2.7.0

<b>追加/更新：</b>

* 3ds MaxプラグインのSubstance エンジンをバージョン9にアップグレードし、パフォーマンスと互換性を強化しました。

<b>修正済み：</b>

* 3ds Maxバージョン2019、2022、2023、2024で、Substance 2ノードをスレートマテリアルエディタにドラッグするとプログラムがクラッシュするクラッシュの問題を修正しました。 Substance 2ノードをスレートマテリアルエディタに安全にドラッグアンドドロップできるようになりました。
* 3ds Max用Substanceプラグインで、「ArnoldへのSubstance」やその他のワークフローを選択しても、マテリアルスレートエディタに関連するノードが作成されず、コンパイルエラーを伴うMaxscriptが誤って開かれる問題を解決しました。 Arnoldなどのワークフローのノードが正しく生成され、自動的に接続されるようになりました。
* Substance 3D Samplerから開始アセット/プリセット（.sbsar - Substance 2 テクスチャマップ）を書き出し、3ds Max内でコロナレンダラー（バージョン6から9hf1）に変換すると、マテリアルが破損し、黒いbase colorでレンダリングされたり、バンプ法線が破損したりする問題を修正しました。 また、このアップデートにより、マテリアルの「Substanceプロパティ」タブがアクセスできなくなるという問題も解決されました。
* Substance 2 テクスチャからコロナマテリアルへの入力のプラグ接続またはプラグ接続の解除がクラッシュを引き起こす3ds Maxプラグインの問題を修正しました
* PythonスクリプトがMaxScriptファイル内に埋め込まれたり、呼び出されたりする3ds Max 2024の互換性に関する問題がデフォルトで許可されていませんでした
* 3Ds Maxプラグインで、SubstanceをCoronaプラグインに読み込んで実行すると、シェーダーのプレビューとレンダリングでマテリアルが黒く光沢が出る問題を修正しました。 この問題は正常に解決され、Coronaレンダラーを使用したSubstanceマップの正しい表示とレンダリングが保証されるようになりました。

このバージョンは3ds Max 2021、2022、および2023用にリリースされています
