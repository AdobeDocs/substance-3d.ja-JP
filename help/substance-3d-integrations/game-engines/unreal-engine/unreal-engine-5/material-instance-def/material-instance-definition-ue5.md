---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-instance-definition-ue5.html"
breadcrumb-title: ''
description: アンリアルエンジン 5でSubstanceマテリアルを使用してマテリアルインスタンス定義を作成し、GPUレンダリングパフォーマンスを最適化します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Instance Definition - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: マテリアルインスタンス定義 – UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---


# マテリアルインスタンス定義 – UE5

UE5 マテリアルインスタンスはSubstanceで使用できます。 これにより、新しいマテリアルがプロセスにアップロードされないので、GPUレンダリングプロセスの大きな手順を省くことができます。 MIDは、実行時に作成することも、エディタ内で作成することもできます。 バージョン5.0.0では、マテリアルインスタンス化の完全なサポートが追加されました。

## エディタでのマテリアル・インスタンスの作成

1. Substanceで作成されたUE5 マテリアルを右クリックし、「マテリアルインスタンスを作成」を選択します。 これにより、UE5インスタンスマテリアルが作成されます。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-31-at-6-07-08-pm?$png$&jpegSize=300&wid=1472)
1. Substanceインスタンスファクトリを右クリックして、「グラフインスタンスを作成」を選択します。 これにより、グラフのインスタンスが作成され、別のUE5 マテリアルが作成されます。 新しく作成されたUE5 マテリアルは使用されないため、削除してください。

   ![](../../../../assets/screen-shot-2022-03-31-at-6-10-38-pm.png)
1. 手順1で作成したマテリアルインスタンスをダブルクリックし、すべてのマップのテクスチャパラメーターを有効にします。
1. 手順2で作成した新しいINST テクスチャにテクスチャを設定します。 これにより、インスタンス化されたグラフのSubstance出力マップを使用するようにマテリアルインスタンスが設定されます。

   ![](../../../../assets/screen-shot-2022-03-31-at-6-13-18-pm.png)

これで、一連のSubstance テクスチャを使用するUE5 マテリアルインスタンスができました。 これは、UE5プロジェクトで複数のサブスタンスを扱う、より最適化された方法です。 ブループリントを使用してMIDを作成する方法については、こちらのページを参照してください。 [Blueprint(UE5)：動的マテリアルインスタンス](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
