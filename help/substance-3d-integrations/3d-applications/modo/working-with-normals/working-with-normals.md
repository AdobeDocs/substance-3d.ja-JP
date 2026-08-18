---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/modo/working-with-normals.html"
breadcrumb-title: ''
description: MODOで法線マップの向きを設定し、Substanceマテリアルを使用して法線マップを正しくレンダリングできるようにします。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Normals
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 法線の操作
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---


# 法線の操作

法線データを使用する – 正しい方向を設定する

ストックSubstanceは、DX法線方向を使用するように作成されています。 ただし、MODOはOGLを使用します。 法線を反転するには、[法線の形式]パラメータを1.0に設定します。 Substanceプラグインは、Substanceで設定されたパラメーターのみを解釈します。 このコントロールをカスタムSubstanceに追加するのはSubstanceの作成者の責任であるため、「normal\_format」パラメーターを持たないSubstanceが発生する可能性があります。 このパラメータを持たないSubstanceが発生した場合は、法線マップのテクスチャレイヤの緑チャンネルをフリップして方向を固定できます。

>[!NOTE]
>
> グリーンチャンネルを反転するのは、Substanceの法線の向きが正しくなく、作成者がSubstanceパラメーターで法線を反転させるコントロールを作成しなかった場合のみです

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/normal-1.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/invert-2.png)

</td>
</tr>
</table>
