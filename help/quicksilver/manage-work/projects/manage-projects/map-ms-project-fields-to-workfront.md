---
product-area: projects
navigation-topic: manage-projects
title: Microsoft Project フィールドのAdobe Workfrontプロジェクトへのマッピング
description: Adobe WorkfrontとMicrosoft Project のプロジェクトは、ほとんど互換性があります。 この記事では、2 つのアプリケーションの最も一般的なプロジェクトフィールドを相互にマッピングする方法について説明します。
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# Microsoft Project フィールドのAdobe Workfrontプロジェクトへのマッピング

Adobe WorkfrontとMicrosoft Project のプロジェクトは、ほとんど互換性があります。 2 つのアプリケーションを使用して、次の操作を実行できます。

* Microsoft Project からプロジェクトを書き出し、Workfrontに読み込む
* Workfrontからプロジェクトを書き出し、Microsoft Project に読み込みます。 

Microsoft Project からWorkfrontにプロジェクトを読み込む方法について詳しくは、 [Microsoft Project からプロジェクトを読み込む](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Workfrontからプロジェクトを書き出してMicrosoft Project に読み込む方法について詳しくは、 [プロジェクトのMicrosoft Project への書き出し](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

このようなデータのインポートを実行する場合、情報がアプリケーション間でどのように変換されるかを理解することが重要です。 ほとんどの場合、インポートが完了した後で、プロジェクトに手動で修正を加える必要があります。 

## フィールドマッピングの概要

>[!NOTE]
>
>計画日は、必ずしも両方のシステムに対応しているとは限りません。 不一致は、スケジュールや、WorkfrontとMicrosoft Project の間のシステム環境設定の違いを通じて計上できます。 これらの日付の不一致は、作業量、期間、完了率の違いにもつながります。

| **Microsoft Project フィールド** | **Workfront Field** |
|---|---|
| プロジェクトタイトル | プロジェクト名 |
| 開始日と終了日 | 計画開始日と完了日 |
| タスク名 | タスク名 |
| タスク期間 | タスク予定期間 |
| タスクの作業 | タスク予定時間 |
| タスク%完了 | タスク%完了（タスクの期間に基づく） |
| タスク作業時間%完了 | タスク%完了（タスクの予定時間に基づく） |
| 予定されている開始と終了 | 計画開始日と完了日 |
| 実際の開始と終了 | 実際の開始日と完了日 |
| リソース名 | タスク割り当て |
| 割り当て単位 | 割り当て配分率 |
| タスクメモ | タスクの説明 |
| 先行タスク | 先行タスク |

## 含まれないデータの概要

Workfrontに読み込まれない、またはから書き出されないプロジェクトフィールドが多数あります。

これらのフィールドには、次のものが含まれます。

* ドキュメントの添付ファイル
* カスタムフィールド（プロジェクトまたはタスクレベル）
* Workfrontのメモ
* 問題
* [ 開始 ]/[ 終了 ] 先行タスクの関係があるタスクの負の遅延（タスクは、遅延なしで読み込まれます）
* 割り当て
* タスクの制約

   >[!NOTE]
   制約はMicrosoft Project とWorkfrontの間でマッピングされないので、タスク間に前に行われた関係があることを確認してください。 そうしないと、インポートされたプロジェクトで、タスクの計画開始日と計画完了日が正確にならない場合があります。 
