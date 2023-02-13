---
content-type: reference
navigation-topic: notifications
title: '''通知：自分が所有するプロジェクトに関する情報'
description: 次の通知は、所有するプロジェクトでおこなわれるアクティビティに関して警告します。 受信する通知の設定については、「独自のイベント通知をアクティブ化または非アクティブ化する」を参照してください。
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 6%

---

# 通知：自分が所有するプロジェクトに関する情報

次の通知は、所有するプロジェクトでおこなわれるアクティビティに関して警告します。 受信する通知の設定については、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>自分が所有しているプロジェクトにドキュメントが追加された</strong> </p> <p>ドキュメントを追加したユーザーがプロジェクト所有者でもない限り、プロジェクト所有者は、ドキュメントがプロジェクトに追加されると電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] で、ドキュメントがプライベートでない場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL ドキュメントが ] に追加されました &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 所有するプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>ドキュメントを追加したユーザーの名前<br>ドキュメント名<br>追加日<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br><strong>[!UICONTROL プレビュー ]</strong> および <strong>[!UICONTROL ダウンロード ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加されたドキュメントの合計数<br>*ドキュメント名<br>*ドキュメントを追加したユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトのマイルストーン タスクが完了した</strong> </p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt; オン &lt;project name=""&gt;</em></p> <p>注意：タスクのステータスが [!UICONTROL 完了 ] に変わった場合でも、電子メールの件名には「[!UICONTROL 完了 ]」と表示されます。</p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 所有するプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前<br>新規タスクステータス<br>タスクが完了した日時<br>前のタスクステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトに遅延が発生した</strong> </p> <p>プロジェクト所有者は、プロジェクトがスケジュールより遅れたときに電子メール通知を受け取ります。 プロジェクトの進行状況ステータスが「[!UICONTROL At Risk]」、「[!UICONTROL Behind]」、「[!UICONTROL Late]」の場合、プロジェクトはスケジュールより遅れています。</p> <p>ベストプラクティスは、この通知をアクティブに保つことです。 </p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL プロジェクトの進行状況の変更 ]: &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 所有するプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクトの進行状況ステータス<br>プロジェクト [!UICONTROL 予定開始日 ]<br>プロジェクト [!UICONTROL 予定完了日 ]<br>プロジェクト [!UICONTROL 予定開始日 ]<br>プロジェクト [!UICONTROL 予測完了日 ]<br>プロジェクト完了率<br>プロジェクトステータス<br>プロジェクト所有者<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトの進行状況のステータス<br>*日別ダイジェストの日付<br></p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトに問題が追加された</strong> </p> <p>プロジェクト所有者は、問題がプロジェクトに追加されると、電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 問題の追加先 ] &lt;project name=""&gt;</em></p> <p> </p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 所有するプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>問題の参照番号<br>イシューを追加したユーザーの名前<br>問題名<br>問題のタイプ<br>入力日<br>問題の優先度<br>割り当て先名 <br>問題ステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトに追加された問題の合計数<br>*問題名<br>*イシューを追加したユーザーの名前<br>*1 日のダイジェストの日付</p> </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトのタスクが完了した</strong> </p> <p>プロジェクト所有者は、プロジェクトでタスクが完了したときに通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt; オン &lt;project name=""&gt;</em></p> <p> <p>注意：タスクのステータスが [!UICONTROL 完了 ] に変わった場合でも、電子メールの件名には「[!UICONTROL 完了 ]」と表示されます。</p> </p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 所有するプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前 <br>タスクステータス<br>タスクが完了した日時<br>前のタスクステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数 <br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトのタスクに遅延が発生した</strong> </p> <p>プロジェクトのタスクがスケジュールより遅れると、プロジェクト所有者に電子メール通知が届きます。 進捗状況ステータスが「[!UICONTROL At Risk]」、「[!UICONTROL Behind]」、「[!UICONTROL Late]」の場合、タスクはスケジュールより遅れています。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL タスクの進捗状況の変更 ]: &lt;task name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 所有するプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>新規タスク進捗状況ステータス<br>タスク [!UICONTROL 予定開始日 ]<br>タスク [!UICONTROL 予定完了日 ]<br>タスク [!UICONTROL 予定開始日 ]<br>タスク [!UICONTROL 予測完了日 ]<br>タスク完了率<br>タスクステータス<br>割り当て先名<br>名前で入力<br>*プロジェクト名<br>*プロジェクト参照番号<br>*スケジュールより後のタスクの合計数<br>*タスク名<br>*名前に割り当て済み<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有しているプロジェクトの問題が完了した</strong> </p> <p>プロジェクト所有者は、プロジェクトで問題が完了したときに電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。 </p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;issue name=""&gt; オン &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 所有するプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名<br>プロジェクト名<br>問題の参照番号<br>問題を完了したユーザーの名前<br>問題ステータス<br>問題が完了した日時<br>以前の問題のステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン <br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了した問題の総数<br>*問題名<br>*問題に割り当てられたユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトに未割り当ての問題が追加された</strong> </p> <p>未割り当ての問題がプロジェクトに追加されると、プロジェクト所有者に電子メール通知が送信されます。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL この新しいイシューに割り当てられる担当者 &lt;project name=""&gt;?</em></p> <p> </p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> 所有しているプロジェクトのダイジェスト &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>問題の参照番号<br>イシューを追加したユーザーの名前<br>問題名<br>問題のタイプ<br>入力日<br>問題の優先度<br>割り当て先名（空）<br>問題ステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加された問題の総数<br>*問題名<br>*イシューを追加したユーザーの名前<br>*日別ダイジェストの日付<br></p> </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>新規プロジェクトの所有者に設定された</strong> </p> <p>ユーザーがプロジェクトの所有者として割り当てられると、そのユーザーに電子メール通知が送信されます。</p> <p>プロジェクト所有者が割り当てを行ったユーザーと同じ場合、電子メール通知は送信されません。</p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>何かに割り当てられているので、これをオンにします。 </p> <p> 何かを割り当て、何かを共有し、何かのアクセスを得る。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 現在、[] のプロジェクト所有者です &lt;project name=""&gt;</em></p> <p>電子メール通知の本文には、次のテキストが含まれます。<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL により [] の所有者になりました &lt;project name=""&gt;. [!UICONTROL プロジェクト所有者は、プロジェクトの活動に関する追加の電子メール通知を受け取ったり、プロジェクトの時間を承認したり、プロジェクトに関連する作業の承認に関与したりすることができます。 全てあなたのものです。]</em> </p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 所有するプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクト完了日<br>*プロジェクト名<br>*プロジェクト参照番号<br>*1 日のダイジェストの日付</p> </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>担当プロジェクトのどれかでタスクのコミット日が変更された</strong> </p> <p>プロジェクト所有者は、コミット日を変更したユーザーがプロジェクト所有者でもない限り、プロジェクトのタスクのコミット日が変更されると、電子メール通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL コミット日：] &lt;task name=""&gt; [!UICONTROL は現在 ] &lt;new commit="" date=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> 所有しているプロジェクトのダイジェスト &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>タスク名<br>プロジェクト名<br>タスク参照番号<br>コミット日を変更したユーザーの名前<br>新しいコミット日<br>タスク [!UICONTROL 予定完了日 ]<br>この変更によるプロジェクトタイムラインの影響に関する情報<br>割り当て先名<br>名前で入力<br>プロジェクト所有者<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*コミット日が変更されたタスクの合計数<br>*タスク名<br>*日別ダイジェストの日付<br></p> </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>と [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>担当プロジェクトのいずれかで問題のコミット日が変更された</strong> </p> <p>プロジェクト所有者は、コミット日を変更したユーザーがプロジェクト所有者と同じユーザーでない限り、プロジェクトの問題に対するコミット日の変更時に電子メール通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL コミット日：] &lt;issue name=""&gt; [!UICONTROL は現在 ] &lt;new commit="" date=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 所有するプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>問題名<br>プロジェクト名<br>問題の参照番号<br>コミット日を変更したユーザーの名前<br>新しいコミット日<br>発行計画完了日<br>割り当て先名<br>名前で入力<br>プロジェクト所有者<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*コミット日が変更された問題の合計数<br>*問題名<br>*日別ダイジェストの日付<br></p> </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>と [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
