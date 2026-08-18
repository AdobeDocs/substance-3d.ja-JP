---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/getting-started/compatible-3d-software.html"
breadcrumb-title: ''
description: Substance Bakersと互換性のある3Dソフトウェアを見つけ、最適なベイク処理の結果を得るためにメッシュを準備する方法を学びましょう。
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Compatible 3D software
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 互換性のある3Dソフトウェア
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 2%

---


# 互換性のある3Dソフトウェア

ほとんどの3Dソフトウェアは、アプリケーションでサポートされているファイル形式のポリゴンとしてメッシュジオメトリを書き出す限り、Substance Bakersと互換性があります。

ただし、これらのメッシュをエクスポートする場合、すべてのソフトウェアが機能と品質の点で同等であるわけではありません。 そのため、メッシュを適切にクリーニングし、ベーカーとの互換性を確保することが重要です。 メッシュの準備の詳細については、さまざまな[ガイド](../../guides/performances-and-opt/performances-and-optimizations.md)を参照してください。

## ソフトウェアの互換性

以下に、一般的に知られている3Dソフトウェアとそのベイカーとの互換性のリストを示します。

| *名前* | *ステータス* |
| --- | --- |
| **ブレンダー** | 互換性あり：書き出す前にモディファイヤを平坦化する必要があります。 |
| **マヤ** | 互換性あり：書き出す前に変形固定とヒストリーの削除が必要です。 |
| **3DS Max** | 互換性あり：書き出す前にxFormのリセットが必要です。 |
| **MODO** | 互換性： [ゲーム]タブエクスポータを[非実在静的メッシュ]に設定して使用することをお勧めします。 |
| **Cinema 4D** | 互換性あり：書き出す前にモディファイヤを平坦化する必要があります。 |
| **zBrush** | 互換性がありません：ローポリメッシュは、最初に別の3Dアプリケーションで処理およびクリーニングする必要があります。 互換性：ベーキング用の高ポリゴンメッシュ。 |

## ファイル形式

ジオメトリをベイク処理する場合、使用するファイル形式も考慮に入れることが重要です。 ファイル形式は、メッシュに保存される情報の量を定義します。

情報が多すぎると有害になったり、エラーが発生したりする場合があります。 エラーが発生した場合は、通常、さまざまなファイル形式を試してみることをお勧めします。これは、問題をトラブルシューティングし、原因がパン屋自体にあるのか、3Dソフトウェアから来ているのかを判断する簡単な方法になります。

Bellowは、ベイカーがサポートする最も一般的な2つのファイル形式を簡単に説明します。

| ファイル形式 | 情報 |
| --- | --- |
| **FBX** | Autodesk FBX(Filmbox)は、Autodeskソフトウェアで使用される主要なファイル形式で、テキストまたはバイナリとして書き込むことができます。  次をサポートします。<ul data-preserve-html="true"><li data-preserve-html="true">UV（複数セット）</li><li data-preserve-html="true">頂点、接線、従法線</li><li data-preserve-html="true">頂点カラー</li><li data-preserve-html="true">三角形の面、四角形の面、N角形の面</li><li data-preserve-html="true">カメラ</li><li data-preserve-html="true">ライト</li><li data-preserve-html="true">メッシュの分割</li><li data-preserve-html="true">スムージンググループ</li><li data-preserve-html="true">マテリアル情報（色など）</li><li data-preserve-html="true">モノクロ 2 階調</li></ul> |
| **オブジェクト** | Wavefront OBJは非常にシンプルなテキストベースのファイル形式で、<ul data-preserve-html="true"><li data-preserve-html="true">UV（1セットのみ）</li><li data-preserve-html="true">頂点法線</li><li data-preserve-html="true">頂点カラー（Pixlogic zBrushから書き出した場合のみ）</li><li data-preserve-html="true">三角形の面、四角形の面、N角形の面</li><li data-preserve-html="true">マテリアルの色（<strong>mtl</strong>ファイルが存在する場合）</li></ul> |
