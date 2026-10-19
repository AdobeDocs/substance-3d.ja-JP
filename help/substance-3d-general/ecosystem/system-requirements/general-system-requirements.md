---
helpx_url: 'https://helpx.adobe.com/substance-3d-general/ecosystem/general-system-requirements.html'
breadcrumb-title: ''
description: Substance 3Dアプリケーションの必要システム構成を確認して、ハードウェアが最小、推奨、または最適な仕様を満たしていることを確認してください。
helpx_creative_field: ''
helpx_description: General Knowledge > Ecosystem > General system requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 一般的な必要システム構成
user-guide-description: ''
user-guide-title: ''
source-git-commit: eef3d78f33034f2c24f4c4471d9ccac805184525
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 2%
---

# 一般的な必要システム構成

## ハードウェア要件

+++Windows

|  | 最小 | おすすめ | 最適 |
| --- | --- | --- | --- |
| **OS** | Windows 11 64ビット版23H2 | Windows 11 64ビット版24H1 | Windows 11 64ビット版24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **ストレージ** | 30 GBの空き容量のあるSSD | 50 GBの空き容量のあるSSD | 70 GBの空き容量のあるSSD |

+++

+++macOS

|  | 最小 | おすすめ | 最適 |
| --- | --- | --- | --- |
| **OS** | macOS 15セコイア | macOS 27ゴールデンゲート | macOS 27ゴールデンゲート |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **ストレージ** | 30 GBの空き容量のあるSSD | 50 GBの空き容量のあるSSD | 70 GBの空き容量のあるSSD |

>[!WARNING]
>
> [VFX Reference Platform](https://vfxplatform.com/)を念頭に置いて構築されたパイプラインでは、Substance 3DアプリケーションをmacOS 14 Sonomaにインストールできます。 ただし、Substanceアプリは最小必要システム構成を下回るOSバージョンではテストされていないため、安定性は保証されません。 新しいバージョンのOSにアップデートすることをお勧めします。

+++

+++Linux

|  | 最小 | おすすめ | 最適 |
| --- | --- | --- | --- |
| **OS** | **エンタープライズ版ETLA** RHEL 8.6以降またはRHEL 9.2以降&#x200B;**Steam** Ubuntu 22.04.1 LTS | **エンタープライズ版ETLA** RHEL 8.6以降またはRHEL 9.4以降&#x200B;**Steam** Ubuntu 22.04.1 LTS以降 | **エンタープライズ版ETLA** RHEL 8.6以降またはRHEL 9.4以降&#x200B;**Steam** Ubuntu 22.04.1 LTS以降 |

**Red Hat Enterprise Linux (RHEL) 9.x**:アプリケーションに必要なxcb-util-cursorパッケージが、2024年5月10日にEPEL 9リポジトリから削除されました。 この日以降、パッケージはRHEL 9.4のリリースと同時に、デフォルトのRHEL 9リポジトリでサポートされます。 9.4より前のバージョンのRHELを使用しているお客様は、2024年5月10日以降、EPEL 9リポジトリからxcb-util-cursorパッケージを取得できなくなります。

既定のRHEL 9リポジトリでのこのパッケージの可用性の詳細については、[Red Hat Enterprise Linux 9 – パッケージマニフェスト – AppStreamリポジトリ](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/9/html-single/package_manifest/index#AppStream-repository)を参照してください。

この変更の詳細については、[Red Hat Bugzilla – バグ2238273](https://bugzilla.redhat.com/show_bug.cgi?id=2238273) 、[Red Hat Bugzilla – バグ2212302](https://bugzilla.redhat.com/show_bug.cgi?id=2212302)を参照してください。

+++

+++VR

| ブランド | モデル |
| --- | --- |
| Meta | Rift、Rift S、クエスト、クエスト2（リンクあり）、クエストPro |

+++

詳しくは、各アプリケーションの要件を参照してください。

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/sa-appicon-noshadow-256.png" alt="Substance 3D Samplerアイコン" width="64px"/><br><a href="https://experienceleague.adobe.com/en/docs/substance-3d-sampler/using/getting-started/system-requirements">Substance 3D Sampler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/ds-appicon-noshadow-256.png" alt="Substance 3D Designerアイコン" width="64px"/><br><a href="https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/getting-started/system-requirements">Substance 3D</a> <a href="https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/getting-started/system-requirements">Designer</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/pt-appicon-noshadow-256.png" alt="Substance 3D Painterアイコン" width="64px"/><br><a href="https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/system-requirements">Substance 3D Painter</a></td>
  </tr>
</table>

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/md-appicon-noshadow-256.png" alt="Substance 3D Modelerアイコン" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-modeler/getting-started/system-requirements.html">Substance 3D Modeler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/sg-appicon-noshadow-256.png" alt="Substance 3D Stagerアイコン" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-stager/getting-started/system-requirements.html">Substance 3D Stager</a></td>
    <td style="border: 0;" valign="top"></td>
  </tr>
</table>

## 追加情報

### サポートされていない設定

* eGPUとユーザーがインストールしたGPUを使用するAppleコンピューター設定はサポートされていません。
* Windows仮想マシンはサポートされていません。
* Windows Serverオペレーティングシステムはサポートされていません。
