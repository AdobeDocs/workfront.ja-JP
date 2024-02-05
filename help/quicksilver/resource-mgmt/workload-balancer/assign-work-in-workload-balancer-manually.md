---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーを使用して作業を手動で割り当てる
description: Adobe Workfront ワークロードバランサーを使用すると、作業アイテムを手動でユーザーに割り当てることができます。
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 100%

---

# ワークロードバランサーを使用して作業を手動で割り当てる

Adobe Workfront ワークロードバランサーを使用すると、作業アイテムを手動でユーザーに割り当てることができます。

ワークロードバランサーを使用してユーザーに作業アイテムを割り当てる方法の概要については、[ワークロードバランサーでの作業割り当ての概要](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン、リソース領域でワークロードバランサーを使用する場合</p>
   <p>ワーク、チームまたはプロジェクトのワークロードバランサーを使用する場合</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>次へのアクセスを編集します。</p> 
    <ul> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>タスク</p> </li> 
     <li> <p>イシュー</p> </li> 
    </ul> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、「<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>」を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスク、イシューに対する参加以上の権限（割り当ての作成を含む）</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## ワークロードバランサーで手動による作業の割り当て

まだユーザーに割り当てられていない作業アイテムを割り当てたり、ワークロードバランサーでユーザーに割り当てられているアイテムを再割り当てしたりできます。

1. 作業を割り当てるワークロードバランサーに移動します。

   ワークロードバランサーを使用して、リソース領域、プロジェクト、またはチームレベルで作業をユーザーに割り当てることができます。ワークロードバランサーの Workfront 内の場所について詳しくは、[ワークロードバランサーの検索](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)を参照してください。

1. （オプション）**未割り当ての作業**&#x200B;エリアを開き、フィルターを適用してタスクまたはイシューを表示します。

   または

   アイテムを再割り当てする場合は、**割り当てられた作業**&#x200B;エリアに移動し、ユーザーの名前を展開して、そのユーザーに割り当てられている作業アイテムを表示します。

1. 作業アイテム名の左側にある&#x200B;**その他メニュー**![](assets/qs-more-menu.png)をクリックし、「**このアイテムを割り当てる**」をクリックします。

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >次のショートカットを使用して、タスクやイシューを割り当てることもできます。
   >
   >* Windows の場合：Ctrl キーを押しながらタスクまたはイシューバーをクリックします。
   >* Mac の場合：Cmd キーを押しながらタスクまたはイシューバーをクリックします。

1. 次のいずれかの操作を行います。

   * 「**ユーザー、チーム、グループまたは会社を検索**」フィールドに項目に割り当てたいユーザー名、役職名、チーム名を入力し、リストに表示されたら選択し、「**保存**」をクリックします。

   >[!TIP]
   >
   >ユーザーを追加する際には、アバター、ユーザーのプライマリの役割、メールアドレスに注目して、同じ名前のユーザーを区別します。
   >
   >ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。
   >
   > ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、[ユーザーへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > お使いの環境で Workfront 管理者またはグループ管理者が委任を有効にしている場合は、「割り当て」タブを使用して、ユーザーをタスクまたはイシューに割り当てます。作業アイテムにデリゲートされたユーザーを表示するには、「デリゲーション」タブを使用します。作業のデリゲーションについて詳しくは、[タスクとイシューのデリゲーションの管理](../../manage-work/delegate-work/how-to-delegate-work.md)を参照してください。


   これにより、指定された担当者に作業アイテムが割り当てられるか、再割り当てされます。

   項目をチームまたは担当業務にのみ割り当てた場合、その項目は未割り当て作業エリアにのみ表示されます。作業アイテムをワークロードバランサーの割り当て済み作業エリアに表示するには、作業アイテムをユーザーに割り当てる必要があります。

   >[!TIP]
   >
   >複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
   >
   >
   >非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
   >
   >   
   >   
   >   * 作業アイテムをアクティブなリソースに再割り当てする。
   >   * 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。
   >   
   >

   * 「**詳細**」をクリックして、「高度な割り当て」にアクセスします。

     高度な割り当ての実行について詳しくは、[高度な割り当てを作成](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)を参照してください。

1. （オプション）**割り当てを表示** ![](assets/show-allocations-icon-small.png) をクリックし、**その他メニュー**![](assets/qs-more-menu.png)／**割り当ての編集**&#x200B;をクリックします。

   または

   日次または週次の割り当てをダブルクリックして、ユーザーが作業アイテムに割り当てられる時間数を変更します。

   ワークロードバランサーでのユーザー割り当ての変更については、[ワークロードバランサーでのユーザー割り当ての管理](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)の記事で「ユーザー割り当ての変更」の節を参照してください。

   ワークロードバランサーを使用して作業項目から割り当てを削除する方法について詳しくは、[ワークロードバランサーでの作業の割り当て解除](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md)を参照してください。

    
