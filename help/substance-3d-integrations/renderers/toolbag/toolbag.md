---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/toolbag.html"
breadcrumb-title: ''
description: リアルタイムのマテリアルプレビューとレンダリングには、ツールバッグ2のSubstanceの粗さとメタリック出力を使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Toolbag
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Toolbag
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 5%

---


# Toolbag

このページでは、Toolbag 2の粗さ/メタリック出力の使用方法を説明します。

Toolbagは、「Specular/光沢」と「メタリック/ラフネス」の両方のワークフローをサポートしています。

Substance 3D Painterでは、デフォルトでメタリックPBRシェーダが使用されますが、Specular/光沢シェーダでも使用できます。 このワークフローでは、Toolbag 2のメタリック出力の使用方法を説明します。 Toolbagはメタリックワークフローをサポートしています。

[サンプルシーンをダウンロード](https://www.dropbox.com/s/qyed3un2zhtuibj/toolbag.zip?dl=0)

## Painterからの書き出し

1. デフォルトのメタリックPBRシェーダを使用する場合は、デフォルトのドキュメントチャンネル+ Normal + AO書き出しプリセットを使用して書き出すことができます。 ***\*ドキュメントチャネルは、プロジェクト構成に基づいて標準マップをエクスポートします。 ツールバッグにはOGL法線マップが必要です。 プロジェクト構成で標準の形式を切り替えることができます。***
1. または、光沢を使用するカスタム書き出し設定を作成することもできます

   ![](../../assets/settings-export.png){width="600px"}
1. 書き出す前に、標準フォーマットをOpenGLに変更できます。  **編集/プロジェクト構成**

   ![](../../assets/settings-normal-format.png)

## マテリアルの設定

1. 反射率をメタネスに設定
1. リフレクションをGGXに設定
1. 次の表に示すように、適切なチャンネルにテクスチャを追加します。

   | Substance 3D Painterテクスチャ | カラースペース | ツールバッグマテリアル |
   | --- | --- | --- |
   | ベースカラー | sRGB | アルベド |
   | 粗さ | sRGBオフ | マイクロサーフェス – 光沢 – クリックして反転 |
   | メタリック | sRGBオフ | 反射率 – メタネスマップ |
   | 法線 | sRGBオフ | 法線 |
   | アンビエントオクルージョン | sRGBオフ | オクルージョン |

![](../../assets/settings-toolbag.jpg){width="600px"}
