---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/gpu-raytracing.html"
breadcrumb-title: ''
description: ハードウェアアクセラレーション対応GPU レイトレーシングを有効にすると、高速なワークフローのためにベイク処理が25倍以上高速化されます。
helpx_creative_field: ""
helpx_description: bakers > Features > GPU Raytracing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU レイトレーシング
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 18%

---


# GPU レイトレーシング

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

一部のベイカーは、GPU上のレイトレーシングのハードウェアアクセラレーションをサポートしています。これにより、通常は計算速度が25倍以上に速くなります。

## ハードウェア要件

システムが次の要件に従う場合、レイトレーシングは自動的に有効になります。

* 互換性のあるGPUがインストールされています\* （RTXシリーズ、Titan VまたはGeForce 10xx）
* GPUドライバーは最新です
* Windows 10 &#39;Fall Creator&#39; / 10月のアップデート(ver 1809)以降がインストールされています\*\*

</td>
<td style="border: 0;" valign="top">

![GPU レイトレーシングオン/オフの比較](../../assets/rtx-ao-demo.gif "GPU レイトレーシングオン/オフの比較"){zoomable="yes"}

</td>
</tr>
</table>

\*：互換性のあるNVIDIA GPUには、パスカルアーキテクチャ以降を使用するすべてのGPUが含まれます。 例：GTX 10シリーズ、Titan Vシリーズ、RTX 20シリーズ以降。

\*\*: Windowsのバージョンを確認するには、[スタート]メニューをクリックし、「winver」と入力してEnterキーを押します。\
アップデートは、Microsoftサポートwebサイトの[専用ページ](https://support.microsoft.com/en-us/help/4028685/windows-10-get-the-update)から入手できます。

>[!TIP]
>
> 問題が発生した場合は、アプリケーションの環境設定でGPU レイトレーシングを無効にすることができます。

## サポート対象のベイカー

以下の表は、Substance 3Dのベイカーバージョンに従った各ベイカーのGPU レイトレーシングサポートを示しています。

+++バージョン3以降

| ベイカー | GPU レイトレーシングをサポート |
| --- | --- |
| アンビエントオクルージョン | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| ベント法線 | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| Color | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 曲率 | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 高さ | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 法線 | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 法線ワールド空間 | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> |



| ベイカー | GPU レイトレーシングをサポート |
| --- | --- |
| 不透明マスク | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 位置 | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 位置 : 低 | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| 厚み | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| 転送されたテクスチャ | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> |
| ワールドから接線 | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> |


+++

+++バージョン2

| ベイカー | GPU レイトレーシングをサポート |
| --- | --- |
| アンビエントオクルージョン | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| メッシュからのアンビエントオクルージョン | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| メッシュからのベント法線 | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| メッシュからのカラー | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| UV を SVG に変換 | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| メッシュからの曲率 | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| メッシュからの高さ | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| メッシュからの法線 | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |



| ベイカー | GPU レイトレーシングをサポート |
| --- | --- |
| メッシュから不透明マスク | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| メッシュからの位置 | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| 位置 | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| メッシュからの厚み | <div><img alt="（ティック）" data-preserve-html="true" src="../../assets/check.svg"/></div> \* |
| メッシュから転送されたテクスチャ | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> \* |
| ワールド空間の方向 | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> |
| ワールド空間法線 | <div><img alt="（エラー）" data-preserve-html="true" src="../../assets/error.svg"/></div> |


\*: CPUレイトレーシングをサポートします。これはGPU レイトレーシングよりも著しく低速です。

+++
