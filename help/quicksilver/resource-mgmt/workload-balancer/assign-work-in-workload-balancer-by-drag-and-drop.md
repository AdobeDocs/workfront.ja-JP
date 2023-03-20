---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ドラッグ&ドロップによりワークロードバランサーで作業を割り当てる
description: 作業項目を正しいユーザーにドラッグ&ドロップすることで、Adobe Workfrontワークロードバランサーを使用して作業項目を割り当てることができます。
author: Alina
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 1%

---

# ドラッグ&amp;ドロップによりワークロードバランサーで作業を割り当てる

<!--remove production and preview preferences at release-->

作業項目を正しいユーザーにドラッグ&amp;ドロップすることで、Adobe Workfrontワークロードバランサーを使用して作業項目を割り当てることができます。

ワークロード・バランサを使用してユーザーに作業を割り当てる方法の一般的な情報については、 [ワークロードバランサーでの作業割り当ての概要](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
   <td> <p>リソース領域のワークロードバランサーで作業を割り当てる計画</p>
   <p>チームまたはプロジェクトのワークロードバランサーで作業を割り当てる作業</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>次へのアクセスを編集します。</p> 
    <ul> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>タスク</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>割り当ての作成を含むプロジェクト、タスク、および問題に権限以上を貢献する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## ドラッグ&amp;ドロップによる項目の割り当て

「未割り当て作業」領域の品目をユーザーに割り当てたり、「割り当て済作業」領域で既に割り当て済の品目を別のユーザーに再割り当てしたりできます。

1. 作業を割り当てるワークロードバランサーに移動します。

   リソースエリア、プロジェクト、またはチームレベルで、ワークロードバランサーを使用して、作業をユーザーに割り当てることができます。 ワークロードバランサーのWorkfront内の場所について詳しくは、 [ワークロード・バランサの検索](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. （オプション） **未割り当ての作業** 領域を開き、フィルターを適用して、ユーザーに割り当てられていないタスクと問題を表示します

   または

   次に移動： **割り当てられた作業** 項目を再割り当てする場合は、領域を開き、ユーザーの名前を展開して、割り当てられた作業項目を表示します。

1. （条件付き）プロジェクトのワークロードバランサーで、 **すべてのユーザーを表示** アイコン ![](assets/show-all-users-icon-project-workload-balancer.png) すべてのWorkfrontユーザーを表示する。

   これにより、表示するアクセス権を持つすべてのユーザーが表示されます。

   プロジェクトチームにも属し、既にプロジェクト上の項目に割り当てられているユーザーの場合は、「割り当てられた作業」領域で、名前の右側にプロジェクトアイコンが表示されます。

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* 「すべてのユーザーを表示」オプションは、プロジェクトのワークロードバランサーでのみ使用できます。
   >* フィルターを使用して、重要なユーザーのみを表示します。 例えば、フィルターを使用して、チームまたはグループのユーザーのみを表示します。




1. 計画されたタイムラインまたは予測されたタイムラインを示す作業項目のバーをクリックし、 **割り当て済み** 領域

   作業項目をドロップするユーザーがハイライト表示されます。

   >[!TIP]
   >
   >リアルタイムで更新にカーソルを合わせるユーザーの計画時間と、作業項目からの日別計画時間数を指定して、新しい品目を追加した場合に全体的な配分に与える影響を示します。

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. 準備が整ったら、選択した作業項目をユーザーの名前と同じ行の「割り当て済み領域」にドロップします。 アイテムが割り当てられ、ユーザーに割り当てられた計画時間が、作業項目からの新しい時間で更新されます。

   品目が、ユーザーが履行できない役職ロールに割り当てられた場合、その品目は「割当作業」領域のユーザー名の下に表示され、「未割当作業」領域にも表示され、関連する役職がまだユーザーに置き換えられていないことを示します。

   >[!TIP]
   >
   >* 「設定」領域で「プロジェクト別にグループ化」を有効にした場合、割り当てられたタスクは対応するプロジェクトの下に表示されます。 この設定が無効な場合、割り当てられたタスクがユーザー領域に表示されます。
      >
      >
      >     作業項目を並べ替えるためのワークロードバランサーの基準に従って項目が表示されます。 詳しくは、 [ワークロード・バランサのナビゲート](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* [ プロジェクトのワークロードバランサーのすべてのユーザーを表示する ] を有効にし、以前にプロジェクトの項目に割り当てられていないユーザーに割り当てられた項目を表示すると、ユーザーはプロジェクトチームに追加されます。 詳しくは、 [プロジェクトチームを管理](../../manage-work/projects/planning-a-project/manage-project-team.md).



1. （オプション）「割り当てられた作業」領域でユーザーの名前の下にある作業項目のバーをクリックし、ドラッグして「未割り当ての作業」領域にドロップし、割り当てを解除します。 アイテムはユーザーから割り当て解除されますが、ジョブロールに割り当てられている場合もあります。その場合は、「未割り当て作業」領域に表示されます。 アイテムが別のユーザーに割り当てられている場合、そのアイテムは、まだ割り当てられているユーザーの名前の下で「割り当て済み作業」領域に残ります。
1. （オプション） **割り当てアイコンを表示** ![](assets/show-allocations-icon-small.png)」、「 **その他のメニュー** ![](assets/qs-more-menu.png) > **割り当てを編集**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   または

   日次または週次の配分をダブルクリックして、ユーザーが作業項目に割り当てられる時間を変更します。

   ワークロードバランサーでのユーザー割り当ての変更の詳細は、この記事の「ユーザー割り当ての変更」の節を参照してください [ワークロードバランサーでのユーザー割り当ての管理](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   ワークロード・バランサを使用して作業項目から割り当てを削除する方法については、 [ワークロードバランサーでの作業の割り当て解除](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

