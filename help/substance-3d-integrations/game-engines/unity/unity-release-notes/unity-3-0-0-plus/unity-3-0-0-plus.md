---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-3-0-0-plus.html"
breadcrumb-title: ''
description: 新機能と改善点については、Unityプラグインバージョン3.0.0以降のリリースノートを確認してください。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 0%

---


# Unity 3.0.0+

## Unity 3.12.0

<b>追加/更新：</b>

* UnityでのSubstance 3D Connectorのサポート。Substance 3D SamplerとUnityの間でアセットを送信するためのSendTo機能を有効にします。
* DesignerからUnityに.sbsarグラフの名前の変更と再公開がサポートされ、更新されたグラフがUnityプラグインに再読み込みされても、Designerで行われた変更が維持されます。
* Unityプロジェクト間で.sbsarファイルを共有するためのドキュメント。
* Unityプラグインのドキュメントのコミュニティコントリビューションページ： https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/community-contributions.html.

<b>修正済み：</b>

* .sbsarファイルを再パブリッシュした後に、Unityプロジェクトアセットフォルダのマテリアルミニチュアが更新されず、現在のマテリアルではなく以前のマテリアルが表示される問題。

## Unity 3.11.0

<b>追加/更新：</b>

* 1000以上のSubstanceグラフを持つプロジェクトのパフォーマンスが向上し、アセットフォルダー内のsbsarファイルを検査するときのUIの応答時間が大幅に短縮されました。
* sbsarファイルを元の状態に戻すリセットボタンが追加され、ワークフローの効率が向上しました。
* 「8ビットにロックされたイメージ入力」問題の回避策を含むドキュメントが更新されました。この問題は、次の場所で確認できます： [UnityでのSubstance 3Dの統合 – プロジェクトのアップグレードと既知の問題](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md)。
* Unityのパネルフォルダを移動する際に発生する「式でのアサーションに失敗しました」というエラーに対処するために、ドキュメントを更新しました： [UnityのSubstance 3D統合 – プロジェクトのアップグレードと既知の問題](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md)。

<b>修正済み：</b>

* Linuxプラットフォームでプラグインが破損する問題を修正しました。
* バージョン2023のUnityプラグインの互換性の問題を修正しました。

## Unity 3.10.1

<b>修正済み：</b>

* Substance 3D for Unityプラグインのsbsario.dllの問題が原因で、Substance engineを読み込めない問題を修正しました。

## Unity 3.10.0

<b>追加/更新：</b>

* プラグインのRenderInstanceAsync APIのコメントセクションを更新しました。

<b>修正済み：</b>

* プラグインのC++コードのメモリリークの問題を修正し、オブジェクトの廃棄時に完全なメモリリカバリを保証します。
* Linuxで、Unityプラグインパッケージをインポートすると「SubstanceException: An invalid argument was gived to the API」エラーが発生する問題を修正し、SBSARファイルのインポートを正常に実行できるようになりました。
* Unityのカスタムエディターウィンドウスクリプトでプリセットを読み込むときにSubstanceGraphSO.CurrentStatePresetが正常に機能しない問題を解決しました。修正スクリプトは、アドビのSubstanceマニュアル(HelpX)ページで入手できます： https://experienceleague.adobe.com/en/docs/substance-3d/ecosystem/game-engines/unity/substance-3d-for-unity-scripting/substance-3d-for-unity-scripting
* Unityエディターでの再選択時にグラフのプロパティが消えてしまうバグを修正しました。
* UnityプラグインのSubstanceGraphSOに関連する「不明なマネージドタイプ参照」の問題が修正され、特にUnity 2022.1およびすべてのUnityバージョンのAndroidプラットフォームで互換性と機能が向上しました。
* 「技術パラメーター」セクションの「標準フォーマット」の選択肢が、DirectXおよびOpenGLオプションを含む予期されるドロップダウンリストではなく、数値入力フィールドとして誤って表示される問題を修正しました。

