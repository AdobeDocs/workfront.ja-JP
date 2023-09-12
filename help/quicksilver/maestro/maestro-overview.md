---
title: Adobeマエストロの概要
description: Adobe・マエストロはAdobe Workfrontからの新しいオファーです。 完全にカスタマイズ可能なワークスペースを作成して、企業の各組織単位のニーズを満たすワークフローを定義できます。
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '1805'
ht-degree: 1%

---


# Adobeマエストロの概要

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--see the separate article I wrote to have the PMs vet it for this: https://adobe-my.sharepoint.com/personal/alinaw_adobe_com/_layouts/15/doc.aspx?sourcedoc={79f94807-3d73-4015-afc0-5c016fc63cfc}&action=edit-->

<!--all the links are hidden for now, so I can share this with customer zero. Activate the links before making this public. -->

<!-- remove the references to closed beta from the entire article-->

>[!IMPORTANT]
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなクローズドベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。

## AdobeMaestro の概要

Adobe・マエストロはAdobe Workfrontからの新しいオファーです。 Maestro の目的は、組織の運用上の詳細に関する包括的な可視性を解き放ち、作業管理ライフサイクルの各段階で重要なビジネス上の質問に答えることです。

チームやリーダーシップは、次のような質問に対する明確な回答を必要とします。

* 第 4 四半期に EMEA で実行しているキャンペーンの数は？
* 同時キャンペーンの間にオーディエンスの重複はありますか？
* 認知プログラムは今どの程度順調に進んでいるのでしょうか？
* 特定のキャンペーンのアセットはどのように表示されますか？ どちらがまだ承認を受ける必要がありますか？

これらの質問に答えるために、リーダーシップは、計画から実行、配信から結果の測定まで、あらゆる作業段階の全体像を提供できるソリューションを必要とします。 現在、組織はプロセスの一部をカバーできるツールを持っていますが、多くの場合、作業のすべての段階に対して適切な接続を持たず、確実に結果を提供することもできません。

以下は、Maestro の主な機能の一部です。

* 作業プロセスに参加するすべてのステージおよびすべての関係者に対して、作業を管理するという問題を解決します。
* 組織で使用するオブジェクトの種類（またはレコードの種類）を決定して、これらのオブジェクトを相互にリンクする方法を設定することで、ワークフローを完全にカスタマイズします。
* 他のシステムのオブジェクトタイプにリンクし、すべてのプロセスに対して一貫性のあるフレームワークを作成します。

## 閉じられたベータプログラム中に Maestro を使用するために必要なアクセス

>[!IMPORTANT]
>
>現在、Maestro には、ユーザや情報に関連するアクセスレベルや権限はありません。 すべてのユーザは、他のユーザが Maestro に追加したすべての情報を表示、編集、および削除できます。

Maestro の使用に必要なアクセスについて詳しくは、 [Adobeマエストロアクセスの概要](../maestro/access/access-overview.md).

<!-- hidden the table after I moved the content to the Access overview article: 

You must have the following access to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader">Access level</td>
   <td> <p>Any</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../maestro/access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

************* Activate note when going to GA: 

>[!NOTE]
>
>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 
-->

## Maestro の用語

マエストロはWorkfrontの一部ですが、独自の概念と用語が付属しています。 Maestro を組織に設定する前に、Maestro の概念に精通していることを確認してください。

Maestro のフレームワークは完全にカスタマイズ可能です。 組織のニーズに合わせて、すべてのレコードタイプ、その属性、および関連付けられたフィールドを作成できます。

主な Maestro オブジェクトとコンセプトは次のとおりです。

