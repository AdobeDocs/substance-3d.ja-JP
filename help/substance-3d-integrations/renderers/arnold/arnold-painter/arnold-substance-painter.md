---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/arnold/arnold-substance-painter.html"
breadcrumb-title: ''
description: Arnoldレンダラーの出力テンプレートと、物理ベースのレンダリング用のaiStandardマテリアルを使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Arnold > Arnold - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: アーノルドSubstance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 3%

---


# アーノルドSubstance Painter

Substance Painter 2020.1 (6.1.0)には、[aiStandardマテリアル](https://docs.arnoldrenderer.com/display/A5AFMUG/Standard+Surface)を使用したArnold用の[出力テンプレート](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/export/output-templates/export-presets)が付属しています。

![](../../../assets/arnold-export.png){width="800px"}

## Arnold標準シェーダ（Arnold 5以降）

| Substance Painter書き出し | Arnold AiStandardSurface |
| --- | --- |
| ベースカラー | ベース/カラー |
| 粗さ | Specular/粗さ |
| 金属度 | ベース/メタル |
| 法線 | (**Maya**)ジオメトリ/バンプマッピング/ bump2d （接線空間法線として使用） (**3ds** **Max**)ビットマップ→法線 |
| 高さ | (**Maya**) ディスプレイスメントシェーダ/ ディスプレイスメント (**3ds** **Max**)オブジェクトモディファイヤ→ Arnoldプロパティ→ ディスプレイスメント →マップの使用 |
| 放射 | エミッション/カラー（エミッションウェイト= 1.0） |
| 異方性レベル（デフォルトのArnold 出力テンプレートには含まれていません） | (**Maya**)コート/ 異方性 (**3ds** **Max**)コート/ 異方性 |
| 異方性レベル（デフォルトのArnold 出力テンプレートには含まれていません） | (**Maya**)コート/回転(**3ds** **Max**)コート/回転 |

>[!NOTE]
>
> データを表すマップは正しく解釈する必要があります。 詳細については、[カラーマネジメント](../../../renderers/color-management/color-management.md)ページを参照してください。
