---
title: Adobe Workfront Planning オブジェクトの制限事項の概要
description: Adobe Workfront Planning には、インスタンスに作成できるオブジェクトの数に制限があります。 Workfront Planning では、製品のパフォーマンスを向上させ、エクスペリエンスを向上させるためにオブジェクトの制限が設定されています。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 63%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Adobe Workfront Planning オブジェクトの制限事項の概要

Adobe Workfront Planning には、インスタンスに作成できるオブジェクトの数に制限があります。 Workfront Planning では、製品のパフォーマンスを向上させ、エクスペリエンスを向上させるためにオブジェクトの制限が設定されています。

Workfront Planning で作成できるオブジェクトの数の制限を次の表に示します。この制限事項は、開発が次の段階に進むにつれて変わる可能性があります。

| Adobe Workfront Planning オブジェクト | 制限 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 1 つの Workfront インスタンスのワークスペース数 | 1,000 |
| 1 つのワークスペースのセクションの数 | 50 |
| 1 つのワークスペースに対するレコードタイプの数 | 1,000（すべてのセクションのレコードタイプと、ワークスペーステンプレートを使用して作成されたレコードタイプを含みます） |
| 1 つのレコードタイプに対するレコード数 | 50,000 |
| 1 つのレコードタイプまたは分類のフィールド数 | 500 |
| テキストフィールドの文字数 | 1,000 文字 |
| レコードタイプのテーブルに貼り付けることができるファイルのサイズ | 1 MB |
| レコードタイプテーブルの API を通じて読み込めるファイルのサイズ | 1.5 MB |
| API リクエストを実行できるレート | 1 分あたり 200 件のリクエスト |
| 1 人のユーザーが 1 つのレコードタイプで作成できるビューの数 | 100 |

<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.

****************KEEP THIS COMMENTED OUT:
| Size of CSV of Excel file you can import** | 5MB |
**This functionality has been temporarily removed and it will be available at a later date.**********************
-->