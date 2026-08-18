---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/changing-parameters.html"
breadcrumb-title: ''
description: UnityでSubstanceのマテリアルパラメーターを変更し、実行時にマテリアルの外観とプロパティをカスタマイズします。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Changing parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: パラメーターの変更
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# パラメーターの変更

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

Substanceマテリアルのパラメータには、Substance グラフオブジェクト(SGO)からアクセスできます。

1. プロジェクトウィンドウで、カスタマイズするグラフのsbsarファイルロゴを選択します。 sbsarには緑色の「SBSAR」ロゴがあります。

   ![](../../../assets/screen-shot-2022-03-29-at-2-27-56-pm.png)

## 手続き型プロパティ

1. **すべての出力を生成**: Substanceのsbsarファイルからすべての出力を生成します。 デフォルトでは、標準シェーダが使用する出力のみが作成されます。
1. **ミップマップの生成**：各Substance出力のミップテクスチャを生成します。
1. **ランダムシード**：このボタンをクリックすると、Substanceグラフがテクスチャの生成に使用するランダムシードが変化します。 この値を変更すると、シード値に基づいて計算されたテクスチャの新しい結果が作成されます。
1. Substanceファイルで公開されているパラメータは、Unityで使用できます。 エディターコントロールは、Substance用に作成されたパラメーターの種類に基づきます。
1. **プリセットの処理：** Substanceプリセットファイル(SARS)をエクスポートまたはインポートできます。 プリセットを書き出すと、Substanceのパラメーター設定に基づいてプリセットファイルが作成されます。 Substance DesignerーおよびSubstance Playerからプリセットファイルを書き出し、「プリセットを読み込み」ボタンを使用してそのプリセットファイルを読み込むことができます。 これは、複数のアプリケーションやチームでSubstanceプリセットを共有する場合に便利です。

</td>
<td style="border: 0;" valign="top">

![](../../../assets/changing-parameters.png)

</td>
</tr>
</table>
