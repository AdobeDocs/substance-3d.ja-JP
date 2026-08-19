---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/features/tangent-space.html"
breadcrumb-title: ''
description: Substance Bakersでの接線空間計算の処理方法と、ワークフローのアルゴリズムのカスタマイズ方法について説明します。
helpx_creative_field: ""
helpx_description: bakers > Features > Tangent Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: タンジェントスペース
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 2%

---


# タンジェントスペース

Substance Bakersは、ローポリメッシュに存在する正接とバイノーマルをロードするか、それらを再計算できます。 それらを再計算すると、カスタムの接線空間アルゴリズムを定義することができます（デフォルトではMikkTSpaceです）。

## 接線空間プラグインリスト

## Substance Painter

Substance Painterでは、接線空間プラグインを変更できません。常に&#x200B;**MikkTSpace**&#x200B;になります。 ただし、他のアプリケーションと互換性を持たせるために、動作を少し変更するパラメーターがあります。

| *パラメーター* | *互換性* *アプリケーション* |
| --- | --- |
| **フラグメントごとの接線空間の計算：無効** | xNormal、Unity 5.3以降と互換性があります。 |
| **フラグメントごとの接線空間の計算：有効** | Unreal Engine 4、Blender、Unity HDRP ワークフローに対応。 |

## Substance Designer

Substance Designerは次のアルゴリズムをサポートしています。

| *ファイル名* | *説明* |
| --- | --- |
| **mikktspace.dll** | Morten S. Mikkelsenの研究に基づいた接線空間アルゴリズムであるMikkTSpaceの研究。xNormal、Unity 5.3以降と互換性があります。 |
| **mikkunrealtspace.dll** | Morten S. Mikkelsenの研究に基づいた接線空間アルゴリズムであるMikkTSpaceの研究。Unreal Engine 4、Blender、Unity HDRP ワークフローに対応。 |
| **unitytspace.dll** | Unity 4に基づく接線空間アルゴリズム。 |

>[!NOTE]
>
> カスタムの接線空間プラグインを記述することができます。 **tangentspaceplugin.h**&#x200B;という名前のヘッダーファイルは、**Substance Designer/SDK/tangentspace**&#x200B;の下のインストールフォルダーで利用でき、インターフェイスとして使用できます。

## カスタム接線空間の設定

## Substance Painter

Substance Painterは、現時点ではカスタムタンジェントスペースプラグインをサポートしていません。 つまり、接線とバイノーマルが（プロジェクトの作成に使用される）ローポリメッシュに存在しない場合、それらはMikkTSpace アルゴリズムに基づいて再計算されます。

## Substance Designer

Substance Designerで接線空間アルゴリズムを設定するには、次の手順に従います。

1. **編集** / **環境設定**&#x200B;を選択します。

   ![](../../assets/sd-edit-pref.png)
1. **プロジェクト**&#x200B;をクリックします。

   ![](../../assets/sd-pref-projects.png)
1. 「**一般**」タブに移動します。 セクション **3D シーン**&#x200B;が表示されるまでスクロールします。

   ![](../../assets/sd-tab-general.png)
1. **3つのドット**&#x200B;をクリックします（。..） カスタム プラグインをロードします。

## Substance Automation Toolkit

Automation Toolkitを使用してベイク処理する場合、特定のコマンドライン引数でTangent Space プラグインを指定できます。

```
sbsbaker normal-from-mesh --tangent-space-plugin "C:/Substance Designer/plugins⁄tangentspace⁄mikktspace.dll" ...
```
