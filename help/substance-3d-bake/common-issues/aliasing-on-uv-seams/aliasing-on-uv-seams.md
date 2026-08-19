---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/aliasing-on-uv-seams.html"
breadcrumb-title: ''
description: アンチエイリアス設定とパディング設定を調整することで、ベイク処理中にUV シームに表示されるエイリアスアーティファクトを修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Aliasing on UV Seams
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV シームのエイリアス
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# UV シームのエイリアス

>[!WARNING]
>
> **問題**
> 
> 焼いた後、UV シームの境界線に暗い斑点またはドットが表示されます。
> 
> ![](../../assets/edge-aliasing.png)

>[!NOTE]
>
> **説明**
> 
> ベイカーがテクスチャに情報を書き込む場合、ジオメトリからピクセルに変換する必要があります。 この情報の処理により、[ エイリアス ](https://en.wikipedia.org/wiki/Aliasing)が発生する可能性があります。 エイリアシングは、UVのジオメトリがピクセルグリッドと整列していないか、UVが十分な解像度を提供するのに十分なピクセルをカバーしていないために頻繁に発生します。
> 
> 次の画像では、ジオメトリが赤いオーバーレイになっています。 ベイカーは、その表面の半分以上がジオメトリで覆われている場合、ピクセルを完全としてマークします（白い正方形は完全なピクセル、黒い正方形は空のピクセルです）。 右側の画像では、ピクセルグリッドが2倍の解像度で、ジオメトリをより正確に表現できます。
> 
> ![](../../assets/aliasing-example-large.png)
> 
> ![](../../assets/aliasing-example-small.png)

>[!NOTE]
>
> **解決策**
> 
> * ベイカーの出力テクスチャ解像度を上げます。
> * アンチエイリアス設定を上げます（注意：計算に時間がかかる場合があります）。
> * 3D モデリングソフトウェアのUV エディターで、UVをピクセルグリッドに合わせます。
> * UVに対してより良いテクセル比を与えます。
