---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity.html"
breadcrumb-title: ''
description: ネイティブプラグインのサポートとランタイムパラメータコントロールにより、UnityゲームエンジンでSubstanceマテリアルを読み込んで使用できます。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---


# Unity

![](../../assets/unity.png)

>[!NOTE]
>
> **Unityがサポートするバージョン**
> 
> Unityバージョン3.0.0用のAdobe Substance 3Dプラグインは、現在Unity 2020.3.27x以降をサポートしています。 [Unityアセットストア](https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208)からダウンロードできます。

>[!WARNING]
>
> プラグインをアップグレードまたは使用する前に、[プロジェクトのアップグレードページ](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html)を確認してください。

>[!WARNING]
>
> カスタムのSubstance資料を作成する前に、[最適化のガイドライン](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md)のページを確認してください。

## 目次

* [Unityリリースノート](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) – バージョン別のUnityプラグインのSubstanceの新機能
* [UnityでSubstance 3Dプラグインをダウンロードする](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) — Unity用Substance 3D Adobeは、Unity Asset Store https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555で入手できます。
* [Unityプラグインの概要](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Unityの環境設定](../../game-engines/unity/unity-preferences/unity-preferences.md) – プラグインの環境設定ウィンドウでは、Substanceのユーザー定義オプションを設定できます。
* [最適化のガイドライン](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) – 独自のカスタムSubstanceマテリアルを作成する場合は、次の最適化のガイドラインを確認してください。
* [プロジェクトのアップグレード/既知の問題](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — UnityプラグインのSubstanceに関する既知の問題
* [Substance グラフの管理](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) — Substance グラフマネージャー(SGM)を使用して、Substanceのマテリアルに基づいて新しいマテリアルを作成できます
* [パラメーターの変更](../../game-engines/unity/changing-parameters/changing-parameters.md) — マテリアルのパラメーターは、Substance グラフオブジェクト(SGO)でアクセスできます。
* [生成されたテクスチャ (パッキング)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) – 生成されたテクスチャは、Substance engineがテクスチャを作成するために計算したSubstanceからの出力を示します
* [レンダリングカラースペース](../../game-engines/unity/rendering-color-space/rendering-color-space.md) – 最良の結果を得るには、Unity Player設定でカラースペースをリニアに設定する必要があります。
* [画像入力の使用](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [モバイル用に公開](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) – モバイルプラットフォームで公開するためのガイドライン
* [Substance 3D for Unityスクリプティング](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) — Substance APIを使用して、実行時にSubstanceパラメーターを更新および変更するスクリプトを作成できます。
* [Unityでのスクリプト作成（非推奨）](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — Substance APIを使用して、実行時にSubstanceパラメーターを更新および変更するスクリプトを作成できます。
* [Substance 3D Assetsライブラリの使用](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Substanceプラグインを削除中](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [UnityTutorialsのSubstance 3D](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [統一物理サイズ](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
* [プロジェクト間でSbsarファイルを共有しています](https://helpx.adobe.com/sharing-sbsar-files-between-projects.html) [&#128279;](../../game-engines/unity/sharing-sbsar-files-bet/sharing-sbsar-files-between-projects.md)

**[フォームが見つかりました – ルールが必要です]**

>[!WARNING]
>
> プラグインをアップグレードまたは使用する前に、[プロジェクトのアップグレードページ](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html)を確認してください。

>[!WARNING]
>
> カスタムのSubstance資料を作成する前に、[最適化のガイドライン](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md)のページを確認してください。

### 目次

* [Unityリリースノート](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) – バージョン別のUnityプラグインのSubstanceの新機能
* [UnityでSubstance 3Dプラグインをダウンロードする](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) — Unity用Substance 3D Adobeは、Unity Asset Store https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555で入手できます。
* [Unityプラグインの概要](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Unityの環境設定](../../game-engines/unity/unity-preferences/unity-preferences.md) – プラグインの環境設定ウィンドウでは、Substanceのユーザー定義オプションを設定できます。
* [最適化のガイドライン](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) – 独自のカスタムSubstanceマテリアルを作成する場合は、次の最適化のガイドラインを確認してください。
* [プロジェクトのアップグレード/既知の問題](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — UnityプラグインのSubstanceに関する既知の問題
* [Substance グラフの管理](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) — Substance グラフマネージャー(SGM)を使用して、Substanceのマテリアルに基づいて新しいマテリアルを作成できます
* [パラメーターの変更](../../game-engines/unity/changing-parameters/changing-parameters.md) — マテリアルのパラメーターは、Substance グラフオブジェクト(SGO)でアクセスできます。
* [生成されたテクスチャ (パッキング)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) – 生成されたテクスチャは、Substance engineがテクスチャを作成するために計算したSubstanceからの出力を示します
* [レンダリングカラースペース](../../game-engines/unity/rendering-color-space/rendering-color-space.md) – 最良の結果を得るには、Unity Player設定でカラースペースをリニアに設定する必要があります。
* [画像入力の使用](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [モバイル用に公開](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) – モバイルプラットフォームで公開するためのガイドライン
* [Substance 3D for Unityスクリプティング](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) — Substance APIを使用して、実行時にSubstanceパラメーターを更新および変更するスクリプトを作成できます。
* [Unityでのスクリプト作成（非推奨）](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — Substance APIを使用して、実行時にSubstanceパラメーターを更新および変更するスクリプトを作成できます。
* [Substance 3D Assetsライブラリの使用](https://helpx.adobe.com/jp/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Substanceプラグインを削除中](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [UnityTutorialsのSubstance 3D](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [統一物理サイズ](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
