---
content-type: reference
navigation-topic: notifications
title: '通知：私に割り当てられた仕事に関する情報'
description: 次の通知は、割り当てられた作業項目でのアクティビティの発生に関して警告します。
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 901605917347297a1ee077f00905b03427582650
workflow-type: tm+mt
source-wordcount: '2090'
ht-degree: 6%

---

# 通知：自分に割り当てられた仕事に関する情報

次の通知は、割り当てられた作業項目でのアクティビティの発生に関して警告します。

受信する通知の設定については、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

関連トピック [イベント通知](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>含まれるフィールド </p> <p> *日別のダイジェストフィールドのみ</p> </th> 
   <th>デフォルトのステータス</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>自分のチームに割り当てられたタスクの先行タスクがア完了しました</strong> </p> <p>割り当てられたチームは、タスクの 1 つの先行チームが完了すると、電子メール通知を受け取ります。 </p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>完了： &lt;task name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>先行タスク名<br>先行タスクプロジェクト<br>先行タスク参照番号<br>先行タスクを完了したユーザーの名前<br>先行タスクのステータス<br>先行者が完了した日時<br>先行タスクの前のステータス<br><strong>詳細を表示</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了した先行タスクの総数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*1 日のダイジェストの日付 </p> </td> 
   <td><strong>日次</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>担当タスクの先行タスクが完了した</strong> </p> <p>タスクの先行タスクの 1 つが完了すると、タスクの担当者は電子メール通知を受け取ります。 </p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>先行タスク名<br>先行タスクプロジェクト<br>先行タスク参照番号<br>先行タスクを完了したユーザーの名前<br>先行タスクのステータス<br>先行者が完了した日時<br>先行タスクの前のステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了した先行タスクの総数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*1 日のダイジェストの日付 </p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>自分が完了するタスクが承認または拒否された</strong> </p> <p>タスクが承認または却下されると、タスクの担当者は電子メール通知を受け取ります。</p> <p>通知は、プロジェクトのステータスが「現在」の場合にのみ送信されます。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt; オン &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>承認を許可したユーザーの名前<br>新規タスクステータス<br>タスクが承認または却下された日時<br>前のタスクステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*承認または却下されたタスクの合計数<br>*タスク名<br>*タスクを承認または却下したユーザーの名前<br>*承認の決定（[!UICONTROL 承認済み ]/[!UICONTROL 却下 ]）<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>自分に割り当てられているタスクが完了した</strong> </p> <p>タスクの担当者は、タスクが完了したときに電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt; オン &lt;project name=""&gt;</em></p> <p> <p>注意：タスクが [!UICONTROL 完了 ] と同じステータスに変更されても、電子メールの件名には「完了」と表示されます。</p> </p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前<br>タスクが完了した日時<br>前のタスクステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日別ダイジェストの日付<br></p> </td> 
   <td><strong>日次</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>自分のチームに割り当てられたタスクの先行タスクがすべて完了しました</strong> </p> <p>割り当てられたチームは、タスクの 1 つの先行チームが完了とマークされると、電子メール通知を受け取ります。</p> <p>レビューまたは要求者のライセンスを持つユーザーには通知は送信されません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>タスク完了： &lt;name&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> 割り当てられた作業のダイジェスト &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> タスク名<br>タスクプロジェクト<br>タスク参照番号<br>先行タスクを完了したユーザーの名前<br>先行タスクのステータス<br>先行者が完了した日時<br>先行タスクの前のステータス<br><strong>詳細を表示</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*1 日のダイジェストの日付 </td>
   <td><strong>今すぐ</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>すべての先行タスクが完了したら、すべての依存タスクの割り当て済みプライマリ ユーザーに E メール通知します。</strong> </p> <p>タスクの担当者は、完了した各先行タスクに関する電子メール通知を受け取ります。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt;</em><br></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> タスク名<br>タスクプロジェクト<br>タスク参照番号<br>先行タスクを完了したユーザーの名前<br>先行タスクのステータス<br>先行者が完了した日時<br>先行タスクの前のステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>自分が解決する問題が承認または拒否された</strong> </p> <p>イシューの担当者は、承認の決定（承認または却下）がおこなわれると、E メール通知を受け取ります。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>承認待ちの問題： &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; in &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> 割り当てられた作業のダイジェスト &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名<br>プロジェクト名<br>問題の参照番号<br>問題を承認または却下したユーザーの名前<br>承認の決定（承認または却下）<br>問題ステータス<br>承認をリクエストしたユーザーの名前<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*承認または却下された問題の合計数<br>*問題名<br>*問題を承認または却下したユーザーの名前<br>*承認の決定（承認または却下）<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>自分が割り当てられている問題が完了した</strong> </p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>完了： &lt;issue name=""&gt; オン &lt;project name=""&gt;</em></p> <p><em> 日次ダイジェスト通知の件名は次のとおりです。割り当てられた作業のダイジェスト &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> 問題名<br>プロジェクト名<br>問題の参照番号<br>問題を完了したユーザーの名前<br>新しい問題ステータス<br>問題が完了した日時<br>前のタスクステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了した問題の総数<br>*問題名<br>*問題を完了したユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が割り当てられた要求に関するドキュメントが追加あるいは更新された</strong> </p> <p>ドキュメントがアップロードされたとき、または追加された問題に関するドキュメントの詳細が変更されたときに、問題の担当者に電子メール通知が届きます。</p> <p>問題をトリガーしたユーザーが問題の担当者である場合、電子メール通知は送信されません。</p> <p>通知は、プロジェクトのステータスが [!UICONTROL Current] で、プロジェクトがヘルプリクエストキューとして設定されている場合 ( <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>) をクリックします。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL ドキュメントが ] に追加されました &lt;request name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>リクエスト名<br>プロジェクト名（リクエストキュー名）<br>ドキュメント参照番号 <br>ドキュメントをアップロードしたユーザーの名前<br>ドキュメント名 <br>追加日<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br>ドキュメントのサムネール<br><strong>[!UICONTROL プレビュー ]</strong> および <strong>[!UICONTROL ダウンロード ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*アップロードまたは変更されたドキュメントの合計数<br>*ドキュメント名<br>*オブジェクト名<br>*ドキュメントをアップロードしたユーザーの名前<br>*1 日のダイジェストの日付</p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分に割り当てられているタスクの完了予定日が変更になった</strong> </p> <p>タスクの [!UICONTROL 計画完了日 ] が変更されると、タスク担当者は電子メール通知を受け取ります。ただし、計画完了日を変更したユーザーがタスクの担当者でもある場合を除きます。</p> <p>プロジェクトのステータスが [!UICONTROL Planning] 以外の場合にのみ通知が送信されます。</p> <p>個人のタスクに関する通知は送信されません。</p> <p> レビューまたは要求者のライセンスを持つユーザーには通知は送信されません。 </p> <p> 即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 期限が変更されました。]</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>新しい期限（[!UICONTROL 予定完了日 ]）<br>期限が変更された日時<br>期限を変更したユーザーの名前<br>*プロジェクト名<br>*プロジェクト参照番号<br>*期限（計画完了日）が変更されたタスクの合計数<br>*タスク名<br>*新しい計画完了日<br>*期限を変更したユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が割り当てられている問題の期日が変更した</strong> </p> <p>[!UICONTROL 計画完了日 ] を変更したユーザーも担当者でない限り、この問題の担当者は、[!UICONTROL 計画完了日 ] が変更されると電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Planning] 以外の場合にのみ通知が送信されます。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 期限が変更されました ]</em></p> <p> </p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>問題名<br>プロジェクト名<br>問題の参照番号<br>新しい期限（[!UICONTROL 予定完了日 ]）<br>期限が変更された日時<br>期限を変更したユーザーの名前<br>*プロジェクト名<br>*プロジェクト参照番号<br>*期限（[!UICONTROL 予定完了日 ]）が変更された問題の合計数<br>*問題名<br>*新しい [!UICONTROL 予定完了日 ]<br>*期限を変更したユーザーの名前<br>*日別ダイジェストの日付<br></p> </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>自分に割り当てられたタスクの状態が変更した</strong> <p>タスクのステータスが変更された場合、ステータスを変更したユーザーも担当者でない限り、タスク担当者は電子メール通知を受け取ります。</p> <p>注意：タスクのステータスが完了に変わった場合、この通知は送信されません。 完了したタスクに対しては、別の通知が使用されます。 詳しくは、 <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">割り当てられているタスクが完了しました</a>、上記の。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;task name=""&gt; から &lt;project name=""&gt; が &lt;new status=""&gt;</em></p> <p> </p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>ステータスを変更したユーザーの名前<br>新しいステータス<br>ステータスが変更された日時<br>プレビューステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*ステータスが変更されたタスクの合計数<br>*タスク名<br>*前のタスクステータス<br>*新規タスクのステータス<br>*ステータスを変更したユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分の作業アイテムの 1 つで状態の変更</strong> </p> <p>自分でステータスを変更しない限り、自分が割り当てられているイシューのステータスが変更されると、電子メール通知が送信されます。 </p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;issue name=""&gt; から &lt;project name=""&gt; が &lt;new status=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 割り当てられた作業のダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名<br>プロジェクト名<br>問題の参照番号<br>ステータスを変更したユーザーの名前<br>新しいステータス<br>ステータスが変更された日時<br>以前の問題のステータス<br><strong>詳細を表示</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*ステータスが変更された問題の合計数<br>*タスク名<br>*以前の問題のステータス<br>*新しい問題のステータス<br>*ステータスを変更したユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
 </tbody> 
</table>
