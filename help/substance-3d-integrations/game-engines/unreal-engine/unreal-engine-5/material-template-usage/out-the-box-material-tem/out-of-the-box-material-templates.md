---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5/out-of-the-box-material-templates.html"
breadcrumb-title: ''
description: SBSARマテリアルをUnreal Engine 5に読み込む際には、事前定義済みのマテリアルテンプレートを使用して、迅速なセットアップとワークフローを行うことができます。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5 > Out-of-the-Box Material Templates
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: すぐに使えるマテリアルテンプレート
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---


# すぐに使えるマテリアルテンプレート

SBSARマテリアルをコンテンツブラウザーに読み込む場合、すぐに使用できる様々なマテリアルテンプレートをドロップダウンで選択できます。

![](../../../../../assets/screen-shot-2022-05-10-at-8-58-45-pm-copy.png)

## Substance標準テンプレート

これは、一般的なUV操作の基本マテリアルテンプレートです。 UV量の基本的なコントロールがいくつか用意されているので、UVをスケールしてテクスチャを伸長することができます。 UVのスプリットオプションを有効にすると、UVのスケーリングをスプリットすることができます。Uの量、Vの量、UV オフセット、UVの回転角度も存在します。 これにより、UVタイリングとUV回転を同時に行うことができます。

![](../../../../../assets/screen-shot-2022-05-10-at-9-06-40-pm-copy.png)

## Substance三平面テンプレート

Tirplanarテンプレートは、メッシュのX、Y、Zの角度または面の三平面マッピングを行うため、テクスチャの3つの異なる投影をブレンドして、角度をシームレスにブレンドできます。 3平面テンプレートを使用すると、オブジェクトの曲げに合わせてマテリアルを異なる面でブレンドできます

![Substanceの三平面マテリアルの詳細メニュー](../../../../../assets/triplanar-template.png)

3Planarテンプレートは物理サイズをサポートしているため、物理サイズを有効にすると、3Planarテンプレートはマテリアルの物理サイズに基づいてイメージをスケーリングします。このため、オブジェクトをどのくらいスケーリングしても、テクスチャは常に同じままで、均一な外観になります。 詳細物理サイズについては、こちらを参照してください： [物理サイズ - UE5](../../../../../game-engines/unreal-engine/unreal-engine-5/physical-size-ue5/physical-size-ue5.md)

## Substance屈折テンプレート

屈折テンプレートは、主にガラスなどの透明なオブジェクトに使用されます。 これにより、ガラスマテリアルや透明マテリアルのIOR値や標準テクスチャを変更できます。

![](../../../../../assets/screen-shot-2022-05-10-at-9-07-38-pm.png)

## Substance車のペイントテンプレート

自動車塗装テンプレートでは、クリアコートのサポートを追加し、調整可能なUVタイルと値、クリアコートの粗さの値、およびフレネルパワーの値のサポートを含んでいます。

![Substanceの車のペイントマテリアルの詳細メニュー](../../../../../assets/car-paint-template.png)

## ディスプレイスメントテンプレートの設定

>[!IMPORTANT]
>
> 試験的テンプレート
> 
> 警告：次のテンプレートは試験的であり、バージョン間で大きな変更が発生する可能性があります。 これらのテンプレートは、エピックのNanite機能を利用しており、この執筆時点ではそれ自体が実験的です。 100%安定していない場合があり、プロジェクトで使用する際には注意が必要です。

プロジェクトでNaniteディスプレイスメントサポートを完全に有効にし、メッシュでディスプレイスメントマテリアルを使用するには、次の手順を実行します。

1. プロジェクトフォルダー/設定/DefaultEngine.iniに移動して開きます
1. [/Script/Engine.RendererSettings]セクションに次を追加します。
   * r.Nanite.AllowTessellation=1
   * r.Nanite.テセレーション=1
1. ディスプレイスメントテンプレートを適用する静的メッシュを選択し、その設定を開きます。
1. 「 Naniteサポートを有効にする」オプションをオンにします。
1. 目的の.sbsarをコンテンツブラウザにインポートし、Substance\_Displaceent\_TemplateまたはSusbtance\_Triplanar\_Displacement\_Templateのいずれかを選択します
1. ディスプレイスメント量を変更するには、マテリアルテンプレートに移動し、出力ノードを選択します。 次に、「ディスプレイスメント」セクションで「マグニチュード」を調整します。

## ディスプレイスメントテンプレート

Substance標準テンプレートと同様に、Naniteディスプレイスメントのサポートを加えながら、U値とV値を調整できます。

ディスプレイスメントマテリアルの![詳細メニュー](../../../../../assets/displacement-template.png)

## Substance三平面ディスプレイスメントテンプレート

ディスプレイスメントテンプレートと同様に、このテンプレートは、Naniteディスプレイスメントサポートに加えて、物理サイズサポートのオプションでトライプラナー投影を適用します。

![Substanceの三平面ディスプレイスメントマテリアルの詳細メニュー](../../../../../assets/triplanar-displacement-template.png)
