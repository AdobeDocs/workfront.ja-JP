---
product-area: projects
navigation-topic: manage-projects
title: Microsoft Project フィールドの Adobe Workfront プロジェクトへのマッピング
description: Adobe Workfront と Microsoft Project のプロジェクトは、ほとんどの場合において互換性があります。この記事では、2 つのアプリケーションの最も一般的なプロジェクトフィールドを、相互にマッピングする方法について説明します。
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: ht
source-wordcount: '396'
ht-degree: 100%

---

# Microsoft Project フィールドの Adobe Workfront プロジェクトへのマッピング

Adobe Workfront と Microsoft Project のプロジェクトは、ほとんどの場合において互換性があります。2 つのアプリケーションを使用して、以下の操作を実行できます。

* Microsoft Project からプロジェクトをエクスポートし、Workfront にインポート
* Workfront からプロジェクトをエクスポートし、Microsoft Project にインポート。 

Microsoft Project から Workfront にプロジェクトをインポートする方法に関して詳しくは、[Microsoft Project からのプロジェクトのインポート](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)を参照してください。

Workfront からプロジェクトをエクスポートして Microsoft Project にインポートする方法に関して詳しくは、[Microsoft Project へのプロジェクトのエクスポート](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)を参照してください。

このようなデータのインポートを実行する場合、情報がアプリケーション間でどのように変換されるかを理解することが重要です。ほとんどの場合、インポートが完了した後で、プロジェクトに手動で修正を加える必要があります。 

## フィールドマッピングの概要

>[!NOTE]
>
>予定日が、必ずしも両方のシステムに対応しているとは限りません。不一致の原因は、スケジュールや Workfront と Microsoft Project の間のシステム設定の違いです。日付の不一致は、作業量、期間、完了率の違いにもつながります。

| **Microsoft Project フィールド** | **Workfront フィールド** |
|---|---|
| プロジェクトタイトル | プロジェクト名 |
| 開始日と終了日 | 予定開始日と完了日 |
| タスク名 | タスク名 |
| タスクの期間 | タスクの予定期間 |
| タスクの作業 | タスクの予定時間数 |
| タスクの完了率 | タスクの完了率（タスクの期間に基づく） |
| タスク作業の完了率 | タスクの完了率（タスクの予定時間数に基づく） |
| 予定開始日および予定終了日 | 予定開始日と完了日 |
| 実際の開始日と終了日 | 実際の開始日と完了日 |
| リソース名 | タスクの割り当て |
| 割り当て単位 | 割り当て配分率 |
| タスクメモ | タスクの説明 |
| 先行タスク | 先行タスク |

## 含まれないデータの概要

Workfront にインポートされない、または Workfront からエクスポートされないプロジェクトフィールドが多数あります。

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
  制約は Microsoft Project と Workfront の間でマッピングされないので、タスク間に先行タスク関係があることを確認してください。確認しないと、読み込まれたプロジェクトで、タスクの予定開始日と予定完了日が正確でない可能性があります。 
