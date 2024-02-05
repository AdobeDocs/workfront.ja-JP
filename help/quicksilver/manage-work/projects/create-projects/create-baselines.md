---
product-area: projects
navigation-topic: create-projects
title: プロジェクトのベースラインを作成
description: ベースラインとは、プロジェクトの初期計画に含まれる主要な情報を表すプロジェクトのスナップショット、またはプロジェクトの存続期間中の任意の時点での情報を表します。
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: bec625b70b39fec9f9a6d4f7b48023702de43675
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 90%

---

# プロジェクトのベースラインを作成

<!-- Audited: 12/2023 -->

ベースラインとは、プロジェクトの初期計画に含まれる主要な情報を表すプロジェクトのスナップショット、またはプロジェクトの存続期間中の任意の時点での情報を表します。

ベースラインを使用して、現在の計画の情報を、元の計画やその他の任意の時点の情報の断片と比較し、問題のタスク、範囲クリープ、その他の経時的なトレンドを特定できます。

## アクセス要件

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
    <td><p>新規：標準</p>
        <p>または</p>
        <p>現在：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ベースラインを表示するには、プロジェクトに対する表示以上の権限</p> <p>プロジェクトに対する権限を管理してベースラインを作成</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## ベースラインを使用する際の考慮事項

* プロジェクトの有効期間中に複数のベースラインを作成して、プロジェクトの進行状況のスナップショットを複数回取り込むことができます。
* プロジェクトのベースラインに含まれる情報は、ベースラインを作成するか、ベースラインレポートを作成することで表示できます。
* ベースラインを作成すると、そのベースラインのベースラインタスクに関するタスク情報も取り込まれます。
* ベースラインタスクレポートを作成すると、ベースラインタスクの情報を表示できます。

>[!IMPORTANT]
>
>ベースラインは、プロジェクトの名前、日付、および財務情報のスナップショットを作成します。ベースラインには、プロジェクト上のカスタムフィールドの値は含まれません。ベースラインに含まれる財務情報の詳細に関しては、[プロジェクトのベースラインに含まれるプロジェクトの財務](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md)を参照してください。

## ベースラインを作成

ベースラインは、次の方法で作成できます。

* **自動**：プロジェクトが現在になったときに、Workfront が自動的にベースラインを作成するように、Workfront 管理者またはグループ管理者がプロジェクトの環境設定を指定します。この設定が有効な場合、プロジェクトのステータスが現在になると、ベースラインが作成されます。この設定が有効になっていない場合は、ベースラインを手動で作成する必要があります。

  プロジェクトの環境設定と、ベースラインの自動作成の設定に関する詳細情報は、[システム全体のプロジェクト環境設定を実行](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

  >[!CAUTION]
  >
  >この設定が有効な場合、プロジェクトのステータスが現在に変わるたびに、プロジェクトのベースラインが自動的に作成されます。最初に作成されたベースラインが、デフォルトのベースラインです。プロジェクトの期間中は、他のすべてのベースラインを手動で作成する必要があります。

* **手動**：プロジェクトの進行に応じて、プロジェクトの新しいベースラインを必要に応じて作成できます。その後ベースラインを比較して、プロジェクトが時間の経過とともにどのように進行したかを確認できます。

ベースラインを作成するには、次のようにします。

1. プロジェクトに移動します。
1. 左側のパネルで、**ベースライン**&#x200B;をクリックします。

   または

   **さらに表示**&#x200B;をクリックし、次に&#x200B;**ベースライン**&#x200B;をクリックします。

   ![プロジェクトのベースラインセクション](assets/baselines-section-on-project-with-header.png)

1. **新しいベースライン**&#x200B;をクリックします。
1. ベースラインの名前を指定します。
1. （オプション）これが最初のベースラインの場合、デフォルトとして選択できます。
1. 「**保存**」をクリックします。

   デフォルトでは、作成したベースラインに関する次の情報が表示されます。

   * ベースライン名
   * ベースラインのエントリ日
   * ベースラインが作成された際のプロジェクトの開始予定日
   * ベースラインが作成された際のプロジェクトの見込み開始日
   * ベースライン計画が作成された際のプロジェクトの実際の期間
   * ベースラインが作成された際のプロジェクトの完了率
   * ベースラインがプロジェクトのデフォルトのベースラインかどうかを示す、デフォルトベースラインインジケーター

     >[!TIP]
     >
     >同じビューまたはレポートで、2 つのベースラインの情報を同時に表示することはできません。同じレポート内で表示できるのは、特定のベースラインとデフォルトのベースラインの情報のみです。プロジェクトの期間中、どのベースラインをデフォルトのベースラインにするかをいつでも変更できます。

1. （オプション） **表示** ボタンをクリックし、新しいビューを作成するか、現在のビューを編集して、ビューにフィールドを追加し、ベースライン間で追加情報を比較します。 詳しくは、[Adobe Workfront でのビューの作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)を参照してください。

## ベースラインのレポートやベースラインのタスクレポートを作成

ベースラインの情報を確認するために、ベースラインのレポートやベースラインのタスクレポートを作成することもできます。これにより、ベースラインやベースラインのタスクに関するフィールドをいくつでも表示して、1 つのビューで比較できます。

>[!TIP]
>
>ベースラインのレポートやベースラインのタスクレポートを作成する前に、ベースラインを作成する必要があります。

レポートの作成について詳しくは、[カスタムレポートを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

読みやすくするために、プロジェクト名のグループをベースラインレポートまたはベースラインタスクレポートに追加することをお勧めします。

グループ化の作成について詳しくは、[Adobe Workfront でグループ化を作成](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)を参照してください。
