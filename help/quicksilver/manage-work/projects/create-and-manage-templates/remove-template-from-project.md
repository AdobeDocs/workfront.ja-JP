---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトからテンプレート情報を削除
description: プロジェクトからテンプレートを削除することはできません。 テンプレートがプロジェクトに添付された後にプロジェクトに追加された情報は、手動でのみ削除することができます。 テンプレートの添付について詳しくは、プロジェクトにテンプレートを添付を参照してください。
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YGb9LSybhejKxNYvxqiw7pcGD5f8p-2BqXbHU1OHEFc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 395
ht-degree: 93%

---

# プロジェクトからテンプレート情報を削除

プロジェクトからテンプレートを削除することはできません。 テンプレートがプロジェクトに添付された後にプロジェクトに追加された情報は、手動でのみ削除することができます。 テンプレートの添付について詳しくは、[プロジェクトにテンプレートを添付](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>Work またはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクへのアクセスを編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクへのアクセス権を管理 </p> <p>プロジェクトへの参加またはそれ以上のアクセス権</p>  </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## プロジェクトからテンプレート情報を削除するオプション

プロジェクトに追加されたテンプレート情報を削除するには、以下のいずれかの操作を行います。

* テンプレートを添付した後で、手動でプロジェクトから情報を削除します。

  詳しくは、[プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

* プロジェクト内の、テンプレートと共に追加されたタスクを削除します。

  詳しくは、この記事にある[テンプレートから作成したタスクを削除](#delete-tasks-created-from-a-template)の節を参照してください。

* Workfrontからテンプレートを削除します。 Workfront からテンプレートを削除しても、テンプレートから追加されたタスクはプロジェクトから削除されません。

  詳しくは、[プロジェクトテンプレートを削除](../../../manage-work/projects/create-and-manage-templates/delete-templates.md)を参照してください。

## テンプレートから作成したタスクを削除 {#delete-tasks-created-from-a-template}

1. プロジェクトの「**タスク**」セクションに移動します。
1. 次のいずれかの操作を行います。

   * テンプレートから作成されたタスクのみを表示するタスクリストのフィルターを、次のステートメントを使用して作成します。

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     フィルターの作成について詳しくは、[Adobe Workfrontでフィルターを作成または編集](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

     フィルターを適用すると、テンプレートタスク ID に関連付けられたタスクのみがリストに表示されます。

   * タスクリストのビューを作成して、列に「**テンプレートタスク ID**」フィールドまたは「**テンプレートタスク名**」フィールドを表示します。

     ビューを適用すると、テンプレートタスク ID 列、またはテンプレートタスク名列に情報を含むタスクがテンプレートを使用して作成されます。

     ビューの作成について詳しくは、[Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)を参照してください。

1. テンプレートから作成された手順2で特定されたすべてのタスクを選択し、**削除アイコン**&#x200B;**>はい、削除**&#x200B;をクリックします。 詳しくは、[タスクの削除](../../../manage-work/tasks/manage-tasks/delete-tasks.md)を参照してください。
