---
content-type: reference
navigation-topic: notifications
title: 「通知：自分に担当割り当てされている作業に関する情報」
description: 次の通知は、割り当てられた作業アイテムでのアクティビティの発生に関して警告します。
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 99%

---

# 通知：自分に担当割り当てされている作業に関する情報

次の通知は、割り当てられた作業アイテムでのアクティビティの発生に関して警告します。

受信する通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

[イベント通知](../../workfront-basics/using-notifications/event-notifications.md)も参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>含まれるフィールド </p> <p> *日次ダイジェストフィールドのみ</p> </th> 
   <th>デフォルトステータス</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>自分のチームに割り当てられたタスクの先行タスクが完了した</strong> </p> <p>割り当てられたチームは、いずれかのタスクの先行タスクが完了すると、メール通知を受け取ります。 </p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名：<em>完了：&lt;Task Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>先行タスク名<br>先行タスクプロジェクト<br>先行タスクの参照番号<br>先行タスクを完了したユーザーの名前<br>先行タスクのステータス<br>先行タスクが完了した日時<br>先行タスクの前のステータス<br><strong>「詳細を見る」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*完了した先行タスクの総数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日刊ダイジェストの日付 </p> </td> 
   <td><strong>日次</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>担当タスクの先行タスクが完了した</strong> </p> <p>タスクの担当者は、いずれかのタスクの先行タスクが完了すると、メール通知を受け取ります。 </p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]：&lt;Task Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>先行タスク名<br>先行タスクプロジェクト<br>先行タスクの参照番号<br>先行タスクを完了したユーザーの名前<br>先行タスクのステータス<br>先行タスクが完了した日時<br>先行タスクの前のステータス<br><strong>「[!UICONTROL See More Details]」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*完了した先行タスクの総数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日刊ダイジェストの日付 </p> </td> 
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
   <td> <p><strong>自分が完了するタスクが承認または拒否された</strong> </p> <p>タスクの担当者は、タスクが承認または却下されると、メール通知を受け取ります。</p> <p>プロジェクトのステータスが「進行中」の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]：&lt;Project Name&gt;の&lt;Task Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスクの参照番号<br>承認を許可したユーザーの名前<br>新規タスクステータス<br>タスクが承認または却下された日時<br>タスクの前のステータス<br><strong>「[!UICONTROL See More Details]」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*承認または却下されたタスクの合計数<br>*タスク名<br>*タスクを承認または却下したユーザーの名前<br>*承認決定（[!UICONTROL Approved]/ [!UICONTROL Rejected]）<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>自分に割り当てられているタスクが完了した</strong> </p> <p>タスクの担当者は、タスクが完了すると、メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]：&lt;Project name&gt;の&lt;Task Name&gt;</em></p> <p> <p>メモ：タスクが「[!UICONTROL Complete]」と同等のステータスに変更された場合も、メールの件名には引き続き「完了」と表示されます。</p> </p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>タスク名<br>プロジェクト名<br>タスクの参照番号<br>タスクを完了したユーザーの名前<br>タスクが完了した日時<br>タスクの前のステータス<br><strong>「[!UICONTROL See More Details]」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日刊ダイジェストの日付<br></p> </td> 
   <td><strong>日次</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>自分のチームに割り当てられたタスクの先行タスクがすべて完了した</strong> </p> <p>割り当てられたチームは、いずれかのタスクの先行タスクが完了とマークされると、メール通知を受け取ります。</p> <p>レビューまたは依頼者のライセンスを持つユーザーには、通知は送られません。</p> <p>インスタント通知メールの件名：<em>タスク完了：&lt;Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em>割り当てられた作業のダイジェスト &lt;Date of daily digest&gt; </em></p> </td> 
   <td> タスク名<br>タスクプロジェクト<br>タスクの参照番号<br>先行タスクを完了したユーザーの名前<br>先行タスクのステータス<br>先行タスクが完了した日時<br>先行タスクの前のステータス<br><strong>「詳細を見る」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日刊ダイジェストの日付 </td>
   <td><strong>即時</strong> </td> 
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
   <td> <p><strong>自分が担当するすべての先行タスクが完了した</strong> </p> <p>タスクの担当者は、それぞれの先行タスクが完了すると、メール通知を受け取ります。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]：&lt;Task Name&gt;</em><br></p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> タスク名<br>タスクプロジェクト<br>タスクの参照番号<br>先行タスクを完了したユーザーの名前<br>先行タスクのステータス<br>先行タスクが完了した日時<br>先行タスクの前のステータス<br><strong>「[!UICONTROL See More Details]」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日刊ダイジェストの日付 </td> 
   <td><strong>即時</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>自分が解決するイシューが承認または拒否された</strong> </p> <p>イシューの担当者は、承認決定（承認または却下）が下されると、メール通知を受け取ります。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名：<em>承認待ちのイシュー：&lt;Planned Start Date&gt; &lt;Issue Reference Number&gt; - &lt;Project Name&gt;の&lt;Issue Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em>割り当てられた作業のダイジェスト &lt;Date of daily digest&gt; </em></p> </td> 
   <td> イシュー名<br>プロジェクト名<br>イシューの参照番号<br>イシューを承認または却下したユーザーの名前<br>承認決定（承認または却下）<br>イシューステータス<br>承認をリクエストしたユーザーの名前<br><strong>「[!UICONTROL See More Details]」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*承認または却下されたイシューの合計数<br>*イシュー名<br>*イシューを承認または却下したユーザーの名前<br>*承認決定（承認または却下）<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>自分が割り当てられているイシューが完了した</strong> </p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名：<em>完了：&lt;Project Name&gt; の &lt;Issue Name&gt;</em></p> <p><em>日刊ダイジェスト通知の件名：割り当てられた作業のダイジェスト&lt;Date of daily digest&gt;</em> </p> </td> 
   <td> イシュー名<br>プロジェクト名<br>イシューの参照番号<br>イシューを完了したユーザーの名前<br>新しいイシューステータス<br>イシューが完了した日時<br>前のタスクのステータス <br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したイシューの総数<br>*イシュー名<br>*イシューを完了したユーザーの名前<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が割り当てられた要求に関するドキュメントが追加あるいは更新された</strong> </p> <p>ドキュメントがアップロードされた際、または自分が追加したイシューに関するドキュメントの詳細が変更された際、イシューの担当者にメール通知が届きます。</p> <p>イシューをトリガーしたユーザーがイシューの担当者である場合、メール通知は送信されません。</p> <p>通知は、プロジェクトのステータスが「[!UICONTROL Current]」、プロジェクトがヘルプリクエストキューとして設定されている場合（<a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>で説明されているとおり）にのみ送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Document added to] &lt;Request Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>リクエスト名<br>プロジェクト名（リクエストキュー名）<br>ドキュメント参照番号<br>ドキュメントをアップロードしたユーザーの名前<br>ドキュメント名<br>追加日<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br>ドキュメントのサムネール<br><strong>[!UICONTROL Preview]</strong> および <strong>[!UICONTROL Download]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*アップロードまたは変更されたドキュメントの合計数<br>*ドキュメント名<br>*オブジェクト名<br>*ドキュメントをアップロードしたユーザーの名前<br>*日刊ダイジェストの日付</p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分に割り当てられているタスクの完了予定日が変更になった</strong> </p> <p>タスクの [!UICONTROL Planned Completion Date] が変更されると、タスクの担当者はメール通知を受け取ります。ただし、予定完了日を変更したユーザーがタスクの担当者でもある場合を除きます。</p> <p>プロジェクト状態が [!UICONTROL Planning] 以外の場合にのみ通知が送信されます。</p> <p>個人のタスクに関する通知は送信されません。</p> <p> レビューまたは依頼者のライセンスを持つユーザーには、通知は送られません。 </p> <p> インスタント通知メールの件名：<em>[!UICONTROL Due Date has been changed.]</em></p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>新しい期日（[!UICONTROL Planned Completion Date]）<br>期日が変更された日時<br>期日を変更したユーザーの名前<br>*プロジェクト名<br>*プロジェクト参照番号<br>*期日（予定完了日）が変更されたタスクの合計数<br>*タスク名<br>*新しい予定完了日<br>*期日を変更したユーザーの名前<br>*日刊ダイジェストの日付 </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>および日次</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が割り当てられているイシューの期日が変更された</strong> </p> <p>[!UICONTROL Planned Completion Date] が変更されると、このイシューの担当者はメール通知を受け取ります。ただし、[!UICONTROL Planned Completion Date] を変更したユーザーが担当者でもある場合は除きます。</p> <p>プロジェクト状態が [!UICONTROL Planning] 以外の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Due Date has been changed]</em></p> <p> </p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>イシュー名<br>プロジェクト名<br>イシューの参照番号<br>新しい期日（[!UICONTROL Planned Completion Date]）<br>期日が変更された日時<br>期日を変更したユーザーの名前<br>*プロジェクト名<br>*プロジェクト参照番号<br>*期日（[!UICONTROL Planned Completion Date]）が変更されたイシューの合計数<br>*イシュー名<br>*新しい [!UICONTROL Planned Completion Date]<br>*期日を変更したユーザーの名前<br>*日刊ダイジェストの日付<br></p> </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>および日次</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>自分に割り当てられたタスクの状態が変更された</strong> <p>タスクのステータスが変更された場合、タスクの担当者はメール通知を受け取ります。ただし、ステータスを変更したユーザーが担当者でもある場合を除きます。</p> <p>メモ：タスクのステータスが完了に変わった場合、この通知は送信されません。完了したタスクには、別の通知が使用されます。上記の<a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">自分に割り当てられているタスクが完了した</a>を参照してください。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名は、「<em>&lt;Project Name&gt; の &lt;Task Name&gt; は &lt;New Status&gt;です</em>」になります。</p> <p> </p> <p> 日刊ダイジェスト通知の件名は、「<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt; </em>」になります。</p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>ステータスを変更したユーザーの名前<br>新しいステータス<br>ステータスが変更された日時<br>プレビューステータス<br><strong>「[!UICONTROL See More Details]」</strong>ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*ステータスが変更されたタスクの合計数<br>*タスク名<br>*以前のタスクのステータス<br>*新しいタスクのステータス<br>*ステータスを変更したユーザーの名前<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分の作業アイテムの 1 つで状態の変更</strong> </p> <p>自分でステータスを変更しない限り、自分が割り当てられているイシューのステータスが変更されると、メール通知が届きます。 </p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名は、「<em>&lt;Project Name&gt; の &lt;Issue Name&gt; は &lt;New Status&gt;です</em>」になります。</p> <p> 日刊ダイジェスト通知の件名は、「<em>[!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest&gt;</em>」になります。</p> </td> 
   <td> イシュー名<br>プロジェクト名<br>イシューの参照番号<br>ステータスを変更したユーザーの名前<br>新しいステータス<br>ステータスが変更された日時<br>以前のイシューのステータス<br><strong>「詳細を表示」</strong>ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*ステータスが変更されたイシューの合計数<br>*タスク名<br>*以前のイシューのステータス<br>*新しいイシューのステータス<br>*ステータスを変更したユーザーの名前<br>*日刊ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
 </tbody> 
</table>
