---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/features/gpu-raytracing.html"
breadcrumb-title: ''
description: ハードウェアアクセラレーションによるGPU レイトレーシングを有効にして、ベイク処理の計算を25倍以上高速化し、ワークフローを高速化できます。
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

一部のベイカーは、GPU上でのレイトレーシングのハードウェアアクセラレーションをサポートしています。通常、計算速度は25倍以上に向上します。

## 必要ハードウェア構成

システムが次の要件に従う場合、レイトレーシングは自動的に有効になります。

* 互換性のあるGPUがインストールされている\*（RTX シリーズ、Titan VまたはGeForce 10xx）
* GPU ドライバーは最新です
* Windows 10 &#39;Fall Creator&#39; / 10月のアップデート（ver 1809）以降がインストールされている\*\*

</td>
<td style="border: 0;" valign="top">

![GPU レイトレーシング オン/オフ比較](../../assets/rtx-ao-demo.gif "GPU レイトレーシング オン/オフ比較"){zoomable="yes"}

</td>
</tr>
</table>

\*：互換性のあるNVIDIA GPUには、Pascal アーキテクチャを使用するすべてのGPUが含まれています。 GTX 10 シリーズ、Titan V シリーズ、RTX 20 シリーズ、またはそれ以上の最近のバージョン。

\*\*: Windowsのバージョンを確認するには、「スタート」メニューをクリックし、「winver」と入力してEnter キーを押します。\
このアップデートは、Microsoft サポート web サイトの[専用ページ &#x200B;](https://support.microsoft.com/en-us/help/4028685/windows-10-get-the-update)から入手できます。

>[!TIP]
>
> 問題が発生した場合は、アプリケーションの環境設定でGPU レイトレーシングを無効にすることができます。

## サポートされているベイカー

以下の表は、Substance 3D ベーカーバージョンに従って、すべてのベイカーのGPU レイトレーシングのサポートを示しています。

+++バージョン 3以降

| ベイカー | GPU レイトレーシングをサポート |
| --- | --- |
| アンビエントオクルージョン | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| ベント法線 | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Color | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| 曲率 | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| 高さ | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| 法線 | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| 法線ワールド空間 | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |



| ベイカー | GPU レイトレーシングをサポート |
| --- | --- |
| 不透明マスク | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| 位置 | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| 位置 : 低 | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| 厚み | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| 転送されたテクスチャ | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| ワールドから接線 | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |


+++

+++バージョン 2

| ベイカー | GPU レイトレーシングをサポート |
| --- | --- |
| アンビエントオクルージョン | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| メッシュからのアンビエントオクルージョン | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| メッシュからのベント法線 | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| メッシュからのカラー | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| UV を SVG に変換 | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| メッシュからの曲率 | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| メッシュからの高さ | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| メッシュからの法線 | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |



| ベイカー | GPU レイトレーシングをサポート |
| --- | --- |
| メッシュからの不透明度マスク | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| メッシュからの位置 | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| 位置 | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| メッシュからの厚み | <div><img alt="（ティック）&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| メッシュからの転送されるテクスチャ | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| ワールド空間方向 | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| ワールド空間法線 | <div><img alt="（エラー）&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |


\*: GPU レイトレーシングよりも大幅に遅いCPU レイトレーシングをサポートします。

+++
