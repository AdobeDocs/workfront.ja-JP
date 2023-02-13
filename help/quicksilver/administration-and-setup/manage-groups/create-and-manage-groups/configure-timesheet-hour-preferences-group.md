---
user-type: administrator
product-area: system-administration;user-management
keywords: グループ，環境設定，タスク，グループ，問題，ロック解除
navigation-topic: create-and-manage-groups
title: グループのタイムシートと時間の基本設定を構成する
description: システムレベルで、Adobe Workfront管理者は、タイムシートと時間の基本設定セクションの [ 一般基本設定 ] と [ タイムシートの事前入力 ] のロックを解除できます。 これにより、グループ管理者は、これらのセクションのオプションを、それぞれのグループに対して個別に設定できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 0%

---

# グループのタイムシートと時間の基本設定を構成する

Adobe Workfrontの管理者は、タイムシートと時間の基本設定の次のセクションをシステムレベルでロック解除して、グループ管理者が独自のグループに対して個別に構成できるようにします。

* 一般設定
* タイムシートの事前入力

管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

[ タイムシートと時間の基本設定 ] ページの次のセクションは、システムレベルでのみ構成可能で、グループのロックを解除できません。

* ログ時間
* プロジェクト、タスクまたは、問題削除設定

Workfront管理者がタイムシートと時間の優先順位のロックを解除する方法の詳細については、「 [グループのタイムシートと時間の基本設定をロック解除](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 記事内 [タイムシートと時間の基本設定を構成する](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>グループレベルの設定は、プロジェクトの環境設定や、タスクと問題の環境設定でも可能です。 詳しくは、 [グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) および [グループのタスクと問題の環境設定を設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## タイムシートと時間の基本設定をグループ化

グループのロック解除されたタイムシートまたは時間の優先順位の構成に関する次の情報を考慮してください。

* グループ管理者が、グループのタイムシートまたは時間の優先順位を設定した場合、グループをホームグループとして使用する人に影響を与えます。
* 通常、ロックが解除された環境設定は、無期限にロックが解除されたままになります。 Workfront管理者が再ロックすると、システム設定が再度有効になり、グループ管理者が行った環境設定は失われます。
* タイムシートは、タイムシート所有者のホームグループに対して構成されたタイムシートと時間の基本設定を継承します。

   <!--
  Add example here?
  -->

* Workfront管理者がシステムレベルで環境設定のロックを解除し、自分のグループに対して設定した後は、下のグループの全員が同じ設定を使用するようにロックできます。 これは、Workfront管理者がシステム内のすべてのユーザーに対して環境設定を設定およびロックする必要がある機能と同じです。 詳しくは、 [グループのタイムシートと時間の優先順位をロックまたはロック解除する](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## グループのロック解除されたタイムシートまたは時間の優先設定を構成する

>[!TIP]
>
>Workfrontの管理者は、[ 設定 ] > [ タイムシートと時間 ] > [ 環境設定 ] に移動して、ページ上部のボックスでグループの名前を検索することで、手順 1 ～ 4 をスキップできます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. タイムシートまたは時間の基本設定を構成するグループの名前をクリックします。
1. 左側のパネルで、 **タイムシートと時間**.

1. 表示されるページの **一般環境設定** セクションで、次のいずれかのオプションを設定します。

   >[!TIP]
   >
   >環境設定の上にマウスポインターを置くと、その設定がロックされていることを示すツールヒントが表示される場合は、Workfront管理者に問い合わせて、組織内のすべてのグループのロックを解除するように依頼できます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">将来の日付のログ時間</td> 
      <td> <p>ユーザーがシステム全体の将来の日付の時刻を次の場所に記録できるようにします。</p> 
       <ul> 
       <li>プロジェクトのグループに関係なく、ログ時間にアクセスできるプロジェクト、タスクおよび問題</li> 
       <li>一般時間としてのタイムシート</li>
       </ul> 
       <p>これは、ユーザーがオフィスを離れる予定で、事前にその時間をログに記録したい場合に便利です。</p> 
       <p><b>注意</b>:ユーザーが終了またはキャンセルしたタスクや問題に対して時間を記録するのを防ぐことはできません。 ユーザーが完了または無効なプロジェクトで時間をログに記録するのを防ぐことができます。 タスクやタスクのリストでフィルターを使用して、完了またはキャンセルしたタスクをユーザーに表示しないようにすることをお勧めします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートから費用を追加</td> 
      <td> <p>ユーザーがタイムシートに時間と費用の両方を記録できるようにします。</p> 
      <p>この環境設定をグループに対して有効にし、グループを特定のユーザーのホームグループとして設定すると、そのユーザーのタイムシートのプロジェクトとタスクの横に費用アイコンが表示されます。 ユーザーはこのアイコンをクリックして、プロジェクトまたはタスクの費用を追加または編集できます。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ジョブの役割を時間エントリに手動で割り当て</td> 
      <td> <p>ユーザープロファイルに割り当てられたジョブロールまたはオブジェクトに割り当てられたジョブロールを、ユーザーが手動で選択できるようにします。</p> <p><b>重要</b>:  
        <ul> 
         <li>時間エントリにジョブの役割を割り当てた後にこの設定を無効にした場合、ユーザーは、プロジェクト、タスク、またはイシューの [ 時間 ] タブで、様々な役割の下に記録される時間を調整する必要があります。</li> 
         <li>ユーザーのプロファイルにジョブの役割が割り当てられていない場合、[ 割り当ての詳細設定 ] ダイアログボックスでタスクの所有者として割り当てられたタスクがあると、そのジョブの役割は、ユーザーがタスクの時間をログに記録したときに表示されます。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">タイムシートの編集を所有者と管理者に制限する</td> 
      <td> <p>プロジェクトのグループとWorkfront管理者に関係なく、編集をタイムシートの所有者に制限します。 このオプションを無効にした場合、タイムシートは次のユーザーも編集できます。</p> 
       <ul> 
        <li> <p>タイムシートおよびアクセスレベルの時間に管理アクセス権を持つユーザー</p> </li> 
        <li> <p>タイムシートで [ 時間の編集が可能 ] が有効になっている場合のタイムシートの承認者</p> </li> 
        <li> <p>タイムシート所有者の管理者</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">所有者と管理者に時間の編集を制限</td> 
      <td>時間を入力したユーザーとWorkfront管理者に編集を制限します。 この設定は、プロジェクトの「時間」タブまたは時間レポートに適用されます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 内 **タイムシートの事前入力** セクションで、次のいずれかのオプションを設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">内にある作業 &lt;number of="" weeks=""&gt; タイムシートの作業範囲の</td> 
      <td> <p>ユーザーに割り当てられたタスクとタスクの日付が含まれるタイムシートの日付範囲の前後の週数を定義します。 デフォルト設定は 1 週間で、この範囲を 4 週間に延長できます。 つまり、タイムシートには、タイムシートの日付範囲の 4 週間前からタイムシートの日付範囲の 4 週間後までの間の日付があるタスクと問題が事前に設定されています。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了したタスクと問題</td> 
      <td>通常、1 つのタスクに複数のリソースが割り当てられる場合は、この設定をお勧めします。 つまり、あるリソースがタスクに対する時間を記録し、完了とマークした場合でも、タスクに割り当てられた他のリソースは、タイムシートでタスクや問題を見つけて、時間を記録できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートの日付範囲に予定日が設定されたタスクとタスク</td> 
      <td> <p>選択すると、タイムシートには、タイムシートの日付範囲に含まれる予定開始日または完了日のタスクとタスクが含まれます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> タイムシートの日付範囲に予測日付があるタスク</td> 
      <td> <p>選択すると、タイムシートには、発行またはタスクの予定日がタイムシートの日付範囲外にある場合でも、プロジェクトの期間内に [ 予定開始日 ] または [ 完了日 ] が設定されたタスクが含まれます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
