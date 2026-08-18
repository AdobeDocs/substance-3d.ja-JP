---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-8-0.html"
breadcrumb-title: ''
description: 新機能、改善点、バグ修正については、 3ds Maxプラグインバージョン2.8.0のリリースノートを確認してください。
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.8.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# 3ds Max 2.8.0

<b>追加/更新：
</b>

* パラメーターの条件付き表示(「visible if」)のサポート。条件が満たされない場合、パラメーターは非表示になり、それぞれのグループは表示されたままになります。
* 3ds Maxプラグインでコロナレンダラをバージョン10にアップグレードし、レンダリング機能を強化し、
* 最新のアップデートでは、Substanceを使用する際の3ds Max 2024のレンダリング速度とCPU使用率が大幅に改善され、パフォーマンスが3ds Max 2022で観察される効率により近いものになります。

<b>修正済み：</b>

* Substanceプラグインが強化され、各パラメーターの実用的な範囲内にキーボード入力の値が制限されるようになりました。これにより、スライダーコントロールや手動での値の調整に関する問題が回避されます。
* スレートマテリアルエディタ内でSubstance2テクスチャ変換(.sbsar)をコピーすると、コピーされたノードが意図しないインスタンス化され、d3d11.dllに関連するクラッシュが発生する可能性がある問題を解決しました
* Corona Interactiveを使用してカスタマイズ/編集されたコピーされたマテリアル物質(.sbsar)をレンダリングする際に、3ds Maxがクラッシュする問題を解決しました。
* 3ds MaxのSubstance 2ノードで、整数3と4の値のスライダが応答せず、手動の数値入力のみが値を更新する問題を修正しました。 また、これらの値がfloat形式で正しく表示されませんでした。 スライダーが機能するようになり、意図する値の種類が正確に反映されるようになりました。
* 3ds Max 2021のCorona Renderで、Substanceマテリアルがビューポートに正しく表示されていましたが、ファイルが別のPCに転送されたときにグレーでレンダリングされる問題を修正しました。 マテリアルをゼロから設定したり、適切にレンダリングするためにプリセットを読み込む必要がなくなりました。
* スレートマテリアルエディタでSubstanceノードを複製しようとすると、3ds Maxプラグインがクラッシュする問題を解決しました。
* 3ds Maxの再起動後に、SubstanceプラグインのCPUコア制限設定が保存されない問題を解決しました。これにより、ユーザ設定の値がセッション間で維持されるようになりました。

このバージョンは3ds Max 2021、2022、および2023用にリリースされています
