---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: タスクリストのプロジェクトおよびイニシアチブのロール割り当てを表示
description: プロジェクトとイニシアチブを結び付けた後、リソースの割り当てを並べて管理し、それらが一致するようにします。 これにより、割り当て超過や過剰な利用を回避できます。
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# タスクリストのプロジェクトおよびイニシアチブのロール割り当てを表示

>[!IMPORTANT]
>
>組織は、 [!DNL Adobe Workfront Scenario Planner] プロジェクトのイニシアチブ情報を表示できます。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 [を使用するために必要なアクセス [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

プロジェクトとイニシアチブを結び付けた後、リソースの割り当てを並べて管理し、それらが一致するようにします。 これにより、割り当て超過や過剰な利用を回避できます。

ここでは、 [!UICONTROL ロールの配分] パネルを使用して、プロジェクトのタスクリストに表示できます。

前提条件を含む、プロジェクトとイニシアチブ間でのリソースの調整に関する一般的な情報については、 [プロジェクトとイニシアチブ間でのリソース割り当て調整の概要](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## アクセス要件

次の操作が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 計画*</b> </p> </td> 
   <td>[!UICONTROL Business] 以降</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> ライセンス*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td><b>製品</b> </td> 
   <td> <p>の追加ライセンスを購入する必要があります。 [!DNL Adobe Workfront Scenario Planner] をクリックして、この記事で説明する機能にアクセスします。</p> <p>詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">を使用するために必要なアクセス [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>[!UICONTROL 表示 ] 以降のプロジェクトへのアクセス </p> <p>注意：まだアクセス権がない場合は、[!UICONTROL Workfront] 管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 [!UICONTROL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクト権限</strong> </p> </td> 
   <td> <p>プロジェクトに対する [!UICONTROL 表示 ] 以上の権限</p> <p>プランへの追加アクセス権のリクエストについて詳しくは、 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">内のプランへのアクセスをリクエスト [!DNL Scenario Planner]</a>.</p> <p>プロジェクトへの追加アクセス権のリクエストについては、 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## タスクリストのプロジェクトおよびイニシアチブのロール割り当てを表示

会社が [!DNL Workfront Scenario Planner] ライセンスを使用すると、イニシアチブと、イニシアチブにリンクされているプロジェクトとの間のリソース割り当てを [!UICONTROL タスク] プロジェクトのセクション。

1. （条件付き） [タスクリストのプロジェクトおよびイニシアチブのロール割り当てを表示](#Connect) 」を参照してください。

   >[!IMPORTANT]
   >
   >イニシアチブのリソースに変更を加える場合、イニシアチブの最新のリソース情報をプロジェクトで更新するには、イニシアチブが属するシナリオを再公開する必要があります。

1. プロジェクトおよび関連するイニシアチブのジョブの役割の割り当てを確認するプロジェクトに移動します。
1. クリック **[!UICONTROL タスク]** をクリックします。
1. 次をクリック： **[!UICONTROL ロール配分を表示]** アイコン ![](assets/show-role-allocation-icon.png) をクリックします。

   この [!UICONTROL ロールの配分] パネルが表示されます。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 次の情報を **[!UICONTROL プロジェクト合計]** 領域 [!UICONTROL ロールの配分] パネル：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ジョブの役割 ]</td> 
      <td> <p>次のいずれかに関連付けられたジョブロールの名前。</p> 
       <ul> 
        <li> <p>プロジェクトのタスク</p> </li> 
        <li> <p>プロジェクトに関する問題</p> </li> 
        <li> <p>プロジェクトにリンクされたイニシアチブ</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>イニシアチブの全期間における、イニシアチブの各ジョブの役割に関連付けられる必要な時間数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 予定時間数 ]</td> 
      <td>プロジェクトの全期間における、プロジェクトのタスクまたは問題の各ジョブの役割に関連する計画時間数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 平方偏差 ]</td> 
      <td> <p>イニシアチブに必要な時間と、プロジェクトの作業に関連する計画時間との差。 [!DNL Workfront] 次の式を使用して [!UICONTROL 平方偏差 ] を計算します。</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>イニシアチブで必要以上の時間リソースが計画されている場合、[!UICONTROL 平方偏差 ] は負の値で、赤で表示されます。 つまり、リソースの割り当てが超過しています。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >プロジェクトからの計画時間は、次のシナリオでは表示されません。
   >
   >   
   >   
   >   * タスクまたはタスクがジョブロールに割り当てられていない場合、またはジョブロールが関連付けられているユーザー。
   >   * タスクまたはタスクの期間がゼロの場合。




1. （オプション） [!UICONTROL 平方偏差] 列には、リソースが割り当て超過になっていることを示し、次のいずれかを調整します。

   * 割り当て超過を示すジョブロールの計画時間数を減らすか、タスクにリソースを追加し、新しいリソースに計画時間を配分します。 割り当てを更新したり、タスクまたはタスクの編集時に予定時間数を更新したりできます。 詳しくは、次の記事を参照してください。

      * [タスクを編集](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [問題の編集](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >タスクと問題を編集するには、追加のアクセス権と権限が必要です。

   * イニシアチブの割り当て超過を示す役割に必要な時間数を増やします。 詳しくは、 [のイニシアチブを作成および編集します [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >プランを編集するには、追加のアクセス権と権限が必要です。



