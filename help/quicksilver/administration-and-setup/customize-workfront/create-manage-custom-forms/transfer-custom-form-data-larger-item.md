---
title: オブジェクトの変換時にカスタムフォームデータを転送する
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 作業項目で定義した作業が大きすぎる場合は、大きい作業項目に変換できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 7b378fdf3530d5e1c06f09d03c23c31afac6aa47
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# オブジェクトの変換時にカスタムフォームデータを転送する

組織のビジネスニーズに応じて、タスクまたはイシューで定義された作業が大きすぎて、タスクまたはイシュー内で管理できない場合があります。 この場合、大きな作業項目に変換できます。

* 問題をタスクまたはプロジェクトに変換できます
* タスクをプロジェクトに変換できます

イシューからタスクまたはプロジェクトにカスタムフォームデータを転送するには、この記事の 2 つのタスクを、次の順序で実行する必要があります。

詳しくは、 [Adobe Workfrontでの変換の問題の概要](../../../manage-work/issues/convert-issues/convert-issues.md) または [Adobe Workfrontでの変換の問題の概要](../../../manage-work/issues/convert-issues/convert-issues.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス</p> <p>Workfront管理者がこのアクセス権を付与する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスタイプ、アクセスレベル設定を確認するには、Workfront管理者に問い合わせてください。

## 最初：カスタムフォームに追加のオブジェクトを追加する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **カスタムForms**.
1. 必要なフォームを見つけて、 **編集**.
1. フォームの上部に、タスクまたはイシューを変換するオブジェクトを追加します。
   >[!INFO]
   >
   >**例**:カスタムフォームデータをプロジェクトに転送する場合は、「プロジェクト」を選択します。

1. クリック **適用** をクリックします。

1. 続行： [2 番目：問題またはタスクを変換し、カスタムフォームデータを転送する](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## 2 番目：問題またはタスクを変換し、カスタムフォームデータを転送する {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 変換する問題やタスクのカスタムフォームに、追加のオブジェクトを追加します。詳しくは、「 [最初：カスタムフォームにオブジェクトを追加する](#first-add-additonal-objects-to-the-custom-form) 」を参照してください。
1. イシューまたはタスクを変換するには、 **カスタムForms** オプションが表示され、必要なカスタムフォームを選択します。 手順については、次の記事を参照してください。

   * [イシューをAdobe Workfrontのプロジェクトに変換する](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [イシューのAdobe Workfrontでのタスクへの変換](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [タスクをプロジェクトに変換する](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 内 **変換後（オブジェクトタイプ）** 表示されるダイアログボックスで、 **Formsを追加** ドロップダウンメニューから、前の節でコピーしたフォームを選択します。

   問題のカスタムフィールドで取り込まれた情報が、タスクのカスタムフォームに転送されるようになりました。


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see the section [Start editing a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->