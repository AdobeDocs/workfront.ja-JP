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
source-git-commit: dc4b6dc284c59281206a457395765e634067ba91
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 94%

---

# オブジェクトの変換時におけるカスタムフォームデータの転送

組織のビジネスニーズによっては、タスクまたはイシューで定義された作業が大きすぎて、タスクまたはイシュー内で管理できない場合があります。この場合、それらをより大きな作業項目に変換できます。

* イシューをタスクまたはプロジェクトに変換
* タスクをプロジェクトに変換

カスタムフォームデータをイシューからタスクまたはプロジェクトに転送するには、この記事の 2 つのタスクを以下の順序で完了する必要があります。

詳しくは、[Adobe Workfront でのイシュー変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)または [Adobe Workfront でのイシュー変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> </td> 
  </tr>  
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## &#x200B;1. カスタムフォームにオブジェクトを追加

{{step-1-to-setup}}

1. 「**カスタムフォーム**」をクリックします。
1. 必要なフォームを見つけて、![編集アイコン](assets/edit-icon.png) をクリックします。
1. フォームの上部に、タスクまたはイシューを変換する予定のオブジェクトを追加します。

   >[!INFO]
   >
   >**例**：カスタムフォームデータをプロジェクトに転送する場合は、プロジェクトを選択します。

1. フォームの下部にある「**適用**」をクリックします。

1. [2. イシューまたはタスクを変換し、カスタムフォームデータを転送](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data)へ進みます。

## &#x200B;2. イシューまたはタスクを変換し、カスタムフォームデータを転送 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. この記事の [1. カスタムフォームにオブジェクトを追加](#first-add-additonal-objects-to-the-custom-form)の節で説明したように、変換するイシューまたはタスクのカスタムフォームにオブジェクトを追加します。
1. 必要なカスタムフォームを選択するために表示されるボックスの「**カスタムフォーム**」オプションを使用して、イシューまたはタスクを変換します。手順について詳しくは、次の記事を参照してください。

   * [イシューをプロジェクトに変換](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [イシューをタスクに変換](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
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
