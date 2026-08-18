---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/3d-applications/3ds-max/troubleshooting.html"
breadcrumb-title: ''
description: スクリプトリスナーを使用して3ds MaxのSubstanceプラグインに関する問題を診断し、解決します。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: トラブルシューティング
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 1%

---


# トラブルシューティング

スクリプトリスナーを使用すると、プラグインの使用中に発生したエラーを診断できます。 スクリプトリスナーを開くには、スクリプトメニュー/スクリプトリスナーに移動します。 プラグインの使用中にエラーが発生すると、対応するエラーメッセージがこの[スクリプトリスナー]ウィンドウに出力されます。 詳細については、[スクリプトエディターの公式ドキュメント](https://help.autodesk.com/view/3DSMAX/2023/ENU/?guid=GUID-C8019A8A-207F-48A0-985E-18D47FAD8F36)を参照してください。

バグを報告するには、[Substance Discordサーバー](https://discord.com/invite/substance3d)の#3dsmax-pluginチャンネルに参加するか、[Adobeコミュニティ](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-autodesk3dsmax)にアクセスしてください。 コンソールログからの関連情報と、問題の再現手順をレポートに含めることができます。

## 既知の問題

* *拡散反射光を使用する.sbsarを、拡散反射光を使用しない.sbsarに置き換えると、欠落している拡散反射光が切断されるため、黒のレンダリングが発生します。*
  * これは、マルチ出力ノードで予期される動作です。 同じノードを使用してこれらの.sbsを読み込むのではなく、それぞれに異なるSubstanceノードを使用することをお勧めします。