## Unity 3.9.0

<b>追加/更新：</b>

* Sbsarファイルをプロジェクトにドラッグ&amp;ドロップできるようになりました。 .sbsarオブジェクトは、Unity 2022.3で想定されるようにメッシュに適用できます。
* プラグインの拡張ドキュメント。

<b>修正済み：</b>

* AndroidでUnityプラグインが機能しない問題を修正しました。
* Unityプラグインの名前付け制約に対処しました。 ファイル名に「。」が含まれていると、プラグインでファイルが正しく読み込まれませんでした。
* 「すべての出力を生成」をオフにしても、余分なテクスチャが自動的に削除されない問題を修正しました。
* Unity 2021.3標準プロジェクトでのSBSARマテリアルの不適切な読み込みを修正しました。 これで、標準テンプレートプロジェクトで、SBSARマテリアルをアセットフォルダーに読み込んで、エラーなしで3Dメッシュに適用できるようになりました。
* Unity 2021/2022 HDRPプロジェクトでのSBSARマテリアルの不適切な読み込みを修正しました。 これで、HDRPテンプレートプロジェクトで、SBSARマテリアルをアセットフォルダーに読み込んで、エラーなしで3Dメッシュに適用できるようになりました。
* Androidビルドを生成してAPKを生成する際のコンパイルエラーを修正しました：「コンパイルに失敗しました。詳しくは、コンパイルエラーの出力を参照してください。」
* Windowsでビルドプロジェクトプロセスがエラーで失敗する問題を修正しました。
* AndroidでUnityEditor.BuildPlayerWindow+BuildMethodExceptionエラーが発生し、ビルドプロジェクトプロセスが失敗する問題を修正しました。
* 実行時にSubstanceGraphの入力を変更する際に発生するUnityExceptionに対処しました。 以前は、SubstanceRuntimeGraph.SetTexturesResolutionとSubstanceRuntimeGraph.Render()を呼び出すと、SubstanceGraphが誤った結果をレンダリングしていました。
* SubstanceEditorTools.csの誤字を修正しました。

## Unity 3.8.0

<b>追加/更新：</b>

* 条件付き表示（Visible If機能）のパラメーターのサポートが導入されました。
* Substanceエンジンをバージョン9にアップグレード。
* カスタムエディターウィンドウスクリプトでNativeGraph.InRenderWorkが機能しない問題に対処するために、ドキュメントを更新しました。 詳しくは、[Unityスクリプティング用Substance 3D – クラスドキュメント](../../../../game-engines/unity/3d-for-unity-scripting/class-documentation/substanceruntime-class/substanceruntime-class.md)を参照してください。

<b>修正済み：</b>

* Androidプロジェクトの通常のマップに影響する問題を解決しました。
* sbsarオブジェクトをシーンビューにドラッグすると、誤ってマウスオーバーしたすべてのオブジェクトのマテリアルがsbsarオブジェクトマテリアルでオーバーライドされるバグを修正しました。
* ランタイムモードでランタイムのみマークされたマテリアルを検査して出力テクスチャマッピングを開くとエラーが発生するバグを修正しました。

## Unity 3.7.0

<b>追加/更新：</b>

* 埋め込みプリセットと外部プリセットのサポート
* Unity 2022.2との互換性

<b>修正済み：</b>

* グラフのコピーボタンを使用してsbsarファイルの新しいグラフを作成する際にエラーが発生しました：「スクリプトクラスの予期しない再帰転送」
* プロジェクトを再度開いた後、Macで余分なマテリアルフォルダーが作成される
* グラフインスタンスの作成時/削除時にSubstanceFileSO配列が更新されない
* Substanceを複製すると、間違った入力オプションが表示される
* .sbsprsファイルの書き出しの空のラベルフィールド
* エディターでのプリセットの書き出し/読み込み中に発生するエラー： EndLayoutGroup: BeginLayoutGroupを最初に呼び出す必要があります。

