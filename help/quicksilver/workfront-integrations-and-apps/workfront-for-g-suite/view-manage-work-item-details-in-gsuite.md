---
product-area: workfront-integrations;projects
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: Google Workspaceからの [!DNL Adobe Workfront]  オブジェクトの詳細の表示と管理
description: Google Workspaceを離れることなく、作業項目の詳細を表示および管理できます。 例えば、Google Workspaceでは、 [!DNL Adobe Workfront] 内でタスクの説明を読み取り、親オブジェクトを表示し、ステータスを変更し、完了としてマークできます。
author: Becky
feature: Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 0f15b05f-3b4a-4f0b-9d9a-21a0f97de1ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 12%

---

# [!DNL Google Workspace] から [!DNL Adobe Workfront] オブジェクトの詳細を表示および管理

>[!IMPORTANT]
>
>そこで、より安定したスケーラブルな統合を提供するために、Adobe Workfrontは、Workfront Automation and Integration （Fusion）を利用した、最新の柔軟な統合アプローチに移行しました。 この移行プロセスの一環として、次のGoogle Workspace向けWorkfront機能&#x200B;**は使用できなくなりました**。
>
>* WorkfrontからGoogle Workspaceの機能にアクセスする
>
>* GmailまたはGoogle カレンダーサイトパネルからのWorkfront タスクの表示と管理
>
>組織のGoogle Workspaceとの統合ニーズには、Workfront Automation and Integrationを使用することをお勧めします。
>
>Workfront の自動処理と統合の概要について詳しくは、[Adobe Workfront Fusion の概要](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)を参照してください。
>
>Google WorkspaceのWorkfront Automation and Integration モジュールの具体的な機能について詳しくは、[Gmail modules](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)および[Google Calendar modules](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)を参照してください。

<!--

You can view and manage the details of a work item without leaving [!DNL Google Workspace]. For example, you can read a task's description, view its parent object, change its status, and mark it as complete, all within [!DNL Adobe Workfront for Google Workspace].

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p><p>Work or higher</p>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you can view and manage work item details in [!DNL Google Workspace], you must

* Install [!DNL Workfront for Google Workspace]\
   For instructions, see [Install [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## View and manage work item details in [!DNL Google Workspace]

1. If the [!UICONTROL Workfront for Google Workspace] panel is not displayed, click the [!DNL Workfront] icon ![Workfront icon](assets/wf-lion-icon.png) in the [!DNL Google Workspace] add-ons sidebar at the far-right of the page.
1. Go to the [!DNL Workfront] task or issue within [!DNL Google Workspace], as described in [Access [!DNL Adobe Workfront] [!UICONTROL Home] content from [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/access-wf-home-content-from-g-suite.md).

   When you select a task or issue, the **[!UICONTROL Details]** tab is open. The area above the **[!UICONTROL Details]** tab displays the name of the parent object, the name of the task or issue, and the [!UICONTROL Due date] (if it's a task) or [!UICONTROL Priority date] (if it's an issue).


   You can do various tasks on this tab without leaving [!DNL Google Workspace], including the following:

   * View the object's **[!UICONTROL Description]** and other details, such as the users assigned to the object, the **[!UICONTROL Priority]**, the requester, the **[!UICONTROL Planned completion date]**, and any custom fields and forms attached to the object.

      Custom forms display only fields where information has been added.

   * Click the **[!UICONTROL Parent project]** area to view the details of the parent object.

      >[!TIP]
      >
      >This can be helpful when you have tasks and issues with the same name and you need to differentiate them.

   * Accept work assigned to you by clicking **[!UICONTROL Work on it]**.
   * Edit various options, such as **[!UICONTROL Done]** option, the **[!UICONTROL Status]**, and the **[!UICONTROL Percent complete]**.

      Under **[!UICONTROL Percent complete]**, type numbers and (optionally) the percentage sign % to indicate your progress on an item.
   * View information about an approval request, including the owner, size, and any attachments.
   * **[!UICONTROL Approve]** or **[!UICONTROL Reject]** approval requests and documents.

   * **[!UICONTROL Grant]** or **[!UICONTROL Ignore]** access requests.

1. (Optional) Click **[!UICONTROL View in [!DNL Workfront]]** to go to the current work item in [!DNL Workfront].

* For information about using the [!UICONTROL Updates] tab in [!DNL Workfront for Google Workspace], see [Update an [!DNL Adobe Workfront] object from [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/update-a-workfront-object-in-gsuite.md).
* For information about using the [!UICONTROL Documents] tab in [!DNL Workfront for Google Workspace], see [View and manage documents from [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/view-and-manage-documents-in-gsuite.md).

-->
