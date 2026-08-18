---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-aggregate-substance.html"
breadcrumb-title: ''
description: Unreal Engine 4では、高度なワークフローを実現するBlueprint集計ノードを使用して、実行時に複数のSubstanceマテリアルを組み合わせることができます。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE4)集約Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Blueprint(UE4)：集約Substance

新しい集約substanceノードを使用すると、2つのsubstanceインスタンスファクトリを使用して、新しいグラフインスタンスの作成に使用できる新しいインスタンスファクトリを実行時に作成できます。 この特別な機能は、一方の複合グラフインスタンスの出力テクスチャを、もう一方の複合グラフインスタンスの入力イメージにコネクトできることです。 この新しいファクトリからsubstance graphインスタンスを作成するには、ランタイムグラフインスタンスに関するドキュメントを参照してください。 [マテリアルインスタンス定義 – UE4](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/material-instance-definition-157352129.html)

1. 使用するSubstanceを読み込みます。
1. **Substance グラフインスタンス**&#x200B;型の変数「AggregateGraphInstance」を作成します。
1. **Material**&#x200B;型および&#x200B;**Material Instance Dynamic**&#x200B;型の変数を作成します
1. **Substance接続を確立**&#x200B;し、出力IDと入力IDを設定します。
1. **集約Substanceインスタンスファクトリ**&#x200B;を作成し、出力ファクトリと入力ファクトリを設定します。
1. **グラフインスタンス**&#x200B;を作成し、インスタンス名を設定します。
1. **集計グラフインスタンス**&#x200B;変数を設定します。
1. 手順7の集約グラフインスタンスから、**「Substanceテクスチャを取得」**&#x200B;を使用してSubstanceテクスチャを取得します。
1. 手順3の材料変数を親として使用して、**動的な材料インスタンス**&#x200B;を作成します。
1. 手順3で定義したMID変数を設定します。
1. MID変数を使用して&#x200B;**マテリアルの設定**&#x200B;を使用して、メッシュのマテリアルを設定します。

   ![](../../../../../assets/a2-3.png){width="800px"}
1. ダイナミックマテリアルインスタンスドキュメントに表示されるマテリアルのチャンネルを設定します（手順11～19）\
   [Blueprint(UE4)：動的なマテリアルインスタンス](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)

   ![](../../../../../assets/a4-3.png){width="800px"}
