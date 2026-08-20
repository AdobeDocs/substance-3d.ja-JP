---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/bakers-settings/curvature-from-mesh.html"
breadcrumb-title: ''
description: レイトレーシングを使用して、高ポリメッシュから正確な曲率テクスチャを生成し、正確なエッジ検出を実現します。
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

メッシュベイカーからの曲率は、高ポリメッシュからの曲率テクスチャを生成します。 ベース [曲率](../../bakers-settings/curvature/curvature.md) ベイカーよりも遅くなりますが、より正確な結果が得られます。

**次の場所で利用できます：**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## パラメーター

| *パラメーター* | *説明* |
| --- | --- |
| **セカンダリ レイ** | 近くのジオメトリを読み取るために放出される光線の量。 値を大きくすると、ノイズは少なくなりますが、計算に時間がかかります。 デフォルトは32です。 |
| **サンプリング半径** | ジオメトリの表面の曲率を計算するために、近くのジオメトリをどの程度考慮するかを考慮します。 値を大きくするとエッジが強くなり、値を小さくするとエッジが細くなりますが、情報が失われます。 |
| バウンディングボックスに対する&#x200B;**相対** | サンプリングの半径がメッシュのサイズに対する相対的なものか、単位ベースの距離として定義されているかを定義します。 |
| **自己交差** | 曲率光線の名前で一致させます。 ベイカーがローポリジオメトリとハイポリジオメトリにどのように一致するかを示します。 これは、手動でメッシュを離す（爆発させる）必要なく、ベーキングプロセスをフィルタリングするために使用できます。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>常に</strong> （既定値）：ローポリメッシュは、すべてのハイポリメッシュと一致します。</li><li data-preserve-html="true"><strong> メッシュ名</strong>: メッシュを名前でフィルタリングして、不要なジオメトリと一致しないようにします。</li></ul>ジオメトリの一致について詳しくは、[名前による一致](../../features/matching-by-name/matching-by-name.md)を参照してください。 |
| **自動トーンマッピングの境界** | 曲率値をテクスチャに書き込む方法を制御します。 有効にすると、値の範囲は、ベイクプロセス中に見つかった最小値と最大値に基づいて0から1の間で正規化されます。 無効にした場合、最小値と最大値は手動で定義されます。  **注：** UDIM/UV タイルをベイク処理する場合、このパラメーターを無効にして、トーンマップを均一にし、タイルごとに特定しないようにします。そうしないと、各テクスチャ間にシームが作成される可能性があります。 適切な最小値/最大値を手動で見つけるには、まずベイクを有効にして、コンソール/ログを見て、ベイカーが出力した値を確認します。 |
| **最小のトーンマッピング** | **自動トーンマッピング境界**&#x200B;が無効になっている場合は、曲率結果をテクスチャに合わせて拡大・縮小するための最小値を定義します。 |
| **最大トンマッピング** | **自動トーンマッピング境界**&#x200B;が無効になっている場合は、曲率結果をテクスチャに合わせて拡大・縮小するための最大値を定義します。 |
| **法線マップ** | 通常のテクスチャへのオプションのパス。 パン屋の内部計算を置き換えるために使用できます。 |
| **ワールド スペース** | 有効にすると、法線テクスチャは接線空間ではなくワールド空間法線として解釈されます。 |
| **通常の向き** | 接線空間の場合の標準テクスチャの形式。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> （既定値）</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
