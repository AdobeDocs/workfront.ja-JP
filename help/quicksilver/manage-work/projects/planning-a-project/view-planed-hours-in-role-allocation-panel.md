---
product-area: projects
navigation-topic: plan-a-project
title: 役割割り当てパネルでのプロジェクト予定時間の表示
description: プロジェクトの役割割り当てパネルで、プロジェクトの作業項目に割り当てられているすべてのジョブロールの役割割り当てを表示できます。
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# 役割割り当てパネルでのプロジェクト予定時間の表示

プロジェクトの役割割り当てパネルで、プロジェクトの作業項目に割り当てられているすべてのジョブロールの役割割り当てを表示できます。

>[!NOTE]
>
>この記事では、プロジェクトの役割割り当てパネルで、プロジェクトのタスクと問題に関連するジョブの役割と、割り当てられた予定時間を表示します。 Adobe Workfront Scenario Planner を使用する際の「役割割当パネル」を使用した計画時間と構想時間の紐付けの詳細は、次を参照してください。
>
>* [タスクリストのプロジェクトおよびイニシアチブのロール割り当てを表示](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [ワークロードバランサーのプロジェクトおよびイニシアチブの役割割り当てを表示](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  「ロール割当」パネルにイニシアチブ時間を表示するには、シナリオ・プランナのライセンスが必要です。 シナリオ・プランナの詳細は、 [シナリオプランナーの概要](../../../scenario-planner/get-started-with-scenario-planning.md) .

## アクセス要件

<!--drafted for P&P:

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
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセス権を表示または高くする</p> <p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示権限以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

以下が必要です。

* ジョブの役割またはジョブの役割に関連付けられたユーザーに割り当てられたタスクまたはタスク。

   >[!TIP]
   タスクまたはタスクが未割り当ての場合、チームに割り当てられた場合、またはジョブロールのないユーザーに割り当てられた場合、プロジェクトの計画時間は「ロール割り当て」パネルでゼロになります。

* 期間が 0 よりも長いタスクおよび問題。

## 役割割り当てパネルでのプロジェクト予定時間の表示

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **プロジェクト**.
1. プロジェクトの名前をクリックしてアクセスします。 「プロジェクト」ページが開きます。
1. 左側のパネルで、次のいずれかをクリックします。

   * **タスク**
   * **ワークロードバランサー**

1. 次をクリック： **ロール配分を表示** アイコン ![](assets/show-role-allocation-icon.png).

   役割割り当てパネルが表示されます。

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. 次の情報を **ロールの配分** パネル： |フィールド |説明| |—|—| | **ジョブの役割** |プロジェクトのタスクとタスクに割り当てられたジョブの役割。 タスクとタスクに直接割り当てられるジョブの役割、またはタスクに割り当てられたユーザーとプロジェクトのタスクに関連付けられるジョブの役割を指定できます。  | | **予定時間** |プロジェクトのジョブロールに関連付けられたジョブロールまたはユーザーに割り当てられたタスクおよびタスクからの予定時間数の合計です。 |



