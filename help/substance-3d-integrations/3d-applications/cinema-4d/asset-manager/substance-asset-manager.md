---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/cinema-4d/substance-asset-manager.html"
breadcrumb-title: ''
description: Cinema 4DのSubstanceアセットマネージャを使用して、シーン内のSubstanceマテリアルを追加、削除、整理します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Substance Asset Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substanceアセットマネージャー
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---


# Substanceアセットマネージャー

Substanceアセットマネージャウィンドウには、シーンにロードされているすべてのSubstanceが一覧表示されます。 ここでは、Substanceを追加、削除、整理できます。

Substanceアセットマネージャー内のSubstanceを選択（左クリック）すると、Cinema 4Dの属性マネージャーでSubstanceが開きます。 Cinema 4Dの他のパラメーターと同様に、パラメーターとキーフレームのSubstance入力を変更できます。

>[!NOTE]
>
> Attribute Managerには特別なSubstanceアセットモードがあり、Cinema 4DレイアウトにSubstance専用のAttribute Managerを用意するのに便利です。

![](../../../assets/cinema-4d-4.png){width="500px"}

## ファイルメニュー

## アセットを読み込み…

シーンに新しいSubstanceをロードします（プラグインメニューと同じ）。

閉じる

Substanceアセットマネージャーを閉じます。 読み込まれたSubstanceはもちろんシーンに残ります。

## 編集メニュー

## すべてのSubstanceを選択

Asset ManagerにリストされているすべてのSubstanceを選択します。 Ctrl+aを押しながらマウスをAsset Managerの上に置くことでも同じことが可能です。

## すべてのSubstanceを選択解除

Asset Managerに表示されているすべてのSubstanceの選択を解除します。 Shift+Ctrl+aを押しながら、マウスをアセットマネージャーの上に置くことでも同様のことが可能です。

## 選択したマテリアルから選択

現在&#x200B;*選択*&#x200B;されているマテリアルによって参照されているすべてのSubstanceを選択します。

## マークされたマテリアルから選択

現在&#x200B;*マークされている*&#x200B;のマテリアルによって参照されているすべてのSubstanceを選択します。 Cinema 4Dでは、このマテリアルを使用するオブジェクトまたはタグが選択されている場合、マテリアルはマークされます。

## マテリアルを選択

現在選択されているマテリアルを参照するすべてのSubstanceを選択します。

## アクションメニュー

## マテリアルを作成

現在選択されているSubstanceから新しいCinema 4Dマテリアルを作成します。 マテリアルチャンネルは、Substanceのそれぞれの出力チャンネルを参照するSubstanceシェーダで自動的に初期化されます。

## Substanceが重複しています

現在選択されているSubstanceを複製します。 これは、複数のマテリアルで異なるパラメータセットを使用して同じSubstanceを使用する場合に便利です。

## Substanceを再読み込み

この関数を使用して、Substanceのデフォルト値に戻したり、外部からの変更（Substance Designerからの変更など）を取り込んだりすることができます。\
注意： Substance入力の&#x200B;**すべての**&#x200B;パラメーターの変更が失われます！

## Substanceを削除

現在選択されているSubstanceをシーンから削除します。 同じことが、Asset Managerの上にマウスを置いた状態でDeleteキーを押すことで実現できます。

## 未使用のSubstanceを削除

現在どのマテリアルからも参照されていないすべてのSubstanceを削除します。

## Substance engineメニュー

このメニューの内容は、Cinema 4Dを実行しているオペレーティング・システムによって異なります。 Substance engineの変更は、Cinema 4Dの再起動後にのみ有効になります。

## コンテキストメニュー

選択したSubstanceを右クリックすると、コンテキストメニューが表示されます。 これらの機能は、前述のメニューで同じ名前が付けられた関数と同じです。

* 削除
* マテリアルを作成
* Substanceを複製
* Substanceを再読み込み
* すべてのSubstanceを選択
* すべてのSubstanceを選択解除
* マテリアルを選択

## ドラッグ&amp;ドロップ

Substanceアセットマネージャーは、ドラッグ&amp;ドロップで操作できます。 次のオプションが用意されています。

* エクスプローラまたはFinderからSubstanceをSubstanceアセットマネージャにドラッグアンドドロップするだけで、アセットをシーンにロードできます。
* SubstanceをSubstanceシェーダのリンクフィールドにドラッグして、シェーダとSubstanceアセットをコネクトすることができます。
* 並べ替え解除モード（以下を参照）の場合は、Substanceを新しい場所にドラッグすると、Asset Managerでアセットを並べ替えることができます。


## Substanceアセットマネージャーでの並べ替え

## ソートされていないモード

## Substanceアセットマネージャーは、既定で&#x200B;**並べ替え解除モード**&#x200B;になっています。 名前列のヘッダーセルの右側に矢印は表示されません。 ドラッグ&amp;ドロップで、好みに合わせて物質を再配置できます。

![](../../../assets/cinema-4d-3.png){width="500px"}

![](../../../assets/cinema-4d-5.png){width="500px"}

## Substanceアセットマネージャーでのプレビュー

## Substanceアセットマネージャーには、各Substanceで使用可能なチャンネルのプレビューを含む小さなアイコンが表示されます。

## プレビューは、Substanceの出力チャンネルの順に表示されるだけです。 プレビューが表示される列に意味はありません。
