---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/getting-started/compatible-3d-software.html"
breadcrumb-title: ''
description: Substance Bakersと互換性のある3Dソフトウェアを確認し、最適なベイク処理結果を得るためのメッシュを準備する方法を学びましょう。
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

ただし、これらのメッシュを書き出すときに、すべてのソフトウェアが機能と品質の点で同等になるわけではありません。 このため、メッシュを適切にクリーニングし、ベイカーと互換性があることを確認することが重要です。 メッシュを準備する方法について詳しくは、さまざまな[ガイド](../../guides/performances-and-opt/performances-and-optimizations.md)を参照してください。

## ソフトウェアの互換性

一般的に知られている3Dソフトウェアとそのベイカーとの互換性のリストを次に示します。

| *名前* | *ステータス* |
| --- | --- |
| **ブレンダー** | 互換性あり：書き出す前にモディファイヤを平坦化する必要があります。 |
| **マヤ** | 互換性あり：書き出す前に、フリーズ変形と削除の履歴が必要です。 |
| **3DS Max** | 互換性あり：書き出す前にxFormのリセットが必要です。 |
| **MODO** | 互換性： [ゲーム]タブのエクスポーターを[非現実的な静的メッシュ]に設定することをお勧めします。 |
| **Cinema 4D** | 互換性あり：書き出す前にモディファイヤを平坦化する必要があります。 |
| **zBrush** | 互換性がありません：ローポリメッシュは、最初に別の3Dアプリケーションで処理およびクリーニングする必要があります。 互換性：ベイク用ハイポリメッシュ。 |

## ファイル形式

ジオメトリをベイクする場合は、使用するファイルフォーマットも考慮することが重要です。 メッシュに保存されるデータの量は、ファイルフォーマットによって決まります。

情報が多すぎると有害になったり、エラーが発生したりする場合があります。 エラーが発生した場合は、トラブルシューティングを行い、原因がソフトウェア自体にあるのか3D ベイカーにあるのかを判断する簡単な方法であるため、通常は様々なファイルフォーマットを試すことをお勧めします。

Bellowは、ベイカーでサポートされている最も一般的な2つのファイル形式の概要を簡単に説明します。

| ファイル形式 | 情報 |
| --- | --- |
| **FBX** | Autodesk FBX (Filmbox)は、Autodesk Softwareで使用される主要なファイルフォーマットで、テキストまたはバイナリとして書き込むことができます。  次をサポートします。<ul data-preserve-html="true"><li data-preserve-html="true">UV（複数セット）</li><li data-preserve-html="true">頂点、正接、および従法線</li><li data-preserve-html="true">頂点カラー</li><li data-preserve-html="true">トライアングル面、クアッド面およびN – ゴン面</li><li data-preserve-html="true">カメラ</li><li data-preserve-html="true">ライト</li><li data-preserve-html="true">メッシュ区画</li><li data-preserve-html="true">スムージンググループ</li><li data-preserve-html="true">マテリアル情報（色など）</li><li data-preserve-html="true">モノクロ 2 階調</li></ul> |
| **オブジェクト** | Wavefront OBJは次をサポートする非常にシンプルなテキストベースのファイルフォーマットです。<ul data-preserve-html="true"><li data-preserve-html="true">UV（1セットのみ）</li><li data-preserve-html="true">頂点法線</li><li data-preserve-html="true">頂点カラー（Pixlogic zBrushから書き出した場合のみ）</li><li data-preserve-html="true">トライアングル面、クアッド面、N – ゴン面</li><li data-preserve-html="true">マテリアルの色（<strong>mtl</strong>ファイルが存在する場合）</li></ul> |
