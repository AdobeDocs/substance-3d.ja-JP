---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-displacement-ue4.html"
breadcrumb-title: ''
description: サーフェスの詳細については、テッセレーションを有効にし、Unreal Engine 4のSubstanceマテリアルからディスプレイスメントマップを使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Displacement - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ディスプレイスメントの操作 – UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# ディスプレイスメントの操作 – UE4

ディスプレイスメントを使用するには、マテリアルでテッセレーションを有効にする必要があります。

![](../../../../assets/tess.png){width="600px"}

Height出力を使用するには、Substance・ファクトリ・インスタンスの出力をダブルクリックしてHeightを作成する必要があります。 デフォルトでは、Heightは有効になっていません。 次に、このHeight出力をマテリアルにドラッグできます。

![](../../../../assets/height-1.png){width="800px"}

Height出力をマテリアルに追加したら、ワールドディスプレイスメントとテッセレーションモディファイヤを動かすためにいくつかのノードを作成する必要があります。

1. 2つのスカラーパラメーターを作成します。 一方は[距離]で、もう一方は面分割のマルチプライヤです。
1. Heightから[距離]パラメータに赤チャンネルを掛けます
1. VertexNormalWSノードを追加し、手順2の乗算結果と乗算します。
1. マテリアルのワールドディスプレイスメントに対するVertexNormalの乗数を入力します。
1. テッセレーション乗数パラメータを取得し、これをマテリアルのテッセレーション乗数に入力します。

![](../../../../assets/setup-3.png){width="800px"}

>[!NOTE]
>
> グラフを簡素化するために、この画像では他のテクスチャ出力が省略されています。 ここでは、ディスプレイスメントノードとマルチプライヤノードのみが分かりやすくするために表示されています。
