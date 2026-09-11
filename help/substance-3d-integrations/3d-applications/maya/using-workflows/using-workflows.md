---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/using-workflows.html"
breadcrumb-title: ''
description: MayaのSubstance出力用のレンダープリセットを作成して使用し、各種レンダラー用のシェーダーネットワークを自動生成します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Using Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ワークフローの使用
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---


# ワークフローの使用

「ワークフロー」では、Substance出力のレンダリングプリセットを選択または作成できます。 これらのプリセットは、ArnoldやVrayなどのレンダラーのシェーダーネットワークです。

>[!NOTE]
>
> **ワークフロープリセットの場所**
> 
> **Windows**:\
> C:\Users\\Documents\maya\2022\substance\workflows\generated\
> **MacOS**:\
> /Users//Library/Preferences/Autodesk/maya//substance/workflows/generated\
> **Linux**:\
> /home//maya//substance/workflows/generated

![](../../../assets/workflows-4.png)

ワークフローを使用するには、ドロップダウンリストからプリセットを選択し、「 シェーダーネットワークを作成」ボタンをクリックします。

![](../../../assets/workflow.gif)

## ワークフローの作成

独自のワークフローを作成して、[レンダラーのワークフロー]リストに追加できます。 新しいワークフローを追加すると、Substanceノードの後に作成されたノードがワークフローに保存されます。 これにより、任意の数のシェーディングノードを作成して、プリセットワークフローとして保存できる完全なカスタムシェーダーネットワークを構築できます。

## ![](../../../assets/saved-workflow.png)ワークフローの管理

### カスタムワークフローの保存

1. Substance出力を手動で作成し、aiStandardSurfaceなどのマテリアルに接続します。
   1. 任意のMayaノードまたはレンダー固有のノードを使用して、シェーダーネットワークを構築できます。
1. 「**ワークフローを作成**」ボタンをクリックして、ワークフロープリセットの名前を入力します。

### ワークフローの複製

「**ワークフローの複製**」ボタンをクリックすると、ワークフローを複製できます。

### ワークフローの名前の変更と上書き

選択した&#x200B;**名前の変更**&#x200B;および&#x200B;**上書き**&#x200B;ボタンを使用して、既存のワークフローの名前を変更したり、更新されたデータでワークフローを上書きしたりできます。

### ワークフローの削除

既存のワークフローを削除するには、「ワークフローを削除」ボタンを使用します。
