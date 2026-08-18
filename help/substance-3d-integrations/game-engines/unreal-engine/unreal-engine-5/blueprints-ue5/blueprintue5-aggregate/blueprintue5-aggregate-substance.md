---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-aggregate-substance.html"
breadcrumb-title: ''
description: Unreal Engine 5では、高度なワークフローを実現するBlueprint集計ノードを使用して、実行時に複数のSubstanceマテリアルを組み合わせることができます。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE5)集約Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Blueprint(UE5)：集約Substance

1. 「集約Substance・ファクトリの作成」ノードを使用して、出力ファクトリと入力ファクトリを設定します。 出力ファクトリには、入力ファクトリパラメータで入力イメージとして使用されるテクスチャマップが必要です。
1. 入力として使用されている各出力テクスチャのSubstanceConnectionオブジェクトを、対応する値の名前（出力グラフからの出力名と入力グラフからの入力パラメータ名）とともに作成します
1. Create Graph Instanceノードを追加し、「Create Aggregate Template Factory」ノードの結果を親マテリアルとともにFactory入力にプラグインし、Substanceとして機能させます（プラグインに含まれるデフォルトの\_substanceマテリアルの1つです）。
1. Substance グラフインスタンス変数を作成し、前のノードの結果を保存します。
1. オプション：必要なSubstanceパラメーターを設定します（この例では、グラフ出力の新しい解像度を設定しています）。
1. AsyncまたはSyncレンダリングノードを作成し、レンダーするインスタンスをSubstance グラフインスタンス変数にコネクトします。
1. 既存のマテリアルインスタンスを作成または取得するには、グラフインスタンスの「ダイナミックマテリアルインスタンスを取得」機能を使用します。 「名前」と「親マテリアル」を空白のままにすると、手順3でインスタンスを生成するときに使用したパラメータが使用されます。
1. セットマテリアルノードを追加し、マテリアル入力としてMID変数の値を設定します。 ターゲットの場合は、マテリアルを適用するオブジェクトに設定します。
