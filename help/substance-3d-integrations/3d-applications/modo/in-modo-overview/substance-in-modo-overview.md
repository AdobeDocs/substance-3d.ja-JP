---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/substance-in-modo-overview.html"
breadcrumb-title: ''
description: MODO用のSubstanceプラグインについて、およびワークフローでSubstanceマテリアルを読み込んで使用する方法について説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Substance in MODO Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MODOのSubstanceの概要
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 5%

---


# MODOのSubstanceの概要

## 概要：

## Substanceのオープン

1. マテリアルを作成するか、マテリアルグループを選択します。
1. テクスチャ/Substanceで、「Substanceを作成」を選択するか、Substanceキットのオプションの下にある「作成」ボタンを使用します。 これにより、シェーダツリーにSubstanceマテリアルが作成されます。
1. 「sbsarを読み込む」をクリックして、sbsarファイルを読み込みます。

   ![](../../../assets/load-1.png)

## 出力の作成

**Default - Principled シェーディングモード**&#x200B;を使用すると、メタリック/ラフネスのワークフローを使用して出力を作成できます。

1. Substanceプロパティの「出力」セクションで、シェーディングに必要な出力をクリックします。 Substanceテクスチャが生成され、適切なマテリアルレイヤーエフェクトとともにシェーダツリーに追加されます。 Principledシェーディングモードの場合は、次のものが必要です。

   | Substance出力 | カラースペース | マテリアルレイヤー効果（原則シェーディングモード） |
   | --- | --- | --- |
   | ベースカラー | sRGB | 拡散カラー |
   | 法線 | 線形 | 法線 |
   | 粗さ | 線形 | 粗さ |
   | メタリック | 線形 | メタリック |

   ![](../../../assets/outputs-3.png)

## 解像度/パラメーターの変更

Substanceパラメータを変更して、生成されたテクスチャを更新または変更できます。 パラメータを変更すると、Substance engineはMODOマテリアルに供給されるテクスチャを再計算します。

1. Substanceマテリアルの[Substanceプロパティ]に移動し、[ツイーク]セクションで任意のパラメータを変更します。

   ![](../../../assets/params.png)
1. 生成されるテクスチャの解像度は、出力サイズドロップダウンメニューを使用して変更できます。 Substanceは、最大8Kを生成するように設定できます。 8K出力には[Substance GPUエンジン](../../../3d-applications/modo/modo-switch-engine/modo-switch-engine.md)が必要です。
