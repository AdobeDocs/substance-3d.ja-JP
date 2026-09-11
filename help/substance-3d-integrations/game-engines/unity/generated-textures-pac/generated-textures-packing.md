---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/generated-textures-packing.html"
breadcrumb-title: ''
description: SubstanceがUnityでテクスチャを生成する方法を理解し、最適なシェーダー入力のためにテクスチャパッキングを設定します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Generated Textures (Packing)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 生成されたテクスチャ(パッキング)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 6%

---


# 生成されたテクスチャ(パッキング)

生成されたテクスチャは、テクスチャを作成するためにSubstance engineによって計算された、Substanceからの出力を示します。 これらのテクスチャは、シェーダー入力に入力されます。 デフォルトでは、シェーダーで使用されるベース入力のみが作成されます。 「すべての出力を生成」が有効な場合は、すべてのテクスチャがここに表示されます。

![](../../../assets/screen-shot-2022-03-29-at-1-24-16-pm-copy.png)

「すべての出力を生成」が有効な場合

![](../../../assets/screen-shot-2022-03-29-at-1-29-35-pm-copy.png)

## 使用状況

1. テクスチャアイコンを選択すると、プロジェクトウィンドウ内のテクスチャが選択されます。 テクスチャがプロジェクトフォルダーで生成されないため、ランタイムマテリアルでは機能しません。
1. sRGBボタンは、 テクスチャ読み込み設定の「 sRGB（カラーテクスチャ） 」オプションと同様に機能します。 テクスチャをガンマ空間(sRGB)で変換するか、リニア化するかを指定できます。 Substanceプラグインはこの変換を自動的に処理しますが、必要に応じて上書きすることができます。

   | Substance出力 | sRGB |
   | --- | --- |
   | ベースカラー | 有効にする |
   | ディフューズ | 有効にする |
   | スペキュラ | 有効にする |
   | 法線 | 無効 |
   | メタリック | 無効 |
   | 粗さ | 無効 |
   | グロシネス | 無効 |
   | 高さ | 無効 |
   | アンビエントオクルージョン | 無効 |

## パッキングチャンネル

ドロップダウンメニューを使用して、テクスチャを別のテクスチャのアルファチャンネルにパックできます。 生成された各テクスチャには、Substanceマテリアルによって生成されたすべてのテクスチャ出力のリストを含むドロップダウンメニューがあります。 リストからマップを選択して、テクスチャのアルファチャンネルにパックします。 ソースオプションは、テクスチャのアルファチャンネルです。

この図では、高さマップを選択しています。

![](../../../assets/screen-shot-2022-03-29-at-2-48-33-pm.png)

次の図では、Height出力がbase colorマップのアルファチャンネルにパックされています。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-29-at-2-53-20-pm-copy?$png$&jpegSize=200&wid=1248)

## 出力テクスチャマッピング

さらに、出力テクスチャマッピングセクションを使用して、Unityマテリアルのサーフェス入力に個別に出力テクスチャを割り当てることができます。 .sbsarによって生成された出力テクスチャは左側の列に表示され、利用可能なUnity Surface Inputsは右側の列に表示されます。 その後は、ドロップダウンを使用して変更できます。

![](../../../assets/image2023-3-27-14-30-24.png)
