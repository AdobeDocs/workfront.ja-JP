---
product-area: calendars
navigation-topic: use-the-home-area
title: ホームカレンダービューの使用
description: '[!UICONTROL ホーム]エリアのカレンダービューを使用して、作業日と作業の割り当てを管理できます。ホームカレンダーを表示して管理できるのは自分だけです。'
author: Lisa
feature: Get Started with Workfront
exl-id: 07b33b56-ae57-4ae5-890e-c21feae1c4fd
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: ht
source-wordcount: '1602'
ht-degree: 100%

---

# [!UICONTROL ホームカレンダー]ビューの使用

[!UICONTROL ホーム]エリアのカレンダービューを使用して、作業日と作業の割り当てを管理できます。[!UICONTROL ホームカレンダー]を表示して管理できるのは自分だけです。

>[!NOTE]
>
>[!UICONTROL ホーム]エリアの[!UICONTROL カレンダー]ビューは、[!DNL Adobe Workfront][!UICONTROL カレンダー]のレポートとは異なり、自分の作業を視覚的に表現した動的なレポートです。[!DNL Workfront][!UICONTROL カレンダー]のレポートについて詳しくは、[カレンダーレポートの概要](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)を参照してください。
>
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Due to a temporary problem, your Workfront Calendar data might not display as described in this article. This problem will be fixed in the near future. (NOTE: From Alina: Spoke with Lisa and Court and they agreed to draft or delete this. Court could not remember what this was referring to and Lisa did not add this note. Lisa might update this if she hears from the team that this is still accurate.)</li>>
>  -->


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>タスクとイシューに対する[!UICONTROL Edit]アクセス権</p> <p>メモ：アクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者に問い合わせてください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>カレンダーに追加するタスクおよびイシューに対する [!UICONTROL Contribute] の権限以上</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者に問い合わせてください。

## [!UICONTROL ホームカレンダー]での作業アイテムのスケジューリング

[!UICONTROL ホームカレンダー]を使用して、週の作業アイテムをスケジュールできます。

>[!NOTE]
>
>[!UICONTROL ホームカレンダー]に作業アイテムを配置しても、その作業アイテムに関連付けられている既存の日付は変更されません。

[!DNL Workfront] 作業アイテムをカレンダーに追加するには、次の手順に従います。

