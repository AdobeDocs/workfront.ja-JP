---
title: Adobe Workfront Planning オブジェクトの制限の概要
description: Adobe Workfront Planningでは、インスタンスで作成できるオブジェクトの数に制限があります。 オブジェクトの制限は、Workfront Planningで製品のパフォーマンスを向上させ、エクスペリエンスを強化するために設定されています。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 21%

---


<!--keep the 30 connection limit in yellow till Jan 2026-->

# Adobe Workfront Planning オブジェクトの制限事項の概要

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.</span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}


Adobe Workfront Planningでは、インスタンスで作成できるオブジェクトの数に制限があります。 オブジェクトの制限は、Workfront Planningで製品のパフォーマンスを向上させ、エクスペリエンスを強化するために設定されています。

Workfront Planning で作成できるオブジェクトの数の制限を次の表に示します。制限は変更される場合があります。

| Adobe Workfront Planning オブジェクト | 制限 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 1つのWorkfront インスタンスのワークスペースの数 | 無制限* |
| 1 つのワークスペースのセクションの数 | 50 |
| 1つのワークスペースのレコードタイプの数 | 100（すべてのセクションのレコードタイプと、ワークスペーステンプレートを使用して作成されたレコードタイプを含みます） |
| 1 つのレコードタイプのレコード数 | 25,000 |
| 1つのワークスペースのレコード数 | Planning Select: 25,000 <br> Planning Prime: 500,000 <br> Planning Ultimate: 1,000,000 |
| Workfront Planningの1つのインスタンスの合計レコード数 | Planning Select: 500,000 <br> Planning Prime: 2,000,000 <br> Planning Ultimate：無制限 |
| 1 つのレコードタイプまたは分類のフィールド数 | 500 |
| 1行のテキストフィールドの文字数 | 1,000 文字 |
| 段落フィールドの文字数 | 10,000 文字 |
| 1つのレコードタイプの段落フィールドの数 | 20段落フィールド |
| レコードタイプテーブルに情報をインポートするために使用できるファイルのサイズ | 1 MB |
| APIを介してレコードタイプテーブルに情報をインポートするために使用できるファイルのサイズ | 1.5 MB |
| API リクエストを実行できるレート | 1 分あたり 200 件のリクエスト |
| 1人のユーザーが1つのレコードタイプに対して作成できるビュー数 | 100 |
| レコードタイプを作成するためにインポートできるExcel ファイルのCSV サイズ | 5 MB |
| レコードタイプを作成するためにCSVまたはExcel ファイルに読み込むことができる行数 | 25,000 |
| レコードタイプを作成するためにCSVまたはExcel ファイルにインポートできる列の数 | 500 |
| 1つのレコードタイプの数式フィールドの数 | 20 |
| 1つのレコードタイプの接続フィールドの数 | 30 |
| 数式フィールド式の文字数 | 50,000 |
| Planning オブジェクトを共有できるエンティティ（ユーザー、役割、チーム、会社、グループ）の数 | 100 |
| 階層内のレコードタイプの数 | 4 |
| ワークスペース内の階層数 | 5 |
| 階層内の、子レコードタイプの1つのレコードに接続された親レコードタイプのレコード数 | 10 |
| 複数選択接続タイプの1つのレコードに接続されたレコードの数（レコード間に階層が設定されていない） | 500 |

* 管理が困難になったり、ワークフローが断片化しすぎたりする可能性があるため、ワークスペースを過剰に多く用意しないことをお勧めします。

Workfront Planningの価格とパッケージについて詳しくは、担当のアカウントマネージャーにお問い合わせください。

<!--
****************KEEP THIS COMMENTED OUT:

**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--
OLD limitations (before GA:)

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

<!--
[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.
-->
