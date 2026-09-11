---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/material-instance-definition-ue4.html"
breadcrumb-title: ''
description: アンリアルエンジン 4でSubstanceマテリアルを使用してマテリアルインスタンス定義を作成し、GPUレンダリングパフォーマンスを最適化します。
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

UE4 マテリアルインスタンスはSubstanceで使用できます。 これにより、新しいマテリアルをプロセスにアップロードしないので、GPUレンダリングプロセスの大きな手順を省くことができます。 MIDは、実行時に作成することも、エディタ内で作成することもできます。 バージョン4.24.0.3では、マテリアルのインスタンス化の完全なサポートが追加され、Substance engineでサポートされる数値出力を含む新しいマテリアルテンプレートワークフローが導入されました。 マテリアルテンプレートを使用すると、UE4でのSubstanceマテリアルシェーダの設定方法を正確に定義できます。

sbsar ファイルを読み込むときに、使用するテンプレートを選択できます。

![](../../../../assets/ue4-material-templates.png)

タイリング、テクスチャサイズ、ディスプレイスメント、emissiveパラメーターを調整するためのコントロールが組み込まれた、ディスプレイスメント、屈折、ワールド整合マテリアルを操作するためのテンプレートが同梱されています。 マテリアルテンプレートシステムでは、独自のカスタムテンプレートを提供することもできます。

![](../../../../assets/ue4-material-instance-params.png)

## エディタでのマテリアル・インスタンスの作成

1. Substanceで作成されたUE4 マテリアルを右クリックし、「マテリアルインスタンスを作成」を選択します。 これにより、UE4インスタンスマテリアルが作成されます。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/01-12?$png$&jpegSize=100&wid=592){width="560px"}
1. Substanceインスタンスファクトリを右クリックして、「グラフインスタンスを作成」を選択します。 これにより、グラフのインスタンスが作成され、別のUE4 マテリアルが作成されます。 新しく作成したUE4 マテリアルは使用しないため、削除します。

   ![](../../../../assets/02-10.png){width="300px"}
1. 手順1で作成したマテリアルインスタンスをダブルクリックし、すべてのマップのテクスチャパラメーターを有効にします。
1. 手順2で作成した新しいINST テクスチャにテクスチャを設定します。 これにより、インスタンス化されたグラフのSubstance出力マップを使用するようにマテリアルインスタンスが設定されます。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/03-6?$png$&jpegSize=200&wid=1011){width="800px"}

これで、特定のSubstance テクスチャのセットを使用するUE4 マテリアルインスタンスができました。 これは、UE4プロジェクトで複数のサブスタンスを扱う、より最適化された方法です。 ブループリントを使用してMIDを作成する方法については、こちらのページを参照してください。 [Blueprint(UE4)：動的マテリアルインスタンス](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
