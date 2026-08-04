---
title: Adobe Workfront Planning の基本を学ぶ
description: Adobe Workfront Planning は、Adobe Workfront の追加機能です。 完全にカスタマイズできるワークスペースを作成して、企業の各組織単位のニーズを満たすワークフローを定義できます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: b1d6e0b3-e6d4-46d1-a6a2-4b8b73f7d3f7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EXDQUUA9-OKoA8Yj3de1TnanFEgXfKPvP8ksBGChiSI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f8dfa5a4aec4541d885bcc45933488cd1fdefac4
workflow-type: tm+mt
source-wordcount: 1228
ht-degree: 68%

---

# Adobe Workfront Planning の基本を学ぶ

<!--

this article is linked to the WF Planning landing page - do not change URL or move it; send the team a new URL after we add the redirects for this page

-->

<!--do not use the snippet for IMPORTANT as it links to this article-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>ここでは、Adobe Workfront計画について説明します。 Workfront Planningは、スタンドアロン製品か、追加購入されたAdobe Workfront機能です。
>
>
>この記事では、WorkfrontまたはWorkflow パッケージも購入した場合のWorkfront計画に関する一般的な情報を説明します。
>
>Adobe Workfront Planningのドキュメントを含む記事の一覧については、[Workfront Planningの一般情報と記事インデックス &#x200B;](/help/quicksilver/planning/planning-information.md)を参照してください。
>
>スタンドアロン製品としてのWorkfront Planningについて詳しくは、[&#x200B; スタンドアロン製品としてのAdobe Workfront Planningの基本を学ぶ](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)を参照してください。


## Workfront計画の可用性

<!--
the bullets repeat in the "Access needed for Planning STA" article
-->

Workfront Planningは、次のいずれかのWorkfront パッケージを購入するとアクセスできます。

* Workfront WorkflowとWorkfront Planningを統合。 組織内のすべてのユーザーには、ワークフローとプランニングライセンスがあります。 これにより、すべてのユーザーは、両方のモジュールのすべてのWorkfront機能に完全にアクセスできます。

* Workfront Workflow for everyone in your organization and Workfront Planning only for some users in your organization. これにより、ユーザーはワークフローのすべての機能に完全にアクセスできるようになり、プランニングライセンスを割り当てられたユーザーはプランニング機能に限定されます。

* Workfront Planningは、組織内のユーザー向けのスタンドアロン製品です。 これにより、Workfront ワークフロー機能やプランニング機能にアクセスできなくなります。

スタンドアロン製品としてのPlanningに含まれる機能について詳しくは、[&#x200B; スタンドアロン製品としてのAdobe Workfront Planningの基本を学ぶ](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)を参照してください。

## Adobe Workfront Planning の概要

ワークフローライセンスと共に購入した場合、Adobe Workfront PlanningはAdobe Workfrontの追加機能です。 Workfront Planning の目的は、組織の運用上の詳細に関する包括的な可視性を解き放ち、作業管理ライフサイクルの各段階で重要なビジネス上の質問に答えることです。

Workfront Planning は、次のような質問に回答できます。

* 第 4 四半期に EMEA で実行しているキャンペーンの数は？
* 同時開催のキャンペーンでオーディエンスが重複していないか？
* 認知プログラムは今どの程度順調に進んでいるのか？
  <!--* What do the assets look like for a particular campaign? Which of them must still be approved?-->

このような質問に答えるために、リーダーシップは、計画から実行、配信から結果の測定まで、あらゆる作業段階の全体像を提供できるソリューションを必要とします。 現在、組織にはそのプロセスの一部をカバーできるツールがあるかもしれませんが、その多くは作業の全段階に適切なつながりがなく、また結果を確実に提供できるものでもありません。

主な機能の一部を次に示します。

* すべての段階にわたって、また作業プロセスに参加するすべての関係者に対して、作業を管理するという問題を解決します。
* 組織で使用するオブジェクトタイプ（またはレコードタイプ）を決定することから、それらのオブジェクトを相互にリンクする方法を設定することまで、ワークフローを完全にカスタマイズします。
* 他のシステムからオブジェクトタイプにリンクし、すべてのプロセスに対して一貫性のあるフレームワークを作成します。

## Workfront インスタンスのユーザーに対する Workfront Planning の有効化

組織で Workfront Planning のパッケージを購入後、ユーザーが Workfront Planning にアクセスする前に、Workfront 管理者として次の点を確認する必要があります。

* コントリビューターまたはライトのアクセスレベルを持つユーザーに、Planningを含むレイアウトテンプレートを割り当てます。

  標準ユーザーとシステム管理者の場合、Planning はデフォルトで有効になっています。

  詳しくは、[レイアウトテンプレートを使用したメインメニューのカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)と[レイアウトテンプレートへのユーザーの割り当て](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

* ユーザーに、WorkfrontおよびPlanningのライセンスと、Workfront Planningでオブジェクトを表示または作成できるWorkfront Planningの権限を割り当てます。

  他のユーザーが Workfront Planning を使用できるようにアクセス権を付与して有効にする方法について詳しくは、[Adobe Workfront Planning へのアクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。

## Workfront Planning の用語

Workfront Planning は Workfront の一部ですが、独自の概念と用語を備えています。 組織で Workfront Planning の設定を開始する前に、新しい概念を十分に理解する必要があります。

Workfront Planning のフレームワークは完全なカスタマイズが可能です。 組織の正確なニーズに合わせて、すべてのレコードタイプとその属性、およびそれらに関連付けられた任意のフィールドを作成できます。

詳しくは、[Workfront計画の用語の概要](/help/quicksilver/planning/general/planning-terminology.md)を参照してください。

<!--the content from this section was moved to the article linked above-->

## Adobe Workfront Planning へのアクセス

Adobe Planning にアクセスする前に、組織に Workfront Planning へのアクセス権が付与されており、システム管理者またはグループ管理者が Planning エリアをメインメニューに追加していることを確認してください。 詳しくは、[Adobe Planning へのアクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。

Workfront Planning にアクセスするには、次の手順に従います。

1. Workfront にログインします。

{{step1-click-main-menu-shell-only}}

1. 「**Planning**」![Planning アイコン](assets/planning-icon.png) をクリックします。

   Workfront Planning のメインページが開きます。

   ![Planning ランディングページの管理者](assets/planning-landing-page-admin.png)

   >[!TIP]
   >
   >    Workfront 管理者は、レイアウトテンプレートの「ランディングページを選択」オプションに Planning エリアを追加できるため、Workfront にログインするとすぐに Planning を開くことができます。 詳しくは、[レイアウトテンプレートを使用したランディングページのカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)を参照してください。

1. （条件付きおよびオプション）Workfront 管理者は、次のいずれかのタブをクリックします。
   * **参加中のワークスペース**：作成したワークスペースまたは共有されているワークスペースが表示されます。
   * **その他のワークスペース**：システム内のその他すべてのワークスペースが表示されます。

   その他のすべてのユーザーには、ユーザーが作成したワークスペースと共有されているワークスペースの両方が&#x200B;**ワークスペース**&#x200B;エリアに表示されます。

1. （オプションおよび推奨）次のいくつかの操作を続行して、作業構造を構築します。

   1. ワークスペースを最初から作成するか、テンプレートを使用して作成します。 詳しくは、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

   1. 新しいワークスペースにセクションを追加します。 詳しくは、[ワークスペースの編集](/help/quicksilver/planning/architecture/edit-workspaces.md)を参照してください。
   1. 新しいワークスペースで既存のセクションの名前を変更します。
   1. 新しいワークスペースにレコードタイプを追加します。 詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   1. レコードタイプの名前をクリックして、レコードタイプのページを開きます。 デフォルトでは、レコードタイプページがテーブルビューで開きます。

      タイムラインビューやカレンダービューを作成することもできます。 詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   1. テーブルビューで、行を追加してレコードを追加していきます。

      または

      列を追加して、レコードフィールドを追加していきます。

      詳しくは、次の記事を参照してください。

      * [レコードの作成](/help/quicksilver/planning/records/create-records.md)
      * [フィールドを作成します](/help/quicksilver/planning/fields/create-fields.md)。

## Workfront Planning のその他のリソース

* [Adobe Workfront計画に関する一般情報と記事のインデックス &#x200B;](/help/quicksilver/planning/planning-information.md): Workfront計画に関するドキュメントを含むすべての記事のインデックスで、関心のある分野ごとにグループ化されています。
* [&#x200B; スタンドアロン製品としてAdobe Workfront Planningを使い始める](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)：スタンドアロン製品として購入した場合のWorkfront Planningに関する一般情報。
* [Adobe Workfront Planning の AI アシスタントの概要](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)：Workfront Planning の AI アシスタントを使用すると、コマンドを実行することによって、レコードの検索、作成、更新、削除などの作業をアシスタントに代行してもらうことができます。

  <!--
    >[!NOTE]
    >
    >The Workfront AI Assistant has been temporarily removed and it will be available at a later date.
    -->

* [Workfront Fusion の Adobe Workfront Planning モジュール](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-planning-modules)：Adobe Workfront Planning モジュールを使用すると、Workfront Planning でイベントが発生した場合にシナリオをトリガーできます。 また、レコードの作成、読み取り、更新、削除、および Adobe Workfront Planning のアカウントへのカスタム API 呼び出しも実行できます。 Workfront Fusionにアクセスするには、追加ライセンスを購入する必要があります。

* [Adobe Workfront Planning API の基本](/help/quicksilver/planning/general/planning-api-basics.md)：Adobe Workfront Planning API の目的は、HTTP 上で動作する RESTful アーキテクチャを導入することで、Planning との統合の構築を簡略化することです。

* [Adobe Workfront Planning とAdobe GenStudio for Performance Marketing との統合の基本を学ぶ &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)：Workfront Planning の GenStudio ワークスペースで、GenStudio for Performance Marketing のレコードを管理できます。 GenStudio for Performance Marketing ライセンスを購入する必要があります。

* [Canvas ダッシュボードの概要](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md): Workfront Canvas ダッシュボードを使用すると、WorkfrontのレポートでWorkfront計画に関する情報を確認できます。 Canvas ダッシュボードにアクセスするには、Workfront Workflow ライセンスを購入する必要があります。


<!--
## Currently available Workfront Planning features
(*****for GA just make a list of what features ARE included in Planning and eliminate the last 2 columns; also update the title of this section*****)

(*****at GA: update the link below to the new place for release notes *****)

For information about new features and when they are released, see [Adobe Workfront Planning release activity for 2024](/help/quicksilver/planning/general/release-activity.md). 

The following features are currently available in Workfront Planning:

* Create workspaces             
* Create record types             
* Create record custom fields             
(************ * Import record types and fields using an Excel or CSV file*****)
          
* Display records in a table view            
* Display records in a timeline view            
* Display records in a calendar view            
* Filter, sort, and group records in a table view
* Filter, group, and color code records in the timeline view
* Filter records in the calendar view 
* Search for records in the table and timeline views             
* Connect records that belong to the same workspace  
* Connect records that belong to different workspaces   
* Connect Workfront Planning records to Workfront projects, programs, portfolios, companies, groups             
* Connect Workfront Planning records to Adobe Experience Manager assets          
    You must have an Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront.
    For information, see [Adobe Workfront for Experience Manager Assets and Assets Essentials: article index](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md). 
* View record information in the Details tab
* View record connections in the Connections tab
* Customize the layout of a record's page             
* Share workspaces             
* Share views             
* Share views publicly with any external resource, even people who are not Workfront users         
* Duplicate views             
* Submit requests to create records            
* Export record details to Word and PDF.
* Add comments to records             
* Receive in-app notifications             
* Receive email notifications             
* Add thumbnails and cover pages to records             
* View the history of changes on a record             
* Rich Text formatting for Paragraph fields             
* Access Planning records from Workfront objects             
* Connect and disconnect Planning records from Workfront objects 
* Create Planning records by submitting a request form            
* Workfront Planning public API             
* Adobe Workfront Planning modules for Adobe Workfront Fusion             
* Workfront Planning AI Assistant
* Reporting on Workfront Planning information
    You can report on Planning information using the Canvas Dashboard. For information, see [Canvas Dashboards overview](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md). 

-->

<!--
<table style="table-layout:auto"> 

|       Feature                                      |     Available now  |     Coming soon   |     In research  |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
|     Create workspaces                              |   ✓                           |                                  |                  |
|     Create record types                |   ✓                           |                                  |                  |
|     Create record custom fields                    |   ✓                           |                                  |                  |
|     Import record types and fields using an Excel  or CSV file                              |                              |           ✓                       |                  |
|     Link records                                   |   ✓                           |                                  |                  |
|     View records in a table                        |   ✓                           |                                  |                  |
|     View records in a timeline                     |   ✓                           |                                  |                  |
|     View records in a calendar                     |   ✓                           |                                  |                  |
|     Filter records                                 |   ✓                           |                                  |                  |
|     Group records in the timeline view             |   ✓                           |                                  |                  |
|     Group records in the table view                | ✓                              |                                 |                  |
|     Sort records in the table view                                 |  ✓                             |                                 |                  |
|     Sort records in the timeline view                                 |                               |   ✓                              |                  |
|     Sort groupings in the table view                                 |                               |   ✓                              |                  |
|     Sort groupings in the timeline view                                 |                               |   ✓                              |                  |
|   Search for records in the table view    | ✓    |   |
|   Search for records in the timeline view    | ✓    |   |
|     Connect Workfront Planning records to Workfront projects, programs, portfolios, companies, groups  |   ✓                            |                                 |                  |
|     Connect Workfront Planning records to Adobe Experience Manager assets                                  |      ✓                         |                                  |                 |
|     Connect Planning records from different workspaces                                  |      ✓                         |                                  |                 |
|     Record page with detailed information                            |   ✓                           |                                  |                  |
|     Update the layout of the record's page              |    ✓                           |                                 |                  |
|  Share workspaces | ✓| |  |
|  Share views |✓ | |  |
|  Share views publicly with external resources |✓ | |  |
|  Duplicate views |✓ | |  |
|     Submit requests                                |                               |          ✓                        |                 |
|     Export record details to Word                                 |    ✓                           |                                  |                 |
|     Export record details to PDF                                 |                               |                                  |       ✓          |
|     Customize the color and icon of a record                                 |      ✓                         |                                  |                 |
|     Add comments to records                                 | ✓                              |                                  |                 |
|     Receive in-app notifications                                 | ✓                              |                                  |                 |
|     Receive email notifications                                 | ✓                              |                                  |                 |
|     Add thumbnails to records                                 | ✓                              |                                  |                 |
|     View history of changes on a record                                 | ✓                              |                                  |                 |
|     Rich Text formatting for Paragraph fields                                 |      ✓                         |                                  |                 |
|     Adobe Workfront Planning modules for Adobe Workfront Fusion                                 |      ✓                         |                                  |                 |
|     Copy and paste information from one field to another                                  |      ✓                         |                                  |                 |
|     Access Planning records from Workfront objects                                  |      ✓                         |                                  |                 |
|     Connect Planning records from Workfront objects                                  |      ✓                         |                                  |                 |
|     Workfront Planning public API                                 |      ✓                         |                                  |                 |
|     Workfront Planning AI Assistant*                                 |      ✓                         |                                  |                 |
|     Reporting on Workfront Planning information (Canvas Dashboard)                              |                               |       ✓                           |                 |
</table>

-->