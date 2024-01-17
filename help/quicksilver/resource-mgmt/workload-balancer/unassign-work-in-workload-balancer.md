---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーでの作業の割り当て解除
description: Adobe Workfront Workload Balancer の「割り当て済み作業」領域で、作業項目の割り当てを解除したり、他のユーザー、ロールまたはチームにユーザーを再割り当てしたりできます。
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 2%

---

# ワークロードバランサーでの作業の割り当て解除

Adobe Workfront Workload Balancer の「割り当て済み作業」領域で、作業項目の割り当てを解除したり、他のユーザー、ロールまたはチームにユーザーを再割り当てしたりできます。

ドラッグ&amp;ドロップまたは一括で、作業項目からユーザーの割り当てを解除できます。 この記事では、ユーザーの割り当てを手動で解除する方法について説明します。

ドラッグ&amp;ドロップによるユーザーの割り当て解除について詳しくは、 [ドラッグ&amp;ドロップによりワークロードバランサーで作業を割り当てる](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

ユーザーの一括割り当て解除について詳しくは、 [ワークロードバランサーを使用して作業を一括で割り当てる](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <td> <p>リソース領域でワークロードバランサーを使用する場合の計画</p>
   <p>チームまたはプロジェクトのワークロードバランサーを使用する場合の作業</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次へのアクセスを編集します。</p> 
    <ul> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>タスク</p> </li> 
     <li> <p>イシュー</p> </li> 
    </ul> <p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>割り当ての作成を含むプロジェクト、タスク、および問題に権限以上を貢献する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

 

## ワークロードバランサーで作業項目の割り当てを解除

ユーザーから項目の割り当てを解除して「未割り当て作業」領域に移動するか、他のユーザーに再割り当てすることができます。

ユーザーに対する作業項目の割り当てを解除するには、次の手順に従います。

1. ワークロードバランサーで、 **割り当てられた作業** をクリックし、ユーザーを展開します。
1. 次のいずれかの操作を行います。

   * ユーザーの領域で割り当てを解除する項目を探し、クリックして、「未割り当て」領域または別のユーザーの領域にドラッグ&amp;ドロップします。
   * 次をクリック： **その他** アイコン ![](assets/more-icon-task-list.png) 作業項目の名前の右側にある **これをに割り当てる**&#x200B;次に、作業項目に割り当てられているエンティティの名前を削除するか、別の名前を入力して、 **保存**.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   その領域のフィルタ条件に一致し、他のユーザーに割り当てられていない場合は未割り当て作業領域に項目が表示され、別のユーザーに割り当てられている場合はユーザー領域に表示されます。

   ワークロード・バランサの情報のフィルタリングの詳細は、 [ワークロードバランサーの情報のフィルタリング](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
