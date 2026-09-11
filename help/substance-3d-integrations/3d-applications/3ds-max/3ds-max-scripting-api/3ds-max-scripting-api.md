---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-scripting-api.html"
breadcrumb-title: ''
description: マテリアルオペレーションを自動化するための3ds Max SubstanceスクリプトAPIのリファレンスドキュメントです。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds MAX Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds MAXスクリプティングAPI
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 2%

---


# 3ds MAXスクリプティングAPI

次に、Substance 2ノードのコマンドとプロパティの一覧を示します。

## プロパティ：

| プロパティ | 説明 | タイプ |
| --- | --- | --- |
| 名前 | Substance2ノードの名前です。 デフォルトは「Substance 2」です | 文字列 |

## コマンド：

| コマンド | 説明 | Return | 戻り値のタイプ： | パラメーター |
| --- | --- | --- | --- | --- |
| getCurrentPackageName | ロードされたパッケージのベースファイル名を取得します（sbsar ファイルはグラフノードにロードされます） | 読み込まれたパッケージ(sbsar ファイル)のファイル名（接頭辞付きディレクトリなし） | 文字列 |  |
| getCurrentGraphName | 現在のグラフの名前を取得する | 現在のグラフインスタンスの識別子 | 文字列 |  |
| getOutputsNamesFromCurrentGraph | 有効な出力の出力使用名のリストを取得します | 有効な出力のチャンネル名のリストを含む表 | リスト |  |
| getPresetIdentities | Substanceグラフからプリセットのリストを取得 | すべてのプリセットの文字列識別子のリストを示す表 | リスト |  |
| setPackageAndGraphNames | ディスクからグラフ・ノードへのsbsar ファイルのロード | 成功の場合はTrue、失敗の場合はFalse | ブーリアン | ***文字列パラメーター***: **substancePackageFilePath** disk ***Stringパラメーター***: **graphInstanceNameToSelect** グラフの文字列識別子 |
| setInputInt | 新しい値で整数入力を設定する |  |  | ***整数パラメーター***: **値**&#x200B;入力を設定するための整数ー値&#x200B;***Stringパラメーター***: **inputIdentifier**&#x200B;入力の一意の文字列識別子 |
| setInputFloat | 新しい値を使用したfloat入力の設定 |  |  | ***浮動小数パラメーター***: **値**&#x200B;入力を設定するための浮動小数ー値&#x200B;***Stringパラメーター***: **inputIdentifier**&#x200B;入力の一意の文字列識別子 |
| setInputString | 新しい値で文字列入力を設定する |  |  | ***文字列パラメーター***: **value**&#x200B;入力を設定する文字列値&#x200B;***文字列パラメーター***: **inputIdentifier**&#x200B;入力の一意の文字列識別子 |
| setInputBool | 新しい値でブール入力を設定する |  |  | ***ブーリアンパラメーター：*&#x200B;値&#x200B;**&#x200B;入力を設定するためのブーリアン値&#x200B;***Stringパラメーター&#x200B;***: **inputIdentifier**&#x200B;入力の一意の文字列識別子 |
| setInputVec2 | 2つの要素を使用したベクトル入力の設定 |  |  | ***Point2パラメーター：**&#x200B;***value**&#x200B;入力を設定するための最大point2値&#x200B;**&#x200B;**&#x200B;**3&rbrace;inputIdentifier**&#x200B;入力の一意の文字列識別子** |
| setInputVec3 | 3つの要素によるベクトル入力の設定 |  |  | ***Point3パラメーター：*&#x200B;値&#x200B;**&#x200B;入力を設定するための最大point3値&#x200B;***Stringパラメーター&#x200B;***: **inputIdentifier**&#x200B;入力の一意の文字列識別子 |
| setInputVec4 | 4つの要素によるベクトル入力の設定 |  |  | ***Point4パラメーター***: **value**&#x200B;入力を設定するための最大point4値&#x200B;***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| setInputColor | 新しい値を使用したカラー入力の設定 |  |  | ***色パラメーター***: **値**&#x200B;入力を設定する最大色値&#x200B;***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| setInputComboSelection | コンボボックス入力の現在選択されている値を設定する |  |  | ***整数パラメーター***: **値**&#x200B;コンボボックスウィジェットのインデックス&#x200B;***文字列パラメーター***: **inputIdentifier**&#x200B;入力の一意の文字列識別子 |
| getInputInt | 整数入力タイプの入力値を取得する | 入力の現在の整数値 | 整数 | ***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| getInputFloat | float入力タイプの入力値を取得する | 入力の現在の浮動小数値 | 浮動小数 | ***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| getInputString | 文字列入力型の入力値を取得する | 入力の現在の文字列値 | 文字列 | ***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| getInputBool | ブール型の入力タイプの入力値を取得する | 入力の現在のブール値 | ブーリアン | ***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| getInputVec2 | point2入力タイプの入力値を取得する | 入力の現在の最大ポイント2値 | Point2 | ***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| getInputVec3 | point3入力タイプの入力値を取得する | 入力の現在の最大ポイント3値 | Point3 | ***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| getInputVec4 | point4入力タイプの入力値を取得する | 入力の現在の最大ポイント4値 | Point4 | ***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| getInputColor | カラー入力タイプの入力値を取得する | 入力の現在のカラー値 | Color | ***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| getInputComboSelection | 識別子に基づいてコンボボックスの選択範囲のインデックスを取得します | 選択したコンボボックス項目のインデックス | 整数 | ***文字列パラメーター：* inputIdentifier &#x200B;** 入力の一意の文字列識別子 |
| getMaterialDependentCount | マテリアルの依存性の数を取得する | マテリアルタイプの依存リファレンスの数 | 整数 |  |
| ApplyValuesToSelectedPreset | 現在選択されているプリセットを現在の入力値で上書きします |  |  |  |
| RemoveAllPresets | 現在のグラフノードのすべてのプリセットを削除 |  |  |  |
| CreatePreset | 現在の入力値から新しいプリセットを作成 |  |  | ***文字列パラメーター：*&#x200B;新しいプリセット名&#x200B;**&#x200B;新しいプリセットの表示名 |
| RemoveOnePreset | 指定された名前のプリセットを削除 |  |  | ***文字列パラメーター：* selectedPresetName &#x200B;** 削除するプリセットの名前 |
| ImportPreset | sbsprsファイルを現在のプリセットに読み込みます |  |  | ***Stringパラメーター：**&#x200B;***filePath**&#x200B;プリセットの読み込み元のファイルパスを含む文字列 |
| ExportPreset&#x200B;**\*非推奨** 2.5.0\*で削除 | 現在選択されているプリセットをsbsprsファイルに書き出し |  |  | ***文字列パラメーター***: **filePath**&#x200B;プリセットをエクスポートするファイルパスを含む文字列 |
| exportPresetList | 与えられたプリセットを1つのプリセットファイルに書き出し |  |  | ***文字列パラメーター***: **filePath**&#x200B;プリセットを書き出すファイルパスを含む文字列&#x200B;***Listパラメーター***: **プリセット**&#x200B;書き出すプリセットの名前を含むリスト |
| BakeOutputsOfSelectedGraph | 選択したグラフインスタンスのビットマップをディスクにベイク処理する |  |  | ***文字列パラメーター：* filePath &#x200B;** 画像を書き込むためのルートパスディレクトリ&#x200B;***文字列パラメーター&#x200B;***: **imageFormatExtension**&#x200B;画像を書き込むためのファイル拡張子/形式 |
