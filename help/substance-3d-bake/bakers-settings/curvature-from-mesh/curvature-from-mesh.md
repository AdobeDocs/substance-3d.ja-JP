---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/curvature-from-mesh.html"
breadcrumb-title: ''
description: レイトレーシングを使用して正確なエッジ検出を行い、ハイポリメッシュから正確な曲率テクスチャを生成します。
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メッシュからの曲率
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# メッシュからの曲率

メッシュベイカーの曲率は、ハイポリメッシュから曲率テクスチャを生成します。 ベースの[曲率](../../bakers-settings/curvature/curvature.md)ベイカーよりも低速ですが、より正確な結果が得られます。

**使用可能：**

* Substance Designer
* Substance自動処理ツールキット
* Substance Painter

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **セカンダリレイ** | 近くのジオメトリを読み取るために放出される光線の量。 値を大きくすると、ノイズは少なくなりますが、計算に時間がかかります。 デフォルトは32です。 |
| **サンプリング半径** | ジオメトリのサーフェスの曲率を計算するために近くのジオメトリが考慮される距離。 値が大きいほどエッジが強くなり、値が小さいほどエッジが薄くなりますが、情報が失われます。 |
| **バウンディングボックスを基準にする** | サンプリング半径がメッシュのサイズに対して相対的であるか、単位ベースの距離として定義されるかを定義します。 |
| **自己交差** | 曲率線の名前による照合。 ベイカーが低ポリゴンおよび高ポリゴンのジオメトリに一致する方法を示します。 手動でメッシュを分解する必要なく、ベイク処理をフィルタするために使用できます。有効な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定）:ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong>メッシュ名で</strong>：不要なジオメトリと一致しないように、メッシュを名前でフィルタします。</li></ul>一致するジオメトリの詳細については、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **自動トーンマッピング範囲** | 曲率の値をテクスチャに書き込む方法を制御します。 有効な場合、値の範囲は、ベイクプロセス中に見つかった最小値と最大値に基づいて0 ～ 1で正規化されます。 無効になっている場合、最小値と最大値は手動で定義されます。  **注意：** UDIM/UVタイルをベイク処理する場合、このパラメーターを無効にしてトーンマッピングを均一にし、タイルごとに特定しないようにする必要があります。無効にすると、各テクスチャの間に継ぎ目が生じる可能性があります。 適切な最小値/最大値を手動で見つけるには、この設定を有効にしてベイク処理を実行してから、コンソール/ログを調べて、ベイカーが出力した値を確認します。 |
| **トーンマッピングの最小値** | **自動トーンマッピング境界**&#x200B;が無効な場合、テクスチャに合わせて曲率結果をスケールするための最小値を定義します。 |
| **トーンマップの最大値** | **自動トーンマッピング境界**&#x200B;が無効な場合、テクスチャに収まるように曲率結果をスケールする最大値を定義します。 |
| **標準マップ** | 法線テクスチャへのパス（オプション）。 ベーカーの内部計算の置き換えに使用できます。 |
| **ワールドスペース** | 有効にすると、法線テクスチャは接線空間ではなくワールド空間法線として解釈されます。 |
| **法線の向き** | 接線空間の場合の法線テクスチャのフォーマット。指定可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> （既定）</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
