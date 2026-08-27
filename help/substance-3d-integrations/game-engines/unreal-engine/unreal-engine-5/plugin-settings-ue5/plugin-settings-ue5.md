---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/plugin-settings-ue5.html"
breadcrumb-title: ''
description: Unreal Engine 5のSubstanceプラグインの設定をプロジェクト設定から変更し、プラグインの動作をカスタマイズします。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Plugin Settings - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: プラグイン設定 – UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---


# プラグイン設定 – UE5

設定にアクセスするには、編集/プロジェクト設定に移動し、「プラグイン」カテゴリまで下にスクロールして、「Substance」をクリックします。

![](../../../../assets/screen-shot-2022-03-31-at-5-50-29-pm.png)

## ハードウェア予算

メモリバジェットは、Substanceエンジンに使用するメモリの最大量です。 この値を大きくすると、Substanceの処理速度が向上しますが、システム・リソースの消費量が増えます。 （プロジェクトレベルでは、必ずしも役に立つ増加ではありません）。

「CPUコア」は、Substanceエンジンで使用可能なコア数を決定します。 これには、物理コアとハイパースレッドの両方が含まれます。 (割り当てられている数がシステムで使用可能なコア数より大きい場合は、デフォルトですべての使用可能コアが使用されます。

## 料理

調理中に取り除かれたMIPレベルカウントにより、パッケージのテクスチャの作成方法が変わります。 この設定により、大きなテクスチャミップレベルを読み込む必要がなくなるため、読み込み時間が大幅に短縮され、パッケージサイズが小さくなります。 低い解像度/小さいLODがロードされ、最高のLODがUE5によってデフォルト設定されます。 SubstanceはSubstanceエンジンを通じて処理され、実行時に高解像度のLODで更新されます。

Substance engineはCPUまたはGPUです。 GPUエンジンを使用すると、4Kテクスチャを作成できます。 CPUエンジンの上限は2Kです。

## 最適化：

これにより、各バッチでsubstanceエンジンに渡すことができる非同期物質の数が制限されます。 数値を小さくすると、非同期タスクの実行速度が上がり、更新されます。数値を大きくすると、バッチレンダリングが実行され、複数のSubstanceが同時に処理されます。 （値が大きいほど、テクスチャの更新間隔が長くなるため、テクスチャの更新間隔が大きくなります）。

## 非同期/同期レンダリング

同期レンダリングは、ブロッキングレンダリング呼び出しです。 このメソッドは、グラフインスタンスを再計算するSubstanceエンジンに渡しますが、SubstanceエンジンがSubstanceの処理を完了するまで実行を停止してから、コードの実行に進みます。 結果は、処理が完了するとすぐに画面で更新されます。

Asyncは、グラフをキューに追加し、プラグインのアップデート中に一度に複数のグラフをSubstanceエンジンに送ります（Substance設定内から設定します）。 同期レンダリングとは異なり、エンジンが完了するのを待つのではなく、送信されるとすぐにプログラムは通常のように動作し続けます。 エンジンがそのバッチを完了すると、結果が返され、出力に適用されて、別のバッチが開始されます。
