---
content-type: reference
navigation-topic: notifications
title: '通知：私がスポンサーしたプロジェクトに関する情報'
description: 次の通知は、スポンサーとしているプロジェクトでのアクティビティの発生に関して警告します。
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 6%

---

# 通知：私がスポンサーしたプロジェクトに関する情報

次の通知は、スポンサーとしているプロジェクトでのアクティビティの発生に関して警告します。

受信する通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>私がスポンサーになっているプロジェクトにドキュメントが追加されました</strong> </p> <p>プロジェクトスポンサーは、ドキュメントがプロジェクトに追加されると、電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] で、ドキュメントが [!UICONTROL Private] でない場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL ドキュメントが ] に追加されました &lt;project name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL スポンサーとなるプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>ドキュメント参照番号<br>ドキュメントを追加したユーザーの名前<br>ドキュメント名<br>追加日<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br>ドキュメントのサムネール<br><strong>[!UICONTROL プレビュー ]</strong> および <strong>[!UICONTROL ダウンロード ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加されたドキュメントの合計数<br>*ドキュメント名<br>*ドキュメントを追加したユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がスポンサーになっているプロジェクトのマイルストーンタスクが完了しました</strong> </p> <p>プロジェクトスポンサーは、プロジェクトのスポンサーでマイルストーンタスクが完了すると、電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt; オン &lt;project name=""&gt;</em></p> <p>注意：タスクがステータス（[!UICONTROL 完了 ]）に変更されても、電子メールの件名には「[!UICONTROL 完了 ]」と表示されます。<br></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> スポンサーのプロジェクトのダイジェスト &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前<br>新規タスクステータス<br>タスクが完了した日時<br>前のタスクのステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン <br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がスポンサーになっているプロジェクトに遅延が発生しました</strong> </p> <p>プロジェクトスポンサーは、プロジェクトがスケジュールに遅れたときに電子メール通知を受け取ります。 進捗状況ステータスが「[!UICONTROL At Risk]」または「[!UICONTROL In Troulb]」の場合、プロジェクトはスケジュールより遅れています。</p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL プロジェクトの進行状況の変更 ]: &lt;project name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。 <em>[!UICONTROL スポンサーとなるプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクトの進行状況ステータス<br>プロジェクト [!UICONTROL 予定開始日 ]<br>プロジェクト [!UICONTROL 予定完了日 ]<br>プロジェクト [!UICONTROL 予定開始日 ]<br>プロジェクト [!UICONTROL 予測完了日 ]<br>プロジェクトの完了率<br>プロジェクトのステータス<br>プロジェクト所有者<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトの進行状況のステータス<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がスポンサーになっているプロジェクトに関するタスクが完了しました</strong> </p> <p>プロジェクトスポンサーが電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt; オン &lt;project name=""&gt;</em></p> <p> <p>注意：タスクがステータス（[!UICONTROL 完了 ]）に変更されても、電子メールの件名には「[!UICONTROL 完了 ]」と表示されます。</p> </p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> スポンサーのプロジェクトのダイジェスト &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前<br>タスクステータス<br>タスクのステータスが変更された日時<br>前のタスクのステータス<br><strong>詳細を見る</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がスポンサーになっているプロジェクトのタスクに遅延が発生しました</strong> </p> <p>プロジェクトスポンサーは、プロジェクト上のタスクがスケジュールより遅れたときに電子メール通知を受け取ります。 進捗状況ステータスが「[!UICONTROL At Risk]」、「[!UICONTROL Behind]」、「[!UICONTROL Late]」の場合、タスクはスケジュールより遅れています。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL タスクの進捗状況の変更 ]: &lt;task name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL スポンサーとなるプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>新規タスク進捗状況ステータス<br>タスク [!UICONTROL 予定開始日 ]<br>タスク [!UICONTROL 予定完了日 ]<br>タスク [!UICONTROL 予定開始日 ]<br>タスク [!UICONTROL 予測完了日 ]<br>タスクの完了率<br>タスクステータス<br>割り当て先名<br>名前で入力<br>*プロジェクト名<br>*プロジェクト参照番号<br>*スケジュールより遅れているタスクの合計数<br>*タスク名<br>*タスクを入力したユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がスポンサーになっているプロジェクトに問題が追加されました</strong> </p> <p>プロジェクトスポンサーは、問題がプロジェクトに追加されると、電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 問題の追加先 ] &lt;project name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。 <em>[!UICONTROL スポンサーとなるプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>問題の参照番号<br>イシューを追加したユーザーの名前<br>問題名<br>問題のタイプ<br>入力日<br>問題の優先度<br>割り当て先名 <br>問題ステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトに追加された問題の合計数<br>*問題名<br>*問題に割り当てられたユーザーの名前<br>*日別ダイジェストの日付<br><br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がスポンサーになっているプロジェクトに関する問題が完了しました</strong> </p> <p>プロジェクトスポンサーが電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;issue name=""&gt; オン &lt;project name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> スポンサーのプロジェクトのダイジェスト &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 問題名<br>プロジェクト名<br>問題の参照番号<br>問題を完了したユーザーの名前<br>問題ステータス<br>問題が完了した日時<br>以前の問題のステータス<br><strong>詳細を見る</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了した問題の総数<br>*問題名<br>*問題に割り当てられたユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がスポンサーになっているプロジェクトに未割り当ての問題が追加されました</strong> </p> <p>未割り当ての問題がプロジェクトに追加されると、プロジェクトスポンサーに電子メール通知が送信されます。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL この新しいイシューに割り当てるユーザー ] &lt;project name=""&gt;?</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL スポンサーとなるプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>問題の参照番号<br>イシューを追加したユーザーの名前<br>問題名<br>問題のタイプ<br>入力日<br>問題の優先度<br>割り当て先名（空）<br>問題ステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加された問題の総数<br>*問題名<br>*イシューを追加したユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私はプロジェクトのスポンサーとして設定されました</strong> </p> <p>プロジェクトスポンサーがプロジェクトのスポンサーとして設定されると、電子メール通知が送信されます。<br></p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL プロジェクトスポンサー ]: &lt;project name=""&gt;</em></p> <p>電子メール通知の本文には、次のテキストが含まれます。</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [!UICONTROL があなたを [] のスポンサーにしました &lt;project name=""&gt;. [!UICONTROL プロジェクトスポンサーは、プロジェクト活動に関する追加の電子メール通知を受け取ったり、プロジェクトに関する作業の承認に関わる電子メールを受け取る場合があります。 お楽しみください。]</em> </p> <p>日次ダイジェスト通知の件名は次のとおりです。 <em>スポンサーのプロジェクトのダイジェスト &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクトの計画完了日<br>*プロジェクト名<br>*プロジェクト参照番号<br>*1 日のダイジェストの日付</p> </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
 </tbody> 
</table>