* **Workspace**：特定の組織の運用ライフサイクルを定義するレコードタイプと分類のコレクションです。 ワークスペースは、組織単位の作業枠です。

  1 つのWorkfrontインスタンスに最大 1,000 個のワークスペースを設定できます。

  ![](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

  詳しくは、 [ワークスペースの作成](../maestro/architecture-and-fields/create-workspaces.md).

* **レコードタイプ**：マエストロメインオブジェクトタイプ。

  オブジェクトタイプが事前に定義されているWorkfrontとは異なり、Maestro では独自のオブジェクトタイプを作成できます。

  例えば、Workfrontでは、プログラム、Portfolio、プロジェクト、タスク、またはイシューのオブジェクトの種類が既に作成されています。

  Maestro では、組織のワークフローに合う任意のレコードタイプを作成できます。 後で、レコードの種類を相互に関連付けたり、フォームの依存関係を定義したりできます。

  詳しくは、 [オペレーショナル・レコード・タイプと分類の概要](../maestro/architecture-and-fields/overview-of-record-types-and-taxonomies.md).

  Maestro には次のレコードタイプがあります。

   * **オペレーショナルレコードの種類**：戦略計画、イニシアチブまたは実行済みの作業を表すレコードタイプ。

     ![](assets/operational-record-type-blank.png)

     例えば、キャンペーン、アクティビティ、プログラムは、運用レコードのタイプにすることができます。

     詳しくは、 [レコードタイプの作成](../maestro/architecture-and-fields/create-record-types.md).

   * **分類**：操作レコードタイプに関する属性をキャプチャするレコードタイプ。

     ![](assets/taxonomy-record-type-blank.png)

     分類の作成は、オペレーショナルレコードタイプの作成と同じですが、Maestro では、オペレーショナルレコードタイプとタクソノミレコードタイプが区別されます。 分類の目的は、オペレーショナル・レコード・タイプを強化することです。 <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

     例えば、Audience、Region、Address は、分類タイプのレコードタイプにすることができます。

     詳しくは、 [分類レコードタイプの作成](../maestro/architecture-and-fields/create-a-taxonomy.md).

* **レコード**: Maestro レコードタイプのインスタンス。 レコードは、オペレーショナルレコードタイプまたは分類を指す場合があります。

  ![](assets/records-highlighted-in-campaign-record-type-list.png)
  ![](assets/records-highlighted-in-region-taxonomy-type-list.png)

  レコードタイプをワークスペースに追加した後、そのタイプのレコードをレコードタイプのページに追加できます。

  例えば、「キャンペーン」は運用レコードタイプ、「EMEA 向け夏キャンペーン」はキャンペーンレコードタイプのレコードです

  または

  「地域」は分類タイプのレコードタイプで、「南北アメリカおよび中南米」は分類レコードです。「EMEA — 中央ヨーロッパ」は分類レコードです。

  詳しくは、 [レコードを作成](../maestro/records/create-records.md).

* **Workspace テンプレート**：定義済みのテンプレートを使用して、ワークスペースを作成できます。 定義済みのレコード・タイプ、分類、およびテンプレートに含まれるフィールドを使用するか、独自のレコードを追加できます。

  ![](assets/workspaces-page-with-templates-thumbnails.png)

  Maestro には、セールス、マーケティング、製品管理の各ワークスペーステンプレートが付属しています。

  詳しくは、 [ワークスペースの作成](../maestro/architecture-and-fields/create-workspaces.md).

* **フィールド**：フィールドは、レコードタイプに関する情報を含む、オペレーショナルレコードタイプまたは分類レコードタイプに追加できる属性です。 <!--check the shot below, "Connection" needs to be in lowercase-->

  ![](assets/drop-down-list-of-record-fields.png)

  マエストロフィールドに関する考慮事項：

   * レコードタイプに追加したフィールドは、自動的にそのタイプのすべてのレコードに関連付けられ、それらのレコードに関するデータを取り込むために使用できます。

   * レコードタイプのページに適用されたテーブルビューでは、フィールドが列として表示されます。 また、レコードの詳細ページにも表示されます。

   * フィールドはレコードタイプに固有で、レコードタイプ間では転送されません。

   * Maestro フィールドは完全にカスタマイズ可能で、Maestro でのみアクセス可能です。 Workfrontから Maestro フィールドにアクセスすることはできません。

  詳しくは、 [フィールドの作成](../maestro/architecture-and-fields/create-fields.md)

  新しいオペレーショナルレコードタイプは、デフォルトで次の定義済みフィールドに関連付けられます。

   * 名前
   * 説明
   * 開始日
   * 終了日
   * ステータス

  新しい分類レコードタイプは、デフォルトで、「名前」フィールドに関連付けられます。

  次のタイプのカスタムフィールドを作成できます。

   * 1 行テキスト
   * 段落
   * 複数選択
   * 単一選択
   * 日付
   * 数値
   * パーセンテージ
   * 通貨
   * チェックボックス

* **リンクされたレコードタイプ**, **リンクされたレコード**、および **リンクされたレコードフィールド**：次のエンティティ間に接続を作成できます。

   * 2 つのマエストロレコードタイプ
   * Maestro レコードタイプとWorkfrontプロジェクト、プログラム、ポートフォリオ、会社、またはグループオブジェクトタイプ。

  ![](assets/new-connection-tab-with-workfront-option.png)

  レコードタイプ間の接続を確立した後で、それらのタイプの個々のレコードを相互に接続できます。 レコード間の接続は、リンクされたレコードフィールドとして表示されます。

* **リンクされたフィールド** （または参照フィールド）:2 つのレコードタイプ間の接続を確立し、個々のレコードをリンクした後、接続元のレコード上のリンクされたレコードのフィールドを参照できます。

  ![](assets/add-lookup-fields-modal.png)

  レコードの種類、レコードのリンク、およびリンクされたフィールドの作成については、次の記事を参照してください。

   * [レコードタイプを接続](../maestro/architecture-and-fields/connect-record-types.md)
   * [レコードを接続](../maestro/records/connect-records.md)

<!--not yet:* Fields are reusable across Record Types.  -->

* **件数**：レコードは、異なるタイプの表示のそれぞれのレコードタイプページに表示されます。

  ![](assets/view-types-drop-down-from-record-type-list.png)

  ビューには、フィールドのリスト（列）、レコードのリスト（行）、順序（並べ替え）、適用または適用可能なフィルターおよびグループ化など、特定のビュータイプのパーソナライズされた設定が含まれます。

  レコードタイプページに適用できるビュータイプは次のとおりです。

   * **テーブル表示**：レコードとそのフィールドを表形式で表示します。 テーブルの行は個々のレコードで、列はレコードフィールドです。 これはデフォルトの表示です。

     ![](assets/table-view-example.png)

   * **タイムライン表示**：少なくとも 2 つの「日付」フィールドを持つレコードを時系列で表示します。

     ![](assets/grouping-applied-in-timeline-view.png)

  詳しくは、 [レコードビューの管理](../maestro/views/manage-record-views.md).


## Maestro オブジェクトの制限

次の表に、Maestro で作成できるオブジェクトの数の制限を示します。 制限は、マエストロの開発の次の段階に進むにつれて変化する場合があります。

| Maestro オブジェクト | 制限 |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| 1 つのWorkfrontインスタンスの Workspaces の数 | 1,000 |
| 1 つのワークスペースのレコードタイプの数 | 1,000（ワークスペースの分類、またはサードパーティのアプリケーションからインポートするオブジェクトを含む） |
| 1 つのレコードタイプのレコード数 | 10,000 |
| 1 つのレコードタイプまたは分類のフィールド数 | 500 |
| テキストフィールドの文字数 | 1,000 文字 |
| レコードタイプのテーブルに貼り付けることができるファイルのサイズ | 1MB |
| API を使用してインポートできる、レコードタイプテーブルのファイルサイズ | 1.5MB |
| API リクエストを実行できる割合 | 1 分あたり 200 リクエスト |
| テーブルにインポートできる Excel ファイルの CSV サイズ | 5MB |

## Workfrontインスタンスのユーザーに対して Maestro を有効にします

Maestro にアクセスする前に、AdobeMaestro クローズ済みベータプログラムに登録する必要があります。 ベータ版プログラムへの登録について詳しくは、アカウント担当者にお問い合わせください。

Maestro へのアクセス権の付与と他のユーザーが Maestro を使用できるようにする方法について詳しくは、 [AdobeMaestro へのアクセスを許可](../maestro/access/grant-access.md).

<!--hidden this after moved it to a separate article

After your organization has been enrolled in the Maestro beta program, you can add the Maestro area for other users by using a layout template. 

To share the Maestro area using a layout template: 

1. Log in to Workfront as a system administrator.  

1. Add the Maestro icon to the Main Menu using a Layout Template. For information, see [Customize the Main Menu using a layout template](../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md). 

1. Assign the  layout template to the users that you want to have access to Maestro.For information, see [Assign users to a layout template](../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

    All users who can access Maestro in their Main Menu can start creating workspaces, records types, records, and fields.  
  -->


## マエストロを探す

組織が Maestro へのアクセス権を受け取り、システムまたはグループ管理者が Maestro 領域をメインメニューに追加したことを確認します。

マエストロを探すには：

1. Adobe Workfrontにログインします。

1. 次をクリック： **メインメニュー** ![](assets/main-menu-workfront.png) をクリックするか、 **メインメニュー** ![](assets/main-menu-shell.png) 左上隅にある場合は、

1. クリック **マエストロ** ![](assets/maestro-icon.png).

   「マエストロワークスペース」(Maestro Workspaces) 領域が開きます。

1. （オプションおよび推奨）次のいくつかの操作を続行して、Maestro で作業構造を構築します。

   1. ワークスペースをゼロから作成するか、テンプレートを使用します。

   1. 新しいワークスペースにレコードタイプを追加します。

   1. 新しいワークスペースに分類を追加します。

   1. レコードタイプの名前をクリックして、レコードのページを開きます。 デフォルトでは、レコードページがテーブルビューで開きます。

   1. 次のいずれかの操作を行って、テーブルビューをカスタマイズします。

      * レコードタイプにフィールドを追加するには、 **+** アイコンが表示されます。 ビューの列は、レコードタイプに関連付けられたフィールドです。
      * レコードを追加するには、 **+** アイコンが表示されます。 ビューの行は、選択したレコードタイプの一意のレコードです。
      * クリック **フィルター** を使用して、レコードタイプのページに表示する情報をフィルタリングします。

   1. レコードの名前をクリックすると、レコードの [ 詳細 ] ページに詳細情報が表示されます。

   1. 以下からタイムラインビューを作成する： **表示** レコードタイプページの右上隅にあるドロップダウンメニュー。

   1. フィルター、グループ化または設定を更新して、タイムライン表示をカスタマイズします。

## 現在 Maestro で利用可能な機能

次の表に、Maestro で使用可能な主な機能と、その使用可能なタイムラインを示します。 このリストには、すべての機能が含まれているわけではありません。

| 機能 | 利用可能 | 近日中に利用可能 | 調査中 |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
| ワークスペースの作成 | ✓ |                                  |                  |
| オペレーショナルレコードタイプの作成 | ✓ |                                  |                  |
| 分類の作成 | ✓ |                                  |                  |
| 個々の名前付きレコードと分類を作成 | ✓ |                                  |                  |
| レコードのカスタムフィールドを作成 | ✓ |                                  |                  |
| Excel または CSV ファイルを使用してレコードの種類とフィールドをインポートする | ✓ |                                  |                  |
| レコードをリンク | ✓ |                                  |                  |
| テーブル内のレコードの表示 | ✓ |                                  |                  |
| タイムラインでのレコードの表示 | ✓ |                                  |                  |
| レコードのフィルタリング | ✓ |                                  |                  |
| タイムラインビューでのレコードのグループ化 | ✓ |                                  |                  |
| テーブルビューでのレコードのグループ化 |                               | ✓ |                  |
| テーブルビューでのレコードの並べ替え | ✓ |                                 |                  |
| タイムラインビューでのレコードの並べ替え |                               | ✓ |                  |
| テーブル表示でのグループの並べ替え |                               | ✓ |                  |
| タイムライン表示でのグループの並べ替え |                               | ✓ |                  |
| ワークスペースの接続 |                               | ✓ |                  |
| Maestro レコードと分類を接続 | ✓ |
| Maestro レコードをWorkfrontプロジェクト、プログラム、ポートフォリオ、会社、グループに接続 | ✓ |                                 |                  |
| レコードの詳細ページ | ✓ |                                  |                  |
| レコードの詳細ページのレイアウトを更新します |                               | ✓ |                  |
| アクセスレベルと権限 | | ✓ |  |
| リクエストを送信 |                               |                                  | ✓ |
| クリエイティブの概要 |                               |                                  | ✓ |
| レコードの色とアイコンのカスタマイズ | ✓ |                                  |                 |

## マエストロリリースアクティビティ

マエストロに新機能を定期的にリリースしています。 リリースされた機能の最新のリストについては、 [Adobeマエストロリリースアクティビティ](../maestro/release-activity.md).

<!--moved the contents of this whole section to its own article: release-activity.md, in the same folder

This section lists the features and patches that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The features are released weekly and are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Preview and Production environments. 

### Week of September 4, 2023

#### Connect Maestro records with Workfront companies and groups

Preview and production: September 5, 2023  

You can now connect a Maestro record with Workfront companies and groups. You must first create a connection between a Maestro record type and the Workfront companies and groups object types. Then, you can connect a single Maestro record of the selected record type to individual Workfront companies and groups.  

Consider the following:  

* You must create a connection between Maestro record types and Workfront companies and groups for each Workspace.  

* You cannot connect taxonomy record types with Workfront object types. 

* You can connect multiple Maestro records to the same Workfront company or group, and multiple companies or groups to the same Maestro record.  

* You cannot edit companies or groups in Maestro. All company or group changes performed in Workfront are visible in Maestro, when reviewing the Maestro linked records.  

#### URL support for single-line text fields 

Preview and production: September 7, 2023 

For better visibility when working with links in the Table view, we have added support for URLs in single-line text fields. Using URLs to other websites or external drives when updating a single-line text field, now identifies them as links and allows you to click them from the table.  

### Week of August 28, 2023

#### Field visibility menu for the Table View toolbar

Preview and production: August 31, 2023

To display the right information on a given set of records, especially if you intend to share the view with others who need to see some but not all fields of a record type, you can now select which fields (or columns) to display and which to hide in the Table view.  

You can hide or show individual fields, from each header of the field columns, or you can manage all fields of the record type from a setting in the table view toolbar.  

### Week of August 21, 2023

#### Connect Maestro records to programs and portfolios 

Preview and production: August 24, 2023

You can now connect a Maestro record with Workfront programs and portfolios. You must first create a connection between a Maestro record type and a program or portfolio which creates a connected field. Then, you can connect any Maestro records from all other record types within the same workspace to specific programs and portfolios which will create a read-only Workfront Program or Workfront Portfolio record type in the same workspace. Consider the following:

* Workfront connector record types are unique for each workspace. 
* You can connect multiple Maestro records to the same Workfront program or portfolio, and multiple programs and portfolios to the same Maestro record. 
* You cannot edit programs and portfolios in Maestro. All program and portfolio changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

#### New sorting functionality for the table view

Preview and production: August 24, 2023

You can now sort records in the table view of a record type page. 
The following capabilities are now available: 

* Sorting at the table-level, where you can sort by multiple fields at the same time. 
* Sorting at the column or field-level, where you can sort by an individual field at a time.

#### Improvements to the timeline view: new look-and-feel for groupings and the Compact/ Standard view switch

Preview and production: August 24, 2023

We have introduced the following improvements to the timeline view: 

* You can now display the timeline view in the following modes:

    * Standard: Displays records in separate lines.
    * Compact: Display the records whose dates don't intersect on the same line. 

* We have changed the look-and-feel of the grouping lines in the timeline view to display above the timeline of the records they contain. Prior to this improvement, the grouping lines displayed across the entire length of the timeline.

### Week of August 14, 2023

#### Reorder columns in the table view

You can now reorder columns in the Maestro table view. Consider the following when reordering columns: 

* The Name field is always the first field in the table view of a record type page 

* You cannot move the Name field to another position 

* The Name field is frozen and is not part of the horizontal scroll. 

#### Horizontal scroll for timeline view

You can now scroll horizontally in the timeline view of a record type. 

### Week of August 7, 2023

#### Import record types from an Excel file 

Preview and production: August 10, 2023

You can now import an Excel file to create record types in a workspace. The sheets of the file become the record types, and the columns of the file become their respective fields.  

#### Improved experience for connecting record types and projects 

Preview and production: August 10, 2023

We have improved the way you connect record types, including connecting to Workfront projects. As part of this improvement, we made the following changes when adding a field for a record type from the table view:  

* Removed the Relationship-type field from the "New field" tab.  

* Add a "New connection" tab where you can directly select the record or object type you want to connect to, eliminating the need for a Relationship-type field. 

### Week of July 10, 2023

#### Update the appearance of a record type

Preview and production: July 13, 2023

You can now select a custom icon for a record type, as well as a custom color for the record type icon.  

#### New Checkbox field type

Preview and production: July 13, 2023 

You can now add a Checkbox field type to Maestro record types. You can use the Checkbox field type to add a single checkbox option to a record. You can use this field to indicate a specific attribute or status for that particular record. For example, you can use it as a flag for tracking completion, approval, or any other binary attribute for each record.  

### Week of June 26, 2023

#### Quick activation of the contextual menu in a table

Preview and production: June 28, 2023
 
We have enabled the ability to activate the contextual menu by right-clicking anywhere in a record row, when viewing the records in the table view or a record type. You can now quickly view, delete, or copy a link to the record's Details page when you access the contextual menu from anywhere in the table view of a record type. Prior to this enhancement, the contextual menu was accessible only from the More menu in the Name column of a record.  

### Week of June 19, 2023

#### Record field names are unique

We have introduced a requirement now that the field names of a Maestro record type should have unique names. Fields that belong to different record types do not have to have unique names.  

### Week of June 5, 2023

#### Connect Maestro records with Workfront projects

Preview and production: June 5, 2023

You can now connect a Maestro record with Workfront projects. You must first create a connector Maestro record type to establish the connection between Maestro records and Workfront projects. Then, you can connect any Maestro records from all other record types to the connector record using the Relationship field. Consider the following:

* You must have a connector record type for Workfront for each Workspace. 
* You can connect multiple Maestro records to the same Workfront project, and multiple projects to the same Maestro record. 
* You cannot edit projects in Maestro. All project changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

### Week of May 29, 2023

#### Two-date requirement for creating a Timeline view

Preview and production: May 31, 2023  

You must have at least two date fields associated with a record type in order to create a Timeline view. 
-->




