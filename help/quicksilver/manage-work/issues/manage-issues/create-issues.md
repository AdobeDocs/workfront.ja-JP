---
product-area: projects
navigation-topic: manage-issues
title: イシューの作成
description: プロジェクトに取り組んでいると、予期しないイベントが発生することがあります。これらの予期しないイベントは、特定のプロジェクトやタスクに対するイシューとして記録できます。適切なアクセス権を持つユーザーは、プロジェクトまたはタスクが完了に向けて進行するにつれてイシューのステータスを表示および監視できるため、長時間にわたるメールチェーンや状況会議の必要がなくなります。予定イベントであるタスクとは異なり、イシューは Adobe Workfront の予定外の作業アイテムを表します。
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 98%

---

# イシューの作成

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

プロジェクトに取り組んでいると、予期しないイベントが発生することがあります。これらの予期しないイベントは、特定のプロジェクトやタスクに対するイシューとして記録できます。適切なアクセス権を持つユーザーは、プロジェクトまたはタスクが完了に向けて進行するにつれてイシューのステータスを表示および監視できるため、長時間にわたるメールチェーンや状況会議の必要がなくなります。予定イベントであるタスクとは異なり、イシューは Adobe Workfront の予定外の作業アイテムを表します。

イシューをリクエストとしてプロジェクトに追加することもできます。詳しくは、[Adobe Workfront リクエストの作成と送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

>[!TIP]
>
>Workfront では、イシューとリクエストは同じ意味で使用されます。プロジェクトとタスクの両方のイシューを記録して、対処する必要がある予期せぬ作業を示すことができます。リクエストを送信することもできます。リクエストは、リクエストキューとして指定されたプロジェクトのイシューとして記録されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プロジェクトまたはタスクにイシューを追加するレビュー権限またはそれ以上の権限</p> <p>リクエストキューを使用し、リクエストとしてイシューを追加するリクエスト以上の権限。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>プロジェクトとタスクへのアクセス権またはそれ以上の権限</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。アクセスレベルにおけるイシューへのアクセス権については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">イシューへのアクセス権の付与</a>を参照してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューを作成したタスクまたはプロジェクトにイシューを追加できる、参加以上の権限</p> <p> イシューへの権限の付与について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有</a>を参照してください。</p> <p>追加権限の要求については、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権の要求</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## イシュー作成の制限

適切なアクセス権と権限を持っている場合は、プロジェクトまたはタスクでイシューを作成できます。ただし、次の場合はイシューを作成できない可能性があります。

* Workfront 管理者またはグループ管理者は、プロジェクト設定エリアで、完了または無効ステータスにあるプロジェクトへのイシューの追加を有効にする必要があります。プロジェクト環境設定の詳細については、[システム全体のプロジェクト環境設定の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。
* 承認保留中のプロジェクトにはイシューを追加できません。

## 新しいイシューフォームの準備

組織では、いつ、どのようにイシューを記録するかについて、明確に定義されたプロセスを導入する必要があります。このプロセスを設定するときの最初の手順は、イシューの送信に必要なフォームを作成することです。イシューをタスクやプロジェクトに直接追加できるようにするか、イシューが送信されるリクエストキューがある場合に、ユーザーが新しいイシューを送信するときに使用できるWorkfront フィールドやカスタムフィールドを定義できます。新しいイシューフォームには、イシューを迅速に解決するのに役立つ重要な情報が含まれている場合があります。

プロジェクトの新しいイシューのフィールドは、イシューが記録されるプロジェクトの「キューの詳細」セクションで定義されます。プロジェクトのキューの詳細セクションの設定については、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

リクエストキューに送信してイシューを作成する方法については、この記事の[新しいリクエストを入力してイシューを作成](#create-issues-by-entering-a-new-request)の節を参照してください。

## 「新規イシュー」ボタンを使用してタスクまたはプロジェクトにイシューを作成します

プロジェクトで新しいイシューフォームのフィールドを定義したら、イシューの作成を開始できます。

<!-- OLD UI: redesigned on Oct 26, 2023:

Creating issues differs depending on which environment you choose to create the issue. 

### Create issues on a task or project using the New Issue button in the Production environment

To create an issue on a task or a project:

1. Go to a project where you want to create the issue. 
1. (Optional) If you want to log the issue for a task, go to the **Tasks** area, then click the name of a task. 
1. Click the **Issues** section.

   
1. Click **New Issue**.

  

1. (Conditional) If the project creator created Queue Topics or Topic Groups on the project they are added to the new issue form. Specify the **Topic Group** or the **Queue Topic** of your new issue. Topic Groups and Queue Topics have names customized to your environment.  
   For more information about creating Topic Groups, see [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * If there is only one Queue Topic set on the project, it is displayed automatically.
   * If the Topic Group does not have any Queue Topics or Topic Groups under it, nothing is available in the Topic Group drop-down.

1. (Conditional) If the project creator allowed for the **Request Type** field to display on the New Issue form, select the type of your issue from the following options:

   * Bug Report
   * Change Order
   * Issue
   * Request  
     Depending on how your Workfront administrator has configured your Project Preferences, the names of the issue types might be different for you. 

   >[!TIP]
   >
   >The Request Types must be enabled in the Queue Details and as well as when creating the Queue Topic to display as a selection in the New Issue form. For information, see the following articles: 
   >* [Create a Request Queue](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Create Queue Topics](../../requests/create-and-manage-request-queues/create-queue-topics.md)


1. Add a name for the new issue in the **Issue Name** field. 
1. Continue specifying the fields available in the **New Issue** form. For more information about the fields available as you enter a new issue, see [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Not all the issue-related fields are available in the New Issue form. The project creator enables the fields available when creating an issue when they define the Queue Details area of the project. For more information, see [Create a Requests Queue](../../requests/create-and-manage-request-queues/create-request-queue.md). 


1. (Conditional) If the Queue Topics are associated with a custom form, that custom form will display in the **New Issue** form.  
   Or  
   If the project is associated with an issue custom form through the Queue Details area, the form displays in the **New Issue** form, after the default Workfront fields.

   For information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Click **Save New Issue.**

Issues can be assigned to multiple users, job roles or to a team. For more information about assigning and managing requests, see [Manage work and team requests](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content:
-->

タスクまたはプロジェクトでイシューを作成する手順は次のとおりです。

1. イシューを作成するプロジェクトに移動します。
1. （オプション）タスクのイシューをログに記録する場合は、**タスク**&#x200B;エリアに移動し、タスクの名前をクリックします。
1. 「**イシュー**」セクションをクリックします。

   プロジェクトの問題のリストが表示されます

1. クリック **新しい問題** をクリックします。
「新規イシュー」ボックスが表示されます。

   ![](assets/new-issue-box-matches-new-request-ui.png)

1. （条件付き）プロジェクト作成者がプロジェクト上にキューのトピックまたはトピックグループを作成した場合、それらは新しいイシューフォームに追加されます。新しいイシューの&#x200B;**トピックグループ**&#x200B;または&#x200B;**キューのトピック**&#x200B;を指定します。トピックグループとキューのトピックには、環境に合わせてカスタマイズされた名前が付いています。\
   トピックグループの作成の詳細については、[トピックグループの作成](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)を参照してください。キューのトピックの作成について詳しくは、[キューのトピックの作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。

   * プロジェクトにキューのトピックが 1 つだけ設定されている場合は、自動的に表示されます。
   * トピックグループの下にキューのトピックまたはトピックグループがない場合、「トピックグループ」ドロップダウンには何も表示されません。

1. 「**件名**」フィールドにイシュー名を追加し、「**説明**」を追加します。

1. （条件付き）「新しい問題」フォームでの「**リクエストタイプ**」フィールドの表示をプロジェクト作成者が許可している場合は、次の選択肢からイシューのタイプを選択します。

   * バグレポート
   * 変更依頼
   * イシュー
   * リクエスト\
     Workfront 管理者がプロジェクト環境設定をどのように設定したかに応じて、イシュータイプの名前が異なる場合があります。

   >[!TIP]
   >
   >リクエストタイプは、キューの詳細で有効にする必要があります。また、新しいイシューフォームで選択項目として表示するキューのトピックを作成するときも有効にする必要があります。詳しくは、次の記事を参照してください。
   >* [リクエストキューの作成](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [キュートピックの作成](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. **新しい問題**&#x200B;フォームで使用可能なフィールドの指定を続行します。新しいイシューを入力する際に使用できるフィールドについて詳しくは、[イシューの編集](../../../manage-work/issues/manage-issues/edit-issues.md)を参照してください。

   >[!IMPORTANT]
   >
   >新しいイシューフォームでは、すべてのイシュー関連フィールドが使用できるわけではありません。プロジェクト作成者が、プロジェクトのキューの詳細エリアを定義するときに、イシューの作成時に使用可能なフィールドを有効にします。詳しくは、[リクエストキューの作成](../../requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。


1. （条件付き）キュートピックがカスタムフォームに関連付けられている場合、そのカスタムフォームは&#x200B;**新しい問題**&#x200B;フォームに表示されます。\
   または\
   プロジェクトがキューの詳細領域を通じてイシューカスタムフォームに関連付けられている場合、そのフォームは、**新しい問題**&#x200B;フォームのデフォルトの Workfront フィールドの後に表示されます。

   詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

1. 「**送信**」をクリックします。

   イシューは、複数のユーザー、担当業務、チームに割り当てることができます。リクエストの割り当てや管理について詳しくは、[作業リクエストとチームリクエストの管理](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)を参照してください。


## タスクまたはプロジェクトでのイシューのインライン作成

>[!IMPORTANT]
>
>イシューをプロジェクトまたはタスクにインラインで追加するには、まず、プロジェクトのイシュー設定を定義する際に、プロジェクト所有者が「**ユーザーがインラインで問題を追加できるようにする**」を有効にする必要があります。プロジェクトでのイシュー設定の指定については、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。
>

複数のイシューを手早く追加したい場合は、イシューのリストに追加することにより、タスクまたはプロジェクトのイシューをインラインで作成することができます。

>[!NOTE]
>
>イシューをインラインで追加する場合、Workfront は新しいイシューに新しい問題フォームを適用しません。イシューの入力時にユーザーに特定の情報を提供してもらいたい場合は、イシューのインライン追加をお勧めしません。インライン追加はイシュー報告に悪影響を与える可能性があり、後で、イシューに割り当てられたユーザーがイシューの解決に必要な情報を十分に入手できなくなる可能性があります。

イシューをインラインで作成するには、次の手順に従います。

1. イシューを作成するプロジェクトに移動します。
1. （オプション）タスクのイシューをログに記録する場合は、「**タスク**」セクションに移動し、タスクの名前をクリックします。
1. 左側のパネルで、「**イシュー**」セクションをクリックします。
1. クリック **問題をさらに追加** をクリックします。

   「問題」セクションのイシューリストに新しい行が作成されます。

   >[!TIP]
   >
   >プロジェクトの編集ボックスで「ユーザーがインラインで問題を追加できるようにする」設定が選択解除されている場合、このオプションはグレー表示になります。詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. 「名前」フィールドにイシューの名前を入力し、イシューに関する詳細情報の追加をインラインで続行します。

   >[!TIP]
   >
   >フィールドがインライン編集可能かどうかは、イシューリストに適用する表示によります。以下のタイプのフィールドは、インライン編集できない可能性があります。
   >   
   >* 別のオブジェクトに属するフィールド
   >* 編集アクセス権がないフィールド
   >* Workfront で自動的に更新される計算フィールド

1. Enter キーを押してインライン編集を終了し、イシューをプロジェクトまたはタスクに追加します。

## 新規リクエストの入力によるイシューの作成 {#create-issues-by-entering-a-new-request}

イシューを受け取る受け皿となるプロジェクトを指定することができます。このタイプのプロジェクトは、Workfront ではリクエストキューと呼ばれます。リクエストキューには、メインメニューの「リクエスト」エリアからアクセスできます。

>[!TIP]
>
>Workfront では、「イシュー」と「リクエスト」という用語を入れ替えることができます。

イシューを受け取るためのリクエストキューとしてプロジェクトを設定する方法に関して詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。リクエストの送信について詳しくは、[Adobe Workfront リクエストを作成および送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。
