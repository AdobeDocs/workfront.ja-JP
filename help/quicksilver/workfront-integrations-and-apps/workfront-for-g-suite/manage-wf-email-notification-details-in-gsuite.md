---
product-area: workfront-integrations
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: Google Workspaceから [!DNL Adobe Workfront] 通知の詳細を管理
description: Google Workspaceでは、Adobe [!DNL Workfront] が送信した通知メールを開くと、関連する作業項目の詳細を表示し、受信トレイから離れることなく応答できます。 リクエストの承認など、アクションが利用可能な場合は、Workfrontから直接Google Workspaceに対してアクションを実行できます。
author: Becky
feature: Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 11%

---

# [!DNL Google Workspace] からの [!DNL Adobe Workfront] 通知の詳細の管理

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
>Workfront の自動処理と統合の概要について詳しくは、[Adobe Workfront Fusion の概要](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)を参照してください。
>
>Google WorkspaceのWorkfront Automation and Integration モジュールの具体的な機能について詳しくは、[Gmail modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)および[Google Calendar modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)を参照してください。

<!--

In [!DNL Google Workspace], when you open a notification email [!DNL Adobe Workfront] has sent, you can view the associated work item details and respond without leaving your [!UICONTROL Inbox]. If actions are available, such as approving a request, you can perform those actions directly from [!DNL Workfront for Google Workspace].

>[!NOTE]
>
> [!DNL Workfront for Google Workspace] supports almost every type of email notification you can receive from [!DNL Workfront] (about 120 different types). [!UICONTROL Daily digest] emails sent from [!DNL Workfront] do not appear in [!DNL Workfront for Google Workspace]. For information about the [!DNL Workfront] email notification types, see [Modify your own email notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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

Before you can manage notification details from [!DNL Google Workspace], you must

* Install [!DNL Workfront for Google Workspace]\
   For instructions, see [Install [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Manage [!DNL Adobe Workfront] notification details from [!DNL Google Workspace]

1. If the [!DNL Workfront for Google Workspace] panel is not displayed, click the [!DNL Workfront] icon ![Workfront icon](assets/wf-lion-icon.png) in the [!DNL Google Workspace] add-ons sidebar at the far-right of the page.
1. In [!DNL Google Workspace], open a [!DNL Workfront] notification email.
1. Click **[!UICONTROL View all updates]** if it is displayed near the top of the panel.
1. Click **[!UICONTROL Details]**.
1. Click any available options.

   The options that might display relate to the type of email notification you have opened. For example, if it's an email notification asking you to approve a task, you see **[!UICONTROL Approve]** and **[!UICONTROL Reject]** instead of options such as **[!UICONTROL Work on It]** or **[!UICONTROL Done]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type of email notification</th> 
      <th>Action</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Task or issue</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, <strong>[!UICONTROL Ignore]</strong> a request for access to it, <strong>[!UICONTROL Work on it]</strong>, or click an option to indicate that you are <strong>[!UICONTROL Done]</strong> with it</td> 
     </tr> 
     <tr> 
      <td>Project</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, or <strong>[!UICONTROL Ignore]</strong> a request for access to it</td> 
     </tr> 
     <tr> 
      <td>Document</td> 
      <td><strong>[!UICONTROL Approve]</strong> it, <strong>[!UICONTROL Reject]</strong> it, <strong>[!UICONTROL Grant]</strong> access to it, or <strong>[!UICONTROL Ignore]</strong> a request for access to it</td> 
     </tr> 
     <tr> 
      <td>Update </td> 
      <td> <p>View any part of the entire list of updates for the item so that you have the context you need to <strong>[!UICONTROL Post]</strong> a new update or a <strong>[!UICONTROL Reply]</strong>. You can click <strong>[!UICONTROL Notify]</strong> to alert particular users about your reply. </p> <p>For more information, see <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">Reply to a [!DNL Adobe Workfront] update notification from [!DNL Google Workspace]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Approval request</td> 
      <td><strong>[!UICONTROL Approve]</strong> or <strong>[!UICONTROL Reject]</strong> it (you can change your mind by clicking the other option), download it, view its owner, or view its reference number</td> 
     </tr> 
     <tr> 
      <td>A change in a project's status</td> 
      <td> View all the current information about the project, including any custom forms. </td> 
     </tr> 
    </tbody> 
   </table>

   -->
