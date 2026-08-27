---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/renderers/redshift/redshift-substance-painter.html"
breadcrumb-title: ''
description: 出力テンプレートと適切なSubstance Painterテクスチャを使用して、Redshiftレンダラーのマテリアル設定を書き出します。
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

Substance Painter 2020.1(6.1.0)では、メタリック/ラフネス(rsMaterial)に対してRedshift [出力テンプレート](https://docs.substance3d.com/display/SPDOC/Export)がサポートされています。 Redshift マテリアルを使用して書き出すだけで、Redshiftテンプレートと互換性のあるテクスチャを作成できます。

![](../../../assets/rs-export.png)

## Redshift マテリアルの設定

| Substance Painter書き出し | Redshift マテリアル |
| --- | --- |
| Color | 拡散反射光/カラー |
| 粗さ | 反射/ラフネス(BRDF = GGX) |
| 金属度 | 反射/メタル（フレネルタイプ=メタル） |
| 法線 | 全体/バンプマップ/ rsBumpMap （入力マップの種類= 接線空間法線 – Heightスケール= 1.0） |
| DisplaceHeightField | シェーダー / rsDisplacement TexMap（マップエンコーディング= Heightフィールド） |
| EmissionColor | 全体/エミッション（エミッションウェイト= 1.0） |

>[!NOTE]
>
> データを表すマップは正しく解釈する必要があります。 詳細については、[カラーマネジメント](../../../renderers/color-management/color-management.md)ページを参照してください。

## Maya/Redshiftの例

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maya-example?$pjpeg$&jpegSize=300&wid=1583){width="800px"}
