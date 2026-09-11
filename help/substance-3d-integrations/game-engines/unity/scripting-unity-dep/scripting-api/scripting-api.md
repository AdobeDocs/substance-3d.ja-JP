---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/scripting-api.html"
breadcrumb-title: ''
description: 旧式のプロジェクトのサポートに関する、非推奨のSubstance UnityスクリプティングAPIのリファレンスドキュメント。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: スクリプトAPI
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 1%

---


# スクリプトAPI

## Unity APIのSubstance- 2.2.0

## マテリアルパラメーター

| Publicメソッド | 説明 | パラメーター |
| --- | --- | --- |
| パブリック&#x200B;**float** *GetInputFloat*（**文字列** inputName） | Substance **浮動小数**&#x200B;の入力を取得 | **文字列** *inputName* SBSARの入力の名前 |
| パブリック&#x200B;**int** *SetInputFloat*（**文字列**&#x200B;入力名、**浮動小数点**&#x200B;値） | Substance **浮動小数**&#x200B;の入力を更新 | **文字列** i *nputName* SBSARの入力の名前&#x200B;**浮動小数** *値*&#x200B;パラメーターの更新に使用される値 |
| パブリック&#x200B;**void** *SetInputVector2*（**文字列** inputName、**ベクトル2**&#x200B;値） | Substance **Vector2**&#x200B;の入力を更新 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Vector2** *input*&#x200B;パラメーターの更新に使用される値 |
| パブリック&#x200B;**vector2** *GetInputVector2*（**文字列** inputName） | Substance **Vector2**&#x200B;の入力を取得 | **文字列** SBSARの入力の「inputName」名 |
| パブリック&#x200B;**void** *SetInputVector3*（**文字列** inputName、**ベクトル3**&#x200B;値） | Substance **Vector3**&#x200B;の入力を更新 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Vector3** *値*&#x200B;パラメーターの更新に使用される値 |
| パブリック&#x200B;**vector3** *GetInputVector3*（**文字列** inputName） | Substance **Vector3**&#x200B;の入力を取得 | **文字列** *inputName* SBSARの入力の名前 |
| パブリック&#x200B;**void** *SetInputVector4*（**文字列** inputName、**ベクトル4**&#x200B;値） | Substance **Vector4**&#x200B;の入力を更新 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Vector4** *値*&#x200B;パラメーターの更新に使用される値 |
| パブリック&#x200B;**vector4** *GetInputVector4*（**文字列** inputName） | Substance **Vector4**&#x200B;の入力を取得 | **文字列** SBSARの入力の名前です。 |
| パブリック&#x200B;**void** *SetInputColor*（**文字列**&#x200B;入力名、**色**&#x200B;値） | Substance **色**&#x200B;の入力を更新 | **文字列** inputNameパラメーターの更新に使用されたSBSAR **Color**&#x200B;値の入力の名前 |
| パブリック&#x200B;**color** *GetInputColor*（**文字列** inputName、**int** dataType） | Substance **色**&#x200B;を取得 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Int** *dataType* |
| パブリック&#x200B;**void** *SetInputBool*（**文字列** inputName、**bool**&#x200B;値） | Substance **ブーリアン**&#x200B;の入力を更新 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Bool** *値*&#x200B;パラメーターの更新に使用される値 |
| パブリック&#x200B;**bool** *GetInputBool*（**文字列** inputName） | Substance **ブーリアン**&#x200B;の入力を取得 | **文字列** *inputName* SBSARの入力の名前 |
| パブリック&#x200B;**void** *SetInputInt*（**文字列**&#x200B;入力名、**int**&#x200B;値） | Substance **Int**&#x200B;入力の更新 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Int** *値*&#x200B;パラメーターの更新に使用される値 |
| パブリック&#x200B;**int** *GetInputInt*（**文字列** inputName） | Substance **Int**&#x200B;入力を取得 | **文字列** *inputName* SBSARの入力の名前 |
| パブリック&#x200B;**void** *SetInputVector2Int*（**文字列**&#x200B;入力Name, **int** x, **int** y） | Substance **Vector2Int**&#x200B;入力を更新 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Int** *x*&#x200B;パラメーターの更新に使用された値&#x200B;**Int** yパラメーターの更新に使用された値 |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector2Int*（文字列inputName） | 2intの配列（Vector2Intのxおよびy値）を取得します。 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Int** *x*&#x200B;パラメーターの更新に使用された値&#x200B;**Int** yパラメーターの更新に使用された値 |
| **void Substance.Game.SubstanceGraph**.*SetInputVector3Int*( string inputName, int x, int y, int z) | SubstanceのVector3Int入力を更新 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Int** *x*&#x200B;パラメーターの更新に使用される値&#x200B;**Int** yパラメーターの更新に使用される値&#x200B;**Int** zパラメーターの更新に使用される値 |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector3Int*（文字列inputName） | 3 intの配列（Vector3Intのx、y、z値）を取得します。 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Int** *x*&#x200B;パラメーターの更新に使用される値&#x200B;**Int** yパラメーターの更新に使用される値&#x200B;**Int** zパラメーターの更新に使用される値 |
| **void Substance.Game.SubstanceGraph**.*SetInputVector4Int*( string inputName, int x, int y, int z, int w) | SubstanceのVector4Int入力を更新 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Int** *x*&#x200B;パラメーターの更新に使用される値&#x200B;**Int** yパラメーターの更新に使用される値&#x200B;**Int** zパラメーターの更新に使用される値&#x200B;**Int** wパラメーターの更新に使用される値 |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector4Int*（文字列inputName） | 4intの配列（Vector4Intのx、y、z、w値）を取得します。 | **文字列** *inputName* SBSARの入力の名前&#x200B;**Int** *x*&#x200B;パラメーターの更新に使用される値&#x200B;**Int** yパラメーターの更新に使用される値&#x200B;**Int** zパラメーターの更新に使用される値&#x200B;**Int** wパラメーターの更新に使用される値 |
| **void Substance.Game.SubstanceGraph**.*SetInputString*（文字列inputName、文字列値） | Substance文字列入力の更新 | **文字列** *inputName*&#x200B;パラメーターの更新に使用されたSBSAR **文字列** *値*&#x200B;の入力の名前 |
| **文字列Substance.Game.SubstanceGraph**.*GetInputString*( string inputName) | Substance文字列入力を取得する | **文字列** *inputName* SBSARの入力の名前 |
| **void Substance.Game.SubstanceGraph**.*SetInputTexture*（文字列inputName、Texture2D値） | Substanceテクスチャ2D入力を更新 | **文字列** *inputName*&#x200B;パラメーターの更新に使用されたSBSAR **テクスチャ2D** *値*&#x200B;の入力名 |
| **テクスチャ2D Substance.Game.SubstanceGraph**.*GetInputTexture*（文字列inputName） | テクスチャ 2D入力を取得 | **文字列** *inputName* SBSARの入力の名前 |
| **VectorInt Substance.Game.SubstanceGraph**.*GetTexturesResolution*() | グラフのターゲット設定テクスチャの解像度を取得します（Vector4Intのx =幅、y =Height、値は32、64、128、256、512、1024、2048、4096です）。 | なし |
| **int Substance.Game.SubstanceGraph**.*SetTexturesResolution*（ Vector2Intサイズ） | グラフのTarget Settingsを設定します。テクスチャの解像度（Vector2Intのx =幅、y =Height、値は32、64、128、256、512、1024、2048、および4096）成功した場合は0を返します。それ以外の場合は–1を返します。 | **Vector2Int** *size*&#x200B;がパラメーターの更新に使用されました**.** |
| **Substance.ゲーム.SubstanceGraph**.*GetGeneratedTextures*() | グラフのマテリアルシェーダーで使用されるすべてのSubstanceテクスチャ2Dオブジェクトを返します。 | なし |
| **int Substance.Game.SubstanceGraph**.*烘焙*（ テクスチャ 2D テクスチャ、文字列absolutePath） | グラフのマテリアルシェーダーで使用されるすべてのSubstanceテクスチャ2Dオブジェクトに対して.pngファイルを生成します。 | なし |
| **** Substance.ゲーム。** SubstanceGraph**.*複製*() | Substance グラフの複製 | なし |
| **Substance.ゲーム.SubstanceGraph**.*複製*（文字列newGraphName） | Substance グラフを複製し、名前を付けます（対応するマテリアルも同じ名前になります）。 | **String newGraphName** |
| **** Substance.ゲーム。** SubstanceGraph**.*GetInputProperties*() | プロシージャル入力情報を照会し、&#39;InputProperties&#39;の配列を返します。:public構造体を持ちます。 InputProperties {public string name; // inputNameパブリック文字列ラベル； // GUIパブリック文字列グループのウィジェットのラベル； // GUIpublic string[] componentLabels; //スライダのグループ（最大4ラベル） public string[] enumOptions; // optionMenupublic InputPropertiesType;public Vector4最大； //スライダpublic float step; //スライダenum InputPropertiesType { ブーリアン = 0,// 0浮動小数, // 1ベクトル2, // 2ベクトル3, // 3ベクトル4, // 4カラー， // 5 Enum, // 6テクスチャ, // 7文字列， // 8無効= -1// -1 }; | なし |
| **bool** **Substance.ゲーム.SubstanceGraph**.*HasInput*（**文字列** inputName） | グラフに入力が存在するかどうかを確認し、true/falseを返します。 | **文字列** *inputName* SBSARの入力の名前 |
| **bool** **Substance.ゲーム.SubstanceGraph**.*IsInputVisible*（**文字列** inputName） | 表示されている入力が表示されているかどうかを確認し、true/falseを返します。 | **文字列** *inputName* SBSARの入力の名前 |

## レンダリング中

| Publicメソッド | 説明 | パラメーター |
| --- | --- | --- |
| パブリック&#x200B;**void** *QueueForRender*() | グラフをキューに追加 | なし |
| ***mySubstance.**RenderAsync()* | キューに登録されているすべてのグラフを非同期でレンダリングする | なし |
| ***mySubstance.**RenderSync()* | キューに登録されているすべてのグラフを同期的にレンダリング | なし |

## エディターモードでのスクリプト：

エディターモードでグラフの変更を永続的にするには、対応する各Substanceを再読み込みする必要があります。 これは、次の関数で実行されます。

```
static void ReImportSubstance(Substance.Game.Substance pSubstance)

{



// Re-import Substance object:

SubstanceImporter importer = AssetImporter.GetAtPath(pSubstance.assetPath) as SubstanceImporter;

importer.CommitSubstanceToImporter(pSubstance); // plugin function

EditorUtility.SetDirty(importer);

importer.SaveAndReimport();



}
```


（「CommitSubstanceToImporter」を使用すると、Substanceプラグイン関数により、変更されたすべてのグラフパラメーターおよび/または入力がSubstanceインポーターオブジェクトにコピーされ、Unityのインポーターメカニズムを介してディスクにシリアル化されます）
