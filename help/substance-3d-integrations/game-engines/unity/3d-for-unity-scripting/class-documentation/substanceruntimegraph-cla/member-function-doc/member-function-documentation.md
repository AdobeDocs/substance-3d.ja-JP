---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class/member-function-documentation.html"
breadcrumb-title: ''
description: UnityスクリプティングのSubstanceRuntimeGraphクラスのすべてのメンバー関数に関する詳細なドキュメント。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class > Member Function Documentation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: メンバー関数のドキュメント
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 2%

---


# メンバー関数のドキュメント

## AttachGraph()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.AttachGraph  

( SubstanceGraphSO graph ) [inline]
```


このランタイムハンドラに新しいグラフオブジェクトをアタッチします。

**パラメーター**

|  |  |
| --- | --- |
| グラフ | ターゲット物質グラフ。 |

### CreatePresetFromCurrentState()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.CreatePresetFromCurrentState ( ) [inline]
```


現在のグラフ状態をプリセットXMLに保存します。

**戻り値**

グラフ入力の現在の状態を使用して作成されたプリセット。

### GetGeneratedTextures()

```
List< Texture2D > Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetGeneratedTextures ( ) [inline]
```


Substanceインスタンスのすべての出力テクスチャを含むリストを返します。

**戻り値**

出力テクスチャ。

### GetInputBool()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputBool ( string inputName ) [inline]
```


Substanceのブール値入力を取得します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前。 |


**戻り値**

現在の入力値。

### GetInputColor()

```
Color Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputColor ( string inputName ) [inline]
```


Substanceカラーを取得

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の入力値。

### GetInputDescription()

```
SubstanceInputDescription Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputDescription ( string inputName ) [inline]
```


ターゲット入力名の完全な入力説明を返します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | ターゲットの入力名。 |


**戻り値**

ターゲット入力の完全な入力説明。

### GetInputFloat()

```
float Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputFloat ( string inputName ) [inline]
```


Substance浮動小数点値を取得する

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の入力値。

### GetInputInt()

```
int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputInt ( string inputName ) [inline]
```


Substanceの整数入力を取得

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の入力値。

### GetInputString()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputString ( string inputName ) [inline]
```


Substance文字列の入力を取得します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の値を入力します。

### GetInputVector2()

```
Vector2 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2 ( string inputName ) [inline]
```


Substanceベクトル2入力を取得

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の入力値。

### GetInputVector2Int()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2Int ( string inputName ) [inline]
```


2 intの配列を取得します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の入力値。

### GetInputVector3()

```
Vector3 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3 ( string inputName ) [inline]
```


Substance Vector3入力を取得します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の入力値。

### GetInputVector3Int()

```
Vector3Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3Int ( string inputName ) [inline]
```


3 intの配列（Vector3Intのx、y、z値）を取得します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の入力値。

### GetInputVector4()

```
Vector4 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4 ( string inputName ) [inline]
```


Substanceベクトル4入力を取得

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の入力値。

### GetInputVector4Int()

```
int[] Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4Int ( string inputName ) [inline]
```


4intの配列（Vector4Intのx、y、z、w値）を取得します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |


**戻り値**

現在の入力値。

### GetOutputTexture()

```
Texture2D Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetOutputTexture ( string outputName ) [inline]
```


指定された出力名の出力テクスチャを返します。

**パラメーター**

|  |  |
| --- | --- |
| outputName | 出力名。 |


**戻り値**

出力テクスチャ。

### GetTexturesResolution()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetTexturesResolution ( ) [inline]
```


インスタンステクスチャの出力解像度を返します。

**戻り値**

現在の出力解像度。

### HasInput()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.HasInput ( string inputName ) [inline]
```


このsubstanceインスタンスに指定された名前の入力がある場合はtrueを返します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | 名前を入力します。 |


**戻り値**

Substanceインスタンスに指定された名前の入力がある場合はTRUE。

### LoadPreset()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.LoadPreset ( string presetXML ) [inline]
```


プリセットXMLを使用して入力パラメーターを設定します。

**パラメーター**

|  |  |
| --- | --- |
| presetXML | プリセットXMLデータ。 |

### RenderAsync()

```
Task Adobe.Substance.Runtime.SubstanceRuntimeGraph.RenderAsync ( ) [inline]
```


Substanceインスタンスを非同期でレンダリングします。

**戻り値**

レンダリングが完了すると終了するタスク。

### SetInputBool()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputBool ( string inputName, 

bool value ) [inline]
```


Substanceのブール値入力を更新

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputColor()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputColor ( string inputName, 

Color value ) [inline]
```


Substanceカラー入力を更新

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputFloat()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputFloat ( string inputName, 

float value ) [inline]
```


Substance浮動小数点入力を更新

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputInt()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputInt ( string inputName, 

int value ) [inline]
```


Substanceの整数入力を更新

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputString()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputString ( string inputName, 

string value ) [inline]
```


Substance文字列入力を更新します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputTexture()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputTexture (string inputName, 

Texture2D value ) [inline]
```


Substanceテクスチャ2D入力を更新します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputVector2()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2 ( string inputName, 

Vector2 value ) [inline]
```


Substanceベクトル2入力を更新

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputVector2Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2Int ( string inputName, 

Vector2Int value ) [inline]
```


Substance Vector2Int入力を更新します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputVector3()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3 ( string inputName, 

Vector3 value ) [inline]
```


Substanceベクトル3入力を更新

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputVector3Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3Int ( string inputName, 

Vector3Int value ) [inline]
```


Substance Vector3Int入力を更新します。

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputVector4()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4 ( string inputName, 

Vector4 value ) [inline]
```


Substanceベクトル4入力を更新

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| 値 | パラメーターの更新に使用する値 |

### SetInputVector4Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4Int ( string inputName, 

int x, 

int y, 

int z, 

int w ) [inline]
```


SubstanceのVector4Int入力を更新

**パラメーター**

|  |  |
| --- | --- |
| inputName | SBSARの入力の名前 |
| X | パラメーターの更新に使用する値 |
| y | パラメーターの更新に使用する値 |
| Z | パラメーターの更新に使用する値 |
| w | パラメーターの更新に使用する値 |

### SetTexturesResolution()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetTexturesResolution ( Vector2Int size ) [inline]
```


インスタンステクスチャ出力解像度を設定します。

**パラメーター**

|  |  |
| --- | --- |
| サイズ |  |
