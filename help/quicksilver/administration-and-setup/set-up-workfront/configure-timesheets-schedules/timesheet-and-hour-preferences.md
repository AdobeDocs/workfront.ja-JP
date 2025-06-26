---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: タイムシートおよび時間設定の構成
description: ' [!DNL Adobe Workfront]  管理者は、 [!DNL Workfront]  でタイムシートと時間の環境設定を指定して、タイムシートに事前入力できる項目とユーザーが時間を記録できる項目を定義できます。'
author: Alina and Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '1414'
ht-degree: 94%

---

# タイムシートおよび時間の環境設定の指定

<!--Audited: 06/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

[!DNL Adobe Workfront] 管理者は、[!DNL Workfront] でタイムシートと時間の環境設定を指定して、タイムシートに事前入力できる項目とユーザーが時間を記録できる項目を定義できます。

>[!IMPORTANT]
>
>この記事で説明した条件に従ってタイムシートに事前入力される項目に加えて、次の項目もタイムシートに既定で表示されます。
>
>* タイムシートの時間枠内でログに記録した項目
>* タイムシートに固定済みの項目
>* 検索し、タイムシートに手動で追加した項目。手動で追加した項目はデフォルトで固定されます。
>
>詳しくは、[ログ時間](../../../timesheets/create-and-manage-timesheets/log-time.md)と[タイムシートの概要](/help/quicksilver/timesheets/timesheets/timesheets-overview.md)を参照してください。

タイムシートに加えた変更は、今後作成されるすべてのタイムシートに影響します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>現在：[!UICONTROL Plan]</p>
   または
   <p>新規：標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
</tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タイムシートおよび時間の環境設定の指定

{{step-1-to-setup}}

1. **[!UICONTROL タイムシートと時間]**／**[!UICONTROL 環境設定]**&#x200B;をクリックします。

   タイムシートと時間の環境設定ページが表示されます。

1. （オプション）「**システムのタイムシートおよび時間設定**」検索ボックスにグループの名前を入力し、リストに表示されたら選択します。

   ![ 「グループを検索」ボックス ](assets/search-for-group-box-in-timesheets-preferences-page.png)

   タイムシートと時間の環境設定ページは、選択したグループの環境設定で更新されます。グループレベルの環境設定を変更するには、システムレベルの環境設定のロックを解除する必要があります。詳細については、この記事の[グループのタイムシートと時間の環境設定のロックを解除](#unlock-timesheet-and-hour-preferences-for-groups)の節を参照してください。

1. 「**[!UICONTROL 一般的な環境設定]**」セクションで、以下のいずれかのオプションを設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Log time for future dates]</td> 
      <td> <p>ユーザーがシステム全体の未来の日付の時間を次の場所で記録できるようにします。</p> 
       <ul> 
        <li>時間の記録にアクセスできるプロジェクト、タスク、イシュー</li> 
        <li>一般的な時間としてのタイムシート</li> 
       </ul> <p>これは、ユーザーがオフィスを離れる予定があり、事前にその時間を記録したい場合に便利です。</p> <p><b>メモ</b>：</p> 
       <p>終了もしくはキャンセルされたタスクやイシューに関する時間をユーザーが記録するのを防ぐことはできません。可能なのは、完了もしくは停止したプロジェクトに関する時間をユーザーに記録させないようにすることだけです。タスクおよびイシューのリストでフィルターを使用して、完了またはキャンセルした項目をユーザーに表示しないようにすることをお勧めします。</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Assign Job Roles to hour entries manually]</td> 
      <td> <p>ユーザープロファイルに割り当てられた、またはオブジェクトに割り当てられた担当業務をユーザーが手動で選択できます。</p> <p><b>重要</b>：  
        <ul> 
         <li>時間エントリにジョブの役割を割り当てた後にこの設定を無効にした場合、ユーザーは、プロジェクト、タスク、またはイシューの [!UICONTROL Hours] タブで、様々な役割の下に記録される時間を調整する必要があります。</li> 
         <li>ユーザーのプロファイルに担当業務が割り当てられていない場合、[!UICONTROL Advanced Assignments] ダイアログボックスで [!UICONTROL Task Owner] として割り当てられたタスクがあると、その担当業務は、ユーザーがタスクの時間を記録したときに表示されます。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict timesheet editing to owners and administrators]</td> 
      <td> <p>編集を、タイムシート所有者と [!DNL Workfront] 管理者に制限します。このオプションを無効にすると、タイムシートは以下のユーザーでも編集できます。</p> 
       <ul> 
        <li> <p>タイムシートおよびアクセスレベルの時間に管理アクセス権を持つユーザー</p> </li> 
        <li> <p>タイムシートで時間の編集が可能が有効になっている場合のタイムシートの承認者</p> </li> 
        <li> <p>タイムシート所有者の管理者</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict hour editing to owners and administrators]</td> 
      <td>編集を、時間を入力したユーザーと [!DNL Workfront] 管理者に制限します。この設定は、プロジェクトの [!UICONTROL Hours] タブまたは時間レポートに適用されます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL ユーザーが時間を記録できる場所]**」セクションで、いずれかのオプションを設定します。

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Directly on projects]</td>
        <td>ユーザーがプロジェクトの時間を記録できます（[!UICONTROL Updates] タブとタイムシートの両方）。ユーザーがプロジェクトレベルで時間を記録しない場合、このオプションはオフのままにする必要があります。</td>
    </tr>
    <tr>
        <td>[!UICONTROL On projects that are complete]</td>
        <td>完了と表示されたプロジェクトに時間を記録できます。このオプションを無効化すると、ユーザーは [!UICONTROL Complete] ステータスのプロジェクトに完了した作業時間を記録できなくなります。</td>
    </tr>
    <tr>
        <td>[!UICONTROL On projects that are dead]</td>
        <td>このオプションを有効にすると、ユーザーは [!UICONTROL Dead] ステータスのプロジェクトに時間を記録できます。</td>
    </tr>
   </table>

