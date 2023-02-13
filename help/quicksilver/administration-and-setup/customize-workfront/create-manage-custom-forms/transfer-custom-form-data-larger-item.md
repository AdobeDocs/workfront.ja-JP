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
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# オブジェクトの変換時にカスタムフォームデータを転送する

組織のビジネスニーズに応じて、タスクまたはイシューで定義された作業が大きすぎて、タスクまたはイシュー内でタスクを管理できない場合があります。 この場合、大きな作業項目に変換できます。

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

## 最初：カスタムフォームをコピーする {#first-copy-the-custom-form}

まず、変換するタスクまたは問題に関するカスタムフォームデータを確実に保持する必要があります。 カスタムフォームデータは変換後の項目と完全に一致する必要があるので、新しいオブジェクトに添付できるようにフォームを複製することをお勧めします。

>[!TIP]
>
>この状況でカスタムフォームデータを保持するもう 1 つの方法は、より大きなオブジェクトタイプをカスタムフォームに追加することです。 手順については、 [カスタムフォームの編集を開始](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) 記事内 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **カスタムForms**.
1. タスクタイプまたは問題報告タイプのカスタムフォームを選択し、 **コピー**.
1. 内 **カスタムフォーム** ダイアログボックスで、新しいフォームの名前を指定します。

1. 次の **フォームタイプ** ドロップダウンメニューから、新しいカスタムフォームを作成するオブジェクトの種類を選択します。

   **例：** カスタムフォームデータをプロジェクトに転送する場合は、「プロジェクト」を選択します。

1. クリック **フォームをコピー**.

   コピーしたカスタムフォームをタスクまたはプロジェクトに添付できるようになりました。

1. 続行： [2 番目：問題またはタスクを変換し、カスタムフォームデータを転送する](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## 2 番目：問題またはタスクを変換し、カスタムフォームデータを転送する {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 変換する問題やタスクに関するカスタムフォームをコピーします。詳しくは、 [最初：カスタムフォームをコピーする](#first-copy-the-custom-form) 」を参照してください。
1. イシューまたはタスクを変換するには、 **カスタムForms** オプションが表示され、コピーしたカスタムフォームを選択します。 手順については、次の記事を参照してください。

   * [イシューをAdobe Workfrontのプロジェクトに変換する](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [イシューのAdobe Workfrontでのタスクへの変換](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [タスクをプロジェクトに変換する](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 内 **変換後（オブジェクトタイプ）** 表示されるダイアログボックスで、 **Formsを追加** ドロップダウンメニューから、前の節でコピーしたフォームを選択します。

   問題のカスタムフィールドで取り込まれた情報が、タスクのカスタムフォームに転送されるようになりました。

