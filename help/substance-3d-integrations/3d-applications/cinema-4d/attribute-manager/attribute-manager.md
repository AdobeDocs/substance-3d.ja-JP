---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/cinema-4d/attribute-manager.html"
breadcrumb-title: ''
description: Cinema 4Dの属性マネージャーを使用して、Substanceアセットのプロパティとマテリアルを構成します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Attribute Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 属性マネージャー
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# 属性マネージャー

Cinema 4Dの属性マネージャーには、Substanceアセット用の新しいモードがあります。

SubstanceアセットマネージャーでSubstanceを選択すると、属性マネージャーは自動的にSubstanceアセットモードに切り替わります。 アトリビュートマネージャのモードメニューでこのモードに手動で切り替えることもできます。

Substanceアセットモードでは、Substanceのすべての入力にアクセスでき、すべての出力チャンネルの概要も表示されます。

![](../../../assets/cinema-4d-9.png){width="500px"}

## Substance入力のグループ化

Substanceの入力がグループ化されている場合、これらのグループは属性管理ウィンドウに表示されます。 事前定義された2つのグループがあります： **基本プロパティ**&#x200B;と&#x200B;**画像入力**。

* 基本プロパティグループには、Substance Designerのグループに割り当てられていないすべての入力が表示されます。
* その名前が既に示すように、外部画像にリンクするすべてのSubstance入力は、画像入力グループに収集されます。

## ファイル名パラメーター

属性マネージャーのファイル名パラメーターを使用すると、Substanceアセットをシーンーに読み込んだ後で、アセットのファイルの場所を変更できます。

![](../../../assets/cinema-4d-10.png){width="500px"}

これは、Substanceファイルを再配置する場合だけでなく、Substanceを完全に異なるディレクトリに置き換える場合にも役立ちます。

この場合、以前のSubstance出力チャンネルに対する既存のリファレンスを新しいSubstanceに再マッピングするかどうかを確認するメッセージが表示されます。

![](../../../assets/cinema-4d-11.png){width="500px"}

質問に「いいえ」と回答した場合、前のSubstanceへのリンクはすべてのSubstanceシェーダから削除されます。 出力チャンネルを再マップするには、最初に同じタイプの出力チャンネルが検索されてから、同じ名前の出力チャンネルが検索されます。

## パラメーターの三状態

複数のSubstanceを同時に選択した場合、これらのSubstance間で共有される入力は3段階として表示され、Cinema 4D内の他のすべてのパラメータと同様に、選択したすべてのSubstanceに対して同時に編集することができます。

このような場合、出力チャンネルは次のように表示されます。

![](../../../assets/cinema-4d-12.png){width="300px"}
