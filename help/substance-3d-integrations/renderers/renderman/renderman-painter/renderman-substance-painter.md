---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/renderers/renderman/renderman-substance-painter.html"
breadcrumb-title: ''
description: pxrSurfaceマテリアルと適切な出力変換を使用して、Renderman用のSubstance Painterテクスチャをエクスポートします。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Renderman > Renderman - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Renderman -Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 1%

---


# Renderman -Substance Painter

Substance Painter 2020.1(6.1.0)は、[**pxrSurface**](https://rmanwiki.pixar.com/display/REN/PxrSurface)とpxrDisney [出力テンプレート](https://docs.substance3d.com/display/SPDOC/Export)をサポートしています。

![](../../../assets/renderman.png)

出力には&#x200B;**pxrSurface**&#x200B;を使用することをお勧めします。

![](../../../assets/pxrsurface.png)

## Rendermanシェーダ(Maya - RM 23.1)

| Substance Painter書き出し | PxrSurface |
| --- | --- |
| DiffuseColor | 拡散反射光/カラー |
| SpecularRoughness | 一次Specular/粗さ |
| SpecularFaceColor | 一次Specular/顔の色 |
| 法線 | グローバル/バンプ/ PxrNormalMap →方向(Open GL) |
| ディスプレイスメント | （赤チャンネル） PxrDispTransform (Result F) → （Dispスカラー） PxrDisplace (Out Color) → （ディスプレイスメントシェーダ） PxrSurfaceSG |
| GlowColor | グロー/カラー（ゲイン= 1.0） |
| 存在 | グローバル/プレゼンス |

>[!NOTE]
>
> データを表すマップは正しく解釈する必要があります。 詳細については、[カラーマネジメント](../../../renderers/color-management/color-management.md)ページを参照してください。
