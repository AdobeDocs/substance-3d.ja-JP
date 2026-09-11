---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/blender/the-substance-3d-panel.html"
breadcrumb-title: ''
description: BlenderでSubstance 3Dパネルを使用して、マテリアル、パラメーター、出力を管理する方法について説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > The Substance 3D Panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3Dパネル
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---


# Substance 3Dパネル

![](../../../assets/blender-substance3dpanel.png)

## パネルコントロール

**作成** – ファイルブラウザーを開いて、Substance 3D マテリアルを選択します。 デフォルトでは、 .sbsar ファイルから生成されたテクスチャを使用してブレンダーマテリアルが作成されます。

**適用** – 選択したSubstance 3D マテリアルを新しいマテリアルスロットの選択したオブジェクトに適用します。 これは、オブジェクトの以前のマテリアル割り当てを上書きしません。

**Substance 3D コミュニティアセット** - WebブラウザーでSubstance 3D コミュニティアセットページを開きます。

**Substance 3D Assets** - WebブラウザーでSubstance 3D Assetsソースページを開きます。

**選択したSubstance 3D マテリアルを複製** – 選択したSubstance 3D マテリアルの新しいインスタンスを読み込みます。 同じマテリアルの異なるインスタンスのパラメーターは、互いに独立して調整できます。

**更新** - Substance 3D マテリアルを再読み込みします

>[!WARNING]
>
> **警告：**
> 
> 「更新」ボタンを使用すると、グラフに対するユーザーの変更が取り消されます。 更新する前にユーザーが追加したノードをコピーして、更新後にグラフに貼り付けます。

**削除** – 選択したSubstance 3D マテリアルをパネルから削除します。

>[!NOTE]
>
> マテリアルから作成されたブレンダーマテリアルはプロジェクトに残ります。 オブジェクトから手動で削除することができます。

**読み込まれた3D マテリアル** - .blendファイルに読み込まれたSubstanceマテリアルの一覧を表示します。

## グラフパラメーター

**出力解像度** – 解像度が「使用」および「Height」のドロップダウンで表示されます。 これらのリンクを解除して、値を個別に調整できます。

**ランダム化とランダムシード** – ランダム化ボタンは、ランダムな値を使用できるパラメーターを変更するために新しいランダムシード値を生成します。 ランダムシードは手動で設定することもできます。

## プリセットの操作

SBSARファイルはプリセットを使用して公開できます。プリセットは、プリセットドロップダウンボックスにあります。 独自のプリセットを作成するには、必要に応じてパラメーターを調整し、「**保存**」ボタンを使用します。 選択したプリセットを.sbsprsファイルとして書き出したり、ドロップダウンリストから選択したプリセットを削除したりするための追加オプションがあります。 「**読み込み**」ボタンを使用すると、.sbsprsファイルからプリセットを読み込むことができます。

## Substanceパラメーター

Substance Designerで表示されたパラメーターは、Substanceパラメーターのコントロールを使用して調整できます。 これらのパラメーターはマテリアルーの作成者によって設定され、マテリアルによって異なります。 これらのパラメーターを調整すると、生成されたテクスチャが更新され、ロードされた3D Substanceマテリアルセクションのマテリアル名の横に処理アイコンが表示されます。

出力テクスチャのファイルフォーマットは、ドロップダウンで切り替えたり変更したりできます。

詳細については、Designerドキュメントページの[パラメーターの表示](https://experienceleague.adobe.com/ja/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter)を参照してください。

## 技術パラメーター

マテリアルには、一連の技術的なパラメーターが含まれる場合があります。 これらは、カラー補正およびその他のマテリアル調整のための追加のコントロールです。
