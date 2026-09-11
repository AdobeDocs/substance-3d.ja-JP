---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/installing-to-source-builds-ue5.html"
breadcrumb-title: ''
description: Substance 3DプラグインをUnreal エンジン 5のソースビルドにインストールし、カスタムのエンジンを修正します。
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: ソースビルドへのインストール – UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# ソースビルドへのインストール – UE5

Substanceプラグインは、ソースから構築されたUnreal エンジンのバージョンで使用できます。 これを行うには、プラグインをC++projectフォルダーまたはソースビルドのエンジンフォルダーにインストールします。

>[!NOTE]
>
> これらの方法では、マーケットプレイスからダウンロードしたプラグインのバージョンが必要です。 Substanceプラグインフォルダーは、コンピューターとUEビルドの間で転送できます。

## C++プロジェクトフォルダーへのインストール

1. プロジェクトのフォルダーにプラグインフォルダーが存在しない場合は、作成します。
1. プラグインフォルダー内に、ランタイムフォルダーを作成します。
1. Substanceフォルダーをランタイムフォルダー内に配置します。 LINUXの場合：手順3の後、Substanceフォルダーで「include」フォルダーを探し、名前を「i」で始まるように変更します(include > Include)。
1. Unreal エンジンを起動します。
1. ランチャーを介してC++プロジェクトを開きます。
1. プロジェクトを立ち上げた後、Unreal エンジンは立ち上げる前にプラグインコンポーネントを再構築するかどうかを尋ねるメッセージを表示します。 これは、Microsoft Visual Studio(Windows、Linux)またはXcode(Mac)を介して実行されます。
1. アンリアルエンジンは終了しますが、コンポーネントはバックグラウンドでビルドされます。 このプロセスには約5分かかります。 完了すると、プロジェクトが開きます。 失敗した場合は、エラーウィンドウが表示されます。

## Engineフォルダーへのインストール

>[!NOTE]
>
> プラグインをエンジンフォルダーにインストールする前に、上記の手順に従ってプラグインバイナリフォルダーを再構築する必要があります。

1. プロジェクトフォルダー/プラグイン/ランタイムからSubstanceフォルダーをコピーします。
1. Unreal Engineバージョンフォルダーを開き、エンジン/プラグイン/マーケットプレイスに移動します。
1. Substanceフォルダーをペーストします。
1. アンリアルエンジンエディタを開きます。 必要に応じて、新しいプロジェクトを作成します。
1. プラグインメニューを開き、「Substanceプラグイン」が有効になっていることを確認します。
