---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: タスクリストのプロジェクトおよびイニシアチブに対する役割の割り当てを表示
description: プロジェクトとイニシアチブを結び付けた後、リソースの割り当てを横に並べ、それらが一致するよう管理できます。これにより、過剰な割り当てや割り当て不足を回避できます。
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 82%

---

# タスクリストのプロジェクトおよびイニシアチブに対する役割の割り当てを表示

<!--Audited: 07/2024-->

プロジェクトとイニシアチブを結び付けた後、リソースの割り当てを横に並べ、それらが一致するよう管理できます。これにより、過剰な割り当てや割り当て不足を回避できます。

この記事では、プロジェクトのタスクリストの[!UICONTROL 役割の割り当て]パネルを使用して、リソースを調整する方法について説明します。

前提条件を含む、プロジェクトとイニシアチブ間でのリソースの調整に関する一般的な情報について詳しくは、[プロジェクトとイニシアチブ間でのリソース割り当て調整の概要](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] プラン*</p> </td> 
   <td> <ul></li>
   <li><p>新規：Ultimate </p></li>
   <p>シナリオプランナーは、新しいWorkfront Select プランまたはWorkfront Prime プランでは使用できません。 </p>
   <li><p>現在：[!UICONTROL Business] 以上</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] ライセンス*</p> </td> 
   <td> <p>新規：ライト以上</p> 
   <p>現在：[!UICONTROL Review] 以上</p> </td> 
  </tr> 
  <tr> 
   <td>製品* </td> 
   <td> <ul><li><p>新しいWorkfrontプランの場合：</p><p> Adobe Workfront</li></p>
   <li><p>現在のWorkfront プランの場合： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront シナリオプランナー</p></li></ul>

<p>詳しくは、<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!DNL Scenario Planner]</a> ールの使用に必要なアクセス権」を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>アクセスレベル </td> 
   <td> <p>プロジェクトへの表示以上のアクセス。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>オブジェクト権限 </p> </td> 
   <td> <p> プロジェクトに対する表示以上の権限。</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfrontへのアクセス要件ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## タスクリストのプロジェクトおよびイニシアチブに対する役割の割り当てを表示

会社が [!DNL Workfront Scenario Planner] ライセンスを購入している場合、プロジェクトの[!UICONTROL タスク]セクションでイニシアチブおよびイニシアチブにリンクされているプロジェクトとの間のリソース割り当てを調整できます。

1. （条件付き）プロジェクトは、この記事の [ タスクリストにプロジェクトとイニシアチブの役割の割り当てを表示 ](#show-role-allocation-for-projects-and-initiatives-in-the-task-list) で説明されている方法の 1 つを使用して、イニシアチブに接続する必要があります。

   >[!IMPORTANT]
   >
   >イニシアチブのリソースに変更を加える場合、イニシアチブの最新のリソース情報をプロジェクトで更新するには、イニシアチブが属するシナリオを再公開する必要があります。

1. プロジェクトおよび関連するイニシアチブの担当業務の割り当てを確認するプロジェクトに移動します。
1. 左側のパネルの「**[!UICONTROL タスク]**」をクリックします。
1. ツールバーの右上隅にある **[!UICONTROL 役割の割り当てを表示]** アイコン ![ 役割の割り当てを表示 ](assets/show-role-allocation-icon.png) をクリックします。

   [!UICONTROL 役割の割り当て]パネルが表示されます。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. [!UICONTROL 役割の割り当て]パネルの&#x200B;**[!UICONTROL プロジェクト合計]**&#x200B;エリアにある次の情報を確認します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Role]</td> 
      <td> <p>次のいずれかに関連付けられた担当業務の名前。</p> 
       <ul> 
        <li> <p>プロジェクトのタスク</p> </li> 
        <li> <p>プロジェクトのイシュー</p> </li> 
        <li> <p>プロジェクトにリンクされたイニシアチブ</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>イニシアチブの全期間における、イニシアチブの各担当業務に関連付けられる必要な時間数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Planned Hours]</td> 
      <td>プロジェクトの全期間における、プロジェクトのタスクまたはイシューの各担当業務に関連付けられた予定時間数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>イニシアチブに必要な時間と、プロジェクトの作業に関連する予定時間数との差。[!DNL Workfront] は、以下の式を使用して [!UICONTROL Variance] を計算します。</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>イニシアチブで必要以上の時間リソースが予定されている場合、[!UICONTROL Variance] は負の値となり、赤で表示されます。つまり、リソースの割り当てが超過しています。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >プロジェクトからの予定時間数は、次のシナリオでは表示されません。
   >
   >   
   >   
   >   * タスクまたはイシューが担当業務に割り当てられていない場合、または担当業務が関連付けられているユーザーの場合。
   >   * タスクまたはイシューの期間がゼロの場合。
   >   
   >



1. （オプション）[!UICONTROL 平方偏差]列にリソースの割り当て超過が表示されている場合、次のいずれかを調整します。

   * 割り当て超過を示す担当業務の予定時間数を減らすか、タスクにリソースを追加し、新しいリソースに対する予定時間数を増やします。割り当てを更新したり、タスクまたはイシューの編集時に予定時間数を更新したりできます。詳しくは、次の記事を参照してください。

      * [タスクを編集](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [イシューを編集](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >タスクとイシューを編集するには、追加のアクセス権と権限が必要です。

   * イニシアチブの割り当て超過を示す役割に必要な時間数を増やします。詳しくは、[ [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md) でのイニシアチブの作成と編集を参照してください。

     >[!NOTE]
     >
     >計画を編集するには、追加のアクセス権と権限が必要です。


