---
helpx_url: "https://helpx.adobe.com/jp/substance-3d-integrations/renderers/maverick/substance-sbsar-integration.html"
breadcrumb-title: ''
description: MaverickレンダラーでSubstanceのSBSARファイルを直接使用すると、リアルタイムのマテリアル編集やパラメーター制御が可能になります。
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Maverick > Substance SBSAR Integration
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance SBSARとの連携
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---


# Substance SBSARとの連携

**&#x200B;**&#x200B;**Substance DesignerまたはSubstanceで** **Alchemist** **から** **Maverick &#x200B;**&#x200B;**次の**&#x200B;**いずれか** **/** **これらの** **2** **方式**&#x200B;**:**&#x200B;**簡単に** **SBSARファイル**&#x200B;を **&#x200B; **&#x200B;簡単に利用できます&#x200B;**&#x200B;**

**メソッド** **1:**

1. SBSARアイコンを使用して、SBSARファイルを選択します。

   ![](../../../assets/maverickrender-sbsar-icon.jpg)
1. [読み込み]ダイアログでは、いくつかのマテリアルパラメータを設定できます。

   ![](../../../assets/maverickrender-sbsar-import-1.jpg)
1. 続行すると、マテリアルパネルにマテリアルが表示され、シーンで使用できるようになります。

   ![](../../../assets/maverickrender-sbsar-drop.jpg)

   **メソッド** **2**&#x200B;**:**
1. SBSARファイルをWindowsエクスプローラーからシーン内の任意のオブジェクトにドロップするだけです。 SBSARファイルはマテリアルパネルにもドロップできます。
1. [読み込み]ダイアログでは、いくつかのマテリアルパラメータを設定できます。

   ![](../../../assets/maverickrender-sbsar-import-1.jpg)
1. マテリアルは、ドロップしたオブジェクトに適用されます。

   **ヒントとコツ:**
1. SBSARパラメーターを編集するには、マテリアルパネルでSubstanceノードを選択するか、マテリアルのチャンネルプラグのいずれかをクリックします。
1. より流動的に編集するために、マテリアルを512または1024の解像度で編集することをお勧めします。 最終レンダリングでは、解像度を2048または4096に上げることができます。
1. 同じSBSARをシーン内の別のオブジェクトで異なるパラメーターを使用する場合は、そのSBSARを複製して新しいオブジェクトに適用します。 Maverickは新しいマテリアルを自動的に作成し、個別に編集することができます。
1. シーンに複数のSBSARがある場合は、いずれかのSBSARで「グローバル解像度に設定」ボタンを使用して、一度にすべてのSBSARの解像度を制御できます。

   ![](../../../assets/maverickrender-sbsar-resolution.jpg)
1. Maverickには、シェーディングライブラリのMaterialsフォルダーとMapsフォルダーおよびSbsar Substanceーの下にある10個のマテリアルとSBSARが含まれています。

   ![](../../../assets/maverickrender-sbsar-library.jpg)
1. 独自のSBSARをMaverickで使用できるようにするには、それらを配置するサブフォルダーを作成します

   「C:\Users\User\Documents\RandomControl\library\Shading\My Maps」。

   次に、オブジェクトの上にそれらをドロップするだけで、対応するラッパーのマテリアルを作成できます。

   MaverickのSBSARの概要ビデオについては、次のリンクをご覧ください： <https://youtu.be/HosZOoMRfcM>

   MaverickでSBSARを使用した実際の例は、次のとおりです： <https://youtu.be/ebVI5jJD71A>

   **サポート** **リンク：**

   [gorilla@maverickrender.com](https://helpx.adobe.com/mailto:gorilla@maverickrender.com)にメールを送信

   Maverick Webサイトでのチャット[www.maverickrender.com](http://www.maverickrender.com/)
