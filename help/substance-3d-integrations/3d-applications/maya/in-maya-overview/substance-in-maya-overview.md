---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/substance-in-maya-overview.html"
breadcrumb-title: ""
description: MayaのSubstanceプラグインと、ワークフローでSubstance マテリアルをインポートおよび使用する方法について説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance in Maya Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MayaのSubstanceの概要
user-guide-description: ""
user-guide-title: ""
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%
---

# MayaのSubstanceの概要

## プラグインの概要

MayaプラグインのSubstanceを使用すると、既存のSubstance 3D マテリアル(.Sbsar ファイル)をMayaに直接ロードすることができます。 Substance 3D マテリアルは、Substance 3D DesignerまたはSubstance 3D SamplerからSBSARファイルとして作成および書き出しでき、Substance 3D Assetsライブラリなどの既存のライブラリからダウンロードできます。 MayaプラグインのSubstanceは、Maya マテリアルを作成し、出力テクスチャを正しいマテリアルチャンネル入力に送ります

>[!NOTE]
>
> 設定/プリファレンス> Mayaプラグインマネージャにプラグインがロードされていることを確認します。

## ハイパーシェードノードエディタでSbsar ファイルを開く

1. **ハイパーシェード**&#x200B;を開き、**ノードエディター**&#x200B;で、マーキングメニューを右クリックして上にスワイプし、**ノードの作成**&#x200B;を選択します。 **ノードの作成ウィンドウ**&#x200B;で、**Substanceノード**&#x200B;を検索して選択します。

   ![](../../../assets/createnode.png)

   ハイパーシェードで&#x200B;**Substanceノード**&#x200B;をクリックして選択します。 **マテリアルエディター**&#x200B;が開き、フォルダーアイコンをクリックしてSubstance 3D マテリアル (Sbsar ファイル)を読み込むことができます。

1. または、Sbsar ファイルをMayaの&#x200B;**ハイパーシェードエディタ**&#x200B;にドラッグアンドドロップし、自動的に作成されたSubstanceノードをクリックして、**マテリアルエディタ**&#x200B;でオプションを直接表示および編集することもできます。

### プロパティエディターでのSBSARパラメーターの再生

![](../../../assets/1.png)

1. Substanceに複数のグラフが含まれている場合は、**選択したグラフドロップダウン**&#x200B;が設定されます。 マテリアルの作成に使用するグラフを選択します。

1. [**グラフ情報]ボタン**&#x200B;は、Substance Designerに設定されているグラフ属性を表示します。

1. **幅**&#x200B;と&#x200B;**Height**&#x200B;の値を設定して解像度を設定します。 **縦横比の固定**&#x200B;を無効にして、非正方形の縦横比を選択します。

1. **ディスクへの出力のキャッシュ**&#x200B;を有効にして、Substanceへの出力をディスクにベイクし、Arnoldなどのレンダラーで使用できるようにします。 キャッシュされたファイルは、プラグインがMayaファイルノードを使用して読み取り戻します。

   ![](../../../assets/outputsettings.png)

1. 使用しているレンダラーのワークフローを選択し、[**シェーダーネットワークの作成**]をクリックします。 レンダラーワークフロー用にシェーダーネットワークが作成されます。 バージョン3.1.1では、ワークフローの一覧にシェーダーネットワークを作成するオプションも表示されます。 シェーダーネットワークが作成されたら、シーンにマテリアルを適用できます。

   ![](../../../assets/createnetwork.gif){width="1000px"}

## トラブルシューティング

バグを報告するには、[Substance Discordサーバー](https://discord.com/invite/substance3d)の#maya-pluginチャンネルに参加するか、[Adobeコミュニティ](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-autodesk3dsmax)にアクセスしてください。 コンソールログからの関連情報と再現手順を含めることで、問題をより効率的に診断できます。