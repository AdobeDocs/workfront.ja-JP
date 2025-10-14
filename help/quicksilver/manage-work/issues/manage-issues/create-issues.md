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
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 88%

---

# イシューの作成

<!--Audited: 03/2025-->

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

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新しいライセンス：</p>
   <ul><li>投稿者以上</li>
   <li>タスクまたはプロジェクトの「イシュー」セクションのイシューを編集するためのライト以上</li></ul>
   <p>現在のライセンス：</p>
  <ul><li>リクエスト以上</li> <li>タスクまたはプロジェクトの「イシュー」セクションでレビュー以上のイシューを編集する</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>プロジェクトとタスクへのアクセス権またはそれ以上の権限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューを作成したタスクまたはプロジェクトにイシューを追加できる、参加以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## イシュー作成の制限

適切なアクセス権と権限を持っている場合は、プロジェクトまたはタスクでイシューを作成できます。ただし、次の場合はイシューを作成できない可能性があります。

* Workfront 管理者またはグループ管理者は、プロジェクト設定エリアで、完了または無効ステータスにあるプロジェクトへのイシューの追加を有効にする必要があります。プロジェクト環境設定の詳細については、[システム全体のプロジェクト環境設定の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。
* 承認保留中のプロジェクトにはイシューを追加できません。

## 新しいイシューフォームの準備

組織では、いつ、どのようにイシューを記録するかについて、明確に定義されたプロセスを導入する必要があります。このプロセスを設定する場合、最初の手順はイシューの送信に必要なフォームを作成することです。

ユーザーは次の方法でイシューをプロジェクトに追加できます。

* タスクやプロジェクトに直接追加できます。
* リクエストキューに送信します。

新しいイシューフォームには、イシューを迅速に解決するのに役立つ重要な情報が含まれている場合があります。

ユーザーがイシューをプロジェクトまたはそのタスクに追加した際に次の情報を含めるように、「新しいイシュー」フォームを設定できます。

* カスタムフィールド
* 承認
* 割当（ルーティング規則）

新しいイシューまたはリクエストのフィールドは、イシューが記録されるプロジェクトの「キューの詳細」セクションで定義されます。

プロジェクトのキューの詳細セクションの設定については、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

リクエストキューに送信してイシューを作成する方法については、この記事の[新しいリクエストを入力してイシューを作成](#create-issues-by-entering-a-new-request)の節を参照してください。

## 「新規イシュー」ボタンを使用してタスクまたはプロジェクトにイシューを作成します

プロジェクトで新しいイシューフォームのフィールドを定義したら、イシューの作成を開始できます。

タスクまたはプロジェクトでイシューを作成する手順は次のとおりです。

1. イシューを作成するプロジェクトに移動します。
1. （オプション）タスクのイシューをログに記録する場合は、**タスク**&#x200B;エリアに移動し、タスクの名前をクリックします。
1. 「**イシュー**」セクションをクリックします。

   プロジェクトのイシューのリストが表示されます。

1. イシューのリストの上部にある「**新しいイシュー**」をクリックします。
「新規イシュー」ボックスが表示されます。

   ![&#x200B; 新しいイシューボックス &#x200B;](assets/new-issue-box-matches-new-request-ui.png)

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
1. イシューのリストの下部にある「**さらにイシューを追加**」をクリックします。

   「問題」セクションのイシューリストに新しい行が作成されます。

   >[!TIP]
   >
   >プロジェクトの編集ボックスで「ユーザーがインラインで問題を追加できるようにする」設定が選択解除されている場合、このオプションはグレー表示になります。詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

   ![&#x200B; 「さらにイシューを追加」ボタン &#x200B;](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

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

イシューを受け取る受け皿となるプロジェクトを指定することができます。このタイプのプロジェクトは、Workfront ではリクエストキューと呼ばれます。リクエストキューは、メインメニューのリクエスト エリアからアクセスできます。

>[!TIP]
>
>Workfront では、「イシュー」と「リクエスト」という用語を入れ替えることができます。

イシューを受け取るためのリクエストキューとしてプロジェクトを設定する方法に関して詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。リクエストの送信について詳しくは、[Adobe Workfront リクエストを作成および送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。
