---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-substance-material-parameters.html"
breadcrumb-title: ''
description: Blueprintノードを使用して動的なマテリアル制御を行い、Unreal エンジン 4で実行時にSubstanceマテリアルパラメーターを変更します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Substance material parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE4)マテリアルパラメーター
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---


# Blueprint(UE4):マテリアルパラメーター

## フロートパラメータを変更する：

[入力浮動小数の設定ノード](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/blueprint-node-reference-151584784.html)を使用して、float、color(float4)、およびブーリアンのsubstanceパラメーターを変更します。

1. 「変数インスタンス」という型を参照としてSubstance グラフを作成します。
1. セット入力浮動小数ノードを作成し、ターゲットをSubstance グラフインスタンス変数として設定します。
1. 「入力浮動小数の設定」ノードで、変更するSubstance識別子の名前をパラメータに設定します。\
   *\* Substance INSTを開き、識別子名の上にカーソルを置くと、パラメーター名が表示されます。 識別子名はツールヒントポップアップに表示されます。*
1. 入力浮動小数ノードで、コネクションをドラッグして配列ノードを作成します。 Make Array Nodeのインデックスは0です。 0のインデックスはfloat値に対応します。
1. AsyncまたはSyncレンダリングノードを作成し、入力の設定ノードからレンダー浮動小数に実行ラインをコネクトします。 レンダリングするインスタンスをSubstance グラフインスタンス変数に設定します。\
   *\*&#x200B;非同期は非ブロックであり、同期はブロックしています。*

![](../../../../../assets/steps.png){width="800px"}

## ブーリアンパラメーター

ブーリアンパラメーターは、Set Input Boolを使用して変更します。

![](../../../../../assets/setbool.png){width="800px"}

## カラーパラメーター

カラーパラメーターは、入力カラーの設定を使用して変更します

![](../../../../../assets/setcolor.png){width="800px"}

## 整数パラメーターの変更：

整数パラメーターは、入力を設定浮動小数ーと同じように機能します。 「入力を設定」整数ノードを使用します。

![](../../../../../assets/int.png)

## 識別子

Substance INSTでパラメーターの識別子を確認できます。 パラメーターの上にマウスを置くと、ツールヒントに識別子名が表示されます。 これは、Substance Designerー内の出力の識別子フィールドで設定された名前です。

![](../../../../../assets/indent-1.png){width="800px"}
