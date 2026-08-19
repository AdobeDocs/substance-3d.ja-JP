---
helpx_url: 'https://helpx.adobe.com/substance-3d-bake/features/matching-by-name.html'
breadcrumb-title: ''
description: 「名前で一致」機能を使用して、ローポリメッシュとハイポリメッシュを分離し、ベイク処理中のジオメトリのブリードを防ぎます。
helpx_creative_field: ''
helpx_description: bakers > Features > Matching by Name
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 名前で一致
user-guide-description: ''
user-guide-title: ''
source-git-commit: d57629bee333101dd9f40f30ed24ff84b6b8c6f1
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---


# 名前で一致

![](../../assets/banner-matching-by-name.jpg)

「名前で一致」は、Substance Bakersで使用して、名前に基づいてローポリメッシュとハイポリメッシュを分離できるフィルタリング方式の名前です。

この機能は、ベイク処理中にジオメトリのブリードを避けて、クリーンなテクスチャを実現するのに非常に便利です。 同じ結果を得るために、メッシュを離れる必要を回避します（「爆発」と呼ばれることが多い）。

## 名前で一致を使用する場合

### メッシュのブリードによる法線マップのベイク処理

この例では、キャラクターの頭の上にあるヘルメットがキャラクターの顔にブリードしています。

「名前で一致」を有効にすると、ヘルメットを無視して顔を適切に焼くことができます。 *この結果は、メインの一致設定に基づいています。*

| *メッシュ* | *名前が一致しない* | *に名前で一致* |
| --- | --- | --- |
| ![](../../assets/baking-demo-vela.png){width="250px"} | ![](../../assets/baking-demo-vela-normal-nomatch.png){width="250px"} | ![](../../assets/baking-demo-vela-normal-withmatch.png){width="250px"} |

### 浮動小数点ジオメトリの背面を無視

この例では、ボックスの上部にある「ボタン」はフローティングジオメトリであり、ハイポリメッシュには接続されていません。 したがって、デフォルトでは、その下のボックスにシャドウが適用され、ジオメトリの境界が表示されます。

「**バックフェイスを無視**」設定で「名前で一致」を有効にすることで、ボタンの下の領域を無視しながらアンビエントオクルージョンをベイク処理して、1つの単一のボックスのように見せることができます。*この結果は、「バックフェイスを無視」設定の使用に基づいています。*

| *メッシュ* | *名前が一致しない* | *に名前で一致* |
| --- | --- | --- |
| ![](../../assets/ignorebf-mesh.png){width="250px"} | ![](../../assets/ignorebf-off.png){width="250px"} | ![](../../assets/ignorebf-on.png){width="250px"} |

## 名前によるマッチングの仕組み

「名前で一致」システムは、ローポリメッシュとハイポリメッシュの両方でジオメトリ名を読み取り、キーワード（サフィックス）を使用して名前を識別または一致させることで機能します。 デフォルトでは、パン屋は特定の接尾辞を使用しますが、変更できます（以下を参照）。

サポートされている現在のサフィックスは次のとおりです。

| *サフィックスの種類* | *デフォルト値* | *使用状況* |
| --- | --- | --- |
| ハイポリ | *\_high* | ハイポリメッシュの名前を分離して、ローポリメッシュと照合するために使用します。 |
| ローポリ | *\_low* | ローポリメッシュの名前を分離して、ハイポリメッシュと照合するために使用します。 |
| 背面を無視 | *\_ignorebf* | Ambient Occlusionなどの二次光線を使用するベイカーのバックフェイスを無視するために使用されます。*このサフィックスは、ハイポリメッシュにのみ存在する必要があります（例：**mesh\_high\_ignorebf***）。 |

この機能を適切に動作させるために考慮すべきルールがいくつかあります。