1. [!UICONTROL ホームカレンダー]ビューに移動します。詳しくは、[[!UICONTROL ホームカレンダーの表示]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)を参照してください。

   自分または自分のグループ、チーム、または担当業務に割り当てられているすべての作業アイテムが左のパネルに表示されます。リストを並べ替えたり、フィルタリングしたりすると、特定のアイテムのみを表示できます。

   詳しくは、この記事の後半の[作業アイテムのフィルタリングと並べ替え](#filter-and-sort-work-items)を参照してください。

1. 左側のパネルから、作業アイテムを作業日時にドラッグします。

   予定完了日より後に、または予定時間数を超える時間でアイテムを作業するようにスケジュールを設定すると、作業アイテムは赤色になり、警告が表示されます。

   作業アイテムの期限と、その期限が[!UICONTROL ホームカレンダー]の割り当て時間にどのように影響するかについて詳しくは、[[!UICONTROL ホームカレンダー]ビュー](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)を参照してください。

1. 次のいずれかの操作を行います。

   * **複数日にわたる作業アイテムをスケジュールする方法：**&#x200B;手順 2 を繰り返して、作業日時ごとにアイテムを追加します。
   * **カレンダーアイテムの期間を変更する方法：**&#x200B;アイテムの下端にカーソルを合わせ、カーソルが二重矢印に変わったら、下端をドラッグして終了時間を指定します。
   * **カレンダーアイテムを削除する方法：**&#x200B;アイテムにカーソルを合わせ、表示される[!UICONTROL ごみ箱]アイコンをクリックします。

## [!UICONTROL ホームカレンダー]の作業アイテムの更新

[!UICONTROL ホームカレンダー]ビューに表示される作業アイテムを更新できます。更新内容は、実際の作業アイテムの「[!UICONTROL 更新]」タブにも表示されます。

1. [!UICONTROL ホームカレンダー]ビューに移動します。詳しくは、[[!UICONTROL ホームカレンダーの表示]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)を参照してください。

1. 更新する作業アイテムの[!UICONTROL 詳細]パネルを開きます。

   * 左側のパネルから作業アイテムを選択して「**[!UICONTROL 詳細]**」をクリックします。
   * カレンダーからスケジュール済みのカレンダーイベントをクリックします。

   作業アイテムの詳細が、画面の右側のパネルに表示されます。

   ![](assets/click-cal-item-to-see-details-350x217.png)

1. 作業アイテムを更新するには、次のいずれかの操作を行います。

   * 「**[!UICONTROL 新しい更新を開始]**」ボックスに更新を入力し、次の情報のいずれかを指定して、「**[!UICONTROL 更新]**」をクリックします。

     <table style="table-layout:auto">
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><strong>[!UICONTROL Notify]</strong></td>
        <td><p> 更新を通知するユーザーにタグを付けます。詳しくは、<a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">更新時の他のユーザーへのタグ付け</a>を参照してください。</p><p> </p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><strong>[!UICONTROL Commit Date]</strong></td>
        <td>ドロップダウンカレンダーで、作業アイテムを完了する予定の日付を選択します。[!UICONTROL Commit Date]の設定について詳しくは、<a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Commit Date]の概要</a>を参照してください。</td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><strong>[!UICONTROL How's this going?]</strong></td>
        <td>タスクまたはイシューの新しい状況を選択します。タスクとイシューの条件について詳しくは、<a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">タスクとイシューの条件の更新</a>を参照してください。</td>
       </tr>
       <tr>
        <td role="rowheader"><strong>社外秘</strong></td>
        <td>社外のユーザーがこの更新を表示できないようにするには、無効にします。</td>
       </tr>
      </tbody>
     </table>

   * 項目の現在の&#x200B;**[!UICONTROL ステータス]**&#x200B;をクリックし、これに続いて表示されるリストで新しいステータスをクリックします。詳しくは、[承認プロセスの概要](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md)を参照してください。

     >[!NOTE]
     >
     >自分に割り当てられた作業項目を[!UICONTROL 完了 - 承認保留中]とマークしている場合は、カレンダーに表示されなくなったことに気付くかもしれません。これは、項目を承認するように設定されているユーザーがその項目を[!UICONTROL 承認済み]とマークするまで、それ以上のアクションが期待されないためです。このような場合、そのアイテムは[!UICONTROL 承認済み]アイテムとしてカレンダーに表示されるようになります。

   * （オプション）既存のコメントまたは更新に返信するには、「**[!UICONTROL 返信]**」をクリックし、**[!UICONTROL 通知]**&#x200B;ボックスで受信者を指定し、返信を入力してから、「**[!UICONTROL 返信]**」をクリックします。

     受信者の指定について詳しくは、[更新時の他のユーザーへのタグ付け](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。

1. （オプション）**[!UICONTROL 詳細]**&#x200B;パネルを閉じるには、パネルの外側をクリックします。

## 統合カレンダーのイベントを更新

[!UICONTROL ホームカレンダー]で統合カレンダーのイベントを更新するには、次の手順に従います。

1. [[!UICONTROL ホームカレンダー]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)の表示の説明に従って、[!UICONTROL ホームカレンダー]ビューに移動します。
1. [!UICONTROL ホームカレンダー]の右上隅にある「**[!UICONTROL カレンダーを更新]**」をクリックします。

   ![](assets/refresh-qs-350x360.png)

   統合カレンダーのイベントは、[!UICONTROL ホームカレンダー]ビューを開いたときや、[!UICONTROL ホームカレンダー]を更新したときに自動的に更新されます。

## 作業アイテムをフィルタリングおよび並べ替え

1. [[!UICONTROL ホームカレンダー]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)の表示の説明に従って、[!UICONTROL ホームカレンダー]ビューに移動します。
1. **[!UICONTROL フィルター]**&#x200B;ドロップダウンメニューをクリックします。

   >[!NOTE]
   >
   >フィルターオプションには、オブジェクト（タスク、リクエスト、イシュー、承認、プルーフおよび個人用）に基づいているものもあれば、状態（[!UICONTROL 作業中]、[!UICONTROL 開始準備完了]、[!UICONTROL 準備未完了]および[!UICONTROL 完了]）に基づいているものもあります。状態が選択されていない場合、[!UICONTROL ホームカレンダー]には、あらゆる状態の選択されたすべてのオブジェクトが表示されます。同様に、オブジェクトが選択されていない場合は、選択された任意の状態のすべてのオブジェクトが表示されます。

1. 以下のフィルターオプションから選択して、表示するアイテムのタイプを指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td><span>すべてのアイテムを表示および選択します。これにはタスク、</span><span data-mc-edit-date="2022-02-16T13:45:46.9712518-05:00" data-mc-editor="alinaw" data-mc-comment="this might need indenting when it goes to Preview" data-mc-initials="AL" data-mc-creator="alinaw" data-mc-create-date="2022-02-16T13:45:23.7889689-05:00">イシュー</span><span>、承認、個人用タスク、完了したタスクおよびイシューが含まれます。</span></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks Working On]</strong></td> 
      <td> <p><span>作業中のタスクのみを表示します。このタスクは、「[!UICONTROL Work On It]」ボタンをクリックして自分に割り当てられたタスクです。</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks Ready to Start]</strong></td> 
      <td> 
       <div> 
        <p>開始する準備が整ったタスクのみを表示します。以下の条件の両方が成り立つ必要があります。</p> 
        <ul style="list-style-type: square;"> 
         <li> <p>タスクとその親には、作業を妨げる先行タスクやタスク制約がない。</p> </li> 
         <li> <p>タスクの[!UICONTROL Planned Start Date]が過去の日付か、最大 2 週間後になっている。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tasks Not Ready]</strong></td> 
      <td> 
       <div> 
        <p>まだ開始する準備ができていないタスクのみを表示します。以下の条件のいずれか 1 つが成り立つ必要があります。</p> 
        <ul> 
         <li> <p>タスクとその親に、作業を妨げる先行タスクやタスク制約がある可能性がある。</p> </li> 
         <li> <p>タスクの[!UICONTROL Planned Start Date]が 2 週間以上後の日付になっている。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues Working On]</strong></td> 
      <td> <p>現在作業中のイシューのみを表示します。このタスクは、「[!UICONTROL Work On It]」ボタンをクリックして自分に割り当てられたイシューです。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Issues Requested]</strong></td> 
      <td><span>「[!UICONTROL Work On It]」ボタンをクリックせずに自分に割り当てられているイシューのみが表示されます。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Personal]</strong></td> 
      <td>個人用タスクのみを表示します。<a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">[!UICONTROL Home]エリアから作業項目を作成</a>記事内の「<a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">[!UICONTROL Create a personal task]</a>」セクションで説明したように、[!UICONTROL To Do] タスクとして作成するタスクです。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>自分に割り当てられた、または委任された承認と、自分が送信した承認のみを表示します。承認には、作業項目（プロジェクト、タスクおよびイシュー）に対する承認、およびドキュメント、プルーフ、アクセス要求およびタイムシートに対する承認が含まれます。承認について詳しくは、次の記事を参照してください。</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">承認の表示</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">承認の管理</a> </p> </li> 
        </ul> 
        <p>メモ：自分が送信し、自分が承認者の 1 人でもある承認は2 回カウントされます。 </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Completed]</strong></td> 
      <td><span>完了したタスク、イシューおよび個人用タスクのみを表示します。完了した作業は、過去 2 週間の期間分が表示され、週ごとにグループ化されて作業リストに表示されます。承認分は含まれません。</span> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/calendar-filters-nwe-350x392.png)

