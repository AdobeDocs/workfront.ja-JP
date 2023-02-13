---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: スケジュール領域の役割およびグループメンバーシップに関係なく、ユーザー割り当てを許可します
description: リソーススケジュール設定では、タスクまたはタスクに割り当てられている問題の役割割り当てに一致する役割がユーザープロファイルで定義されているユーザーに対してのみ割り当てを行うことができます。
author: Alina
feature: Resource Management
exl-id: 0f90ffde-6f07-4c3c-b963-de28b1b55dc1
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---

# スケジュール領域の役割およびグループメンバーシップに関係なく、ユーザー割り当てを許可します

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer.</span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;***LINKED TO THE UI FROM Resource Scheduling (People> Teams>Working On>Settings>Limit Assignments to the Group Associated with the Project) - ALSO FROM THE WORKING ON TAB OF TEAMS and AT THE PROJECT STAFFING TAB TOO)</p>
<p>NOTE: Alina; broken off the original article; retitle, reformat, relink sections) </p>
</div>
-->

既定では、割り当ては、リソーススケジュールツールを使用して割り当てられているタスクまたはタスクの役割割り当てに一致する役割がユーザープロファイルで定義されているユーザーに対してのみ実行できます。

Adobe Workfrontを設定すると、タスクの役割割り当てに一致する役割がユーザープロファイルに定義されているかどうかに関係なく、タスクとタスクを任意のユーザーに割り当てることができます。 タスクまたはイシューにユーザーを割り当て、そのユーザーがタスクまたはイシューに対するロール割り当てに一致するロールを持たない場合、元のロール割り当ては削除され、ロール割り当ては割り当てるユーザーのロールに変更されます。

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
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プロジェクト、タスク、問題へのアクセス権を表示または高くする</p> <p><strong>メモ</strong>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスク、および割り当てを更新するタスクに、権限以上を貢献する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 役割に関係なくユーザーへの割り当てを許可

1. 複数のプロジェクト、個々のプロジェクト、またはチームのスケジューリングタイムラインに移動します。

   * **複数のプロジェクトの場合**:  次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅にある **リソース > ワークロードバランサー**&#x200B;を選択し、「 **スケジュール** をクリックします。
   * **個々のプロジェクトの場合**:プロジェクトに移動し、 **ワークロードバランサー** セクションを開き、 **スケジュール** を選択します。
   * **チームの場合**:次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅で、 **チーム**、チームを選択して、 **ワークロードバランサー** 左のパネルで、「 **スケジュール** を選択します。

1. 次をクリック： **設定** アイコンをクリックします。
1. オプションを無効にする **ロールが一致するユーザーに割り当てを制限**.
1. クリック **スケジュールに戻る**.

## グループのメンバーシップに関係なく、ユーザーへの割り当てを許可

<!--
<p>(NOTE: Alina: **^ This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!!) </p>
-->

既定では、割り当ては、プロジェクトに関連付けられたグループのメンバー（プロジェクトの編集時に定義されるグループ）であるユーザーに対してのみ実行できます。

>[!IMPORTANT]
>
>この設定では、プロジェクトに関連付けられたグループのメンバーのみが考慮され、そのグループのサブグループのメンバーは考慮されません。

Workfrontを設定すると、タスクまたはイシューが存在するプロジェクトに関連付けられたグループのメンバーかどうかに関係なく、タスクおよびイシューを任意のユーザーに割り当てることができます。

1. 複数のプロジェクト、個々のプロジェクト、またはチームのスケジューリングタイムラインに移動します。

   * **複数のプロジェクトの場合**:  次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅にある **リソース > ワークロードバランサー**&#x200B;を選択し、「 **スケジュール** をクリックします。
   * **個々のプロジェクトの場合**:プロジェクトに移動し、 **ワークロードバランサー** セクションを開き、 **スケジュール** を選択します。
   * **チームの場合**:次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅で、 **チーム**、チームを選択して、 **ワークロードバランサー** 左のパネルで、「 **スケジュール** を選択します。

1. 次をクリック： **設定** アイコンをクリックします。
1. オプションを無効にする **割り当てをプロジェクトに関連付けられたグループに制限**.
1. クリック **スケジュールに戻る**.

 
