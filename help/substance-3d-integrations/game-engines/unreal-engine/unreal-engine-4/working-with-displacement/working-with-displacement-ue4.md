---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-displacement-ue4.html"
breadcrumb-title: ''
description: サーフェスの詳細については、アンリアルエンジン 4でSubstanceマテリアルのディスプレイスメントマップを使用してテセレーションを有効にします。
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

ディスプレイスメントを使用するには、マテリアルーのテセレーションを有効にする必要があります。

![](../../../../assets/tess.png){width="600px"}

Height出力を使用するには、Substance・ファクトリ・インスタンスの出力をダブルクリックしてHeightを作成する必要があります。 デフォルトでは、Heightは有効になっていません。 次に、このHeight出力をマテリアルにドラッグできます。

![](../../../../assets/height-1.png){width="800px"}

マテリアルにHeight出力を追加したら、ワールドディスプレイスメントとテセレーションモディファイヤを駆動するノードをいくつか作成する必要があります。

1. 2つのスカラーパラメーターを作成します。 1つは[距離]で、もう1つは[テセレーション]の乗数です。
1. Heightから[距離]パラメータに赤チャンネルを掛けます
1. VertexNormalWSノードを追加し、手順2の乗算結果と乗算します。
1. VertexNormalの乗数をマテリアルのワールドディスプレイスメントに入力します。
1. [テセレーションマルチプライヤ]パラメータを指定し、マテリアルの[テセレーションマルチプライヤ]にこのパラメータを入力します。

![](../../../../assets/setup-3.png){width="800px"}

>[!NOTE]
>
> この図では、グラフを簡素化するために、他のテクスチャ出力が省略されています。 ここでは、ディスプレイスメントノードとマルチプライヤノードのみが分かりやすくするために表示されています。
