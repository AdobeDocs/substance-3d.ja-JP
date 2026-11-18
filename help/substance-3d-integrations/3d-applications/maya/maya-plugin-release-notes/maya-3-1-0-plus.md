---
description: Mayaプラグインバージョン3.0.0以降のリリースノートを参照して、新機能、改善点、およびバグ修正について確認してください。
title: Maya 3.0.0
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%
---

# Maya 3.1.0以降

## Maya 3.1.1

**リリース日：** 2026年11月18日

**互換性：** Maya 2025以降

### 追加/更新

* Substance engineアップデート(9.6.1.) セキュリティの修正を含める
* Maya 2025、2026、2027（ArnoldおよびV-Ray）のOpenPBRサポート

### 既知の制限

* Emission weight: emission_weightパラメータは、OpenPBR 1.1仕様の一部ではなく、自動的には接続されません。 マテリアルでエミッションを使用する場合は、ワークフローの適用後にOpenPBRノードでエミッションウェイト値を手動で設定します。
* OpenPBR - V-Ray – サブサーフェス半径スケール： OpenPBR - V-Rayワークフローを使用する場合、 subsurface_radius_scaleは0の値を返すことがあります。 この場合は、接続を削除し、V-Rayノードで値を手動で設定します。
* レンダラー間の視覚的な違い： Substance 3D Designerでのマテリアルプレビューと、ArnoldまたはV-Rayでのレンダリング結果では、レンダラーごとのOpenPBR仕様の実装の違いにより若干のばらつきがあります。
* Substance 3D Painter 12.2.0から書き出されたSBSARファイル または以前のバージョンでは、OpenPBRワークフローMaya 3.1.0を使用する場合に正しく接続されない可能性があります。追加/更新： Substance engineアップデート(9.6.1) セキュリティの修正を含む。

## Maya 3.1.0

**リリース日：** 2026年11月18日

**互換性：** Maya 2024

### 追加/更新

* Substance engineアップデート(9.6.1.) セキュリティの修正を含める