1. 「**[!UICONTROL タイムシートに事前入力]**」セクションで、以下のいずれかのオプションを設定できます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Work that is within] &lt;週数&gt; [!UICONTROL of the timesheet's work range]</td> 
      <td> <p>ユーザーに割り当てられたタスクとイシューの日付を含むタイムシートの日付範囲の前後の週数を定義しています。</p> 
      <p>デフォルト設定は 1 週間ですが、この範囲を 4 週間まで拡張できます。</p> 
      <p>つまり、タイムシートの日付範囲に 4 週間を選択した場合、タイムシートの日付範囲の 4 週間前から 4 週間後までの間の日付を持つタスクと課題がタイムシートにあらかじめ入力されます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks and issues that have been completed]</td> 
      <td>複数のリソースが通常 1 つのタスクに割り当てられる場合は、この設定をお勧めします。つまり、あるリソースがタスクに対する時間を記録し、完了とマークした場合でも、タスクに割り当てられた他のリソースは、タイムシートでタスクやイシューを見つけて、時間を記録できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks and issues that have Planned Dates in timesheet's date range]</td> 
      <td> <p>選択した際、タイムシートには、開始予定日または完了予定日がタイムシートの日付範囲内にあるタスクとイシューが含まれます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tasks that have Projected Dates in timesheet's date range]</td> 
      <td> <p>選択した際、タイムシートには、イシューやタスクの予定日がタイムシートの日付範囲外にある場合でも、見込み開始日または見込み完了日がプロジェクト期間内にあるタスクが含まれます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 削除されたプロジェクト、タスクおよびイシュー]**」セクションで、次のように指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> プロジェクトを削除するタイミング</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Keep logged time already added to timesheets as general time]</strong>：後でこのプロジェクトが復元された場合、時間はタイムシートに残ります。</li> 
        <li><strong>[!UICONTROL Delete any logged time]</strong>：後でこのプロジェクトが復元された場合、記録済みのログ時間はプロジェクトに復元されます。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タスクまたはイシューを削除するタイミング</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Move any logged time to the project]</strong>：タスクまたはイシューが存在する場所。このタスクまたはイシューが後で復元された場合、時間はプロジェクトに残ります。<br></li> 
        <li> <p><strong>[!UICONTROL Delete any logged time]</strong>：後でこのタスクまたはイシューが後で復元された場合、ログ時間はタスクまたはイシューに復元されます。</p> <p>これらのオプションについて詳しくは、<a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">オブジェクトが削除および復元された場合の時間に対する [!UICONTROL Configure affect]</a> を参照してください。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 保存]**」をクリックします。

## グループのタイムシートおよび時間環境設定のロック解除

組織内のグループでは、独自のワークフローに合わせてタイムシートや時間設定を異なる設定にする必要が生じる場合があります。組織全体のすべてのグループの環境設定のロックを解除すると、各グループで独自に設定できるようになります。

環境設定のロックが解除されてグループ管理者が変更を加えると、グループがホームグループである場合は、タイムシートの所有者に影響します。

グループ管理者がグループのタイムシートと時間環境設定を指定する方法について詳しくは、[グループのタイムシートと時間環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)を参照してください。

>[!NOTE]
>
>[!DNL Workfront] 管理者がシステムレベルで環境設定のロックを解除したら、任意のグループ管理者はその設定に変更を加えてロックし、当該グループおよびその下のサブグループの全員が同じ設定を使用するように指定できます。これは、[!DNL Workfront] 管理者がシステム内のすべてのユーザーの環境設定を指定してロックする必要がある機能と同じです。詳しくは、[グループのタイムシートと時間環境設定をロックまたはロック解除](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md)を参照してください。

プロジェクトの環境設定をロック解除して、グループが設定できるようにするには、次の手順を実行します。

{{step-1-to-setup}}

1. 左パネルで「**[!UICONTROL タイムシートと時間]**」をクリックし、「**[!UICONTROL 環境設定]**」をクリックします。

1. 次のいずれかの操作を行います。

   * グループ管理者がグループの環境設定を設定できるようにする場合は、「**ロック解除**」切り替え ![ ロック解除 ](assets/unlock-toggle-button.png) 切り替えをクリックして、ロックを解除します。
   * すべてのグループで環境設定を使用する場合は、ロックされた切替スイッチ ![ ロックされた環境設定の切替スイッチ ](assets/locked-preference-toggle.png) デフォルト）であることを確認します。

     >[!IMPORTANT]
     >
     >ロックされた環境設定を決める際、すべてのニーズに対応できるよう、システム全体のグループの管理者やユーザーとコミュニケーションを取ることをお勧めします。
     >
     >ロックすると、その設定がシステム内のすべてのグループに継承されます。また、環境設定のロックが一定期間解除されている場合、設定はグループ管理者が指定した設定と置き換えられます。

1. 「**[!UICONTROL 保存]**」をクリックします。
