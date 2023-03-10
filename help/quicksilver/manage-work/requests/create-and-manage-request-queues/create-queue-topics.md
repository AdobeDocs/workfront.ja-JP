---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: キュートピックを作成
description: キュートピックは、ルーティングルールと連携して、ユーザー、ジョブロール、チームに着信作業を自動的に割り当てたり、プロジェクトに配置したりします。 キュー・トピックでは、ルーティング・ルールを実装するために必要な条件を定義します。
author: Alina
feature: Work Management
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 3%

---

# キュートピックを作成

キュートピックは、ルーティングルールと連携して、ユーザー、ジョブロール、チームに着信作業を自動的に割り当てたり、プロジェクトに配置したりします。 キュー・トピックでは、ルーティング・ルールを実装するために必要な条件を定義します。

トピックグループまたはプロジェクトに割り当てることができるキュートピックの数に制限はありません。 キュートピックは、レポート可能なオブジェクトタイプです。

## アクセス要件

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p> プロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください

## キュートピックの作成

1. ルーティングルール、トピックグループ、およびカスタムフォームを作成します（これらをキュートピックに関連付ける場合）。\
   ルーティングルール、トピックグループ、またはカスタムフォームの作成方法の詳細は、次の記事を参照してください。

   * [ルーティングルールの作成](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [トピックグループの作成](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. ヘルプリクエストキューとして有効にしたプロジェクトと、新しいキュートピックを作成する場所に移動します。\
   プロジェクトをヘルプリクエストキューとして指定する方法の詳細は、次の記事を参照してください。\
   [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

   関連するキュートピックは、トピックグループの下、またはヘルプリクエストキューとして指定されたプロジェクトの下に直接整理できます。 これにより、リクエストを行う際に、リクエスト元に一連のドロップダウンメニューが表示されます。\
   キュートピックは、ヘルプリクエストキューとして指定されたプロジェクトの下に、トピックグループを指定せずに直接ネストできます。

   トピックグループの作成について詳しくは、 [トピックグループの作成](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. クリック **トピックをキュー** をクリックします。 クリックが必要になる場合があります **さらに表示**&#x200B;を、 **トピックをキュー**.
1. クリック **新しいキュートピック**.
1. の **新しいキュートピック** フォームで、以下を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名前</strong> </td> 
      <td> キュートピックの名前。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td>リクエストキューの説明 説明は、新しいリクエストを送信する際に、ユーザーがキュートピックを選択する際に表示されます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>トピック グループに追加</strong> </td> 
      <td> プロジェクトにトピックグループがない場合、プロジェクトの名前は既定でトピックグループとして表示されます。<br>ここから追加のトピックグループを作成する場合は、 <strong>新しいトピックグループを作成</strong> を選択します。<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>カスタムフォーム</strong> </td> 
      <td>キューのトピックに関連付けるカスタムフォームを選択します。 問題をキューのトピックに関連付ける前に、問題のカスタムフォームを作成する必要があります。 カスタムフォームの作成について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">デフォルトの承認</td> 
      <td> <p>このキュートピックに承認プロセスを関連付けます。 このドロップダウンメニューには、問題の承認プロセスのみが表示されます。 このキューに送信されたすべての問題は、この承認プロセスに関連付けられます。 Adobe Workfront管理者は、キュートピックに関連付ける前に、システムレベルの承認プロセスを定義する必要があります。 <span>承認プロセスへの管理者アクセス権を持つユーザーは、グループ固有の承認プロセスを作成することもできます。</span> 承認プロセスの作成について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業項目の承認プロセスの作成</a>.<br></p> 
       <div> 
        <p>重要：プロジェクトのグループが変更されると、既存の問題に関連付けられたグループ固有の承認プロセスが、単一使用の承認プロセスになります。 プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループと承認プロセスの変更が、割り当てられた承認プロセスに及ぼす影響</a>.</p> 
        <p>キューのトピックに承認プロセスを追加する際は、次の点を考慮してください。 </p> 
        <ul style="list-style-type: circle;"> 
         <li>アクティブな承認プロセスのみがリストに表示されます。 </li> 
         <li> <p>システム全体およびグループ固有の承認プロセスがリストに表示されます。 プロジェクトの承認プロセス以外のグループに関連付けられている承認プロセスは、リストに表示されません。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>デフォルトの期間</strong> </td> 
      <td>これはリクエストのデフォルト期間で、リクエストの計画完了日はこの値に基づいて計算されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>既定のルート</strong> </td> 
      <td>キュートピックに関連付けるルーティングルールを指定します。 ルーティングルールをキュートピックに添付する前に、ルーティングルールを作成する必要があります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>リクエストタイプ</strong> </td> 
      <td> <p>このキュートピックに保存するリクエストの種類を選択します。 表示されるオプションは、 <strong>キューの詳細</strong> 」タブをクリックします。 必須フィールドです。 </p> <p>注意：「要求タイプ」は、「キューの詳細」ページと「キューのトピック」ページの両方で「要求タイプ」が選択されている場合にのみ、「要求」領域に選択として表示されます。 プロジェクトの Queue Details 領域の設定については、 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>. </p> <p>次のタイプから選択します。</p> 
       <ul> 
        <li>バグ報告書</li> 
        <li>変更依頼</li> 
        <li>問題</li> 
        <li>リクエスト</li> 
       </ul> <p>Workfront管理者が、これらのオプションの一部の名前を変更している可能性があります。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-queue-topic-box-nwe-350x375.png)

1.  
1. 「**保存**」をクリックします。\
   Queue Topic が使用できるようになり、Request Queue と Topic Group を選択した後、Workfrontの Requests 領域に表示されます。
