---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-substance-material-parameters.html"
breadcrumb-title: ''
description: Unreal Engine 4では、動的なマテリアルコントロール用のBlueprintノードを使用して、実行時にSubstanceマテリアルパラメーターを変更します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Substance material parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE4)Substanceのマテリアルパラメーター
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---


# Blueprint(UE4):Substanceのマテリアルパラメーター

## フロートパラメータを変更する：

[入力浮動小数点の設定](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-node-reference-151584784.html)を使用して、float、color(float4)、およびブール型substanceパラメーターを変更します。

1. 「変数インスタンス」という型を参照としてSubstance グラフを作成します。
1. Set Input Float Nodeを作成し、ターゲットをSubstance グラフインスタンス変数として設定します。
1. [入力実数を設定]ノードで、変更するSubstanceパラメータの名前を[識別子]に設定します。\
   *\* Substance INSTを開き、パラメーター名の上にマウスポインタを置くと、ID名を検索できます。 識別子の名前は、ツールヒントポップアップに表示されます。*
1. 入力実数ノード上で、接続をドラッグして配列ノードを作成します。 Make Array Nodeのインデックスは0です。 0のインデックスはfloat値に対応します。
1. AsyncまたはSyncレンダリングノードを作成し、Set Input FloatからRender Nodeに実行ラインを接続します。 レンダリングするインスタンスをSubstance グラフインスタンス変数に設定します。\
   *\*&#x200B;非同期は非ブロックであり、同期はブロックしています。*

![](../../../../../assets/steps.png){width="800px"}

## ブール値パラメーター

ブール値のパラメータは、Set Input Boolを使用して変更します。

![](../../../../../assets/setbool.png){width="800px"}

## カラーパラメーター

カラーパラメーターは、入力カラーの設定を使用して変更します

![](../../../../../assets/setcolor.png){width="800px"}

## 整数パラメータの変更：

整数パラメータは、入力浮動小数点の設定と同じように機能します。 「入力整数を設定」ノードを使用します。

![](../../../../../assets/int.png)

## 識別子

パラメータの識別子はSubstance INSTで確認できます。 パラメーターの上にマウスを移動すると、ツールヒントに識別子名が表示されます。 これは、Substance Designer内の出力のIDフィールドで設定された名前です。

![](../../../../../assets/indent-1.png){width="800px"}
