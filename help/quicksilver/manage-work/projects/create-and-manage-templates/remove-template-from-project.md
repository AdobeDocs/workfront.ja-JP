---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトからテンプレート情報を削除
description: プロジェクトからテンプレートを削除することはできません。テンプレートがプロジェクトに添付された後にプロジェクトに追加された情報は、手動でのみ削除することができます。テンプレートの添付について詳しくは、プロジェクトにテンプレートを添付を参照してください。
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 97%

---

# プロジェクトからテンプレート情報を削除

プロジェクトからテンプレートを削除することはできません。テンプレートがプロジェクトに添付された後にプロジェクトに追加された情報は、手動でのみ削除することができます。テンプレートの添付について詳しくは、[プロジェクトにテンプレートを添付](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規：標準</p>
   <p>現在：ワーク以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクへのアクセスを編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクへのアクセス権を管理 </p> <p>プロジェクトへの参加またはそれ以上のアクセス権 </p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プロジェクトからテンプレート情報を削除するオプション

プロジェクトに追加されたテンプレート情報を削除するには、以下のいずれかの操作を行います。

* テンプレートを添付した後で、手動でプロジェクトから情報を削除します。

  詳しくは、[プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

* プロジェクト内の、テンプレートと共に追加されたタスクを削除します。

  詳しくは、この記事にある[テンプレートから作成したタスクを削除](#delete-tasks-created-from-a-template)の節を参照してください。

* Workfront からテンプレートを削除します。Workfront からテンプレートを削除しても、テンプレートから追加されたタスクはプロジェクトから削除されません。

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

1. ステップ 2 でテンプレートから作成されたものとして特定されたすべてのタスクを選択し、**「削除」アイコン**&#x200B;**／はい、削除します** をクリックします。詳しくは、[タスクの削除](../../../manage-work/tasks/manage-tasks/delete-tasks.md)を参照してください。
