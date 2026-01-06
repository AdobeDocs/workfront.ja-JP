---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートを削除
description: プロジェクトに関する履歴情報を長期にわたって保持できるように、使用しなくなったテンプレートは削除するのではなく、非アクティブ化することをお勧めします。
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 91%

---

# プロジェクトテンプレートを削除

プロジェクトに関する履歴情報を長期にわたって保持できるように、使用しなくなったテンプレートは削除するのではなく、非アクティブ化することをお勧めします。テンプレートの非アクティブ化について詳しくは、[プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。

>[!IMPORTANT]
>
>テンプレートを削除しても、そのテンプレートを使用しているプロジェクトはまったく変更されません。ただし、プロジェクトのテンプレートフィールドに、元のテンプレートの名前が表示されなくなります。さらに、タスクビューでプロジェクト上のタスクのテンプレートタスクの名前を表示できなくなります。プロジェクト上のテンプレートフィールドとタスク上のテンプレートタスクフィールドは、プロジェクトに最初に関連付けられていたテンプレートが削除された後は空白のままです。

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
   <td><p>標準</p> 
   <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>削除へのアクセスを含む、テンプレートへの編集アクセス</p> <td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>テンプレートを削除する権限を含む、テンプレートへの管理権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates that includes access to Delete</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the template that includes permissions to Delete it</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## テンプレートの削除に関する考慮事項

* テンプレートが添付されたときにプロジェクトに追加されたタスクは、プロジェクトに残ります。ただし、タスクに関連付けられているテンプレートタスク情報は削除されます。
* テンプレートの名前は、プロジェクトの「**概要**」サブタブの「**テンプレート**」フィールドにリスト表示されなくなります。

* 最近削除したテンプレートはごみ箱から復元できます。ごみ箱からアイテムを復元する方法については、[削除したアイテムの復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください。

## テンプレートを削除

{{step1-to-templates}}

これにより、テンプレートのリストが開きます

1. テンプレート名の左側にあるチェックボックスをクリックして、削除するテンプレートを選択し、**「削除」／「はい、削除します」**&#x200B;をクリックして削除を確定します。

   または

   アクセスするテンプレートの名前をクリックし、**詳細** メニュー ![ 詳細アイコン ](assets/more-icon.png) をクリックして、**テンプレートを削除/はい、削除** をクリックします。

   テンプレートが利用できなくなり、プロジェクトに関連付けることができなくなります。
