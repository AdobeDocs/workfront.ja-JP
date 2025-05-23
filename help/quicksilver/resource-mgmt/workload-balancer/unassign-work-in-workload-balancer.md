---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーでの作業の割り当て解除
description: Adobe Workfront ワークロードバランサーの割り当て済み作業エリアの作業アイテムから、ユーザーの割り当てを解除したり、他のユーザー、役割、またはチームに再割り当てしたりできます。
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 23c6d9335b0adcafc4e2ecdd8ef2d0ab09709fa8
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 80%

---

# ワークロードバランサーで作業を割り当て解除する

Adobe Workfront ワークロードバランサーの割り当て済み作業エリアの作業アイテムから、ユーザーの割り当てを解除したり、他のユーザー、役割、またはチームに再割り当てしたりできます。

ドラッグ＆ドロップまたは一括で、作業アイテムからユーザーの割り当てを解除できます。この記事では、ユーザーの割り当てを手動で解除する方法について説明します。

ドラッグ＆ドロップによるユーザーの割り当て解除について詳しくは、[ドラッグ＆ドロップによりワークロードバランサーで作業を割り当てる](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)を参照してください。

ユーザーの一括割り当て解除について詳しくは、[ワークロードバランサーを使用して作業を一括で割り当てる](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)を参照してください。

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
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：リソース領域でワークロードバランサーを使用する場合は、計画します。</br>
       チームまたはプロジェクトのワークロードバランサーを使用する場合の作業</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>以下の項目についてアクセス権を編集します。</p> 
    <ul> 
     <li>リソース管理</li> 
     <li>プロジェクト</li> 
     <li>タスク</li> 
     <li>イシュー</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>プロジェクト、タスク、イシューに対する参加以上の権限（割り当ての作成を含む）</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ワークロードバランサーで作業アイテムを割り当て解除する

ユーザーから項目の割り当てを解除して未割り当て作業エリアに移動するか、他のユーザーに再割り当てすることができます。

ユーザーから作業アイテムの割り当てを解除するには、以下の手順を実行します。

1. ワークロードバランサーで、**割り当てられた作業**&#x200B;エリアに移動し、ユーザーを展開します。
1. 次のいずれかの操作を行います。

   * ユーザーのエリアで割り当てを解除する項目を探し、クリックして、未割り当てエリアまたは別のユーザーのエリアにドラッグ＆ドロップします。
   * **その他** アイコン ![ その他のアイコン ](assets/more-icon-task-list.png) 作業項目の名前の右側にある「**割り当て先**」をクリックし、作業項目に割り当てられたエンティティの名前を削除するか、別の名前を入力して「**保存**」をクリックします。

     ![ 割り当て先 ](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   項目がそのエリアのフィルタリング基準に一致し、他のユーザーに割り当てられていない場合、項目は未割り当て作業エリアに表示されます。また、別のユーザーに割り当てられている場合は、ユーザーエリアに表示されます。

   ワークロードバランサーでの情報のフィルタリングについて詳しくは、[ワークロードバランサーで情報をフィルタリング](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)を参照してください。
