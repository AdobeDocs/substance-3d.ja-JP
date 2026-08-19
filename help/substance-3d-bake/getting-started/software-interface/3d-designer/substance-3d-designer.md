---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/getting-started/software-interface/substance-3d-designer.html"
breadcrumb-title: ''
description: Substance 3D Designerのベイキングウィンドウにアクセスして使用し、モデル情報をテクスチャにベイク処理する方法について説明します。
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Software Interface > Substance 3D Designer
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D Designer
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 2%

---


# Substance 3D Designer

![](../../../assets/sd-mesh-right-click.png)

ベイク処理ウィンドウには、[Explorer](https://helpx.adobe.com/substance-3d/unlisted/documentation/sddoc/the-explorer-129368147.html) ウィンドウのメッシュファイルからアクセスできます。 メッシュ名を右クリックし、「**Bake Model Information**」を選択してベイクウィンドウを開きます。

## 概要

![](../../../assets/sd-window-overview.png){width="500px"}

のベーキングウィンドウは、以下に説明する複数のパネルに分かれています。

### ベイクするエレメント

![](../../../assets/sd-mesh-selection.png)

このパネルは、ベイク処理に使用するローポリメッシュの一部を制御します。

このパネルには、ローポリメッシュ ファイル内にあるジオメトリが一覧表示されます。 デフォルトでは、リストはファイル内の個々のマテリアルに基づいていますが、必要に応じてサブメッシュに切り替えることができます。 ベイクプロセス中に無視する必要がある要素のチェックを外すことができます。

### 出力

![](../../../assets/sd-output.png)

このパネルは、ベイク処理されたテクスチャの位置を制御します。

| *パラメーター* | *説明* |
| --- | --- |
| **メソッド** | ベイクしたテクスチャをSubstance パッケージと一緒に保存する方法を制御します。使用可能な値：<ul data-preserve-html="true"><li data-preserve-html="true"><strong>埋め込み</strong>：ベイク処理されたテクスチャは、特定の名前を持つSubstance パッケージの横にあるサブフォルダーに保存されます。</li><li data-preserve-html="true"><strong> リンク済み</strong> （デフォルト）：ベイクされたテクスチャは、定義されたフォルダーに保存され、その後Substance パッケージ内で参照されます。</li></ul> |
| **フォルダー** | 保存時のベイク処理されたテクスチャの場所。 3つのドットボタンをクリックしてファイルダイアログを開き、エクスポートフォルダーを選択します。フォルダーが実際に存在するかどうかを示すチェックマークが右側に表示されます。 |
| **名前** | 焼きテクスチャの命名規則。 3つのドットボタンをクリックしてドロップダウンを開き、他のプレースホルダー（ベークネーム、カスタム、マテリアル、メッシュ）を挿入します。 |
| **サンプル** | ファイル名をシミュレートして、命名規則をテストします。 |
| **リソースをメッシュ固有のフォルダーに配置** | 有効にすると、ベイクしたテクスチャは、メッシュファイルという名前のフォルダー内に保存されます。 |

### 高精細メッシュ

![](../../../assets/sd-high.png)

このパネルは、ハイポリメッシュのリストと関連する設定を制御します。 詳しくは、[共通パラメーター](../../../bakers-settings/common-parameters/common-parameters.md)を参照してください。

### デフォルト値

![](../../../assets/sd-default-values.png)

詳しくは、[共通パラメーター](../../../bakers-settings/common-parameters/common-parameters.md)を参照してください。

### ベーカーリストと設定

![](../../../assets/sd-baker-list.png)

パン屋は、生成する焼きテクスチャを選択できる場所です。 デフォルトでは、リストは空です。

* **新しいパン屋を追加：** ボタン「パン屋を追加」をクリックします。
* **パン屋の削除：** リストからパン屋を選択し、「パン屋を削除」ボタンをクリックします。
* **パン屋を一番上に移動：** リストからパン屋を選択し、「一番上に引く」ボタンをクリックします。
* **&#x200B; パン屋を下に移動：**&#x200B;リスト内のパン屋を選択し、「押し下げる」ボタンをクリックします。

デフォルトでは、デフォルト値を継承する各ベイカー（上記を参照）。 例えば、サイズ（解像度）は、パン屋の行のセルをクリックして上書きできます。 これは、線の他の設定に当てはまります。

リスト内のベイカーをクリックすると、ベイカーのパラメータービューが特定のパラメーターで更新されます。

特定のパラメーターについて詳しくは、[&#x200B; ベイカー設定](../../../bakers-settings/bakers-settings.md)を参照してください。
