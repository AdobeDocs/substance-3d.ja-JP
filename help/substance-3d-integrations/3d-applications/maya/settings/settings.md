---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/maya/settings.html"
breadcrumb-title: ''
description: MayaのSubstanceプラグイン設定をSubstanceシェルフまたはメニューを使用して設定し、動作をカスタマイズします。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 設定
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---


# 設定

Substance設定メニューには、SubstanceシェルフまたはSubstanceメニューからアクセスできます。 このメニューの設定は、編集可能な設定ファイル「substance.cfg」に保存されます。

>[!NOTE]
>
> **構成ファイルの場所**
> 
> **Windows**:\
> C:\Users\\Documents\maya\\substance\\
> **MacOS**:\
> /Users//Library/Preferences/Autodesk/maya//substance/\
> **Linux**:\
> /home//maya//substance/

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## デフォルトの解像度

sbsarファイルが読み込まれるときのSubstanceノードのデフォルト解像度を設定します。

## レンダリングワークフロー

Substanceノードで使用する既定のレンダリングワークフローを設定します。

## Substance Engine

Substanceに固有の環境設定およびすべてのSubstance engineノードに対するグローバル設定。 Substanceエンジンは、Substanceテクスチャの計算に使用されます。

### エンジンタイプ

このSubstance engineは、CPUおよびGPUエンジンとして利用できます。 エンジンを切り替えるには、Mayaを再起動する必要があります。 GPUエンジンでは、CPUエンジンよりも高い解像度が使用できます。

>[!WARNING]
>
> CPUエンジンとGPUエンジンには演算の違いがある場合があるため、一貫した結果を得るには、Substance Designerで使用するエンジンと同じ種類のエンジンを使用することをお勧めします。

CPUコアとエンジンメモリは、Substanceエンジンが使用できるリソースの量に関する設定です。

### レンダリングのブロック

Substanceエンジンの計算がMaya UIプロセスをブロックするかどうかを設定します。 有効にすると、Substanceエンジンが優先され、Maya UIプロセスがブロックされます。 無効にすると、Maya UIプロセスはエンジン計算によってブロックされません。

## 出力をディスクにキャッシュ

プロジェクト内に新しく作成されたすべてのSubstanceノードの既定のキャッシュの場所、ファイルの種類、キャッシュフォルダを設定します。

## 拡張機能のレンダリング

Arnoldシェーダで直接Substance出力を使用するには、レンダリング拡張機能を有効にします。

## 物理サイズ

sbsarファイルの読み込み時にデフォルトで物理サイズを使用し、sbsarの再読み込み時に再計算する必要がある場合は、このオプションを有効にします。

</td>
<td style="border: 0;" valign="top">

![](../../../assets/settings-35.png)

</td>
</tr>
</table>
