---
product-area: workfront-integrations;projects
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: メールコンテンツを使用したGoogle Workspaceからのア  [!DNL Adobe Workfront]  テムの更新
description: Adobe Workfront 以外のメールに含まれている情報を使用して、既存のプロジェクト、タスクまたはイシューを更新できます。
author: Becky
feature: Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: ddd1c964c4c885f71dfa30d1790cfbc6e26d6781
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 26%

---

# メールコンテンツを使用した [!DNL Google Workspace] からの [!DNL Adobe Workfront] アイテムの更新

>[!IMPORTANT]
>
>より安定した拡張性の高い統合を実現するために、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しました。 このトランジションプロセスの一環として、Google Workspaceの次のWorkfront機能は **使用できなくなりました**。
>
>* Workfront内からのGoogle Workspace機能へのアクセス
>
>* Gmail またはWorkfrontのカレンダーサイトパネルからのGoogle タスクの表示と管理
>
>Google Workspaceを使用した組織の統合のニーズに対しては、Workfront Automation and Integration を使用することをお勧めします。
>
>Workfront の自動処理と統合の概要について詳しくは、[Adobe Workfront Fusion の概要](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)を参照してください。
>
>Google WorkspaceのWorkfront Automation and Integration モジュールの具体的な機能については、{Gmail モジュール [&#x200B; および &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)2}Google カレンダーモジュール [&#x200B; を参照してください。](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)

<!--

You can update an existing project, task, or issue with information from a non-[!DNL Adobe Workfront] email.

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

Before you can update a [!DNL Workfront] item using email content from [!DNL Google Workspace], you must

* Install [!DNL Workfront for Google Workspace]\
   For instructions, see [Install [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Update a [!DNL Workfront] item using email content from [!DNL Google Workspace]

1. If the [!UICONTROL Workfront for Google Workspace] panel is not displayed, click the Workfront icon ![Workfront icon](assets/wf-lion-icon.png) in the [!DNL Google Workspace] add-ons sidebar at the far-right of the page.
1. With the email message open in [!DNL Google Workspace], click **[!UICONTROL Post as a new update]** in the [!DNL Google Workspace] panel.
1. Under **[!UICONTROL Type]**, click the drop-down arrow, then click the type of object where you want to add the update.
1. Click the **[!UICONTROL Search for]** option, start typing the name of the object where you want to add the update, then select the item when it appears in the list below.

   This option varies, depending on what you selected in step 3. It might be **[!UICONTROL Search for a project]**, **[!UICONTROL Search for a task]**, or **[!UICONTROL Search for an issue]**.

   >[!NOTE]
   >
   >When you are typing the name of a task, ad hoc personal tasks are excluded from the list of name that appears below.

1. Make any of these optional changes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>Edit any part of this text, which is taken from the email's subject line and body text.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td><p>(Available only if the email contains at least one attachment.) Click this option to save attachments in the [!UICONTROL Documents] tab for the task or issue. </p><p>If you do not want to save an attachment, click the X to the right of its name. </p><p>If the email contains links to documents in [!DNL Google Drive], the links are saved to the [!UICONTROL Overview] tab of the task or issue you are creating. </p><p>Important: <span style="color: #ff1493;"><span style="color: #000000;">In order for this to work, your</span></span>[!DNL Workfront] administrator<span style="color: #ff1493;"><span style="color: #000000;"> must authorize [!DNL Google Drive] to work with [!DNL Workfront]</span></span></p>
      <p>If you enable this option, it remains enabled for other emails you convert to tasks, issues, and updates.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notify</td> 
      <td>Click <strong>[!UICONTROL Notify]</strong>, click the <strong>[!UICONTROL Search for a user or team]</strong> option that appears, then start typing the name of the person or team and click it when it appears in the list below. Repeat this for each person and team you want to add, then click <strong>[!UICONTROL Save]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Update]**.

   When you refresh your browser, a message with a link at the bottom of the [!DNL Workfront for Google Workspace] panel confirms that you have converted the email to an update:

   You can click the link to go to the [!UICONTROL Updates] tab in [!DNL Workfront] for the object you specified in step 4.

   You can repeat these steps to convert the same email to updates, task, and issues (see [Create an Adobe Workfront issue in [!DNL Google Workspace] using email content](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). When you refresh your browser or return to the email at another time, all links you have created for the email are listed at the bottom of the [!UICONTROL Workfront for Google Workspace] panel.

1. (Optional) Continue to work with the update in the [!DNL Workfront] add-on panel by doing any of the following:

   * To add another update on the **[!UICONTROL Updates]** tab, click **[!UICONTROL Start a new update]** and type the information.

   * To reply to an update on the **[!UICONTROL Updates]** tab, click **[!UICONTROL Reply]** and type your reply.

      For both of the options above, you can click **[!UICONTROL Notify]** to specify recipients for the reply as in step 5. When you are ready, click **[!UICONTROL Post]** to add the update or reply.

   * Click the **[!UICONTROL Details]** tab to view the details for the new project, task, or issue.

   -->
