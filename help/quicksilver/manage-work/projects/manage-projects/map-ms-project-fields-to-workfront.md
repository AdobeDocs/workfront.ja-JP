---
product-area: projects
navigation-topic: manage-projects
title: Microsoft プロジェクトフィールドをAdobe Workfront プロジェクトにマッピングする
description: Adobe Workfront と Microsoft Project のプロジェクトは、ほとんどの場合において互換性があります。 この記事では、2 つのアプリケーションの最も一般的なプロジェクトフィールドを、相互にマッピングする方法について説明します。
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
TQID: https://experienceleague.adobe.com/WdFf5O8kKyY43PsHLEINDaLzsEa0idHZPNz83O12bTI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 396
ht-degree: 84%

---

# Microsoft Project フィールドの Adobe Workfront プロジェクトへのマッピング

Adobe Workfront と Microsoft Project のプロジェクトは、ほとんどの場合において互換性があります。 2 つのアプリケーションを使用して、以下の操作を実行できます。

* Microsoft Project からプロジェクトをエクスポートし、Workfront にインポート
* Workfront からプロジェクトをエクスポートし、Microsoft Project にインポート。

Microsoft Project から Workfront にプロジェクトをインポートする方法に関して詳しくは、[Microsoft Project からのプロジェクトのインポート](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)を参照してください。

Workfront からプロジェクトをエクスポートして Microsoft Project にインポートする方法に関して詳しくは、[Microsoft Project へのプロジェクトのエクスポート](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)を参照してください。

このようなデータのインポートを実行する場合、情報がアプリケーション間でどのように変換されるかを理解することが重要です。 ほとんどの場合、インポートが完了した後で、プロジェクトに手動で修正を加える必要があります。

## フィールドマッピングの概要

>[!NOTE]
>
>予定日は、両方のシステム間で必ずしも一致するわけではありません。 不一致の原因は、スケジュールや Workfront と Microsoft Project の間のシステム設定の違いです。 こうした日付の不一致により、労力、期間、完了率に違いが生じる可能性もあります。

| **Microsoft Project フィールド** | **Workfront フィールド** |
|---|---|
| プロジェクトタイトル | プロジェクト名 |
| 開始日と終了日 | 予定開始日と完了日 |
| タスク名 | タスク名 |
| タスクの期間 | タスクの予定期間 |
| タスクの作業 | タスクの予定時間数 |
| タスク %完了 | タスクの完了率（タスクの期間に基づく） |
| タスク作業%完了 | タスクの完了率（タスクの予定時間数に基づく） |
| 予定開始日および予定終了日 | 予定開始日と完了日 |
| 実際の開始と終了 | 実際の開始日と完了日 |
| リソース名 | タスクの割り当て |
| 割り当て単位 | 割り当て配分率 |
| タスクメモ | タスクの説明 |
| 先行タスク | 先行タスク |

## 含まれないデータの概要

Workfrontに読み込まれたり、から書き出されたりしないプロジェクトフィールドがいくつかあります。

これらのフィールドには、以下のものが含まれますが、これらに限定されません。

* ドキュメントの添付ファイル
* カスタムフィールド（プロジェクトレベルまたはタスクレベル）
* Workfront のメモ
* イシュー
* 開始や終了の先行タスク関係があるタスクの負の遅延（タスクは遅延なしで読み込まれます）
* 割り当て
* タスクの制約

  >[!NOTE]
  >
  >制約は Microsoft Project と Workfront の間でマッピングされないので、タスク間に先行タスク関係があることを確認してください。 確認しないと、読み込まれたプロジェクトで、タスクの予定開始日と予定完了日が正確でない可能性があります。
