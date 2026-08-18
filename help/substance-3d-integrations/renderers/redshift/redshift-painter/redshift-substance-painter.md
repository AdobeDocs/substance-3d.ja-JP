---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/redshift/redshift-substance-painter.html"
breadcrumb-title: ''
description: 出力テンプレートと適切なマテリアル設定を使用して、Redshiftレンダラー用のSubstance Painterテクスチャを書き出します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Redshift > Redshift - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Redshift -Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%

---


# Redshift -Substance Painter

Substance Painter 2020.1(6.1.0)では、金属/粗さ(rsMaterial)に対してRedshift [出力テンプレート](https://docs.substance3d.com/display/SPDOC/Export)がサポートされています。 Redshiftテンプレートを使用して書き出すだけで、Redshiftマテリアルと互換性のあるテクスチャを作成できます。

![](../../../assets/rs-export.png)

## Redshiftマテリアルの設定

| Substance Painter書き出し | Redshiftマテリアル |
| --- | --- |
| Color | 拡散反射光/カラー |
| 粗さ | 反射/粗さ(BRDF = GGX) |
| 金属度 | 反射/メタル（フレネルタイプ=メタル） |
| 法線 | Overall / Bump Map / rsBumpMap (Input Map Type = Tangent Space Normal - Tangent Scale = 1.0) |
| DisplaceHeightField | ディスプレイスメントシェーダ/ rsDisplacement TexMap （マップエンコーディング= Heightフィールド） |
| EmissionColor | 全体/エミッション（エミッションウェイト= 1.0） |

>[!NOTE]
>
> データを表すマップは正しく解釈する必要があります。 詳細については、[カラーマネジメント](../../../renderers/color-management/color-management.md)ページを参照してください。

## Maya/Redshiftの例

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maya-example?$pjpeg$&jpegSize=300&wid=1583){width="800px"}
