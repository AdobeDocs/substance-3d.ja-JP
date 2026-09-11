---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-bake/features/tangent-space.html"
breadcrumb-title: ''
description: Substance Bakersで正接容量の計算を行い、アルゴリズムをカスタマイズする方法について説明します。
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

Substance Bakersは、ローポリメッシュに存在する正接と従法線を読み込むか、再計算することができます。 再計算時には、カスタム接線空間アルゴリズムを定義することができます（デフォルトではMikkTSpaceです）。

## 接線空間プラグインリスト

## Substance Painter

Substance Painterでは、接線空間プラグインは変更できません。常に&#x200B;**MikkTSpace**&#x200B;になります。 ただし、他のアプリケーションとの互換性を確保するために、動作を若干変更するパラメーターがあります。

| *パラメーター* | *互換性のある* *アプリケーション* |
| --- | --- |
| **フラグメントごとのコンピューティング正接領域：無効** | xNormal、Unity 5.3以降と互換性があります。 |
| **フラグメントごとの計算正接領域：有効** | Unreal エンジン 4、Blender、Unity HDRPワークフローと互換性があります。 |

## Substance Designer

Substance Designerでは、次のアルゴリズムがサポートされています。

| *ファイル名* | *説明* |
| --- | --- |
| **mikktspace.dll** | MikkTSpace、Morten S. Mikkelsenの作業に基づいた接線空間アルゴリズム。xNormal、Unity 5.3以降と互換性があります。 |
| **mikkunrealtspace.dll** | MikkTSpace、Morten S. Mikkelsenの作業に基づいた接線空間アルゴリズム。Unreal エンジン 4、Blender、Unity HDRPワークフローと互換性があります。 |
| **unitytspace.dll** | Unity 4に基づく接線空間アルゴリズム。 |

>[!NOTE]
>
> カスタム接線空間プラグインを書き込むことができます。 **tangentspaceplugin.h**&#x200B;という名前のヘッダーファイルは、**Substance Designer/SDK/tangentspace**&#x200B;の下のインストールフォルダーで利用でき、インターフェイスとして使用できます。

## カスタム接線空間の設定

## Substance Painter

Substance Painterは現在、カスタム接線空間プラグインをサポートしていません。 つまり、正接と従法線が（プロジェクトを作成するために使用される）ローポリメッシュに存在しない場合、MikkTSpaceアルゴリズムに基づいて再計算されます。

## Substance Designer

Substance Designerに正接空間アルゴリズムを設定するには、次の手順に従います。

1. **編集**/**環境設定**&#x200B;を選択します。

   ![](../../assets/sd-edit-pref.png)
1. **プロジェクト**&#x200B;をクリックします。

   ![](../../assets/sd-pref-projects.png)
1. 「**一般**」タブに移動します。 セクション&#x200B;**3D シーン**&#x200B;が表示されるまでスクロールします。

   ![](../../assets/sd-tab-general.png)
1. **3つのドット** (...)をクリックします カスタムプラグインを読み込みます。

## Substance自動処理ツールキット

Automation Toolkitを使用してベイクする場合は、コマンドライン引数で接線空間プラグインを指定できます。

```
sbsbaker normal-from-mesh --tangent-space-plugin "C:/Substance Designer/plugins⁄tangentspace⁄mikktspace.dll" ...
```
