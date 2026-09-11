---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/vray/vray-next-substance-painter.html"
breadcrumb-title: ''
description: 出力テンプレートと適切なワークフローテクスチャを使用して、V-Ray NextレンダラーのSubstance Painter設定を書き出します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Vray > Vray Next - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 次を選択 – Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 3%

---


# 次を選択 – Substance Painter

Substance Painter 2020.1 (6.1.0)には、メタリックとSpecularの両方のワークフロー用の[VrayMtl](https://docs.chaosgroup.com/display/VRAY4MAYA/VRayMtl)シェーダーが付属しています。 **VrayMtlテンプレート**&#x200B;を使用して[Substance Painterプロジェクトを設定](https://docs.substance3d.com/display/SPDOC/Project+Creation)すると、ビューポートシェーダーを構成できます。

![](../../../assets/template-16.jpg)

[シェーダー設定]で、VrayMtlを使用するためのVray シェーダーを設定できます。

>[!NOTE]
>
> [UDIMレガシー](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html)を使用するようにプロジェクトが設定されている場合。 [次のUDIMを選択]出力テンプレートを使用します。

![](../../../assets/vray-mtl-shader.png){width="800px"}

Vray Nextでレンダリングするためにテクスチャを書き出すには、「Vrayマテリアル」出力テンプレートを選択します。

![](../../../assets/template-project.jpg){width="800px"}

## Vray マテリアル(Vray Next -メタリック/ラフネス)

| Substance Painter書き出し | VRayMtl |
| --- | --- |
| ベースカラー | (**Maya**) Diffuseカラー（量= 1.0） (**3ds Max**) Diffuse |
| 粗さ | (**Maya**)リフレクション/ ラフネス (BRDF = GGX) + （ラフネスを有効にする）(**3ds Max**) ラフネス → BRDF/ GGXを使用してラフネスを使用を有効にする |
| メタリック | (**Maya**)リフレクション/メタネス(**3ds Max**)メタネス |
| 法線 | (**Maya**)バンプマッピングと法線マッピング/マップ（マップの種類=接線空間の法線）(**3ds** **Max**)ビットマップ→法線 |
| 高さ | (**Maya**) ディスプレイスメント シェーダー / ディスプレイスメント (**3ds** **Max**)オブジェクトモディファイヤ→ VrayDisplacementMod → Texマップ |
| 放射 | 自己照明 |
| 透過 | (**Maya**)サブサーフェススキャッタリング/半透明カラー(**3ds Max**)半透明→裏面カラー |
| AnisotropyAngle | (**Maya**)異方性/異方性回転(**3ds** **Max**) BRDF/回転 |
| AnisotropyLevel | (**Maya**)異方性/異方性(**3ds Max**) BRDF/角度 |

## Vray マテリアル(Vray Next - Specular/光沢度

| Substance Painter書き出し | VRayMtl |
| --- | --- |
| ディフューズ | (**Maya**) Diffuseカラー（量= 1.0） (**3ds Max**) Diffuse |
| スペキュラ | (**Maya**)反射/反射カラー（量= 1.0） (**3ds Max**)反射 |
| グロシネス | (**Maya**)リフレクション/ ラフネス (BRDF = GGX) + （ラフネスを有効にする）(**3ds Max**) 光沢度 → BRDF / GGXを使用して光沢度を使用を有効にする |
| 法線 | (**Maya**)バンプマッピングと法線マッピング/マップ（マップの種類=接線空間の法線）(**3ds** **Max**)ビットマップ→法線 |
| 高さ | (**Maya**) ディスプレイスメント シェーダー / ディスプレイスメント (**3ds** **Max**)オブジェクトモディファイヤ→ VrayDisplacementMod → Texマップ |
| 放射 | 自己照明 |
| 透過 | (**Maya**)サブサーフェススキャッタリング/半透明カラー(**3ds Max**)半透明→裏面カラー |
| AnisotropyAngle | (**Maya**)異方性/異方性回転(**3ds** **Max**) BRDF/回転 |
| AnisotropyLevel | (**Maya**)異方性/異方性(**3ds Max**) BRDF/角度 |

>[!NOTE]
>
> データを表すマップは正しく解釈する必要があります。 詳細については、[カラーマネジメント](../../../renderers/color-management/color-management.md)ページを参照してください。

このサンプルは、Vrayメタリック/ラフネスシェーダーを使用したSubstance Painterビューポートと、Mayaを使用したVrayレンダーを示しています。

![](../../../assets/vray-maya.jpg){width="800px"}
