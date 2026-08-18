---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-dynamic-material-instance-skip-to-end-of-metadata.html"
breadcrumb-title: ''
description: Unreal Engine 5で実行時にSubstanceのマテリアルから動的なマテリアルインスタンスを作成するには、ブループリントを使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Dynamic Material Instance Skip to end of metadata
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE5)動的マテリアルインスタンスメタデータの最後にスキップ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---


# Blueprint(UE5)：動的なマテリアルインスタンスメタデータの最後にスキップします

1. Substanceインスタンス・ファクトリ・タイプの変数を作成し、デフォルト値をインポートされたSubstance・ファクトリに設定します。
1. グラフインスタンスの作成(Create Graph Instance)ノードを追加し、Substanceインスタンスファクトリを親マテリアルとともにファクトリ入力にプラグインして、テンプレートとして機能させます（プラグインに含まれるデフォルトの\_substanceマテリアルの1つです）。
1. 前の手順で作成したSubstance グラフインスタンスオブジェクトを格納する別の変数を作成します。
1. 既存のマテリアルインスタンスを作成または取得するには、グラフインスタンスの「ダイナミックマテリアルインスタンスを取得」機能を使用します。 「名前」と「親マテリアル」を空白のままにすると、手順2でインスタンスを生成するときに使用したパラメータが使用されます。
1. マテリアルタイプの変数を作成します。 これは、マテリアルインスタンスダイナミック(MID)になります。 「動的マテリアルインスタンスを取得」の戻り値を変数に設定します。

   ![](../../../../../assets/dynamic-material-annotated-1.png)
1. セットマテリアルノードを追加し、マテリアル入力としてMID変数の値を設定します。 ターゲットの場合は、マテリアルを適用するオブジェクトに設定します。
1. オプション：必要なSubstanceパラメーターを設定します（この例では、既存のSubstance Graphインスタンスを使用し、値を新しいインスタンスにコピーしています）。
1. AsyncまたはSyncレンダリングノードを作成し、レンダーするインスタンスをSubstance グラフインスタンス変数にコネクトします。
