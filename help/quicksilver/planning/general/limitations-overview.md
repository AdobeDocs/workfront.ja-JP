---
title: Adobe Workfront Planning オブジェクトの制限事項の概要
description: Adobe Workfront Planning には、インスタンスに作成できるオブジェクトの数に制限があります。 Workfront Planning では、製品のパフォーマンスを向上させ、エクスペリエンスを向上させるためにオブジェクトの制限が設定されています。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: f9abcd9ff4c80376bed229a1d65e0efcbfc332b0
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 46%

---


<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Adobe Workfront Planning オブジェクトの制限事項の概要

{{planning-important-intro}}


Adobe Workfront Planning には、インスタンスに作成できるオブジェクトの数に制限があります。 Workfront Planning では、製品のパフォーマンスを向上させ、エクスペリエンスを向上させるためにオブジェクトの制限が設定されています。

Workfront Planning で作成できるオブジェクトの数の制限を次の表に示します。この制限事項は、開発が次の段階に進むにつれて変わる可能性があります。

| Adobe Workfront Planning オブジェクト | 制限 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 1 つの Workfront インスタンスのワークスペース数 | unlimited* |
| 1 つのワークスペースのセクションの数 | 50 |
| 1 つのワークスペースに対するレコードタイプの数 | 1,000（すべてのセクションのレコードタイプと、ワークスペーステンプレートを使用して作成されたレコードタイプを含みます） |
| 1 つのレコードタイプに対するレコード数 | 25,000 |
| 1 つのワークスペースのレコード数 | 計画プランを使用しているお客様の場合は 25,000<br> 計画プラスを使用しているお客様の場合は 500,000 |
| Workfront Planning タイプの 1 つのインスタンスの合計レコード数 | Planning Plus プランのお客様の場合は 500,000<br>Planning Plus プランのお客様の場合は 200 万 |
| 1 つのレコードタイプまたは分類のフィールド数 | 500 |
| テキストフィールドの文字数 | 1,000 文字 |
| レコードタイプのテーブルに貼り付けることができるファイルのサイズ | 1 MB |
| レコードタイプテーブルの API を通じて読み込めるファイルのサイズ | 1.5 MB |
| API リクエストを実行できるレート | 1 分あたり 200 件のリクエスト |
| 1 人のユーザーが 1 つのレコードタイプで作成できるビューの数 | 100 |

*管理が困難になり、ワークフローが断片化される可能性があるので、ワークスペースが多くなりすぎることはお勧めしません。

Workfront Planning の価格とパッケージについては、[Adobe Workfrontの価格とパッケージ ](https://business.adobe.com/products/workfront/pricing.html) を参照してください。

<!--
****************KEEP THIS COMMENTED OUT:
| Size of CSV of Excel file you can import** | 5MB |
**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->

