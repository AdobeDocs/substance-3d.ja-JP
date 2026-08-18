---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-node-reference.html"
breadcrumb-title: ''
description: Unreal Engine 4でマテリアルオペレーションに使用できるすべてのSubstanceBlueprintノードのリファレンスガイド。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Node Reference
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE4)ノードリファレンス
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%

---


# Blueprint(UE4)：ノード参照

## 一般Substanceノード：

| 名前 | 入力 | 説明 |
| --- | --- | --- |
| **GetSubstances** | マテリアル | マテリアルによって使用されるSubstance グラフインスタンスの配列を返します。 2つの異なるグラフインスタンスのテクスチャ出力を使用するマテリアルを作成した場合、この関数はそれらの2つのグラフインスタンスを返します。 |
| **GetSubstanceTextures** | **SubstanceGraphInstance** | Substance グラフインスタンス入力パラメータから、有効なテクスチャと現在計算されているテクスチャの配列を返します。 |
| **GetGraphName** | **SubstanceGraphInstance** | Designerで設定されたグラフ名を返します。 |
| **GetFactoryName** | **SubstanceGraphInstance** | このノードに渡される&#x200B;**SubstanceGraphInstance**&#x200B;の作成に使用された&#x200B;**GraphInstanceFactory**&#x200B;の名前を返します。 |
| **GetSubstanceLoadingProgress** | なし | 完全に読み込まれたサブスタンスの数のパーセンテージを示す0 ～ 1の浮動小数点を返します。 |
| **CreateGraphInstance** | 入力： **SubstanceInstanceFactory** – グラフインスタンスを作成するファクトリ。入力： **GraphIndex** (int) – 作成するグラフのインデックス。 入力： **InstanceName** (FString) – 新しいインスタンスに付ける名前。 | アプリケーションが閉じるまで保持される新しいスタンドアロングラフインスタンスを返します。 |
| **DuplicateGraphInstance** | **SubstanceGraphInstance** – コピーを作成するグラフインスタンス。 | アプリケーションが閉じるまで保持される新しいスタンドアロングラフインスタンスを返します。 |
| **EnableInstanceOutputs** | 入力： **SubstanceGraphInstance** – 入力を有効にする出力を含むグラフインスタンス： **OutputIndices** （int32配列） – 有効にする出力のインデックス。 （変更される場合があります） | 以前に無効にされていた場合は、**SubstanceGraphInstance**&#x200B;に渡されたのテクスチャ出力が作成されます。 これは、**SubstanceGraphInstance**&#x200B;エディターからの出力を有効にするのと同じ機能を持ちます。 *注意：これにより、新しく作成されたテクスチャでマテリアルが更新されることはありません。 この問題は、新しい出力を使用して実行時にsamplerパラメーターを設定することで処理する必要があります。* |
| **DisableInstanceOutputs** | 入力： **SubstanceGraphInstance** – 値を適用するグラフインスタンス。入力： **SubstanceGraphInstance** – 値を取得するグラフインスタンス。 | Substance グラフインスタンス入力パラメーターの変更された入力値をすべて復元します。 |
| **SetGraphInstanceOutputSize** | 入力： **SubstanceGraphInstance**&#x200B;入力：幅 – X座標のテクスチャ解像度入力：Height- Y座標のテクスチャ解像度 | このグラフインスタンスから生成されたすべての出力のテクスチャ解像度を、パラメーターから渡されたサイズで設定します。 メモ – CPUエンジンのMax 2048注意 – GPUエンジンのMax 4096 |
| **AsyncRendering** | **SubstanceGraphInstance** | Substance グラフインスタンス入力の出力テクスチャを再計算します。 （ブロックなし） |
| **SyncRendering** | **SubstanceGraphInstance** | Substance グラフインスタンス入力の出力テクスチャを再計算します。 （遮断） |

## グラフインスタンス固有の関数：

グラフインスタンスからのみ呼び出すことができます

| 名前 | 入力 | 説明 |
| --- | --- | --- |
| **GetInputNames** | なし | すべての入力パラメータ名を含む文字列の配列を返します。 |
| **GetInputType** | なし | この入力に関連付けられたデータ型を返します。 |
| **SetInputInt** | 入力： **識別子** （文字列）入力： **入力値** （int配列） | 識別子によって検出された入力の値を変更します。 ゲーム内から、変更を適用するには、**AyncRender**&#x200B;または&#x200B;**SyncRender**&#x200B;を使用してサブスタンスをレンダリングする必要があります。 |
| **SetInputFloat** | 入力： **Identifier** （文字列）入力： **InputValues** （実数配列） | 識別子によって検出された入力の値を変更します。 ゲーム内から、変更を適用するには、**AyncRender**&#x200B;または&#x200B;**SyncRender**&#x200B;を使用してサブスタンスをレンダリングする必要があります。 |
| **GetInputInt** | 入力： **識別子** （文字列） | 入力パラメーターの現在の値を含むintの配列を返します。 |
| **GetInputFloat** | 識別子（文字列） | 入力パラメータの現在の値を持つ浮動小数点の配列を返します。 |
| **SetInputBool** | 入力： **Bool** （ブール値）入力： **識別子** （文字列） | 切り替え可能な入力値タイプを割り当てるブール値を取ります。 以前は、これはboolにキャストされたint値を1または0に設定することによってのみ実現できました。 |
| **GetInputBool** | 入力： **識別子** （文字列） | 入力の現在のブール値を返します。 |
| **SetIputColor** | 入力： **Color** (LinearColor)入力： **識別子** (FString) | 入力カラー値のタイプを割り当てるFLinearColor値を取ります。 以前は、float値を設定し、floatの配列を渡すことによってのみ、この操作が可能でした。 |
| **GetInputColor** | 入力：識別子(FString) | 現在のカラー値をUE4形式で返します。 |
| **CreateAggregateSubstanceFactory** | 入力： **出力ファクトリ** (SubstanceInstanceFactory)*入力ファクトリへの入力として使用される出力を作成するファクトリ。*&#x200B;入力： **出力ファクトリグラフインデックス** （整数）*結合に使用するSubstance内のどのグラフ。* 入力： **入力ファクトリ** (SubstanceInputFactory)*出力ファクトリからの入力画像として出力を使用するファクトリ。*入力：**接続**（SubstanceConnectionsの配列）*これは、ブループリントノードのMake Arrayを使用して作成できます。 Substance接続は、入力した集計ノードを、どの出力にリンクさせるかを指定する方法です。* **&#x200B; Return (SubstanceInstanceFactory)***新しい結合されたインスタンスのグラフインスタンスを作成するために使用できます。* | 新しい集約substanceノードでは、2つのsubstanceインスタンスファクトリを使用して、実行時に新しいインスタンスファクトリを作成できます。このファクトリを使用して、新しいグラフインスタンスを作成できます。 この特別な機能は、一方の複合グラフインスタンスの出力テクスチャを、もう一方の複合グラフインスタンスの入力イメージにコネクトできることです。 この新しいファクトリからsubstance graphインスタンスを作成するには、ランタイムグラフインスタンスに関するドキュメントを参照してください。 |
| **SubstanceConnectionStruct** | 入力： **出力識別子** (FString)*入力にチェーンするテクスチャ出力の識別子。* 入力： **入力識別子** (FString) | 集約Substanceファクトリの作成で、各出力テクスチャを新しい入力テクスチャでチェーンする方法を指定するために使用します。 |
