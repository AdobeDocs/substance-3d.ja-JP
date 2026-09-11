---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/modo-switch-engine.html"
breadcrumb-title: ''
description: MODOでCPUモードとGPU Substanceのエンジンを切り替えると、ハードウェアに応じて最適なパフォーマンスが得られます。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Modo Switch Engine
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modoスイッチエンジン
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Modoスイッチエンジン

## スイッチングSubstance engine

Substance engineには、CPUとGPUの2つのバージョンがあります。 GPU エンジンを使用して2Kを超えるテクスチャを作成している。 CPUエンジンは、最大2Kのテクスチャしか生成できません。 高解像度のテクスチャが必要な場合は、GPU エンジンに切り替える必要があります。

Substanceキットメニューの「 Substance設定」オプションに移動し、「 Substance engineの切り替え」を選択します。 GPU エンジンを有効にするには、MODOを再起動する必要があります。 この設定はグローバル環境設定として機能します。 GPU エンジンは、手動で切り替えるまで、MODOを実行するたびに有効になります。

>[!NOTE]
>
> **Substance GPU エンジンを使用するには、1 GB以上の専用ビデオRAMを搭載したGPUが必要です。 統合GPUはサポートされていません。**\
> Nvidia: GeForce 650M 1 GB以上\
> AMD: 6870M以上

![](../../../assets/switch.png)
