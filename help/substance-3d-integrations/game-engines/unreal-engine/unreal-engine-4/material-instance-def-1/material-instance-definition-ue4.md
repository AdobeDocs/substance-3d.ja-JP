---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/material-instance-definition-ue4.html"
breadcrumb-title: ''
description: Unreal Engine 4でSubstanceマテリアルを使用してマテリアルインスタンス定義を作成し、GPUレンダリングパフォーマンスを最適化します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Material Instance Definition - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: マテリアルインスタンス定義 – UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---


# マテリアルインスタンス定義 – UE4

UE4マテリアルインスタンスはSubstanceで使用できます。 これにより、処理する新しいマテリアルをアップロードしないので、GPUレンダリングプロセスの大きなステップを節約できます。 MIDは、実行時に作成することも、エディタ内で作成することもできます。 バージョン4.24.0.3では、マテリアルのインスタンス化の完全なサポートが追加され、Substance engineでサポートされる数値出力を含む新しいマテリアルテンプレートワークフローが導入されました。 マテリアルテンプレートを使用すると、UE4でのSubstanceマテリアルシェーダの設定方法を正確に定義できます。

sbsarファイルを読み込むときに、使用するテンプレートを選択できます。

![](../../../../assets/ue4-material-templates.png)

タイリング、テクスチャサイズ、ディスプレイスメント、放射パラメータを調整するためのコントロールが組み込まれた、ディスプレイスメント、屈折、ワールド整合マテリアルを扱うためのテンプレートが同梱されています。 材料テンプレートシステムでは、独自のカスタムテンプレートを提供することもできます。

![](../../../../assets/ue4-material-instance-params.png)

## エディタでマテリアルインスタンスを作成する

1. UE4マテリアルで作成されたSubstanceを右クリックし、「マテリアルインスタンスを作成」を選択します。 これにより、UE4インスタンス化されたマテリアルが作成されます。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/01-12?$png$&jpegSize=100&wid=592){width="560px"}
1. Substanceインスタンスファクトリを右クリックして、「グラフインスタンスを作成」を選択します。 これにより、グラフのインスタンスが作成され、別のUE4マテリアルが作成されます。 新しく作成したUE4マテリアルは使用されないため、削除してください。

   ![](../../../../assets/02-10.png){width="300px"}
1. 手順1で作成したマテリアルインスタンスをダブルクリックし、すべてのマップのテクスチャパラメータを有効にします。
1. テクスチャを手順2で作成した新しいINSTテクスチャに設定します。 これにより、マテリアルインスタンスが、インスタンス化されたグラフからサブスタンス出力マップを使用するように設定されます。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/03-6?$png$&jpegSize=200&wid=1011){width="800px"}

特定のSubstanceテクスチャのセットを使用するUE4マテリアルインスタンスができました。 これは、UE4プロジェクトで複数のサブスタンスを扱う、より最適化された方法です。 ブループリントを使用してMIDを作成する方法については、こちらのページを参照してください。 [Blueprint(UE4)：動的なマテリアルインスタンス](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
