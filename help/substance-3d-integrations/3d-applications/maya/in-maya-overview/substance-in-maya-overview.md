---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/substance-in-maya-overview.html"
breadcrumb-title: ''
description: MayaのSubstanceプラグインと、ワークフローでSubstance マテリアルをインポートおよび使用する方法について説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance in Maya Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MayaのSubstanceの概要
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# MayaのSubstanceの概要

## プラグインの概要

Substanceプラグインを使用すると、Substance Designerで作成したSubstance マテリアルを直接Mayaにロードできます。 このプラグインはMaya マテリアルを作成し、substance テクスチャをマテリアルチャンネルの入力に送ります。 その後、substanceパラメーターに変更を加えると、テクスチャが自動的に更新されます。

>[!NOTE]
>
> 設定/プリファレンス> Mayaプラグインマネージャにプラグインがロードされていることを確認します。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/plugin-4?$png$&jpegSize=100&wid=618)

## Substanceのオープン

1. ハイパーシェードを開き、ノードエディタで右クリックし、マーキングメニューを上にスワイプしてノードの作成を選択します。 「ノードを作成」ウィンドウが開きます。 ここから、Substanceノードを検索できます。

   ![](../../../assets/createnode.png)

   ノードエディターのtabを押して、テキストフィールドに「substance」と入力すると、substanceオプションにフィルターされます。 オプションから、「テクスチャ」を選択します。
1. Substanceノードを選択し、プロパティーエディタで参照してSubstance (.sbsar)ファイルを読み込みます。

   ![](../../../assets/1.png)
1. Substanceに複数のグラフが含まれている場合は、「選択したグラフ 」ドロップダウンが表示されます。 選択したグラフは、マテリアルの作成に使用されます。
1. 「グラフ情報」ボタンをクリックすると、Substance Designerに設定されているグラフ属性が表示されます。
1. 幅とHeightのドロップダウンボックスから値を選択して、解像度を設定します。 ロック比率はデフォルトで有効になっています。
1. ディスクへのキャッシュ出力を有効にして、Substance出力をディスクにベイクし、Arnoldなどのレンダラーで使用できるようにします。 キャッシュされたファイルは、プラグインがMayaファイルノードを使用して読み取り戻します。

   ![](../../../assets/outputsettings.png)
1. 使用しているレンダラーのワークフローを選択し、「 シェーダーネットワークを作成」ボタンをクリックします。 レンダラーワークフロー用にシェーダーネットワークが作成されます。 これで、シーンでマテリアルを適用できます。

   ![](../../../assets/createnetwork.gif){width="1000px"}
