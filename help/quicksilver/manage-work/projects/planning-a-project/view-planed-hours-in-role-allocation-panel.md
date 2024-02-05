---
product-area: projects
navigation-topic: plan-a-project
title: 役割の配分パネルでプロジェクトの予定時間数を表示
description: プロジェクトの役割の配分パネルでは、プロジェクトの作業アイテムに割り当てられているすべての担当業務について、役割の配分を表示できます。
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: ht
source-wordcount: '468'
ht-degree: 100%

---

# 役割の配分パネルでプロジェクトの予定時間数を表示

プロジェクトの役割の配分パネルでは、プロジェクトの作業アイテムに割り当てられているすべての担当業務について、役割の配分を表示できます。

>[!NOTE]
>
>この記事では、プロジェクトの役割の配分パネルでの、プロジェクトのタスクとイシューに関連する担当業務と、配分された予定時間数の表示について説明します。Adobe Workfront Scenario Planner を使用する際に、役割の配分パネルを使用して予定時間数とイニシアチブの時間数を調整する方法について詳しくは、以下を参照してください。
>
>* [タスクリストのプロジェクトとイニシアチブの役割の配分を表示](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [ワークロードバランサーのプロジェクトとイニシアチブの役割の配分を表示](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  役割の配分パネルにイニシアチブの時間数を表示するには、シナリオプランナーのライセンスが必要です。シナリオプランナーについては、[シナリオプランナーの概要](../../../scenario-planner/get-started-with-scenario-planning.md)を参照してください。
>

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトに対する表示以上のアクセス権</p> <p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がユーザーのアクセスレベルを変更する方法については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 前提条件

以下が必要です。

* 担当業務または担当業務に関連付けられたユーザーに割り当てられたタスクまたはイシュー。

  >[!TIP]
  >
  >タスクまたはイシューが未割り当ての場合、チームに割り当てられた場合、または担当業務のないユーザーに割り当てられた場合、プロジェクトの予定時間数は役割の配分パネルでゼロになります。

* 期間が 0 よりも長いタスクとイシュー。

## 役割の配分パネルでプロジェクトの予定時間数を表示

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**プロジェクト**」の順にクリックします。
1. プロジェクト名をクリックしてアクセスします。プロジェクトページが開きます。
1. 左側のパネルで、次のいずれかをクリックします。

   * **タスク**
   * **ワークロードバランサー**

1. **役割の配分を表示**&#x200B;アイコン ![](assets/show-role-allocation-icon.png) をクリックします。

   役割の配分パネルが表示されます。

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. **役割の配分**パネルで次の情報を確認します。
|フィールド | 説明|
|---|---|
| **担当業務** |プロジェクトでタスクとイシューに割り当てられた担当業務です。これは、プロジェクトのタスクとイシューに直接割り当てられた担当業務、またはタスクとイシューに割り当てられたユーザーに関連付けられた担当業務である場合があります。|
| **予定時間数** |プロジェクトの担当業務、または担当業務に関連付けられたユーザーに割り当てられた、タスクとイシューからの予定時間数の合計です。|



