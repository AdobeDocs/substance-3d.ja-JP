---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/optimization-guidelines.html"
breadcrumb-title: ''
description: 最適化のガイドラインに従って、マテリアルの複雑さとUnityのレンダリングパフォーマンスのバランスをとります。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Optimization Guidelines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 最適化ガイドライン
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# 最適化ガイドライン

Substanceマテリアルが複雑になるほど、レンダリングに必要な処理能力が高まります。 したがって、Substanceマテリアルは&#x200B;**複雑さとレンダリング速度のバランスを取る**&#x200B;必要があります。 ゲームなどのリアルタイムグラフィックスアプリケーションで使用する場合は、*特に*&#x200B;重要です。

独自のカスタムマテリアルを作成する場合は、次の最適化のガイドラインを確認してください。

[Substance Designerの最適化に関するガイドライン](https://docs.substance3d.com/display/SDDOC/Performance+Optimization+Guidelines)

注意すべき重要な注意点は、4K以上の絶対解像度を持つノードです。

>[!WARNING]
>
> **解像度と親に対する相対解像度の設定に注意してください。**\
> 値を大きくするとパフォーマンスに重大な影響が生じるため、マテリアルがどのように使用されるか、および使用するデータサイズを減らすことができるかどうかを考慮してください。
>   
> Substance CPUエンジンは4Kで演算を行うことができますが、非常に遅いため、インテグレーションがハングしたり、クラッシュする可能性があります。

次の例では、[タイルSampler](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/node-library/texture-generators/patterns/tile-sampler)ノードの出力サイズが[絶対](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/output-size) 4096に設定されています。 これにより、ダウンストリームのいくつかのノードが4Kで計算されてから、最終的な2048出力解像度に合わせてダウンスケールされます。

![](../../../assets/absolute.png){width="1000px"}
