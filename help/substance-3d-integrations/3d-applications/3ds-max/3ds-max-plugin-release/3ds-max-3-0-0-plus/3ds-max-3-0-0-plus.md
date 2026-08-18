---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-3-0-0-plus.html"
breadcrumb-title: ''
description: 新機能、改善点、バグ修正については、 3ds Maxプラグインバージョン3.0.0以降のリリースノートを確認してください。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3Ds Max 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# 3ds Max 3.0.0以降

## 3ds Max 3.0.4

<b>追加/更新：</b>

* Substanceプラグインのアイコンを最新のアイコンに更新しました。
* プラグインのコネクタを使用したプリセットの送受信のサポートが追加されました。
* 通知パラメーターから統合メニューマネージャーを選択して、コアインターフェイスの使用を置き換えます。

<b>修正済み：</b>

* スレートマテリアルエディターが開いており、Substance2テクスチャマップが選択されている場合、コロナを使用したSubstance2マテリアルのIR/Productionでのレンダリングが失敗する問題を解決しました。
* Samplerコネクタの更新で、既存のノードを更新するのではなく、新しいSubstance 2ノードが作成される問題を解決しました。
* Substance2ノードを追加する際に3ds Maxプラグインがクラッシュする問題を解決しました。また、バッチインポートを使用して.sbsarファイルをロードしても、スクリプトエディタが開かないようになりました。
* .msiインストーラーの使用時に互換性のない.dllファイルが原因で3DSMax 2025プラグインを読み込めない問題を解決しました。

## 3ds Max 3.0.2

<b>追加/更新：</b>

* 既存のすべてのアイコンをqrcファイルとrccファイルに組み込み、Autodeskの好ましい方式に合わせ、SBSARグラフパネルで一貫性のあるロードを実現することで、Substanceプラグインで標準化されたアイコン管理。
* プラグインのSubstance設定ウィンドウの応答性が向上し、ウィンドウのサイズを調整する際に入力フィールドとその説明が適切に収まるようになりました。
* SubstanceプラグインがCorona 11と互換性を持つようになりました。

<b>修正済み：</b>

* V-Rayマテリアルで光沢カラーと光沢の粗さが自動的に接続されない問題を解決しました。 これで、V-RayとArnoldでワークフローを作成すると、両方のプロパティが自動的にリンクされます。
* プラグインのUIの問題で、保存された値が1桁の場合にCPUコア数制限の設定を調整すると、2桁の値が正しく表示されない問題を修正しました。
* Substance互換機能に関連する3ds Maxプラグインv3.0.0のコンソールのレンダリングエラーを修正しました。 これで、Substanceバッチ読み込みメニューを使用して作成したSubstanceノードが正常にレンダリングされるようになりました。
