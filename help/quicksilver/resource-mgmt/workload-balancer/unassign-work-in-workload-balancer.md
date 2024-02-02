---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーで作業を割り当て解除する
description: Adobe Workfront ワークロードバランサーの割り当て済み作業エリアの作業アイテムから、ユーザーの割り当てを解除したり、他のユーザー、役割、またはチームに再割り当てしたりできます。
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: ht
source-wordcount: '434'
ht-degree: 100%

---

# ワークロードバランサーで作業を割り当て解除する

Adobe Workfront ワークロードバランサーの割り当て済み作業エリアの作業アイテムから、ユーザーの割り当てを解除したり、他のユーザー、役割、またはチームに再割り当てしたりできます。

ドラッグ＆ドロップまたは一括で、作業アイテムからユーザーの割り当てを解除できます。この記事では、ユーザーの割り当てを手動で解除する方法について説明します。

ドラッグ＆ドロップによるユーザーの割り当て解除について詳しくは、[ドラッグ＆ドロップによりワークロードバランサーで作業を割り当てる](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)を参照してください。

ユーザーの一括割り当て解除について詳しくは、[ワークロードバランサーを使用して作業を一括で割り当てる](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)を参照してください。

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
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>以下の項目についてアクセス権を編集します。</p> 
    <ul> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>タスク</p> </li> 
     <li> <p>イシュー</p> </li> 
    </ul> <p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、「<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスク、イシューに対する参加以上の権限（割り当ての作成を含む）</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

 

## ワークロードバランサーで作業アイテムを割り当て解除する

ユーザーから項目の割り当てを解除して未割り当て作業エリアに移動するか、他のユーザーに再割り当てすることができます。

ユーザーから作業アイテムの割り当てを解除するには、以下の手順を実行します。

1. ワークロードバランサーで、**割り当てられた作業**&#x200B;エリアに移動し、ユーザーを展開します。
1. 次のいずれかの操作を行います。

   * ユーザーのエリアで割り当てを解除する項目を探し、クリックして、未割り当てエリアまたは別のユーザーのエリアにドラッグ＆ドロップします。
   * 作業アイテム名の右側にある&#x200B;**その他**&#x200B;アイコン ![](assets/more-icon-task-list.png) をクリックし、「**割り当て先**」をクリックして、作業アイテムに割り当てられたエンティティの名前を削除するか、別の名前を入力して、「**保存**」をクリックします。

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   項目がそのエリアのフィルタリング基準に一致し、他のユーザーに割り当てられていない場合、項目は未割り当て作業エリアに表示されます。また、別のユーザーに割り当てられている場合は、ユーザーエリアに表示されます。

   ワークロードバランサーでの情報のフィルタリングについて詳しくは、[ワークロードバランサーで情報をフィルタリング](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)を参照してください。
