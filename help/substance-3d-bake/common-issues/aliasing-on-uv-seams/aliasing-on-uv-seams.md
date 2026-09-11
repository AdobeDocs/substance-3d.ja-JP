---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/aliasing-on-uv-seams.html"
breadcrumb-title: ''
description: アンチエイリアスとパディングの設定を調整して、ベイク中にUVシームに表示されるエイリアスの斑点を修正します。
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Aliasing on UV Seams
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: シームのエイリアス
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# シームのエイリアス

>[!WARNING]
>
> **問題**
> 
> ベイク後、UVシームの境界に暗い点やドットが表示されます。
> 
> ![](../../assets/edge-aliasing.png)

>[!NOTE]
>
> **説明**
> 
> ベイカーが情報をテクスチャに書き込むときには、ジオメトリからピクセルに変換する必要があります。 この情報を処理すると、[エイリアス](https://en.wikipedia.org/wiki/Aliasing)が発生する可能性があります。 エイリアスが発生するのは、UVのジオメトリがピクセルの解像度に合っていなかったり、UVのグリッドがピクセルを十分にカバーしていないことが原因です。
> 
> 次の図では、ジオメトリは赤のオーバーレイです。 サーフェスの半分以上がジオメトリで覆われている場合（白い正方形は完全なピクセル、黒い正方形は空のピクセル）、ベイカーはピクセルに完全とマークします。 右側の図では、ピクセルグリッドはジオメトリをより正確に表現できる解像度の2倍です。
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
> * 3DモデリングソフトウェアのUVエディタで、UVをピクセルグリッドに位置合わせします。
> * UVに対するテクスチャの比率を上げます。
