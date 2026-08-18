---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/vray/vray-next-substance-painter.html"
breadcrumb-title: ''
description: 出力テンプレートと適切なワークフロー設定を使用して、V-Ray NextレンダラーのSubstance Painterテクスチャを書き出します。
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

Substance Painter 2020.1 (6.1.0)には、メタリックとSpecularの両方のワークフロー用の[VrayMtl](https://docs.chaosgroup.com/display/VRAY4MAYA/VRayMtl)シェーダーが付属しています。 **VrayMtlテンプレート**&#x200B;を使用して[Substance Painterプロジェクトを設定](https://docs.substance3d.com/display/SPDOC/Project+Creation)できます。このテンプレートにより、ビューポートシェーダが設定されます。

![](../../../assets/template-16.jpg)

Shader Settingsでは、VrayMtlを操作するためにVrayシェーダを設定できます。

>[!NOTE]
>
> [UVタイルUDIMレガシー](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html)を使用するようにプロジェクトが設定されている場合 Vray Next UDIM 出力テンプレートを使用します。

![](../../../assets/vray-mtl-shader.png){width="800px"}

Vray Nextでレンダリングするためにテクスチャを書き出すには、Vray Mtl 出力テンプレートを選択します。

![](../../../assets/template-project.jpg){width="800px"}

## Vrayマテリアル（次のVray – メタリック/粗さ）

| Substance Painter書き出し | VRayMtl |
| --- | --- |
| ベースカラー | (**Maya**)拡散反射光カラー（量= 1.0） (**3ds Max**)拡散反射光 |
| 粗さ | (**Maya**)リフレクション/粗さ(BRDF = GGX) + （粗さを使用有効）(**3ds Max**)粗さ→ BRDF/ GGXを使用して粗さを使用を有効にする |
| メタリック | (**Maya**)リフレクション/メタネス(**3ds Max**)メタネス |
| 法線 | (**Maya**)バンプマッピングと法線マッピング/マップ（マップの種類=接線空間の法線）(**3ds** **Max**)ビットマップ→法線 |
| 高さ | (**Maya**) ディスプレイスメントシェーダ/ ディスプレイスメント (**3ds** **Max**)オブジェクトモディファイヤ→ VrayDisplacementMod → Texマップ |
| 放射 | 自己照明 |
| 透過 | (**Maya**)サブサーフェススキャッタリング/半透明カラー(**3ds Max**)半透明→裏面カラー |
| AnisotropyAngle | (**Maya**)異方性/異方性回転(**3ds** **Max**) BRDF/回転 |
| AnisotropyLevel | (**Maya**)異方性/異方性(**3ds Max**) BRDF/角度 |

## Vrayマテリアル(Vray Next - Specular/光沢

| Substance Painter書き出し | VRayMtl |
| --- | --- |
| ディフューズ | (**Maya**)拡散反射光カラー（量= 1.0） (**3ds Max**)拡散反射光 |
| スペキュラ | (**Maya**)反射/反射カラー（量= 1.0） (**3ds Max**)反射 |
| グロシネス | (**Maya**)リフレクション/粗さ(BRDF = GGX) + （粗さを使用有効）(**3ds Max**)光沢→ BRDF / GGXを使用して光沢を使用を有効 |
| 法線 | (**Maya**)バンプマッピングと法線マッピング/マップ（マップの種類=接線空間の法線）(**3ds** **Max**)ビットマップ→法線 |
| 高さ | (**Maya**) ディスプレイスメントシェーダ/ ディスプレイスメント (**3ds** **Max**)オブジェクトモディファイヤ→ VrayDisplacementMod → Texマップ |
| 放射 | 自己照明 |
| 透過 | (**Maya**)サブサーフェススキャッタリング/半透明カラー(**3ds Max**)半透明→裏面カラー |
| AnisotropyAngle | (**Maya**)異方性/異方性回転(**3ds** **Max**) BRDF/回転 |
| AnisotropyLevel | (**Maya**)異方性/異方性(**3ds Max**) BRDF/角度 |

>[!NOTE]
>
> データを表すマップは正しく解釈する必要があります。 詳細については、[カラーマネジメント](../../../renderers/color-management/color-management.md)ページを参照してください。

この例は、Vray Metallic/Roughnessシェーダを使用したSubstance Painterビューポートと、Mayaを使用したVrayレンダーを示しています。

![](../../../assets/vray-maya.jpg){width="800px"}
