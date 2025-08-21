---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: リクエストキューを作成
description: ユーザーがプロジェクトの予定作業ではない臨時のリクエストを入力できるよう、リクエストキューを設定できます。例えば、IT 部門に寄せられるすべてのユーザーリクエストを取り込むよう、ヘルプデスクのリクエストキューを設定できます。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: ce611ec0c91b114f1a10977970e42fa753f62f22
workflow-type: tm+mt
source-wordcount: '2868'
ht-degree: 65%

---


# リクエストキューを作成

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

<!--hide/ comment out the entire "create requests in Production" section and just edit and leave  only the preview section when it releases to Production; also remove the template blurb when the queue details is unshimmed for templates-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


ユーザーがプロジェクトの予定作業ではない臨時のリクエストを入力できるよう、リクエストキューを設定できます。例えば、IT 部門に寄せられるすべてのユーザーリクエストを取り込むよう、ヘルプデスクのリクエストキューを設定できます。

リクエストはAdobe Workfrontでイシューになり、プロジェクトに追加されます。

リクエストキューを設定すると、プロジェクトに追加されるイシューに関する情報を形式化するのに役立ちます。 プロジェクトに送信されたすべての問題は、同じ方法で送信され、同じパスに従って完了します。

Workfrontでは、リクエストキューとして次のオブジェクトを設定できます。

* プロジェクト
* テンプレート。 リクエストキューとして設定されたテンプレートから作成されたプロジェクトは、リクエストキューになります。

プロジェクトまたはテンプレートをリクエストキューとして設定するには、プロジェクトまたはテンプレートの「キューの詳細」領域を編集する必要があります。

この記事では、ユーザーがリクエストを送信できるリクエストキューとしてプロジェクトを設定する方法について説明します。 テンプレートのキューの詳細の設定は、プロジェクトでのキューの詳細の設定に似ています。

リクエストキューに新しいリクエストを送信する方法について詳しくは、[リクエストのコピーと送信](../create-requests/copy-and-submit-requests.md)を参照してください。

