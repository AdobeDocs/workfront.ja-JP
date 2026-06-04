---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーでの作業の割り当て解除
description: Adobe Workfront ワークロードバランサーの割り当て済み作業エリアの作業アイテムから、ユーザーの割り当てを解除したり、他のユーザー、役割、またはチームに再割り当てしたりできます。
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
TQID: https://experienceleague.adobe.com/AREKzNODjF60azs3tXIndVE9QuXXw-14Qlv2nUl9Po4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 382
ht-degree: 81%

---

# ワークロードバランサーで作業を割り当て解除する

Adobe Workfront ワークロードバランサーの割り当て済み作業エリアの作業アイテムから、ユーザーの割り当てを解除したり、他のユーザー、役割、またはチームに再割り当てしたりできます。

ドラッグ＆ドロップまたは一括で、作業アイテムからユーザーの割り当てを解除できます。 この記事では、ユーザーの割り当てを手動で解除する方法について説明します。

ドラッグ＆ドロップによるユーザーの割り当て解除について詳しくは、[ドラッグ＆ドロップによりワークロードバランサーで作業を割り当てる](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)を参照してください。

ユーザーの一括割り当て解除について詳しくは、[ワークロードバランサーを使用して作業を一括で割り当てる](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>計画：リソーシング領域でワークロードバランサーを使用する場合、作業：チームまたはプロジェクトのワークロードバランサーを使用する場合</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>以下の項目についてアクセス権を編集します。</p> 
    <ul> 
     <li>リソース管理</li> 
     <li>プロジェクト</li> 
     <li>タスク</li> 
     <li>イシュー</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>プロジェクト、タスク、イシューに対する参加以上の権限（割り当ての作成を含む）</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ワークロードバランサーで作業アイテムを割り当て解除する

ユーザーから項目の割り当てを解除して未割り当て作業エリアに移動するか、他のユーザーに再割り当てすることができます。

ユーザーから作業アイテムの割り当てを解除するには、以下の手順を実行します。

1. ワークロードバランサーで、**割り当てられた作業**&#x200B;エリアに移動し、ユーザーを展開します。
1. 次のいずれかの操作を行います。

   * ユーザーのエリアで割り当てを解除する項目を探し、クリックして、未割り当てエリアまたは別のユーザーのエリアにドラッグ＆ドロップします。
   * 作業項目の名前の右側にある&#x200B;**詳細** アイコン ![詳細アイコン ](assets/more-icon-task-list.png)をクリックし、**これを**&#x200B;に割り当ててから、作業項目に割り当てられたエンティティの名前を削除するか、別の名前を入力して、**保存**&#x200B;をクリックします。

     ![これを](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)に割り当てる

   項目がそのエリアのフィルタリング基準に一致し、他のユーザーに割り当てられていない場合、項目は未割り当て作業エリアに表示されます。また、別のユーザーに割り当てられている場合は、ユーザーエリアに表示されます。

   ワークロードバランサーでの情報のフィルタリングについて詳しくは、[ワークロードバランサーで情報をフィルタリング](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)を参照してください。
