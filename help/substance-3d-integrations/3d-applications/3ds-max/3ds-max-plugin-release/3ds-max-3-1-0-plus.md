---
description: 新機能、改善点、バグ修正については、 3ds Maxプラグインバージョン3.0.0以降のリリースノートを確認してください。
title: 3Ds Max 3.1.0以降
source-git-commit: 28a9d8cf7a4eed4163f99e8158c9cb8f9da88302
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%
---

# 3ds Max 3.1.0以降

## 3ds Max 3.1.1

**リリース日：** 2026年11月18日

**互換性：** 3ds Max 2025以降

### 追加/更新

* Substance engineアップデート(9.6.1.) セキュリティの修正を含める
* 3ds Max 2025、2026、2027 （ArnoldおよびV-Ray）のOpenPBRサポート

### 既知の制限

* Emission weight: emission_weightパラメータは、OpenPBR 1.1仕様の一部ではなく、自動的には接続されません。 マテリアルでエミッションを使用する場合は、ワークフローの適用後にOpenPBRノードでエミッションウェイト値を手動で設定します。
* レンダラー間の視覚的な違い： Substance 3D Designerでのマテリアルプレビューと、ArnoldまたはV-Rayでのレンダリング結果では、レンダラーごとのOpenPBR仕様の実装の違いにより若干のばらつきがあります。
* Substance 3D Painter 12.2.0から書き出されたSBSARファイル または以前のバージョンは、OpenPBRワークフローを使用する際に正しく接続されない場合があります

## 3ds Max 3.1.0

**リリース日：** 2026年11月18日

**互換性：** 3ds Max 2024

### 追加/更新

* Substance engineアップデート(9.6.1.) セキュリティの修正を含める
