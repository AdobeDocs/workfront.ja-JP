---
user-type: administrator
product-area: system-administration;user-management
keywords: グループ,環境設定,タスク,グループ,イシュー,ロック解除
navigation-topic: create-and-manage-groups
title: グループのタイムシートおよび時間設定を構成する
description: Adobe Workfront 管理者は、タイムシートおよび時間設定の「一般的な環境設定」セクションと「タイムシートに事前入力」セクションをシステムレベルでロック解除できます。これにより、グループ管理者がこれらのセクションのオプションを自分のグループに対して個別に設定できるようになります。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 97%

---

# グループのタイムシートおよび時間環境設定の指定

Adobe Workfront 管理者は、タイムシートおよび時間設定の次のセクションをシステムレベルでロック解除でき、その結果、グループ管理者が自分のグループに対してこれらのセクションのオプションを個別に設定できるようになります。

* 一般的な環境設定
* ユーザーが時間をログに記録できる場所
* タイムシートに事前入力

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

タイムシートおよび時間設定ページの次のセクションは、システムレベルでのみ設定可能で、グループに対してロック解除できません。

* 削除されたプロジェクト、タスク、問題

Workfront 管理者がタイムシートおよび時間環境設定のロックを解除する方法については、[タイムシートおよび時間環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)の記事の[グループのタイムシートおよび時間環境設定のロック解除](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock)を参照してください。

