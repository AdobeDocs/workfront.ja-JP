---
title: オブジェクトの変換時にカスタムフォームデータを転送
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 作業項目に定義された作業が大きすぎる場合は、それをより大きな作業項目に変換できます。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 95%

---

# オブジェクトの変換時におけるカスタムフォームデータの転送

組織のビジネスニーズによっては、タスクまたはイシューで定義された作業が大きすぎて、タスクまたはイシュー内で管理できない場合があります。この場合、それらをより大きな作業項目に変換できます。

* イシューをタスクまたはプロジェクトに変換
* タスクをプロジェクトに変換

カスタムフォームデータをイシューからタスクまたはプロジェクトに転送するには、この記事の 2 つのタスクを以下の順序で完了する必要があります。

詳しくは、[Adobe Workfront でのイシュー変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)または [Adobe Workfront でのイシュー変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 1. カスタムフォームにオブジェクトを追加

{{step-1-to-setup}}

1. 「**カスタムフォーム**」をクリックします。
1. 必要なフォームを見つけて、![編集アイコン](assets/edit-icon.png) をクリックします。
1. フォームの上部に、タスクまたはイシューを変換する予定のオブジェクトを追加します。

   >[!INFO]
   >
   >**例**：カスタムフォームデータをプロジェクトに転送する場合は、プロジェクトを選択します。

1. フォームの下部にある「**適用**」をクリックします。

1. [2. イシューまたはタスクを変換し、カスタムフォームデータを転送](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data)へ進みます。

## 2. イシューまたはタスクを変換し、カスタムフォームデータを転送 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. この記事の [1. カスタムフォームにオブジェクトを追加](#first-add-additonal-objects-to-the-custom-form)の節で説明したように、変換するイシューまたはタスクのカスタムフォームにオブジェクトを追加します。
1. 必要なカスタムフォームを選択するために表示されるボックスの「**カスタムフォーム**」オプションを使用して、イシューまたはタスクを変換します。手順について詳しくは、次の記事を参照してください。

   * [Adobe Workfront でのイシューからプロジェクトへの変換](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Adobe Workfront でのイシューのタスクへの変換](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [タスクをプロジェクトに変換](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 表示される&#x200B;**（オブジェクトタイプ）に変換**&#x200B;ダイアログボックスで、**フォームを追加**&#x200B;ドロップダウンメニューをクリックし、前の節でコピーしたフォームを選択します。

   イシューのカスタムフィールドでキャプチャした情報が、タスクのカスタムフォームに転送されるようになりました。


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->