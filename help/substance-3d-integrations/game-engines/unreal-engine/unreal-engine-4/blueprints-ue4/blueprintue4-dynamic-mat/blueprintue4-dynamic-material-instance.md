---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-dynamic-material-instance.html"
breadcrumb-title: ''
description: Unreal Engine 4では、実行時にSubstanceのマテリアルから動的なマテリアルインスタンスを作成できます。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Dynamic Material Instance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE4)動的マテリアルインスタンス
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Blueprint(UE4)：動的なマテリアルインスタンス

Substance グラフインスタンスを作成すると、実行時に動的グラフインスタンスを作成できます。

1. Substanceインスタンス・ファクトリ・タイプの変数を作成し、デフォルト値をインポートされたSubstance・ファクトリに設定します。
1. グラフインスタンスの作成ノードを追加し、Substanceインスタンスファクトリをファクトリ入力にプラグインします。 インスタンス名を設定します。
1. Substanceインスタンスファクトリ型の別の変数を作成します。 これにより、動的なsubstanceマテリアルへの参照が保持されます。
1. 動的なSubstanceマテリアルの変数を、グラフインスタンスの作成ノードの戻り値で設定します。
1. マテリアルタイプの変数を作成します。 これがマテリアルテンプレートになります。 [コンテンツブラウザ]で、Substanceによって生成されたUE4マテリアルの複製を作成します。 複製した材料を材料テンプレート変数の入力値として設定します。
1. ダイナミックマテリアルインスタンスの作成を追加し、マテリアルテンプレート変数を親として設定します。

   ![](../../../../../assets/rt-01.png){width="800px"}
1. マテリアルタイプの変数を作成します。 これは、マテリアルインスタンスダイナミック(MID)になります。 ダイナミックマテリアルインスタンスの戻り値を変数に設定します。

   ![](../../../../../assets/rt-02.png){width="800px"}
1. セットマテリアルノードを追加し、マテリアル入力としてMID変数の値を設定します。 ターゲットの場合は、マテリアルを適用するオブジェクトに設定します。
1. Name型の変数を作成します。 この変数には、マテリアルで設定されたチャンネルの名前が保持されます。 「NONE」の値を使用して、これを初期化します
1. Substanceテクスチャの取得ノードを追加し、グラフインスタンスをダイナミックグラフインスタンス変数に設定します。
1. Forループノードを追加します。 ここでは、Substanceテクスチャをループします。 [Substanceテクスチャを取得]の結果を入力配列にします。

   ![](../../../../../assets/rt-03.png){width="800px"}
1. forループの配列要素を入力として使用して、SubstanceのGet Channelノードを追加します。
1. シーケンスノードを追加します。 ここでは、最初にGet Channelノードの結果を実行します。
1. シーケンスの後にESubChannelTypeのスイッチを追加し、選択範囲としてチャンネルの戻り値を使用して0を追加します。 ここでは、チャンネル名を確認します。
1. MID Name変数に、手順5でコピーしたSubstanceマテリアルのチャンネル名を設定します。 *素材の画像を表示します。*
1. [シーケンス]ノードの[次へ1]で、動的マテリアルにチャンネル名を割り当てるプロセスを設定します。
1. MID名前変数を取得し、「NONE」の値を持つ等文字列ノードを追加します。これは、変数を初期化する値です。
1. 「等しい」ノードから「条件」を含む分岐ノードを追加します。
1. Substanceセットテクスチャパラメータ値を追加します。 ターゲットはMID変数で、パラメータ名はMID名前変数です。 値はForEachLoopノードの配列要素です。

![](../../../../../assets/material-1.png){width="800px"}