<b>削除済み：</b>

* ユーザーの値が不足しているため、UnityプラグインのChannelsセクション

## Unity 3.6.0

<b>追加/更新：</b>

* 個々のInt 4値を個別に編集可能にする機能。

<b>修正済み：</b>

* プロジェクトを再度開いたときにマテリアルが以前の状態に戻る問題
* マテリアルグラフを変更しようとすると、「グラフが見つかりません」というメッセージが表示されるエラー
* 物理サイズフィーチャーの「回転オフセット」パラメータの入力値が変わらない問題
* 重複したグラフインスタンスで入力のGraphID値が正しくない問題
* エディタスクリプト（カスタムエディタウィンドウ）を使用してグラフを変更しているときに、エディタでSubstanceジェネレータが正しく初期化されない問題
* カスタムエディターウィンドウスクリプトからSubstanceGraphSO.CurrentStatePresetを書き出すと、キャッシュされたバージョンのグラフが書き出される問題
* インスペクターウィンドウがロックされているときにパラメーターの変更が保存されない問題
* 物理サイズオプションの「位置のオフセット」セクションでキーボードを手動で入力しても、エディターモードのマテリアルに影響しない問題
* SBSARオブジェクトでパラメーター値を手動で入力したときに発生したエラー

## Unity 3.5.0

<b>追加/更新：</b>

* 出力テクスチャをUnityマテリアルに割り当てる方法を変更するユーザのサポート
* 最新のUnity 2022.2バージョンとのプラグイン互換性

<b>修正済み：</b>

* マテリアルにInt4入力がある場合のNull参照エラー
* Int4入力のエラーで、W値がData3ではなくData2に割り当てられます
* 関数名「\_OcclusionStrength」に誤りがあります

## Unity 3.4.0

<b>追加/更新：</b>

* 物理サイズパネルでテクスチャをサーフェス全体に移動するための位置オフセットコントロール
* プロジェクト設定でのSubstance 3D AssetsとSubstanceコミュニティアセットのダウンロード用リンク

## Unity 3.3.0

<b>追加/更新：</b>

* HDRPの物理サイズ機能。マテリアルを実際のサイズに基づいて適用したり、拡大縮小したりできます。
* プロジェクト設定でのGPU有効化のUI

<b>削除済み：</b>

* ほとんどのAPI呼び出しのグラフID

## Unity 3.2.1

<b>修正済み：</b>

* プラグインを3.0.0および3.1.0から最新バージョンにアップグレードする際の問題。

## Unity 3.2.0

<b>追加/更新：</b>

* スクリプトの再コンパイル時のパフォーマンスの向上

<b>修正済み：</b>

* カスタムSbsarマテリアルを読み込むときに、Unityプラグインでアセットの読み込みに失敗しました
* エラー：「ArgumentException：値が期待値範囲内にありません」
* &quot;ArgumentOutOfRangeException: Index was out of range&quot;エラー

## Unity 3.1.0

<b>追加/更新：</b>

* Macの1.38倍のパフォーマンス向上
* MacのGPUエンジンで、OpenGLではなくMetalが使用されている

<b>修正済み：</b>

* 出力テクスチャのRチャンネルとBチャンネルがフリップするMacの問題

## Unity 3.0.0

<b>追加/更新：</b>

* Apple Siliconのサポート
* プラグインの使用方法に関する新しいYouTubeチュートリアル
* 新しいスクリプト作成文書

<b>修正済み：</b>

* ランダム化ボタンを何度も押すと、インスペクターにバグが表示される
* Substanceのアップデートを中断するヌルテクスチャ入力
* 「すべての出力を生成」、「ミップマップを生成」および「ランタイムのみ」トグルが機能しない
* 名前空間に関する問題
* グラフアセットを選択して再生モードに入ると、Null参照エラーが発生する
* ランタイムのみのマテリアルを使用する場合のUnityの最新バージョン2021.3 LTSのHDRPおよびURPの問題
