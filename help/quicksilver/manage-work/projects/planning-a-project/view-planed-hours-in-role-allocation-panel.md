---
product-area: projects
navigation-topic: plan-a-project
title: 役割の配分パネルでプロジェクトの予定時間数を表示
description: プロジェクトの役割の配分パネルでは、プロジェクトの作業アイテムに割り当てられているすべての担当業務について、役割の配分を表示できます。
author: Alina, Lisa
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 61%

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
>  役割割り当てパネルにイニシアティブ時間を表示するには、シナリオ プランナ ライセンスが必要です。 シナリオプランナーについては、[ シナリオプランナーの基本を学ぶ ](../../../scenario-planner/get-started-with-scenario-planning.md) を参照してください。
>
>過去に会社がAdobe Scenario Planner を購入したことがある場合は、新しいバージョンに変更されています。 シナリオプランナーは購入できなくなりました。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>Adobe WorkfrontUltimate</p>
   <p>Adobe ワークフローUltimate</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>ライト以上</p>
   <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトに対する表示以上のアクセス権</p>
   <p>シナリオプランナーへのアクセスを編集してイニシアティブの時間を更新</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

able style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
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
</table>-->

## 前提条件

以下が必要です。

* 担当業務または担当業務に関連付けられたユーザーに割り当てられたタスクまたはイシュー。

  >[!TIP]
  >
  >タスクまたはイシューが未割り当ての場合、チームに割り当てられた場合、または担当業務のないユーザーに割り当てられた場合、プロジェクトの予定時間数は役割の配分パネルでゼロになります。

* 期間が 0 よりも長いタスクとイシュー。

## 役割の配分パネルでプロジェクトの予定時間数を表示

{{step1-to-projects}}

1. アクセスするプロジェクトの名前をクリックします。 これにより、プロジェクト ページが開きます。
1. 左側のパネルで、次のいずれかをクリックします。

   * **タスク**
   * **ワークロードバランサー**

1. **役割配分を表示** アイコン ![ 役割配分を表示アイコン ](assets/show-role-allocation-icon.png) をクリックします。

   役割の配分パネルが表示されます。

   ![ 予定時間数のみを含む役割割り当てパネル ](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. **役割の割り当て** パネルで次の情報を確認します。

   | フィールド | 説明 |
   |---|---|
   | **担当業務** | 担当業務は、プロジェクトのタスクおよびイシューに割り当てられています。 タスクやイシューに直接割り当てられた担当業務や、プロジェクトのタスクやイシューに割り当てられたユーザーに関連付けられた担当業務を指定できます。 |
   | **予定時間数** | プロジェクトの担当業務または担当業務に関連付けられたユーザーに割り当てられたタスクと問題からの予定時間数の合計です。 |

