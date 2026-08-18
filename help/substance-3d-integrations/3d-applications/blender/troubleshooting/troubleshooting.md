---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/troubleshooting.html"
breadcrumb-title: ''
description: システムコンソールを使用して、BlenderのSubstance 3Dアドオンに関する一般的な問題を診断し、解決します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: トラブルシューティング
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# トラブルシューティング

システムコンソールを使用すると、アドオンの使用中に発生したエラーを診断できます。 Blenderのシステムコンソールウィンドウが開く方法は、オペレーティングシステムによって異なります。 詳しい手順については、ブレンダーのシステムコンソール[ドキュメントページ](https://docs.blender.org/manual/en/2.79/advanced/command_line/introduction.html#console-window-status-and-error-messages)を参照してください。 コンソール出力は、テクスチャが読み込まれない、マテリアルが処理で動かなくなるなど、予期しない問題が発生した場合に役立ちます。

バグを報告するには、[Substance Discordサーバー](https://discord.com/invite/substance3d)の#substance-blender-betaチャンネルに参加するか、[Adobeコミュニティ](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-blender)にアクセスしてください。 コンソールログからの関連情報と、問題の再現手順をレポートに含めることができます。

## 一般的な問題と解決策

* *WMIC関連のコンソールエラーです。*
  * *WindowsのインストールにWMICが含まれない場合があります。この場合はWMICが必要です。 これを手動で修正する方法は次のとおりです：*
    * 設定 – システム – オプション機能に移動します
    * 「view features」を選択し、「Add Option feature」を選択します。
    * これにより新しいウィンドウが表示され、リストを下にスクロールしてWMICを見つけ、チェックボックスをチェックして「次へ」を押します。次のウィンドウで「追加」を押します。
    * ここで、最近のアクションの下にWMICインストールの進行状況を示す新しいウィンドウが表示されます。
    * *ダウンロードには数分かかる場合があります。 その後、コンピューターをリセットし、Blenderとアドオンを再起動します。 Substance 3Dパネルで「読み込み」をクリックすると、ファイルブラウザーウィンドウが表示されます。*
  * これで問題が解決しない場合は、PATH変数でWMICを定義する必要があります。 ご使用のWindowsのバージョンに応じたマニュアルを参照してください。
* *アドオンの更新とマテリアルの読み込み後は、一部の設定がSubstance 3Dパネルに表示されません。*
  * これは、古いバージョンのアドオンを削除し、同じセッションに新しいバージョンをインストールした場合に発生する可能性があります。古いファイルがシステムにキャッシュされている可能性があるためです。\
    ブレンダーを再起動すると、変更が有効になります。
* *アドオンのインストール時に問題が発生します。/マテリアルは、セッション間の処理でスタックします。 /マテリアルはセッション間でテクスチャを生成しません。 / .sbsarファイルの読み込み中にエラーが発生しました。*
  * これは統合ツールのインストールに問題がある可能性があり、通常はツールを手動で削除することで修正されます。 手動で削除する方法については、[アドオンのアンインストール](../../../3d-applications/blender/uninstalling-the-add-on/uninstalling-the-add-on.md)のページにアクセスしてください。
* *サイクルレンダリングビューでマテリアルが更新されません*。
  * デフォルトでは、サイクルレンダービューのテクスチャは更新されません。 ただし、アドオンの環境設定で<b>[テクスチャを自動更新]</b>を有効にすると、強制的に更新できます。
* サイクルのレンダービューで保存すると、パラメータが元に戻る。
  * これは、Blender側の既知のキャッシュの問題で、ビジュアル専用です。 保存時に、生成されたテクスチャファイルを更新するためのメッセージがリモートエンジンに送信されません。 サイクルレンダー表示から切り替えて元に戻すと、テクスチャは正常に表示されます。
* *パラメーターを元に戻した後、または変更した後、マテリアルが更新されなくなりました。*
  * 操作を元に戻した後、マテリアルの更新に失敗することがあります。 パラメータは前の状態に戻りますが、一致するようにテクスチャは元に戻りません。 テクスチャを再び更新するには、[更新]ボタンを使用してパラメータを既定値に戻し、テクスチャを再ロードします。
* *Substance Designerで設定された色がブレンダーのカラーピッカーでは若干異なって表示され、カラー値が同じではありません。*
  * ガンマ補正は、ブレンダーのカラーピッカーのカラーにのみ適用されます。 これにより、カラーピッカーが異なる場合がありますが、テクスチャに表示される色は、Substanceアプリで設定された値に対して正確です。
* *「wmicが認識されません」というコンソールエラーが、Windowsでマテリアルを読み込むときに発生します。*
  * この問題は、C:\Windows\System32\wbem\がPATHシステム変数に含まれていない場合に発生します。 ご使用のWindowsのバージョンに応じたマニュアルを参照してください。
* *Macで「CPUの種類が正しくありません」というエラーが発生しました。*
  * この問題は、ARM MacマシンでRosettaが有効になっていない場合に発生します。 詳しくは、[AppleのRosettaページ](https://support.apple.com/en-us/102527)を参照してください。 さらに、詳しい手順については、この[インストールガイド](https://medium.com/@jithmisha/fix-for-macbook-air-m1-m2-bad-cpu-type-in-executable-error-3719a0a1cb6)を参照してください。
* *[更新]ボタンを使用するか、パラメーターを更新すると、シェーダーグラフへの変更は元に戻されます。*
  * アドオンは、変更または更新後にグラフ内の接続を更新しました。 この問題を回避するには、.sbsarから作成されたブレンダーマテリアルを複製し、新しい名前を選択します。 複製にのみノードを追加します。 ユーザが追加したノードを維持したまま、ノードグループ内のテクスチャが更新されます。 更新するときは、これらのノードをコピーして、更新後に新しいグラフに貼り付けます。
