---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: スケジュール領域で未割り当てタスクとタスクを手動で割り当てる
description: スケジューリングタイムラインを使用すると、各ユーザーが作業項目に割り当てる時間を指定するだけでなく、ユーザー割り当てを管理できます。
author: Alina
feature: Resource Management
exl-id: 627e4442-767a-41a2-9700-76f2ad2dc9cf
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# スケジュール領域で未割り当てタスクとタスクを手動で割り当てる

>[!IMPORTANT]
>  
><span class="preview">この記事で説明するスケジュール機能は、2023 年 1 月の 23.1 リリースから廃止され、Adobe Workfrontから削除されました。   </span>
>  
> <span class="preview"> この記事は、2023 年初頭の 23.1 リリースの直後にも削除されます。 現時点では、ブックマークを適宜更新することをお勧めします。 </span>
> 
><span class="preview"> これで、ワークロードバランサーを使用して、リソースの作業をスケジュールできます。 </span>
>  
> <span class="preview">ワークロード・バランサを使用したリソースのスケジュール設定の詳細は、「 [ワークロードバランサー](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

スケジューリングタイムラインを使用すると、各ユーザーが作業項目に割り当てる時間を指定するだけでなく、ユーザー割り当てを管理できます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プロジェクト、タスク、問題へのアクセス権を表示または高くする</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスク、問題に対する権限の寄与</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## スケジュールタイムラインでタスクと問題を割り当てる前の前提条件

この節で説明するように、ユーザー割り当ての管理を開始する前に、Workfrontでのリソーススケジュールの動作について理解しておいてください ( [リソーススケジュールの概要](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

この節で説明するように、ユーザー割り当てを正しく管理するには、まず、ユーザー、プロジェクト、タスクおよび問題が、「 [Workfrontのスケジュールツールを使用するための前提条件](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#prerequisites) 記事のセクション [リソーススケジュールの概要](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

次の項では、ユーザー割り当てを手動で変更する方法、自動で変更する方法、またはユーザーまたは役割による割り当てを入れ替える方法について説明します。

## 未割り当てのタスクまたはタスクをユーザーに手動で割り当てる

スケジュールタイムラインは、ユーザーがタスクやイシューを完了するのに必要な視覚性を提供します。\
スケジューリングタイムラインについて詳しくは、 [リソーススケジュールの概要](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Workfrontの次の領域で、スケジュールタイムラインを使用して、個々のタスクやイシューをユーザーに割り当てることができます。

* （複数のプロジェクトのリソースをスケジュールする場合）リソースの下のスケジュール設定セクション。
* プロジェクトの下のスケジュール設定セクション（単一のプロジェクトのリソースをスケジュールする場合）。
* チームの下のスケジュールセクション（チームのリソースをスケジュールする場合）。

スケジューリング・タイムラインの最上部に表示される「未割当」領域の情報は、（複数プロジェクトのリソースをスケジュールする場合は）「スケジュール」セクション、（1 つのプロジェクトのリソースをスケジュールする場合は）「スケジュール」セクションです。 詳しくは、 [「スケジュール設定」領域で使用できる機能](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md#functionality-available-in-the-scheduling-area) 記事内 [スケジューリング領域の概要](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

スケジューリングタイムラインを表示しているWorkfrontの領域によっては、作業を割り当てる資格があるユーザーが一部に限られる場合があります。 詳しくは、 [スケジューリング領域の概要](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

スケジュール設定タイムラインで未割り当てのタスクまたはタスクをユーザーに割り当てるには、次の手順に従います。

1. 複数のプロジェクト、個々のプロジェクト、またはチームのスケジューリングタイムラインに移動します。

   * **複数のプロジェクトの場合**:  次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅にある **リソース > ワークロードバランサー**&#x200B;を選択し、「 **スケジュール** をクリックします。
   * **個々のプロジェクトの場合**:プロジェクトに移動し、 **ワークロードバランサー** セクションを開き、 **スケジュール** を選択します。
   * **チームの場合**:次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅で、 **チーム**、チームを選択して、 **ワークロードバランサー** 左のパネルで、「 **スケジュール** を選択します。

   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

1. （オプション）スケジューリングタイムラインに表示するコンテンツをカスタマイズするフィルターを作成します。詳しくは、 [スケジュール領域の情報のフィルタリング](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) . [スケジュール領域の情報のフィルタリング](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md). 例えば、イシューがスケジュールタイムラインに表示されるようにするには、フィルターを作成する必要があります。

1. （オプション）スケジュールタイムラインに表示される日付範囲を変更します。詳しくは、 [スケジュール領域の日付範囲を調整する](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [リソーススケジュールの概要](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

1. 未割り当てのタスクまたはイシューを割り当てるには、以下の手順を実行します。

   * 割り当てるユーザーの行にタスクまたはタスクをドラッグします。\
      特定のユーザーに対して 1 日あたり最大 10 個のタスクが表示されます。 リストを展開して、そのユーザーに現在割り当てられているすべてのタスクを表示できます。 （スケジュールタイムラインで割り当てを行うと、10 個を超えるタスクが一時的に表示される場合があります）。\
      項目をドラッグすると、タスクまたは問題を解放し、割り当てを完了する前に、次の情報が表示されます。

   * スケジューリング・タイムラインでユーザー割当が有効になっている場合、割当が完了すると、割当が完了すると、赤色の割当超過指標が表示され、割当が超過したユーザーが表示されます。\
      割り当て超過の指標について詳しくは、 [配分指標](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators) 記事内 [スケジューリング領域でユーザー割り当てを管理します](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      この **一致する役割を持つユーザーに割り当てを制限** 「設定」領域の「 」オプションが有効になっている場合は、割り当てを受け取る資格のないユーザーは淡色表示になります。 このオプションを無効にした場合、すべてのユーザーが割り当てを受け取ることができます。 このオプションは、デフォルトで有効になっています。\
      このオプションについて詳しくは、 [](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md#allowing-assignmennts-to-users-regardless-of-role) in [スケジュール領域の役割およびグループメンバーシップに関係なく、ユーザー割り当てを許可します](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

      ユーザーの行にドロップインジケーターが表示されます。 これにより、割り当てを行う前に項目が割り当てられている場所を確認できます。

      割り当てるタスクまたは問題を展開し、 **割り当て** 「 」フィールドに割り当てるユーザーの名前を入力し、ドロップダウンリストでユーザーの名前をクリックします。\
      ![schedule_task_expanded.png](assets/schedule-task-expanded-350x170.png)

1. （条件付き）未割り当てのタスクまたはイシューをユーザーに割り当てた後、スケジュールタイムラインで、タスクおよびイシューの既存のアサインを調整する必要が生じる場合があります。 プロジェクトのリソースをスケジュールする場合（「スケジュール設定」タブまたは「スタッフィング」タブ）、同じジョブロールを持つユーザーのみが割り当てを受け取ることができます。\
   タスクまたはイシューを別のユーザーに再割り当てするには、あるユーザーの行から別のユーザーの行にタスクをドラッグします。
1. （オプション）割り当てられた各ユーザーをタスクまたはイシューに割り当てる時間数を設定します。詳しくは、 [スケジューリング領域でユーザー割り当てを管理します](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) .
