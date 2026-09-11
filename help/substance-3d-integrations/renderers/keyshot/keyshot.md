---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/keyshot.html"
breadcrumb-title: ''
description: 書き出されたテクスチャマップを使用して製品をビジュアル化するには、キーショットレンダラーのSubstanceマテリアルを使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Keyshot
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Keyshot
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 8%

---


# Keyshot

*Keyshot 6.1.72*[&#x200B;サンプルシーンをダウンロード](https://www.dropbox.com/s/rvjsbbcx7c74aah/keyshot.zip?dl=0)

## Substance Painter書き出し

1. キーショットの場合は、Diffuse、リフレクション、メタリック、ラフネス、法線（ダイレクトX）を使用して書き出しプリセットを設定する必要があります。

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/key-01?$png$&jpegSize=300&wid=1794)

## マテリアルの詳細設定

2つの詳細マテリアルを使用します。 1つはメタリック用で、もう1つは誘電体用です。

1. マテリアルを「詳細」に設定し、マテリアルをグラフします。

   **メタリック:**\
   a. 屈折インデックスを10に設定します\
   b. 以下の表に示すようにマップを設定します

   | テクスチャ | 詳細マテリアルチャンネル |
   | --- | --- |
   | ディフューズ | ディフューズ |
   | メタリック | 不透明度 |
   | 法線 | バンプ\*法線が有効 |
   | 粗さ | 粗さ |
   | 反射 | スペキュラ |

1. 新しい高度なマテリアルを作成する

   **誘電体：**\
   a. 屈折インデックスを1.5に設定します\
   b. 以下の表に示すようにマップを設定します

   | テクスチャ | 詳細マテリアルチャンネル |
   | --- | --- |
   | ディフューズ | ディフューズ |
   | 法線 | バンプ\*法線が有効 |
   | 粗さ | 粗さ |
   | 反射 | スペキュラ |

1. メタリックアドバンスドマテリアルの出力を取り、誘電体アドバンスドマテリアルの+に加えます。 これにより、マテリアルに「ラベル」フィールドが作成されます。

   ![](../../assets/key-02.png)
