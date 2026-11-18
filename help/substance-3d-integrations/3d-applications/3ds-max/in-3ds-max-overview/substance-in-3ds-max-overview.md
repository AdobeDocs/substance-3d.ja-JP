---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/substance-in-3ds-max-overview.html"
breadcrumb-title: ""
description: 3ds MaxのSubstanceプラグインと、Substance マテリアルをプロジェクトに読み込んで使用する方法について学習します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Substance in 3ds Max Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds MaxのSubstanceの概要
user-guide-description: ""
user-guide-title: ""
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%
---

# 3ds MaxのSubstanceの概要

## プラグインの概要

## Substanceのオープン

1. スレートエディタを開き、「Substance」を検索し、「Substance2」ノードをビューにドラッグします。
1. Substanceノードをダブルクリックしてプロパティをアクティブにし、[Substanceパッケージブラウザ]でSubstanceをロードします。

   >[!NOTE]
   >
   > .sbsar ファイルをスレートエディターにドラッグ&amp;ドロップして、ノードを自動作成し、スバーを読み込むこともできます。

1. Substanceに複数のグラフが含まれている場合は、マテリアルとして出力するグラフを「選択したグラフ 」ドロップダウンメニューで選択できます。

   ![](../../../assets/max1.png)

1. Substanceノードを選択した状態で、「Substance」メニューに移動し、サポートされているレンダラーを選択します。 マテリアルが作成され、オブジェクトに適用できるようになります。 テクスチャはレンダリングマテリアルに接続されます。

>[!NOTE]
>
> **«Substance2 »**&#x200B;ノードを選択したら、最初に&#x200B;**[読み込み] Substance...**&#x200B;をクリックしてsbsar ファイルを選択し、上部メニューからサポートされているレンダラーを選択する必要があります（「ArnoldにSubstance」など）。
>
>サポートされるレンダラーには、Arnold、V-Ray、Corona、Octaneなどがあります。 [OpenPBR マテリアルの使用方法については、3DS Maxのワークフローを参照してください。](../using-workflows-3ds-max/using-workflows-in-3ds-max.md)

![](../../../assets/max3.png)

## 解像度の変更

1. Substanceの出力の設定で、計算されたSubstanceテクスチャの解像度を設定します。
1. 解像度を最大8Kにするには、[Substance設定](../../../3d-applications/3ds-max/settings-1/substance-settings.md)で設定されているGPU エンジンを使用していることを確認してください。

   ![](../../../assets/max6.png)

## パラメータの変更

1. Substanceノードをダブルクリックして、パラメータウィンドウにSubstanceパラメータを読み込みます。
1. パラメーターを変更すると、テクスチャが自動的に更新されます。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/max4?$png$&jpegSize=200&wid=1276){width="500px"}

## 出力プレビューの設定

Substanceノードのサムネールにチャンネルを指定できます。

1. 出力プレビュードロップダウンで、ノードサムネールに使用するチャンネルを選択します。

   ![](../../../assets/max7.png)

## Substance

[座標]プロパティを使用すると、テクスチャを並べて表示したり、マップチャンネルを設定することができます。

![](../../../assets/max10.png)

## OpenPBRワークフロー

**Substanceメニュー**&#x200B;の&#x200B;**ワークフローの一覧**&#x200B;では、次の2つのOpenPBRワークフローを使用できます： **OpenPBRへのSubstance**&#x200B;および&#x200B;**V-Ray OpenPBRへのSubstance**。 これらのワークフローは、Substance 3D DesignerまたはSamplerのOpenPBRマテリアルモデルを使用して作成されたSBSARファイルで使用するように設計されています（OpenPBRは、Designer V16.0以降およびSampler V6.0以降のデフォルトのモデルです）。

![](../../../assets/maya-max-v3-1/3ds-max-openpbr-node-preview.png)

### OpenPBRとは

OpenPBRは、Adobeとオートデスクが開発したオープンで物理的なマテリアルシェーディングモデルであり、Academy Software Foundation(ASWF)に寄稿されています。 レンダラ間で互換性のある統合されたマテリアル定義を提供します。 詳細については、[OpenPBRドキュメント](https://experienceleague.adobe.com/en/docs/substance-3d/general-knowledge/openpbr/openpbr-overview)を参照してください。

### OpenPBRワークフローを使用するタイミング

Substance 3D DesignerまたはSubstance 3D SamplerのOpenPBRワークフローを使用してSbsar ファイルを作成した場合は、OpenPBRマテリアルモデルを使用します。 SBSARがAdobe標準マテリアルモデル(ASM)を使用して作成された場合は、レンダラーと互換性のある従来のワークフロー（Arnold、V-RayまたはV-Ray 6）を使用します。

>[!NOTE]
>
> OpenPBRワークフローをASM マテリアルに適用する場合、または標準ワークフローをOpenPBR SBSARに適用する場合、プラグインは両方のマテリアルモデルに共通する出力のみを接続します。 結果が不完全になる場合があります。

### 使用可能なOpenPBRワークフロー

**OpenPBR**

ネイティブの3ds Max openPBRSurfaceノードを使用します。 ArnoldおよびV-Rayに対応しています。 これは、3ds MaxでOpenPBR マテリアルを使用しているほとんどのユーザに推奨されるワークフローです。

**OpenPBR - V線**

OpenPBRモードでV線マテリアル(VRayMtl)を使用します。 パイプラインがV線マテリアル設定を中心に構築されている場合にお勧めします。

### OpenPBRワークフローの適用方法

![](../../../assets/maya-max-v3-1/3dsmax-substance-to-openpbr.png)

1. 「Substanceのロード」ボタンを使用して、Sbsar ファイル(OpenPBR)を選択します。
1. 上部のメニューで、[OpenPBR]または[OpenPBR - V線]を選択します。
1. スレートマテリアルエディタでシェーダーネットワークを作成するには、[ネットワークを作成]をクリックします。
1. プラグインは、SBSAR出力をOpenPBRノードの対応する入力に自動的に接続します。
1. 通常どおり、マテリアルをメッシュに割り当てます。

![](../../../assets/maya-max-v3-1/3ds-max-openpbr-overview.png)
