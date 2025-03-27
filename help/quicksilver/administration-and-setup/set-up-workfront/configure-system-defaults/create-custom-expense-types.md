---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Create Custom Expense Types
description: ' [!DNL Adobe Workfront]  管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。費用は、タスクやプロジェクトに関連付けることができる労力以外のコストです。'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: ff4a9b317bd75b298a7a39814b4ae265c92c6d2a
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 82%

---

# カスタム費用タイプを作成

{{highlighted-preview}}

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

[!DNL Adobe Workfront] 管理者は、カスタム費用タイプを作成して、タスクやプロジェクトに関連する費用を定義および追跡できます。費用は、タスクやプロジェクトに関連付けることができる労力以外のコストです。

作成した費用タイプは、編集や削除することができます。組み込みの [!DNL Workfront] 費用タイプは、削除したり編集したりすることができません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規：[!UICONTROL Standard]</p>
   または
   <p>現在：[!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Default expense types

The default expense types in [!DNL Workfront] that cannot be deleted or edited include the following:

* [!UICONTROL 広告宣伝費]
* [!UICONTROL コンサルティング]
* [!UICONTROL 接待交際費]
* [!UICONTROL 一般]
* [!UICONTROL 部材費]
* [!UICONTROL 交通費]

## カスタム費用タイプを作成

{{step-1-to-setup}}

1. 「**[!UICONTROL 費用タイプ]**」をクリックします。
1. Click **[!UICONTROL New expense type]**.
1. In the **[!UICONTROL New Expense Type]** dialog box, specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>費用の名前を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>費用の説明を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Calculated Unit]</td> 
      <td> <p>費用タイプの測定単位をドロップダウンリストから選択します。</p> <p>以下の測定単位が使用できます。</p> 
       <ul> 
        <li>マイル</li> 
        <li>キロメートル</li> 
        <li>キログラム</li> 
        <li>ドル</li> 
        <li>ドル</li> 
        <li>日</li> 
        <li>その他 - このオプションを選択すると、測定単位に名前を付け、測定単位を組織にとってなじみのあるものとして定義するよう求められます。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">レート</td> 
      <td> <p>単位あたりの価格を指定します。これは通貨形式のフィールドで、<strong>[!UICONTROL Calculated Unit]</strong>フィールドで確立された各ユニットのコストを表します。 </p> <p>レートには、小数点以下 4 桁までの数値を含めることができます。例えば、1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Create Expense Type** <span class="preview">or **[!UICONTROL Save]**.</span>

   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

## Modify custom expense types

{{step-1-to-setup}}

1. 「**[!UICONTROL 費用タイプ]**」をクリックします。
1. 変更する費用タイプを選択してから、「**[!UICONTROL 編集]**」をクリックします。

   The **[!UICONTROL Edit Expense Type]** dialog box appears.

1. Make your desired changes, then click **Save Changes** <span class="preview">or **[!UICONTROL Save]**.</span>

   これで、ユーザーが費用タイプをプロジェクトとタスクの費用に関連付けることができるようになりました。

費用の使用方法とプロジェクトのコストに与える影響に関して詳しくは、「[プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md)」の記事を参照してください。
