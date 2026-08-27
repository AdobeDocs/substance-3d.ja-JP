---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/modo/custom-materials.html"
breadcrumb-title: ''
description: 特殊なワークフロー用のSubstanceプラグインを使用して、MODOでUnreal、Unity、およびglTFカスタムマテリアルを使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Custom Materials
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: カスタムマテリアル
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 12%

---


# カスタムマテリアル

Substanceプラグインは、Unreal、Unity、およびglTFのカスタムマテリアルをサポートしています。 sbsarファイルを読み込む前に、使用するシェーディングモードを選択できます。

## 目次

## Unityマテリアル

Unityマテリアルを使用する場合は、自動的にマテリアルレイヤー効果が設定されます。 Substanceプラグインは、Unity MaterialをSubstance項目Materialの真上に配置します。

| Substance出力 | カラースペース | マテリアルレイヤー効果 |
| --- | --- | --- |
| ベースカラー | sRGB | Unity アルベド |
| グロシネス | 線形 | Unity Smoothness |
| メタリック | 線形 | ユニティメタリック |
| 法線 | 線形 | Unity標準 |
| 放射 | sRGB | 静止画のUnity発光&#x200B;**\*sRGBに設定** |
| 高さ | 線形 | ユニティバンプ |
| アンビエントオクルージョン | 線形 | Unity環境オクルージョン |

![](../../../assets/unity-1.png){width="600px"}

## 非現実的な素材

アンリアルマテリアルを使用する場合、マテリアルレイヤエフェクトは自動的に設定されます。 Substanceプラグインは、UnrealマテリアルをSubstance項目のマテリアルの上に直接配置します。

| Substance出力 | カラースペース | マテリアルレイヤー効果 |
| --- | --- | --- |
| ベースカラー | sRGB | 非現実Base color |
| 粗さ | 線形 | 非現実ラフネス |
| メタリック | 線形 | 非現実メタリック |
| 法線 | 線形 | 非現実的な標準 |
| 高さ | 線形 | 非現実バンプ |
| 放射 | sRGB | 非現実Emissive **\*静止画のsRGBに設定** |
| アンビエントオクルージョン | 線形 | 非現実Ambient occlusion |
| 不透明度 | 線形 | 非現実の不透明度&#x200B;**\*テクスチャレイヤーの反転を解除する必要があります** |

![](https://helpx-prod.scene7.com/is/image/HelpxProd/unreal?$png$&jpegSize=200&wid=1343){width="600px"}

法線を反転する必要がある場合があります。 これは、Substanceに法線の方向のコントロールがある場合は、[ツイーク]メニューから実行できます。 そうでない場合は、テクスチャ自体に対して実行できます。 詳細については、「**[法線の操作](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**」ページを参照してください。

## glTFマテリアル

glTFマテリアルを使用する場合は、マテリアルレイヤーエフェクトが自動的に設定されます。 Substanceプラグインは、glTF マテリアルをSubstance項目マテリアルの上に直接配置します。

| Substance出力 | カラースペース | マテリアルレイヤー効果 |
| --- | --- | --- |
| ベースカラー | sRGB | glTFBase color |
| 粗さ | 線形 | glTFラフネス |
| メタリック | 線形 | glTFメタリック |
| 法線 | 線形 | glTF標準 |
| 放射 | sRGB | glTF Emissive **\*静止画のsRGBに設定** |
| アンビエントオクルージョン | 線形 | glTFAmbient occlusion |

![](../../../assets/gltf.png){width="600px"}

法線を反転する必要がある場合があります。 これは、Substanceに法線の方向のコントロールがある場合は、[ツイーク]メニューから実行できます。 そうでない場合は、テクスチャ自体に対して実行できます。 詳細については、「**[法線の操作](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**」ページを参照してください。
