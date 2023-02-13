---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトからテンプレート情報を削除する
description: プロジェクトからテンプレートを削除することはできません。 手動で削除できるのは、テンプレートをプロジェクトにアタッチした後にプロジェクトに追加された情報のみです。 テンプレートの添付については、「プロジェクトへのテンプレートの添付」を参照してください。
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# プロジェクトからテンプレート情報を削除する

プロジェクトからテンプレートを削除することはできません。 手動で削除できるのは、テンプレートをプロジェクトにアタッチした後にプロジェクトに追加された情報のみです。 テンプレートのアタッチについて詳しくは、 [プロジェクトへのテンプレートの添付](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクへのアクセスを管理 </p> <p>プロジェクトへのコントリビューションまたはそれ以上のアクセス権 </p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトからテンプレート情報を削除するオプション

プロジェクトに追加されたテンプレート情報を削除するには、次のいずれかの操作を行います。

* テンプレートを添付した後で、手動でプロジェクトから情報を削除します。

   詳しくは、 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

* テンプレートと共に追加されたプロジェクト内のタスクを削除します。

   詳しくは、 [テンプレートから作成したタスクを削除](#delete-tasks-created-from-a-template) 」の節を参照してください。

* Workfrontからテンプレートを削除します。 Workfrontからテンプレートを削除しても、テンプレートから追加されたタスクはプロジェクトから削除されません。

   詳しくは、 [プロジェクトテンプレートを削除](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## テンプレートから作成したタスクを削除 {#delete-tasks-created-from-a-template}

1. 次に移動： **タスク** プロジェクトのセクション。
1. 次のいずれかの操作を行います。

   * 次のステートメントを使用して、テンプレートから作成されたタスクのみを表示するタスクリスト用のフィルターを作成します。

      ```
      Task >> Template Task ID >>Is Not Blank
      ```

      フィルターの作成について詳しくは、 [Adobe Workfrontでフィルターを作成または編集](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

      フィルターを適用すると、テンプレートタスク ID に関連付けられたタスクのみがリストに表示されます。

   * タスクリストのビューを作成して、 **テンプレートタスク ID** または **テンプレートタスク名** 列のフィールド。

      ビューを適用すると、「テンプレートタスク ID 」列または「テンプレートタスク名」列に情報が含まれるタスクが、テンプレートを使用して作成されます。

      ビューの作成について詳しくは、 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 手順 2 で特定されたすべてのタスクをテンプレートから選択し、「 **削除アイコン****> はい、削除します**。 詳しくは、 [タスクを削除](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
