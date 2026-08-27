---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/renderers/color-management/substance-textures-in-maya.html"
breadcrumb-title: ''
description: 正確なカラーマネジメントとレンダリングを行うために、Mayaのテクスチャのカラースペース設定を行います。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management > Substance textures in Maya
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MayaのSubstanceテクスチャ
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---


# MayaのSubstanceテクスチャ

マップに対して設定するカラースペースは、[Mayaカラーマネジメント設定](https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-B260195C-A0FE-4F51-9EA2-099B61B7725A)で確立された設定とルールによって異なります。

MayaプラグインのSubstanceは、ファイルノードで「カラースペースファイルルールを無視」に設定されています。 プラグインは、次を使用して、カラーマネジメントに関係なくカラースペースの設定を処理します。

BaseColor、Diffuse、Emissive、Specular = sRGB\
標準、Height、ディスプレイスメント、ラフネス、メタリック= RAW

通常、色以外のデータを表す画像の場合は、カラースペースをRAWに設定する必要があります。 ただし、この設定はカラーマネジメントで設定した規則の影響を受ける場合があります。

![](../../../assets/raw.png)
