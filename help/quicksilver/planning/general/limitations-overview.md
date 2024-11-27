---
title: Adobe Workfront Planning オブジェクトの制限事項の概要
description: Adobe Workfront Planning には、インスタンスに作成できるオブジェクトの数に制限があります。 Workfront Planning では、製品のパフォーマンスを向上させ、エクスペリエンスを向上させるためにオブジェクトの制限が設定されています。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: d962d60294295dd1f3771d1f0b737c9d1f03dfef
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 38%

---

<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Adobe Workfront Planning オブジェクトの制限事項の概要

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}


Adobe Workfront Planning には、インスタンスに作成できるオブジェクトの数に制限があります。 Workfront Planning では、製品のパフォーマンスを向上させ、エクスペリエンスを向上させるためにオブジェクトの制限が設定されています。

Workfront Planning で作成できるオブジェクトの数の制限を次の表に示します。この制限事項は、開発が次の段階に進むにつれて変わる可能性があります。

| Adobe Workfront Planning オブジェクト | 制限 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 1 つの Workfront インスタンスのワークスペース数 | unlimited* |
| 1 つのワークスペースのセクションの数 | 50 |
| 1 つのワークスペースに対するレコードタイプの数 | 1,000（すべてのセクションのレコードタイプと、ワークスペーステンプレートを使用して作成されたレコードタイプを含みます） |
| 1 つのレコードタイプに対するレコード数 | 25,000 |
| 1 つのワークスペースのレコード数 | Planning を使用しているお客様の場合は 25,000<br>Planning Plus を使用しているお客様の場合は 500,000 |
| Workfront Planning の 1 つのインスタンスの合計レコード数 | Planning Plan を利用するお客様は 500,000 <br> Planning Plus を利用するお客様は 200 万 |
| 1 つのレコードタイプまたは分類のフィールド数 | 500 |
| 1 行のテキストフィールドの文字数 | 1,000 文字 |
| 段落フィールドの文字数 | 10,000 文字 |
| 1 つのレコードタイプの段落フィールドの数 | 20 個の段落フィールド |
| レコードタイプのテーブルに貼り付けることができるファイルのサイズ | 1 MB |
| レコードタイプテーブルの API を通じて読み込めるファイルのサイズ | 1.5 MB |
| API リクエストを実行できるレート | 1 分あたり 200 件のリクエスト |
| 1 人のユーザーが 1 つのレコードタイプで作成できるビューの数 | 100 |
| レコードタイプを作成するために読み込むことができる Excel ファイルの CSV のサイズ | 5 MB |
| <span class="preview">CSV または Excel ファイルに読み込んでレコードタイプを作成できる行数 </span> | 10,000 |
| <span class="preview">CSV または Excel ファイルに読み込んでレコードタイプを作成できる列数 </span> | 500 |

*管理が困難になり、ワークフローが断片化される可能性があるので、ワークスペースが多くなりすぎることはお勧めしません。

Workfront Planning の価格とパッケージについては、[Adobe Workfrontの価格とパッケージ ](https://business.adobe.com/products/workfront/pricing.html) を参照してください。

<!--
****************KEEP THIS COMMENTED OUT:

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
