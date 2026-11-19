---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/using-workflows-in-3ds-max.html"
breadcrumb-title: ""
description: 3ds Maxのレンダリングワークフローを使用して、Substance マテリアルから各種レンダラー用のシェーダーネットワークを自動作成します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Using Workflows in 3ds Max
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Maxでのワークフローの使用
user-guide-description: ""
user-guide-title: ""
source-git-commit: 335f3107fb325bb769325bff8c150b3e8b7ff054
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%
---

# 3ds Maxでのワークフローの使用

3ds MaxプラグインのSubstanceには、レンダラーをサポートするシェーダーネットワークを自動作成するためのワークフローが含まれています。 レンダリングワークフローは、Substanceメニューにあります。

![](../../../assets/maya-max-v3-1/3dsmax-all-presets.png)

ワークフローを使用するには、ワークフローエディターでSubstanceノードを選択し、マテリアルメニューからSubstanceを選択します。

![](../../../assets/max-workflow.gif)

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
