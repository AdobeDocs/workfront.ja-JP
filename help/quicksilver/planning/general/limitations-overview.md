---
title: Adobe Workfront Planning オブジェクトの制限の概要
description: Adobe Workfront Planningでは、インスタンスで作成できるオブジェクトの数に制限があります。 オブジェクトの制限は、Workfront Planningで製品のパフォーマンスを向上させ、エクスペリエンスを強化するために設定されています。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/WmG-52JaTKD-0-bH2qKniwUBrpGyOKz5jJ3s9nwd12A
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: f8667931-f646-4dd3-af2a-b9d0cb8098ad
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 537
ht-degree: 23%

---

<!--keep the 30 connection limit in yellow till Jan 2026-->

# Adobe Workfront Planning オブジェクトの制限事項の概要


<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 すべてのユーザーのプレビュー環境でのみ使用できます。 プレビューへのリリース後、高速リリースを有効にしたユーザーの実稼動環境では、同じ機能を毎月使用することもできます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


{{planning-important-intro}}


Adobe Workfront Planningでは、インスタンスで作成できるオブジェクトの数に制限があります。 オブジェクトの制限は、Workfront Planningで製品のパフォーマンスを向上させ、エクスペリエンスを強化するために設定されています。

Workfront Planning で作成できるオブジェクトの数の制限を次の表に示します。 制限は変更される場合があります。

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
| <span class="preview">一度に一括で共有できるレコードの数</span> | 100 |
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