* [共通パラメーター](../../bakers-settings/common-parameters/common-parameters.md)で名前による照合を有効にする必要があります。既定では&#x200B;**オフです**。
* 一部のベイカー（[Ambient Occlusion](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)など）では、セカンダリレイが生成されるため、セカンダリマッチングの設定が有効になる場合があります。
* 一致は大文字と小文字が区別されます。つまり、「**Vela**」という名前のメッシュは「**vela**」という名前のメッシュと一致しません。
* ジオメトリ名のサフィックスが存在する場所に基づいて、複数のメッシュを一致させることができます。

次に、マッチングの動作の例を示します（デフォルトの接尾辞を使用）。

| ローポリ名 | ハイポリと一致します | 高いPolyと一致しません |
| --- | --- | --- |
| <ul data-preserve-html="true"><li data-preserve-html="true">body_low</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">body_high</li><li data-preserve-html="true">body_high_top</li><li data-preserve-html="true">body_high_1</li><li data-preserve-html="true">body_high_2</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">body-high</li><li data-preserve-html="true">body_top_high</li></ul> |
| <ul data-preserve-html="true"><li data-preserve-html="true">Head_low</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Head_high</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">head_high</li></ul> |
| <ul data-preserve-html="true"><li data-preserve-html="true">Leg_low_top</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Leg_high</li><li data-preserve-html="true">Leg_high_top</li><li data-preserve-html="true">Leg_high_high_top</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Leg_top_high</li></ul> |

## ベーカーのセットアップ方法

### 名前による照合の有効化

名前による照合は、Baker設定の[共通パラメーター](../../bakers-settings/common-parameters/common-parameters.md)で有効にできます。

| *ソフトウェア* | *設定* |
| --- | --- |
| **Substance Painter** | <ol class="steps" data-preserve-html="true"> <li class="step" data-preserve-html="true">     （テクスチャセット設定を使用して）ベイキングウィンドウを開きます。    </li> <li class="step" data-preserve-html="true">     共通パラメーターを表示します。    </li> <li class="step" data-preserve-html="true">     設定<strong>Match</strong>を「Always」から「By Mesh Name」に変更します。<br/> <img data-preserve-html="true" src="../../assets/baking-match-setting-sp.png"/>    </li> </ol> |
| **Substance Designer** | <ol class="steps" data-preserve-html="true"> <li class="step" data-preserve-html="true">     ベイキングウィンドウを開きます（エクスプローラーウィンドウでリンクされたメッシュを右クリックします）。    </li> <li class="step" data-preserve-html="true">     設定<strong>Match</strong>を「Always」から「By Mesh Name」に変更します。<br/> <br/>    </li> </ol> |

### 接尾辞の名前の変更

デフォルトの接尾辞は\_lowと\_highで、次のように変更できます。

* **Substance Painter**: [ ベーキングウィンドウ ](../../getting-started/software-interface/3d-painter/substance-3d-painter.md)で、共通パラメーター内に配置します。
* **Substance Designer**: [ プロジェクト設定](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/workspace/preferences/project-settings)のベイク設定で行います。

## zBrushからのハイポリメッシュ

zBrushから書き出されたハイポリメッシュは、「名前で一致」機能を使用してベイク処理に使用できますが、次の設定に従う場合があります。

| *ファイル形式* | *説明* |
| --- | --- |
| **FBX** | 有効/無効にする特定のパラメーターはありません。メッシュファイルをそのまま使用できます。 |
| **OBJ** | zBrushによって書き出されたOBJ ファイルは、デフォルトで&#x200B;**名前で一致**&#x200B;しても機能しません。 代わりに、Substance Painterにメッシュファイル名を使用するように指示して、名前でメッシュを一致させることができます。そのために、次のことを確実に実行する必要があります。<ol data-preserve-html="true"><li data-preserve-html="true"><strong>各</strong> サブツールのグループ （Grp） パラメーターを</strong>無効にします。<strong></li><li data-preserve-html="true"><strong>OBJ ファイルに適切な名前を付けます（例：<strong>body_high.obj</strong>）。</strong></li></ol> ![](../../assets/zbrush-setting.png) |