1. 作業のリストをグループ化して並べ替えるには、**[!UICONTROL グループ化]**&#x200B;ドロップダウンメニューをクリックし、使用する条件を選択します。

   項目は、基準と指定した順序に従って、カレンダーの左側に表示されます。

   ![](assets/home-calendar-sort-group-nwe-350x288.png)

   次のオプションから選択します。

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Planned Completion]</strong></td>
        <td>タスクとイシューは、[!UICONTROL Planned Completion dates]の順に並べ替えられます。[!UICONTROL Planned Completion dates]について詳しくは、<a href="../../../manage-work/tasks/task-information/planned-hours.md">予定時間数の概要</a>を参照してください。</td>
        <td></td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Planned Start]</strong></td>
        <td>タスクとイシューは、[!UICONTROL Planned Start dates]の順に並べ替えられます。タスクの[!UICONTROL Planned Start Dates]の詳細については、<a href="../../../manage-work/tasks/task-information/task-planned-start-date.md">タスクの[!UICONTROL Planned Start Date]の概要</a>を参照してください。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Commit Date]</strong></td>
        <td>タスクとイシューは、[!UICONTROL Commit dates]の順に並べ替えられます。[!UICONTROL Commit dates]について詳しくは、<a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md">[!UICONTROL Commit Date]の概要</a>を参照してください。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Project]</strong></td>
        <td>作業項目はプロジェクト別に並べ替えられます。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL My Priority]</strong></td>
        <td>項目は、選択した順序で表示されます。詳しくは、<a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md">[!UICONTROL Home]エリアの作業の優先順位付け</a>を参照してください。</td>
    </tr>
   </table>

## 別の週への移動

1. [[!UICONTROL ホームカレンダーの表示]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)の説明に従って、[!UICONTROL ホームカレンダー]ビューに移動します。
1. **[!UICONTROL カレンダーツールバー]**&#x200B;で、カレンダービューを 1 週間前に戻すには日付インジケーターの左向き矢印をクリックし、1 週間前に進むには右向き矢印をクリックします。

   ![](assets/week-arrows-350x206.png)

   「**[!UICONTROL 今日]**」をクリックすると、現在の週に戻ります。

## 表示するカレンダーを指定

[!UICONTROL ホームカレンダー]に表示する統合カレンダー（PTO、誕生日、休日カレンダーなど）を指定できます。手順については、[[!UICONTROL ホームカレンダー]の表示設定の指定](../../../workfront-basics/using-home/using-the-home-area/configure-home-calendar-view.md)を参照してください。
