---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/getting-started/compatible-3d-software.html"
breadcrumb-title: ''
description: Substance Bakersと互換性のある3D ソフトウェアを見つけ、最適なベーキング結果を得るためにメッシュを準備する方法を学びます。
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Compatible 3D software
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 互換性のある3D ソフトウェア
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 2%

---


# 互換性のある3D ソフトウェア

ほとんどの3D ソフトウェアは、アプリケーションでサポートされているファイル形式でメッシュジオメトリをポリゴンとして書き出す限り、Substance Bakersと互換性があります。

ただし、これらのメッシュを書き出す際に、すべてのソフトウェアが機能と品質の点で同等であるわけではありません。 そのため、メッシュを適切にクリーニングし、ベーカーと互換性があることを確認することが重要です。 メッシュの準備方法について詳しくは、様々な[&#x200B; ガイド &#x200B;](../../guides/performances-and-opt/performances-and-optimizations.md)を参照してください。

## ソフトウェアの互換性

以下は、一般的に知られている3D ソフトウェアのリストとベイカーとの互換性です。

| *名前* | *ステータス* |
| --- | --- |
| **ブレンダー** | 互換性：書き出す前に修飾子を統合する必要があります。 |
| **Maya** | 互換性：書き出し前にフリーズ変換と履歴の削除が必要です。 |
| **3DS Max** | 互換性：書き出し前にxFormをリセットする必要があります。 |
| **MODO** | 互換性：ゲームタブエクスポーターを「Unreal Static Mesh」に設定することをお勧めします。 |
| **Cinema 4D** | 互換性：書き出す前に修飾子を統合する必要があります。 |
| **zBrush** | 互換性がない：低ポリメッシュは、最初に別の3D アプリケーションで処理およびクリーニングする必要があります。 互換性：ベーキング用のハイポリメッシュ。 |

## ファイル形式

ジオメトリをベイク処理する場合は、使用するファイル形式も考慮することが重要です。 ファイル形式は、メッシュに保存される情報の量を定義します。

情報が多すぎると、有害な結果を招き、エラーにつながる場合があります。 エラーが発生した場合は、問題をトラブルシューティングし、原因がパン屋そのものにあるか、3D ソフトウェアに由来しているかを簡単に判断できるため、通常、さまざまなファイル形式を試すことをお勧めします。

以下は、パン屋でサポートされている2つの最も一般的なファイル形式の概要です。

| ファイル形式 | 情報 |
| --- | --- |
| **FBX** | Autodesk FBX（Filmbox）は、Autodesk Softwareが使用する主要なファイル形式です。テキストまたはバイナリとして書き込むことができます。  次の機能をサポートしています。<ul data-preserve-html="true"><li data-preserve-html="true">UV （複数のセット）</li><li data-preserve-html="true">頂点、正接および従法線</li><li data-preserve-html="true">頂点カラー</li><li data-preserve-html="true">三角形の面、四角形の面およびN字面</li><li data-preserve-html="true">カメラ</li><li data-preserve-html="true">ライト</li><li data-preserve-html="true">メッシュサブディビジョン</li><li data-preserve-html="true">スムージンググループ</li><li data-preserve-html="true">マテリアル情報（カラーなど）</li><li data-preserve-html="true">モノクロ 2 階調</li></ul> |
| **OBJ** | Wavefront OBJは、以下をサポートする非常にシンプルなテキストベースのファイルフォーマットです。<ul data-preserve-html="true"><li data-preserve-html="true">UV （1 セットのみ）</li><li data-preserve-html="true">頂点法線</li><li data-preserve-html="true">頂点カラー（Pixologic zBrushから書き出した場合のみ）</li><li data-preserve-html="true">三角形の面、四角形の面、およびN字面</li><li data-preserve-html="true">マテリアルカラー（<strong>mtl</strong> ファイルが存在する場合）</li></ul> |