>[!TIP]
>
>グループレベルの設定は、プロジェクト環境設定やタスクおよびイシュー環境設定でも可能です。詳しくは、[グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)および[グループのタスクおよびイシュー環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>グループのグループ管理者またはシステム管理者である必要があります。</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループのタイムシートおよび時間環境設定

ロック解除されたタイムシートまたは時間環境設定のグループへの指定については、以下を考慮してください。

* グループ管理者が、グループのタイムシートまたは時間環境設定を指定した場合は、そのグループをホームグループとして使用するユーザーに影響を与えます。
* 通常、ロック解除された環境設定は、無期限にロック解除されたままになります。Workfront 管理者が再ロックすると、システム設定が再度有効になり、グループ管理者が行った環境設定は失われます。
* タイムシートは、タイムシート所有者のホームグループに対して指定されたタイムシートおよび時間環境設定を継承します。

  <!--
  Add example here?
  -->

* Workfront 管理者がシステムレベルで環境設定のロックを解除し、グループ管理者が自分のグループに対して設定した後は、配下のグループの全員が同じ設定を使用するようにロックできます。これは、Workfront 管理者がシステム内のすべてのユーザーに対して環境設定を指定およびロックするための機能と同じです。詳しくは、[グループのタイムシートおよび時間環境設定のロックまたはロック解除](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md)を参照してください。

## ロック解除されたタイムシートまたは時間環境設定のグループへの指定

>[!TIP]
>
>Workfront 管理者は、設定／タイムシートと時間／環境設定に移動して、ページ上部のボックスでグループの名前を検索することで、手順 1～4 をスキップできます。

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**![ グループ ](assets/groups-icon.png)」をクリックします。

1. タイムシートまたは時間環境設定を指定するグループの名前をクリックします。
1. 左パネルで、「**タイムシートと時間**」をクリックします。

1. 表示されるページの「**一般的な環境設定**」セクションで、次のオプションのいずれかを設定します。

   >[!TIP]
   >
   >環境設定にポインタを合わせると、その設定がロックされていることを示すツールヒントが表示される場合は、Workfront 管理者に問い合わせて、組織内のすべてのグループについてロックを解除するように依頼します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">未来の日付の時間を記録</td> 
      <td> <p>ユーザーがシステム全体の未来の日付の時間を次の場所で記録できるようにします。</p> 
       <ul> 
       <li>プロジェクトのグループに関係なく、時間を記録するためのアクセス権があるすべてのプロジェクト、タスクおよびイシュー</li> 
       <li>一般的な時間としてのタイムシート</li>
       </ul> 
       <p>これは、ユーザーがオフィスを離れる予定があり、事前にその時間を記録したい場合に便利です。</p> 
       <p><b>メモ</b>：終了した、またはキャンセルされたタスクやイシューの時間をユーザーが記録することを防ぐことはできません。可能なのは、完了もしくは停止したプロジェクトに関する時間をユーザーに記録させないようにすることだけです。タスクおよびイシューのリストでフィルターを使用して、完了またはキャンセルした項目をユーザーに表示しないようにすることをお勧めします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートから費用を追加</td> 
      <td> <p>ユーザーがタイムシートに時間と費用の両方を記録できるようにします。</p> 
      <p>この環境設定をグループに対して有効にし、グループを特定のユーザーのホームグループとして設定すると、そのユーザーのタイムシートのプロジェクトとタスクの横に費用アイコンが表示されます。ユーザーはこのアイコンをクリックして、プロジェクトまたはタスクの費用を追加したり編集したりできます。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">手動で担当業務を時間エントリに割り当て</td> 
      <td> <p>ユーザープロファイルに割り当てられた、またはオブジェクトに割り当てられた担当業務をユーザーが手動で選択できます。</p> <p><b>重要</b>：  
        <ul> 
         <li>時間エントリに担当業務を割り当てた後に、この設定を無効にした場合、ユーザーは、プロジェクト、タスク、またはイシューの「時間」タブで、様々な役割の下に記録された時間を調整する必要があります。</li> 
         <li>ユーザーのプロファイルに担当業務が割り当てられていない場合、割り当ての詳細設定ダイアログボックスでタスクの所有者として割り当てられたタスクがあると、その担当業務は、ユーザーがタスクの時間をログに記録したときに表示されます。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">タイムシートの変更を所有者と管理者に制限します。</td> 
      <td> <p>プロジェクトのグループと Workfront 管理者に関係なく、編集をタイムシートの所有者に制限します。このオプションを無効にすると、タイムシートは以下のユーザーでも編集できます。</p> 
       <ul> 
        <li> <p>タイムシートおよびアクセスレベルの時間に管理アクセス権を持つユーザー</p> </li> 
        <li> <p>タイムシートで時間の編集が可能が有効になっている場合のタイムシートの承認者</p> </li> 
        <li> <p>タイムシート所有者の管理者</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">時間の編集を所有者と管理者に制限</td> 
      <td>時間を入力したユーザーと Workfront 管理者に編集を制限します。この設定は、プロジェクトの「時間」タブまたは「時間」レポートに適用されます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**ユーザーが時間を記録できる場所**」セクションで、いずれかのオプションを設定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">プロジェクトに直接時間を記録</td> 
      <td>プロジェクトの時間を記録できます（「更新」タブとタイムシートの両方）。ユーザーがプロジェクトレベルで時刻を記録するのを制限する場合は、このオプションのチェックを外してください。</td>
     </tr>
     <tr>
      <td role="rowheader">完了済みプロジェクトに時間を記録</td>
      <td>完了と表示されたプロジェクトに時間を記録できます。このオプションを無効にすると、ユーザーは完了ステータスのプロジェクトに完了した作業時間を記録できなくなります。</td>
     </tr>
     <tr>
      <td role="rowheader">終了したプロジェクトに時間を記録</td> 
      <td>このオプションを有効にすると、ユーザーは無効ステータスのプロジェクトに数時間を記録できます。</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >この環境設定は、ユーザーのホームグループの環境設定に基づいて適用されます。ユーザーのホームグループ環境設定でこれらの設定が有効になっている場合、プロジェクトのグループ環境設定で許可されているかどうかに関係なく、完了したプロジェクトや無効になったプロジェクトを含むプロジェクトに直接時間を記録できます。

1. 「**タイムシートに事前入力**」セクションで、以下のいずれかのオプションを設定できます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">タイムシートの勤務範囲から〈週数〉以内の仕事</td> 
      <td> <p>ユーザーに割り当てられたタスクと課題の日付を含むタイムシートの日付範囲の前後の週数を定義しています。デフォルト設定は 1 週間ですが、この範囲を 4 週間まで拡張できます。つまり、タイムシートの日付範囲に 4 週間を選択した場合、タイムシートの日付範囲の 4 週間前から 4 週間後までの間の日付を持つタスクと課題がタイムシートにあらかじめ入力されます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了済みのタスクとイシュー</td> 
      <td>複数のリソースが通常 1 つのタスクに割り当てられる場合は、この設定をお勧めします。つまり、あるリソースがタスクに対する時間を記録し、完了とマークした場合でも、タスクに割り当てられた他のリソースは、タイムシートでタスクやイシューを見つけて、時間を記録できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートの日付範囲内に予定日があるタスクとイシュー</td> 
      <td> <p>選択した際、タイムシートには、開始予定日または完了予定日がタイムシートの日付範囲内にあるタスクとイシューが含まれます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> タイムシートの日付範囲に見込み日付があるタスク</td> 
      <td> <p>選択した際、タイムシートには、イシューやタスクの予定日がタイムシートの日付範囲外にある場合でも、見込み開始日または見込み完了日がプロジェクト期間内にあるタスクが含まれます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
