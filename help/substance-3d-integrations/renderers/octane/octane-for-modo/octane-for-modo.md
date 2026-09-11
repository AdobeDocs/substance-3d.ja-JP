---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/octane/octane-for-modo.html"
breadcrumb-title: ''
description: MODOのオクタンレンダラーでは、ライブDBマテリアルと適切な出力マテリアルを使用して、Substance構成を使用します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Octane > Octane for MODO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MODOのオクタン
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# MODOのオクタン

## MODOプラグインのSubstance

Substanceはオクタンでネイティブに動作を出力します。 次のSubstance出力とテクスチャレイヤーエフェクトの設定を使用できます。

1. Substanceを作成/テクスチャ/Substanceを作成を選択し、Unreal Materialを選択します。 アンリアルマテリアルを使用すると、高度なOGLビューポートでテクスチャを表示できます。
1. ベースカラー、メタリック、粗さ、法線の出力を作成します。
1. MODOはOGL 法線マップを使用します。 Substanceプロパティで、法線方向をOpenGLに変更する必要があります。

   ![](../../../assets/ogl.png)
1. Substance PBRプリセットを読み込みます。 このプリセットはオクタンオーバーライドです。 シェーダーグループにドラッグします。

   [Substance\_PBR.lxp](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/integrations/files/162005234/162005272/1/1502792782697/substance-pbr.lxp)
1. 上書きを選択し、Substance出力をクリップブラウザからスケマティクビューにドラッグします。 ファイル名出力のあるノードを、適切な入力ノード（ベースカラー→ベースカラー）に接続します。

   ![](../../../assets/connect-6.png)
1. 残りのSubstance出力をフックします

   ![](../../../assets/outputs-4.png){width="640px"}