Adobe Workfront Planning でリクエストフォームを設定する方法については、[Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>新規のライセンス：標準 </p>
   または
   <p>現在のライセンス：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p> プロジェクトの管理権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リクエストキューの概要

リクエストキューをプロジェクトとして設定します。プロジェクトをリクエストキューとして指定すると、Adobe Workfront のリクエストエリアからキューにアクセス可能になります。リクエストキューをカスタマイズすると、ユーザーがリクエストを送信する際に入力するフォームもカスタマイズされます。

この記事では、既存のプロジェクトからリクエストキューを作成する方法について説明します。ただし、リクエスト取り込みプロセスの一貫性を作成したり、レポート作成や管理の向上のために複数のレイヤーを追加したりする場合は、次の表で説明するリクエストキューの追加の構成要素を設定することもできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">キューの詳細</td> 
   <td> <p>キューの詳細エリアで、プロジェクトをリクエストキューとして設定する必要があります。この手順は必須です。 </p> <p>詳しくは、この記事の<a href="#create-a-request-queue" class="MCXref xref">リクエストキューを作成</a>の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">トピックグループ</td> 
   <td> <p>これらは、共通の機能に基づいてリクエストを分類する追加のメニューです。例えば、IT リクエストキューの場合、「オンサイト」と「リモート」のトピックグループが必要な場合があります。 </p> <p>詳しくは、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">トピックグループを作成</a>を参照してください。 </p> <p>この機能はオプションです。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">キューのトピック</td> 
   <td> <p>これらは、同じトピックグループに属するリクエストを共通の特徴に基づいて分類する追加メニューです。1 つのトピックグループには複数のキュートピックを含めることができます。 </p> <p>例えば、IT リクエストキューの「オンサイト」トピックグループには、「ハードウェア」、「ソフトウェア」、「ネットワーク」のキュートピックが含まれる場合があります。 </p> <p>詳しくは、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">キュートピックを作成</a>を参照してください。 </p> <p>この機能はオプションです。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ルーティングルール</td> 
   <td> <p>これにより、それぞれのリクエストをユーザー、担当業務、チームやプロジェクトにルーティングできます。 </p> <p>詳しくは、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">ルーティングルールの作成</a>を参照してください。 </p> <p>この機能はオプションです。</p> </td> 
  </tr> 
 </tbody> 
</table>

## リクエストキューを作成

<!--at production release on April 10, do the following: take the first sentence here out; hide/ comment out the first section (Create a Request Queue in the Production environment); remove the title of the "Create a Request Queue in the Preview environment and leave that section as the only way to create request queues; search for any visible references of production/ preview and remove them from the entire article-->

リクエストキューの作成は、使用する環境によって異なります。

<!--

### Create a Request Queue in the Production environment

This section describes how you can define Queue Details for the following objects:

* A project in the Production environment
* A template in the Production or Preview environment

When you set up a project as a Request Queue, the project status must be Current in order to display in the Requests area of Workfront.

>[!TIP]
>
>Your Workfront or group administrator might assign you to a custom Layout Template that might not include some of the sections described in the following steps.


To create a Request Queue:

1. Go to the project that you want to set up as a Request Queue.
1. (Optional) Click **Project Details** in the left panel and add a **Description** to the project in the **Overview** area. This information displays on all new requests.
1. Click **Queue Details** in the left panel. 

   This opens the Queue Details section.

   ![Queue Details top of the section](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)   

1. Specify the following information:

   * **Publish as Help Request Queue:** Select this option to identify this project as a request queue. All incoming issues are considered Requests.  
     When this option is not selected, the project behaves like a standard project in Workfront and all incoming issues are issues.
   
   * **Who can add requests to this queue:** Select which users have access to add requests to this queue. You can allow the following groups of people to see the Request Queue in their Requests area of the Global Navigation Bar when they add a new request:

     |Who can enter requests | Description|
     |---|---|
     | Anyone  |Any Workfront user with an active account can view this request queue and add requests to it |
     | People with view access to this project |Users with View permissions to the project can view and add requests to this queue |
     | People in this project's company |Users who belong to the company associated with this project can view and add requests to this queue. If there is a company associated with the project, the name of the company is listed in parentheses after this setting.  |
     | People in this project's group |Users who belong to the group associated with this project can view and add requests to this queue. If there is a group associated with the project, the name of the group is listed in parentheses after this setting, in gray font.  |

   * **Share with these links:** The following options enable you to provide direct access to the Request Queue and the forms associated with it to users outside of Workfront or to Workfront users using an external page. For information about embedding a request queue in a dashboard as an external page, see [Embed a request queue in a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Users must already have access rights to the Request Queue in order to gain direct access. Using either option described here does not automatically grant access to users.

     >[!TIP]
     >
     >Users must first log in to Workfront before gaining access to the request queue when they access the Request Queue page from another application.

      * **Direct Access URL:** When a user accesses this URL from a browser, the user is taken directly to the New Request  section in the Requests area and this request is selected by default for them.

        ![Share request queue with direct URL embedded in dashboard](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >You can display a Request Queue in a dashboard as an external page. In this case, the request queue is preselected, but you can select any other request queue from the Request Type field. users can change the Request Type. Navigation components of the Requests also display.

      * **Embed Code:** Use this HTML code to embed the request queue form as an iframe within any HTML page.  
        If users are not already authenticated to Workfront when they view the page where the code is embedded, the Workfront login dialog box is displayed. After users log in, the Request Queue form is displayed.

        >[!NOTE]
        >
        >When displaying a Request Queue in an iframe, only the request form displays, the request name is preselected and dimmed. User cannot change the Request type. Navigation components of the Requests area do not display.

        In order for the request queue form to be displayed when using this embed code, you must enable the "Allow embedding of Workfront in an iframe" setting in your system setup. For more information about enabling embedding of Workfront in an iframe, see [Configure system security preferences](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). If this setting is not enabled, the iframe is displayed as blank.

        You can adjust various aspects of how the embedded form is displayed, as follows:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Functionality</strong> </p> </th> 
           <th> <p><strong>Solution</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Adjust the size of the frame</p> </td> 
           <td> <p>Modify the "width" and "height" attributes.</p> <p>By default, the width is "500" and the height is "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direct users to a specific Queue Topic or Topic Group</p> </td> 
           <td> <p>Add the "path" parameter to the src URL. You can find the path parameter by navigating to the desired Queue Topic or Topic Group in the non-embedded form and inspecting the URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Show and allow users to change the pre-configured Topic Group drop-down list</p> </td> 
           <td> <p>Use the "path" parameter by adding the <code>showPreSelectedOptions=true</code> parameter to the <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detect when the form has been submitted</p> </td> 
           <td> <p>Add a "message" event listener to your web page's window and checking if <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> will be set to the ID of the created issue.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Request Types:** Select from the default options below.

     The Workfront administrator can rename the default request types. For more information about renaming the request types, see [Customize default issue types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Bug Report
      * Change Order
      * Issue
      * Request

        This is a required field and you must select at least one option.

     >[!NOTE]
     >
     >Request Types display as a selection in the Requests area only if the Request Type is selected in both the Queue Details and the Queue Topic pages. For information about setting up the Queue Details area of a project, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Each type selected here will be available on the form (you can select more than one). Selecting more than one type can help organize multiple requests coming in.  
     For example, if you are using the form on a request queue for an IT project, the following request types can come in to the queue: hardware, software, bug fixes, and issues.

   * **Default Duration:** The default duration is the length of time it typically takes to complete an issue. This becomes the default for all incoming issues and can be modified manually. Duration is generally set in hours, days, or weeks. The Default Duration of an issue is the same as the Planned Hours on the issue. The Planned Completion Date of the issue calculates based on this field.  
     The default for the issue Duration is 1 day or 8 hours. If your Workfront administrator set the Typical Hours per Work Day as less than 8 hours, the Default Duration for issues is still 8 hours. For example, if the Typical Hours per Work Day is set to 7 hours, the Default Duration for issues is 1.14 Days or 8 hours. For more information about how to set up the system Typical Hours per Work Day, see the "Timeline Calculations" section in the article [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
   
   * **People from the same company will inherit the same permissions for all requests.:** When selected, all requests submitted to the queue are visible for users in the same company. Users can view these requests in the All Requests  section , located within the Requests area. At the time that this setting is enabled or disabled, it impacts all future requests; it does not retroactively impact information. 
   * **When someone makes a request, automatically grant:** When a user makes a request to the request queue, the user is automatically granted the level of permission that you choose to that request. Select from the following permissions levels: 

      * **View Access** 
      * **Contribute Access**. This is the default selection.
      * **Manage Access**

     For information about the Workfront permissions model, see [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).   
     Setting permissions here saves time, rather than having to grant permissions for each individual incoming request. Choosing this option impacts all future requests, but does not retroactively impact existing requests. 
   
   * **Default Approval**: Associate an approval process with this request queue. Only Issue Approval Processes are visible in this drop-down menu. All issues submitted to this queue will be associated with this approval process. Your Workfront administrator must define system-level approval processes before you can associate them with request queues. Users with administrative access to Approval processes can also create group-specific approval processes.

     >[!IMPORTANT]
     >
     >If the group of the project changes, the group-specific approval process attached to existing issues becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see [How group and approval process changes affect assigned approval processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     If you have multiple queue topics associated with a request queue, we recommend that you associate approval processes with the queue topics instead. For more information about creating queue topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md). 
   
     Consider the following when adding approval processes to request queues:

      * Only active approval processes display in the list. 
      * System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.

   * **Default Route**: Associate a Routing Rule with this request queue. Use Routing Rules to automatically assign new issues submitted to a Request Queue to the correct resource (user, job role, or team), and to the correct project. All issues submitted to this queue will be associated with this Routing Rule. You must configure Routing Rules before they display in the Queue Details section and before you can associate them with request queue.  
     If you have multiple queue topics associated with a request queue, we recommend that you associate routing rules with the queue topics instead. For more information about creating routing rules, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
   
   * **New Issue Fields:** In the **Show the following selected fields to all users** section, select any fields that you want to be visible to all users who submit a request to the project or add an issue to the project or the tasks.

     >[!TIP]
     >
     >New Issue Fields selected in the Queue Details section are also associated with any new issue added to the project <!--this is confusing: or to the tasks in the Issues section-->.

<!--     When you enable any of the Assigned to, Job Role, or the Team fields, they are always renamed to Assignments in the request form, but you can only specify the type of assignment selected here.

      >[!NOTE]
      >
      >If you selected Assigned To in the Queue Details area, you can enter only users in the Assignments field on the request form. In this case, you cannot enter job roles or a team. 
   
   * **Documents**: If you select to display the Documents section in the new request form, select where the document uploading section should be positioned. Select from the following:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">After custom forms</td> 
        <td><span>The Documents section displays at the bottom of the request form.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Before custom forms</td> 
        <td> <p><span>The Documents section displays between the Workfront fields and the custom fields of the request form.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>   
   
     ![New issue fields area with documents](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Show all selected and unselected fields to:** Select which users you want to see all the fields on the new request form. The following options control the access to the fields on the form.
    
      |Which users can see all fields on the request form | Description|  
      |---|---| 
      | All Users (Plan Licenses) |All users who have a Plan license can see the selected as well as the unselected fields. |
      | People with view access to this project (Plan License) |Those users with a Plan license that also have View rights to this project can see the selected as well as the unselected fields. The rest of the users who can submit requests to this project can see just the selected fields. |
      | No Users |No users can see the unselected fields. All users who can submit requests to this project can only see the fields selected.  |
  
   * **Custom Forms**: Select a custom form to associate with the Request Queue. Only Issue Custom Forms are available to select from this drop-down menu. All issues submitted to the Request Queue will have the selected forms associated with them. You must create issue custom forms before you can see them displayed in the Queue Details section. 
     If you have multiple Queue Topics associated with a Request Queue, we recommend that you associate custom forms with the Queue Topics instead. For more information about creating sub-sections for the Request Queue, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Custom forms on Queue Details](assets/custom-forms-on-queue-details.png)

     If you have multiple custom forms associated with the Request Queue, drag and drop the forms to sort them in the desired order, in the **Reorder Forms** section.

     >[!TIP]
     >
     >Custom forms added to the Queue Details section are also associated with any new issue added to the project <!--this is confusiong: or the tasks in the Issues  section-->.

<!--1. Continue selecting information for the settings in the **Email Queue Settings** area, to allow users to email requests to the request queue project. 

    For more information, see [Enable users to email an issue into a Request Queue project](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Click **Save**.  
   Your project has now been configured to be a Request Queue and users can now add requests to it. 

1. (Optional) To enhance the Request Queue functionality, build additional sub-sections for your queue, as well as rules to route the incoming requests to the correct team, assignee or project.

   * For information about creating sub-sections for the Request Queue, see the articles [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) and [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).  
   * For information about routing the requests to the appropriate assignee, team, and appropriate project, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   -->


### リクエストキューを作成

プロジェクトをリクエストキューとして設定する場合、Workfront のリクエストエリアに表示するには、プロジェクトのステータスが現在になっている必要があります。

>[!TIP]
>
>Workfront 管理者またはグループ管理者が、以下の手順で説明する一部の節を含まないカスタムレイアウトテンプレートを割り当てる場合があります。

リクエストキューを作成するには、以下のように行います。

1. リクエストキューとして設定するプロジェクトに移動します。
1. （オプション）左パネルの「**プロジェクト詳細**」をクリックし、「**概要**」エリアのプロジェクトに「**説明**」を追加します。この情報は、すべての新規リクエストに表示されます。
1. 左側のパネルで **キューの詳細** をクリックします。

   「キューの詳細」セクションが開きます。

   ![ 「キューの詳細」領域の「キュータイプ」セクション ](assets/unshimmed-queue-type-section-queue-details-area.png)

1. 次の情報を指定します。

   * **ヘルプリクエストキューとして公開**：このプロジェクトをリクエストキューとして識別するには、このオプションを選択します。 受信するイシューはすべて、リクエストと見なされます。\
     このオプションを選択しない場合、プロジェクトは Workfront の標準プロジェクトのように動作し、受信するすべてのイシューがイシューになります。

   * **このキューにリクエストを追加できるユーザー**：このキューにリクエストを追加するアクセス権を持つユーザーを選択します。 次のグループのユーザーに対して、新規のリクエストを追加するとき、グローバルナビゲーションバーのリクエストエリアにリクエストキューを表示できます。

     | リクエストを入力できるユーザー | 説明 |
     |---|---|
     | 全員 | アクティブなアカウントを持つすべての Workfront ユーザーが、このリクエストキューを表示してリクエストを追加できます |
     | このプロジェクトの表示アクセス権限を持つユーザー | プロジェクトに対する表示権限を持つユーザーは、リクエストを表示してこのキューに追加できます。 |
     | このプロジェクトの会社のユーザー | このプロジェクトに関連付けられた会社に所属するユーザーは、リクエストを表示してこのキューに追加できます。プロジェクトに関連する会社がある場合、会社の名前は、この設定を行った後に括弧内に表示されます。 |
     | このプロジェクトのグループのユーザー | このプロジェクトに関連付けられたグループに所属するユーザーは、リクエストを表示してこのキューに追加できます。プロジェクトに関連するグループがある場合、グループの名前はこの設定の後に括弧内に灰色のフォントで表示されます。 |

     {style="table-layout:auto"}

   * 以下のオプションを使用して、リクエストキューとそれに関連付けられたフォームへのダイレクトアクセスを、Workfront外部のユーザー、または埋め込みの外部ページを使用するWorkfront ユーザーに提供します。

   リクエストキューを外部ページとしてダッシュボードに埋め込む方法について詳しくは、[リクエストキューをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md)を参照してください。

   ユーザーが直接アクセスするには、まずリクエストキューへの権限が必要です。 ここで説明するいずれのオプションを使用しても、ユーザーにアクセス権が自動的に付与されるわけではありません。

   >[!TIP]
   >
   >ユーザーが別のアプリケーションからリクエストキューページにアクセスする場合、リクエストキューにアクセスする前に、まず Workfront にログインする必要があります。

   * **直接アクセス URL：**&#x200B;ユーザーがブラウザーからこの URL にアクセスすると、ユーザーはリクエストエリアの「新規リクエスト」セクションに直接移動し、デフォルトではこのリクエストが選択されます。

     ![ ダイレクト URL 共有からの新しいリクエストボックス ](assets/new-request-box-from-direct-url-share.png)

     >[!NOTE]
     >
     >リクエストキューは、ダッシュボードに外部ページとして表示することができます。この場合、リクエストキューは事前に選択されていますが、「リクエストタイプ」フィールドから他の任意のリクエストキューを選択できます。リクエストを送信するユーザーは、別のリクエストタイプを選択できます。 トピックグループとキュートピックも表示されます。

   * **埋め込みコード：**&#x200B;この HTML コードを使用して、リクエストキューフォームを Iframe として任意の HTML ページ内に埋め込みます。\
     コードが埋め込まれているページを表示するときにユーザーが Workfront に対してまだ認証されていない場合は、Workfront ログインダイアログボックスが表示されます。ユーザーがログインすると、リクエストキューフォームが表示されます。

     >[!NOTE]
     >
     >Iframe にリクエストキューを表示すると、リクエストフォームのみが表示され、リクエスト名は事前に選択されていて、グレー表示されます。ユーザーはリクエストタイプを変更できません。リクエストエリアのナビゲーションコンポーネントは表示されません。

     この埋め込みコードを使用する場合にリクエストキューフォームを表示するには、Workfront管理者がシステム設定エリアの「iframe へのWorkfrontの埋め込みを許可」設定を有効にする必要があります。

     Iframe での Workfront の埋め込みの有効化について詳しくは、[システムセキュリティの環境設定を指定](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。この設定が有効になっていない場合、Iframe は空白として表示されます。

     埋め込みフォームの表示方法に関する様々な要素を、以下のように調整できます。

     <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>機能</strong> </p> </th> 
           <th> <p><strong>ソリューション</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>フレームのサイズを調整</p> </td> 
           <td> <p>「幅」属性と「高さ」属性を変更します。</p> <p>デフォルトでは、幅は「500」、高さは「600」です</p> </td> 
          </tr> 
          <tr> 
           <td> <p>特定のキュートピックまたはトピックグループにユーザーを誘導する</p> </td> 
           <td> <p>src URL に「パス」パラメーターを追加します。非埋め込みフォームで目的のキュートピックまたはトピックグループに移動し、URL を調べることにより、パスパラメーターを見つけることができます。</p> </td> 
          </tr> 
          <tr> 
           <td> <p>事前設定済みのトピックグループドロップダウンリストを表示し、ユーザーに変更を許可</p> </td> 
           <td> <p><code>showPreSelectedOptions=true</code> パラメーターを <code>src URL</code> に追加して、「パス」パラメーターを使用します。</p> </td> 
          </tr> 
          <tr> 
           <td> <p>フォームが送信されたタイミングを検出する</p> </td> 
           <td> <p>Web ページのウィンドウに「メッセージ」イベントリスナーを追加し、<code>event.data.type</code> が <code>requestSubmitted</code> であるか確認します。<code>event.data.newIssueID</code> が作成されたイシューの ID に設定されます。</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **リクエストタイプ：** 「**キューのプロパティ**」セクションで、次のオプションから選択します。

   * バグレポート
   * 変更依頼
   * イシュー
   * リクエスト

   これは必須フィールドであり、少なくとも 1 つのオプションを選択する必要があります。

   Workfront 管理者は、デフォルトのリクエストタイプの名前を変更できます。リクエストタイプの名前の変更について詳しくは、[デフォルトのイシュータイプをカスタマイズ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md)を参照してください。

   >[!NOTE]
   >
   >ユーザーが「要求」領域から要求キューにアクセスすると、「キューの詳細」ページと「キューのトピック」ページの両方で「要求タイプ」が選択されている場合にのみ、「要求タイプ」が選択として表示されます。
   >
   >プロジェクトの「キュートピック」領域の設定については、[ キュートピックの作成 ](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) を参照してください。

   ここで選択したそれぞれのタイプは、フォームで使用できます（複数選択できます）。複数のタイプを選択すると、寄せられる複数のリクエストを整理するのに役立ちます。\
   例えば、IT プロジェクトのリクエストキューでフォームを使用している場合、ハードウェア、ソフトウェア、バグ修正、イシューなどのリクエストタイプがキューに入る可能性があります。

   * **デフォルトの期間：** 期間の数値を入力し、ドロップダウンメニューから次のいずれかの期間単位を選択します。

      * 日
      * 時間
      * 分
      * 週

   デフォルトの期間は、このリクエストキューに送信されたイシューを完了するのに通常かかる時間です。 これは、すべての入力問題のデフォルトになり、手動で変更できます。
イシューのデフォルト期間は、イシューの予定時間数と同じです。イシューの予定完了日は、このフィールドに基づいて計算されます。\
   変更しない場合、イシュー期間のデフォルト値は 1 日または 8 時間です。
Workfront管理者が設定エリアで稼働日の標準的な時間数を 8 時間未満に設定した場合、イシューのデフォルト期間は 8 時間のままです。
例えば、Workfrontの設定領域で稼働日の標準的な時間数が 7 時間に設定されている場合、イシューのデフォルト期間は 1.14 日または 8 時間です。
システム稼働日の標準的な時間数の設定方法について詳しくは、[システム全体のプロジェクト環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)の記事にある、「タイムラインの計算」の節を参照してください。

   * **同じ会社のユーザーは、すべてのリクエストに対して同じ権限を継承します。**：選択すると、キューに送信されたすべてのリクエストが、同じ会社のユーザーに表示されます。 これらのリクエストは、リクエストエリア内にある、「すべてのリクエスト」のセクションに表示されます。この設定を有効または無効にすると、その後のすべてのリクエストに影響します。情報に遡及的に影響を与えることはありません。
   * **リクエストが行われると、自動的に付与する…:** リクエストキューに対してリクエストが行われると、そのリクエストに対して選択したレベルの権限がユーザーに自動的に付与されます。 「アクセス」ボタンをクリックして、次の権限レベルから選択します。

      * **表示アクセス権**
      * **参加アクセス権**&#x200B;これは、デフォルトの選択であり、「アクセス」ボタンの名前です。
      * **管理アクセス権**

     Workfront 権限モデルについて詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。\
     ここで権限を設定すると、各受信リクエストに対して個別に権限を付与する必要がなくなり、時間を節約できます。 このオプションを選択した場合、今後のすべてのリクエストに影響が及びますが、既存のリクエストに遡及的に影響を与えることはありません。

   * **デフォルトの承認**：ドロップダウンメニューをクリックして、このリクエストキューの承認プロセスを選択します。 このドロップダウンメニューには、イシューの承認プロセスのみが表示されます。このキューに送信されたすべてのイシューが、この承認プロセスに関連付けられます。リクエストキューに関連付ける前に、Workfront 管理者がシステムレベルの承認プロセスを定義する必要があります。承認プロセスへの管理者アクセス権を持つユーザーは、グループ固有の承認プロセスを作成することもできます。

     >[!IMPORTANT]
     >
     >プロジェクトのグループが変更されると、既存のイシューに付随するグループ固有の承認プロセスが、1 回限りの承認プロセスになります。プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、[グループと承認プロセスの変更が割り当てられた、承認プロセスに及ぼす影響](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md)を参照してください。

     リクエストキューに複数のキュートピックが関連付けられている場合は、代わりに承認プロセスをキュートピックに関連付けることをお勧めします。

     キュートピックの作成について詳しくは、[キュートピックを作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。

     リクエストキューに承認プロセスを追加する際は、以下の点を考慮してください。

      * アクティブなイシューの承認プロセスのみがリストに表示されます。
      * システム全体およびグループ固有のイシュー承認プロセスがリストに表示されます。 プロジェクトの承認プロセス以外のグループに関連付けられている承認プロセスは、リストに表示されません。

   * **デフォルトルート**：ドロップダウンメニューをクリックして、このリクエストキューのルーティングルールを選択します。 ルーティングルールは、リクエストキューに送信された新しいイシューを、適切なリソース（ユーザー、担当業務、チーム）と適切なプロジェクトに自動的に割り当てます。 このキューに送信されたすべての問題は、このルーティング規則に関連付けられます。 ルーティングルールは、「キューの詳細」セクションに表示してリクエストキューに関連付けることができるようにするには、事前に設定しておく必要があります。\
     複数のキュートピックがリクエストキューに関連付けられている場合は、代わりにルーティングルールをキュートピックに関連付けることをお勧めします。ルーティングルールの作成について詳しくは、[ルーティングルールを作成](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)を参照してください。

   * **新しい問題フィールド：** 「**すべてのユーザーに次の選択されたフィールドを表示**」セクションで、プロジェクトに要求を送信したり、このプロジェクトまたはプロジェクトのタスクに問題を追加するすべてのユーザーに表示するフィールドを選択します。

     >[!NOTE]
     >
     >* 「割り当て先」、「担当業務」、または「チーム」フィールドを有効にすると、ユーザーがリクエストを送信する際にリクエストフォームでは常に「割り当て」に名前が変更されます。 「キューの詳細」領域では、割り当てのタイプのみを指定できます。
     >
     >* キューの詳細エリアで「割り当て先」を選択した場合は、リクエストフォームの「割り当て」フィールドにユーザーのみを入力できます。この場合、担当業務やチームを入力することはできません。

   * **ドキュメント**：このオプションを選択すると、新しいリクエストフォームにドキュメント セクションが表示され、ドキュメントアップロードセクションの位置を選択できます。 次の中から選択します。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">カスタムフォームの後</td> 
        <td><span>「ドキュメント」セクションは、リクエストフォームの下部に表示されます。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">カスタムフォームの前</td> 
        <td> <p><span>「ドキュメント」セクションは、Workfront フィールドとリクエストフォームのカスタムフィールドの間に表示されます。</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![ 新しいイシューフィールドとキュー詳細のドキュメント ](assets/new-issue-fields-and-documents-on-queue-details.png)

   * **選択および選択解除されたすべてのフィールドを表示する先：** 新しいリクエストフォームのすべてのフィールドを表示するユーザーを選択します。 次のオプションは、フォーム上のフィールドへのアクセスを制御します。

     | リクエストフォーム上のすべてのフィールドを表示できるユーザー | 説明 |
     |---|---| 
     | すべてのユーザー（プランライセンス） | プランライセンスを持つすべてのユーザーには、選択されたフィールドと未選択のフィールドが表示されます。 |
     | このプロジェクトで表示アクセス権限を持つユーザー（プランライセンス） | このプロジェクトの表示権限もあるプランライセンスのユーザーには、選択されたフィールドと選択されていないフィールドが表示されます。このプロジェクトにリクエストを送信できる、その他のユーザーには、選択したフィールドのみが表示されます。 |
     | ユーザーなし | 未選択のフィールドを表示できるユーザーは、いません。このプロジェクトにリクエストを送信できるすべてのユーザーは、選択されたフィールドのみを表示できます。 これはデフォルトの選択です。 |

   * **カスタムForms**：ドロップダウンメニューからリクエストキューに関連付けるカスタムフォームを選択します。 複数のフォームを選択し、リクエストフォームに表示する順序でドラッグ&amp;ドロップできます。
このドロップダウンメニューから選択できるのは、イシューカスタムフォームのみです。 このリクエストキューに送信され、プロジェクトまたはそのタスクに追加されたすべてのイシューには、選択したフォームが関連付けられます。
イシューのカスタムフォームを「キューの詳細」セクションに表示するには、カスタムフォームを事前に作成しておく必要があります。
リクエストキューに複数のキュートピックが関連付けられている場合は、代わりにカスタムフォームをキュートピックに関連付けることをお勧めします。
詳しくは、[キュートピックの作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。

     ![ キューの詳細のカスタムフォームボックス ](assets/custom-forms-box-on-queue-details.png)

1. 続いて、**メールキュー設定**&#x200B;エリアで、ユーザーがリクエストをリクエストキュープロジェクトにメールで送信できるようにするには、設定の情報を選択します。

   詳しくは、[ユーザーが問題をリクエストキュープロジェクトにメールで送信できるようにする](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md)を参照してください。

1. 「**保存**」をクリックします。\
   プロジェクトがリクエストキューに設定されたので、ユーザーはリクエストを追加できるようになりました。

1. （オプション）リクエストキュー機能を強化するには、キュー用の追加のサブセクションと、受信リクエストを正しいチーム、担当者またはプロジェクトにルーティングするルールを作成します。

   * リクエストキューのサブセクションの作成について詳しくは、次の記事を参照してください
   * [キュートピックの作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)
   * [ トピックグループの作成 ](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

     適切な担当者、チーム、および正しいプロジェクトにリクエストをルーティングする方法については、[ルーティングルールの作成](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)を参照してください。

