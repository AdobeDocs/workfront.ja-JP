---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: キュートピックを作成
description: キューのトピックは、ルーティングルールと連携して、作業依頼をユーザー、担当業務、チームにを自動的に割り当てたり、プロジェクトに配置したりします。キューのトピックでは、ルーティングルールを実装するために必要な条件を定義します。
author: Alina
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 86%

---

# キュートピックを作成

<!-- Audited: 12/2023 -->

キューのトピックは、ルーティングルールと連携して、作業依頼をユーザー、担当業務、チームにを自動的に割り当てたり、プロジェクトに配置したりします。キューのトピックでは、ルーティングルールを実装するために必要な条件を定義します。

トピックグループまたはプロジェクトに割り当てることができるキューのトピックの数に制限はありません。キューのトピックは、レポート可能なオブジェクトタイプです。

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>
    <p>新規：標準</p>
    <p>または</p>
    <p>現在：プラン</p></td>  
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

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## キューのトピックを作成

1. ルーティングルール、トピックグループ、およびカスタムフォームをキューのトピックに関連付ける予定がある場合は、それらを作成します。\
   ルーティングルール、トピックグループ、またはカスタムフォームの作成方法について詳しくは、次の記事を参照してください。

   * [ルーティングルールの作成](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [トピックグループの作成](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. ヘルプリクエストキューとして有効にしたプロジェクトと、新しいキューのトピックを作成する場所に移動します。\
   プロジェクトをヘルプリクエストキューとして指定する方法の詳細については、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   関連するキュートピックは、トピックグループの下に整理できます。 これにより、リクエストを行う際に、要求者に一連のドロップダウンメニューが表示されます。

   または

   キューのトピックは、ヘルプリクエストキューとして指定されたプロジェクトの下に、トピックグループを指定せずに直接ネストできます。

   トピックグループの作成について詳しくは、[トピックグループの作成](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)を参照してください。

1. 左側のパネルで「**キューのトピック**」をクリックします。「**さらに表示**」をクリックし、「**キューのトピック**」をクリックする必要がある場合があります。
1. 「**新規キュートピック**」をクリックします。
1. 次の日： **新しいキュートピック** フォームで、次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名前</strong> </td> 
      <td> キューのトピックの名前。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td>リクエストキューについて説明します。説明は、新規リクエストを送信するプロセスで、ユーザーがキューのトピックを選択する際に表示されます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>トピック グループに追加</strong> </td> 
      <td> プロジェクトにトピックグループがない場合、プロジェクトの名前は既定でトピックグループになります。<br>追加のトピックグループを作成する場合は、ドロップダウンメニューから「<strong>新規トピックグループを作成</strong>」を選択します。<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>カスタムフォーム</strong> </td> 
      <td>キューのトピックに関連付けるカスタムフォームを選択します。イシューをキューのトピックに関連付ける前に、イシューのカスタムフォームを作成する必要があります。カスタムフォームの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>デフォルトの承認</strong></td> 
      <td> <p>このキューのトピックに承認プロセスを関連付けます。このドロップダウンメニューには、イシューの承認プロセスのみが表示されます。このキューに送信されたすべてのイシューが、この承認プロセスに関連付けられます。キュートピックに関連付ける前に、Adobe Workfront 管理者がシステムレベルの承認プロセスを定義する必要があります。<span>承認プロセスへの管理者アクセス権を持つユーザーは、グループ固有の承認プロセスを作成することもできます。</span>承認プロセスの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業アイテムの承認プロセスの作成</a>を参照してください。<br></p> 
       <div> 
        <p>重要：プロジェクトのグループが変更されると、既存のイシューに関連付けられたグループ固有の承認プロセスが、1 回限りの承認プロセスになります。プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループと承認プロセスの変更が割り当てられた承認プロセスに及ぼす影響</a>を参照してください。</p> 
        <p>キューのトピックに承認プロセスを追加する際は、次の点を考慮してください。 </p> 
        <ul style="list-style-type: circle;"> 
         <li>アクティブな承認プロセスのみがリストに表示されます。 </li> 
         <li> <p>システム全体およびグループ固有の承認プロセスがリストに表示されます。プロジェクトの承認プロセス以外のグループに関連付けられている承認プロセスは、リストに表示されません。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>デフォルトの期間</strong> </td> 
      <td>これはリクエストのデフォルトの期間で、リクエストの計画完了日はこの値に基づいて計算されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>既定のルート</strong> </td> 
      <td>キューのトピックに関連付けるルーティングルールを指定します。ルーティングルールをキュートピックに添付する前に、ルーティングルールを作成する必要があります。詳しくは、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">ルーティングルールの作成</a>を参照してください。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>リクエストタイプ</strong> </td> 
      <td> <p>このキュートピックに保存するリクエストの種類を選択します。表示オプションは、プロジェクトの「<strong>キューの詳細</strong>」タブで設定します。必須フィールドです。 </p>

   <p><b>メモ</b>：

   「キューの詳細」ページと「キュートピック」ページの両方で「リクエストタイプ」が選択されている場合にのみ、タイプが「要求」エリアに選択肢として表示されます。プロジェクトの「キューの詳細」エリアの設定について詳しくは、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>を参照してください。 </p> <p>次のタイプから選択します。</p>
   <ul>
   <li>バグレポート</li>
   <li>変更依頼</li>
   <li>イシュー</li>
   <li>リクエスト</li>
   </ul> <p>Workfront 管理者が、これらのオプションの一部の名前を変更している可能性があります。 </p> </td>
   </tr> 
    </tbody> 
   </table>

   ![「新規キュートピック」ボックス](assets/new-queue-topic-box.png)

1. 「**保存**」をクリックします。\
   「リクエストキュー」と「トピックグループ」が選択されたので、「キュートピック」が使用可能になり、Workfront の「要求」エリアに表示されます。
