---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/blender/substance-in-blender-overview.html"
breadcrumb-title: ''
description: Substance 3D Blender版のアドオンについて説明し、プロジェクトでSubstanceのマテリアルを読み込んで操作する方法を説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Substance in Blender Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: BlenderでのSubstanceの概要
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---


# BlenderでのSubstanceの概要

## プラグインの概要

Substance 3Dアドオンを使用すると、SubstanceのマテリアルをBlenderに読み込むことができます。 Substance 3Dパネルを使用すると、プロジェクト内のSubstanceマテリアルを1か所で管理およびカスタマイズできます。 このアドオンは、.sbsarファイルからテクスチャマップを生成し、それを使用してブレンダーマテリアルを作成します。 これらのテクスチャは、Substanceパラメータを調整すると自動的に更新されます。

## Substanceマテリアルを読み込む

1. Substance 3Dパネルの「**読み込み**」ボタンをクリックします。
1. 開いたウィンドウで、.sbsarファイルが保存されている場所に移動し、1つ以上を選択します。 次に、[**Substanceマテリアルの読み込み**]ボタンをクリックします。
1. マテリアルパネルの球アイコンをクリックしてドロップダウンを開き、Substanceマテリアルを選択します。 これにより、マテリアルが現在のスロットに割り当てられます。 または、Substance 3Dパネルの「適用」ボタンを使用して、現在の割り当てをオーバーライドしない新しいマテリアルスロットにマテリアルを割り当てます。

>[!NOTE]
>
> オブジェクトにマテリアルがない場合は、[**適用**]ボタンをクリックすると、Substanceのマテリアルが自動的に適用されます。

![](../../../assets/blender-overview-steps.png)

## Substance 3Dパネル

Substance 3Dパネルは、プロジェクト内のSubstanceマテリアルを管理し、個々のパラメーターを調整するために使用されます。 グラフパラメーターセクションでは、テクスチャの解像度、タイル表示、ランダム化、プリセットを制御できます。 出力セクションには、生成されたテクスチャの画像形式用のコントロールがあります。 Substanceパラメーターセクションでは、Substanceパラメーターを調整することができます。

詳しくは、[Substance 3Dパネル](../../../3d-applications/blender/the-3d-panel/the-substance-3d-panel.md)を参照してください。

## 環境設定

デフォルトの動作およびその他の設定は、アドオンの環境設定で調整できます。 [マテリアルを自動的にアタッチ]を有効にすると、Substanceマテリアルをオブジェクトに自動的にアタッチして、現在のマテリアル割り当てをオーバーライドできます。 「選択したオブジェクトのマテリアルを自動的にハイライト表示」を選択すると、そのマテリアルを含むオブジェクトが選択されている場合、Substance 3Dパネルでハイライト表示されたマテリアルが変わります。 「サイクルの自動アップデートテクスチャ」を有効にすると、サイクルレンダリングビューの使用中に3Dビューポートでテクスチャを更新できます。

ディスプレイスメントは、「出力」セクションのHeightの切り替えで有効にできます。 ここでは、各出力のファイル形式とビット深度を調整することもできます。

詳細については、[環境設定](../../../3d-applications/blender/preferences/preferences.md)のページを参照してください。

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/blender-overview-preferences-1-v2.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/blender-overview-preferences-2-v2.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/blender-overview-preferences-3.png)

</td>
</tr>
</table>

## Substance資料に関する詳細をご覧ください

プロが作成した何千ものマテリアルやその他のアセットは、[Substance 3D Assetsページ](https://helpx.adobe.com/jp/substance-3d/unlisted/assets.html)からダウンロードできます。 コミュニティによって無料で共有されているアセットの多くは、[Substance 3D Community Assetsページ](https://helpx.adobe.com/jp/substance-3d/unlisted/community-assets.html)でご覧いただけます。

## Community

一般的なヘルプ、フィードバック、または問題を報告するには、[Substance不一致サーバー](https://discord.com/invite/substance3d)または[Adobeコミュニティ](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-blender)の#substance-blender-betaチャンネルにご参加ください。
