---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/color-management.html"
breadcrumb-title: ''
description: 異なるレンダラーを使用するSubstanceマテリアルを使用する場合のカラーマネジメントとガンマ補正について説明します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: カラーマネジメント
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 2%

---


# カラーマネジメント

線形空間レンダリングが照明計算に適切な数値計算を提供することを述べる際に、単純化したアプローチを取ります。 これにより、光の相互作用を信頼できる現実世界の方法で表現できる環境が作成されます。 リニアスペースレンダリングの議論のために、ガンマ補正の概念を導入する必要があります。 表示と保存の目的で画像をエンコードする場合、ガンマ補正は帯域幅とビット割り当てを減らす最適化プロセスです。 このプロセスでは、人間の目の明るさの知覚を利用します。これは、輝度の立方体のルートにほぼ従います。

>[!NOTE]
>
> 線形空間レンダリングは非常に複雑な被写体です。 詳しくは、[Substanceアカデミー](https://academy.substance3d.com/)の無料の[PBRガイド第1巻](https://academy.substance3d.com/courses/the-pbr-guide-part-1)をご覧ください。

## カラーマネジメント

この文書では、[3D Substance Designer](https://www.adobe.com/products/substance3d/3d-augmented-reality.html)およびレンダラーの&#x200B;**ソフトウェア**&#x200B;および&#x200B;**Substance Painter**&#x200B;から書き出されたテクスチャの操作プロセスについて詳しく説明します。

マテリアルチャンネルへの入力として使用される画像の正しい変換方法は、シーン内での画像の使用方法によって異なります。 カラースペース、エンコード、およびカラー値が&#x200B;**シーン参照の輝度**&#x200B;または&#x200B;**ディスプレイ参照の輝度**&#x200B;のどちらに比例するかも重要な役割を果たします。

* **色以外のデータ**&#x200B;を表すために使用される画像は変換できません。 これらは通常、**通常**、**粗さ**、**金属**、**ディスプレイスメント**&#x200B;および&#x200B;**周囲****オクルージョン**&#x200B;のマップです。
* 表示されるカラーを表す画像には、複数のシナリオがある場合があります。 たとえば、既に&#x200B;**シーン線形**&#x200B;の画像は、通常、**OpenEXR**&#x200B;や&#x200B;**HDR**&#x200B;などの形式で保存された&#x200B;**ハイダイナミックレンジ**&#x200B;画像のように変換する必要はありません。
* 表示用(**display-referred**)に作成された画像は、ガンマを削除する必要があります。 これらの形式には、**PNG**、**JPEG**、**BMP**&#x200B;などのほとんどの形式が含まれます。 これらの画像は、**ベース** **カラー**、**拡散**、**Specular**&#x200B;および&#x200B;**放射能**&#x200B;です。

これは過剰な簡略化ですが、次のようにプロセスを考えると役に立ちます。

* 「シーン参照(例： linear)&quot; ：変換を適用しません
* “display-referred (ex. sRGB) 」：逆変換を適用して画像を「リニア化」し、適切に計算します

>[!NOTE]
>
> ガンマ空間からリニア空間への変換に使用されるsRGBデコード関数(EOTF)は、Substance PainterとSubstance Designerに使用され、IEC 61966-2-1:1999規格で定義されています

Substance Designerは、カラーマネジメントに[OpenColorIO](https://opencolorio.org/)を使用するように構成できます。 これにより、複数のアプリケーション間で&#x200B;*一貫*&#x200B;した色変換と画像表示を行うことができます。 このモードでは、Substance Designerは&#x200B;**線形RGB**&#x200B;色で内部的に機能します。 通常、8 ビット深度ではリニアな色を表現できないため、[グラフ](https://docs.substance3d.com/display/SDDOC/Graph+View)のカラーテクスチャには&#x200B;*少なくとも* **16ビット**&#x200B;の深度を使用することをお勧めします。

![](https://helpx-prod.scene7.com/is/image/HelpxProd/sd-cm?$png$&jpegSize=200&wid=686)

[ACES](https://www.oscars.org/science-technology/sci-tech-projects/aces)を導入すると、リニアsRGB （sRGBのガンマなしのバージョン）と[ACEScg](https://acescolorspace.com/)の2つの異なるカラースペースが作成されます。これは、CGレンダリングにより適した広色域（「シーン参照」またはリニア）のカラースペースです。

*プロットグラフィックの色域 –<https://acescolorspace.com/>*

Substance Designerは&#x200B;**Adobe Color Engine (ACE)**&#x200B;もサポートしています。 **ACE**&#x200B;では、**sRGB**、**リニアsRGB**、**ACEScg**&#x200B;の間の作業用カラースペースを選択できます。 **sRGB**&#x200B;を使用する場合、**ACE**&#x200B;はレガシーモードとほとんど同じです。 リニアカラースペースを使用する場合、**ACE**&#x200B;は[OpenColorIO](https://opencolorio.org/index.html)と多少は似ています。

## Substance プラグイン

Substanceインテグレーションプラグインを使用してSubstanceのマテリアルを使用する場合、出力はインテグレーションとホストアプリケーションのカラーマネジメントを介して自動的にリニア/ガンマのフラグが付けられます。 ただし、このプロセスを理解することは重要です。SubstanceマップをSubstanceマテリアルではなく書き出されたビットマップとして使用する場合、使用しているレンダラーに応じて、テクスチャに&#x200B;**ガンマエンコード**&#x200B;または&#x200B;**raw**&#x200B;のフラグを手動で設定する必要があります。 通常、8ビットまたは16ビットの.png、.jpg、.tgaまたは.tifファイルはガンマでエンコードされ、**sRGB OETF**&#x200B;および.exrファイルはリニアです。

## 3Dアプリケーション

### テクスチャの操作

* [MayaのSubstanceテクスチャ](../../renderers/color-management/textures-in-maya/substance-textures-in-maya.md)
* [3ds MaxのSubstanceテクスチャ](../../renderers/color-management/textures-in-3ds-max/substance-textures-in-3ds-max.md)
