---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/common-issues/aliasing-on-uv-seams.html"
breadcrumb-title: ''
description: アンチエイリアスとパディングの設定を調整して、ベイク処理時にUVシームに表示されるエイリアシングアーティファクトを修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Aliasing on UV Seams
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UVシーム上のエイリアス
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# UVシーム上のエイリアス

>[!WARNING]
>
> **問題**
> 
> ベイク処理後にUVの継ぎ目の境界に暗いスポットまたはドットが表示される：
> 
> ![](../../assets/edge-aliasing.png)

>[!NOTE]
>
> **説明**
> 
> ベイカーがテクスチャに情報を書き込むときには、ジオメトリからピクセルに変換する必要があります。 この情報を処理すると、[エイリアス](https://en.wikipedia.org/wiki/Aliasing)が発生する可能性があります。 エイリアスが発生するのは、UVのジオメトリがピクセルグリッドと揃っていなかったり、UVが十分な解像度を提供するのに十分なピクセルをカバーしていないことが原因です。
> 
> 次の図では、ジオメトリは赤のオーバーレイです。 表面の半分以上がジオメトリで覆われている場合（白い正方形は完全なピクセル、黒い正方形は空のピクセル）、ベイカーはピクセルに完全とマークします。 右側の画像では、ピクセルグリッドの解像度が2倍に設定されているため、ジオメトリをより正確に表現できます。
> 
> ![](../../assets/aliasing-example-large.png)
> 
> ![](../../assets/aliasing-example-small.png)

>[!NOTE]
>
> **解決策**
> 
> * ベーカーの出力テクスチャ解像度を上げます。
> * アンチエイリアス設定を上げます（注意：計算に時間がかかる場合があります）。
> * 3DモデリングソフトウェアのUVエディターで、UVをピクセルグリッドにアラインします。
> * UVに対するテクスチャの比率を上げます。
