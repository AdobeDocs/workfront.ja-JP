---
content-type: reference
navigation-topic: notifications
title: 通知：所有するプロジェクトに関する情報
description: 次の通知は、所有するプロジェクトで行われるアクティビティに関して警告します。受信する通知の設定について詳しくは、「独自の電子メール通知を変更する」を参照してください。
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 98%

---

# 通知：所有するプロジェクトに関する情報

次の通知は、所有するプロジェクトで行われるアクティビティに関して警告します。受信する通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>自分が所有しているプロジェクトにドキュメントが追加された</strong> </p> <p>ドキュメントを追加したユーザーがプロジェクト所有者でない限り、プロジェクト所有者は、ドキュメントがプロジェクトに追加されるとメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] で、ドキュメントがプライベートでない場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Document added to] &lt;Project Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>ドキュメントを追加したユーザーの名前<br>ドキュメント名<br>追加日<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br><strong>[!UICONTROL Preview]</strong> および <strong>[!UICONTROL Download]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加されたドキュメントの総数<br>*ドキュメント名<br>*ドキュメントを追加したユーザーの名前<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトのマイルストーンタスクが完了した</strong> </p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]: &lt;Project Name&gt; の &lt;Task Name&gt;</em></p> <p>注意：タスクが [!UICONTROL Complete] と同等のステータスに変更された場合も、メールの件名には [!UICONTROL Complete] と表示されます。</p> <p> 日刊ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前<br>新規タスクステータス<br>タスクが完了した日時<br>前のタスクのステータス<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日刊ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトに遅延が発生する</strong> </p> <p>プロジェクト所有者は、プロジェクトがスケジュールより遅れたときにメール通知を受け取ります。プロジェクトの進捗ステータスが [!UICONTROL At Risk]、[!UICONTROL Behind]、[!UICONTROL Late] の場合、プロジェクトはスケジュールより遅れています。</p> <p>ベストプラクティスは、この通知をアクティブに保つことです。 </p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Project Progress Change]：&lt;Project Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>プロジェクトの進捗ステータス<br>プロジェクトの [!UICONTROL Planned Start Date]<br>プロジェクトの [!UICONTROL Planned Completion Date]<br>プロジェクトの [!UICONTROL Projected Start Date]<br>プロジェクトの [!UICONTROL Projected Completion Date]<br>プロジェクトの完了率<br>プロジェクトのステータス<br>プロジェクト所有者<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトの進捗ステータス<br>*日刊ダイジェストの日付<br></p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトにイシューが追加される</strong> </p> <p>プロジェクト所有者は、イシューがプロジェクトに追加されるとメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Issue added to] &lt;Project Name&gt;</em></p> <p> </p> <p> 日刊ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>イシューの参照番号<br>イシューを追加したユーザーの名前<br>イシュー名<br>イシューのタイプ<br>エントリ日<br>イシューの優先度<br>割り当て先名 <br>イシューステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトに追加されたイシューの合計数<br>*イシュー名<br>*イシューを追加したユーザーの名前<br>*日刊ダイジェストの日付</p> </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>および日次</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトのタスクが完了する</strong> </p> <p>プロジェクト所有者は、プロジェクトでタスクが完了すると通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]: &lt;Project Name&gt; の &lt;Task Name&gt;</em></p> <p> <p>注意：タスクが [!UICONTROL Complete] と同等のステータスに変更された場合も、メールの件名には [!UICONTROL Complete] と表示されます。</p> </p> <p> 日刊ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前 <br>タスクステータス<br>タスクが完了した日時<br>前のタスクのステータス<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトのタスクに遅延が発生する</strong> </p> <p>プロジェクトのタスクがスケジュールより遅れると、プロジェクト所有者にメール通知が届きます。進捗ステータスが [!UICONTROL At Risk]、[!UICONTROL Behind]、[!UICONTROL Late] の場合、タスクはスケジュールより遅れています。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Task Progress Change]：&lt;Task Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>新規タスク進捗ステータス<br>タスクの [!UICONTROL Planned Start Date]<br>タスクの [!UICONTROL Planned Completion Date]<br>タスクの [!UICONTROL Projected Start Date]<br>タスクの [!UICONTROL Projected Completion Date]<br>タスクの完了率<br>タスクステータス<br>割り当て先名<br>名前で入力<br>*プロジェクト名<br>*プロジェクト参照番号<br>*スケジュールより遅れているタスクの合計数<br>*タスク名<br>*割り当て先の名前<br>*日刊ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有しているプロジェクトのイシューが完了する</strong> </p> <p>プロジェクト所有者は、プロジェクトでイシューが完了したときにメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。 </p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]：&lt;Project Name&gt; の &lt;Issue Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> イシュー名<br>プロジェクト名<br>イシューの参照番号<br>イシューを完了したユーザーの名前<br>イシューステータス<br>イシューが完了した日時<br>以前のイシューステータス<br><strong>[!UICONTROL See More Details]</strong> ボタン <br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したイシューの総数<br>*イシュー名<br>*イシューに割り当てられたユーザーの名前<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するプロジェクトに未割り当てのイシューが追加される</strong> </p> <p>プロジェクト所有者は、未割り当てのイシューがプロジェクトに追加されるとメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Who should be assigned to this new issue on] &lt;Project Name&gt;?</em></p> <p> </p> <p> 日刊ダイジェスト通知の件名：<em>所有するプロジェクトのダイジェスト &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>イシューの参照番号<br>イシューを追加したユーザーの名前<br>イシュー名<br>イシューのタイプ<br>エントリ日<br>イシューの優先度<br>割り当て先名（空）<br>イシューステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加されたイシューの総数<br>*イシュー名<br>*イシューを追加したユーザーの名前<br>*日刊ダイジェストの日付<br></p> </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>および日次</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>新規プロジェクトの所有者に設定された</strong> </p> <p>ユーザーがプロジェクト所有者として割り当てられると、そのユーザーにメール通知が届きます。</p> <p>割り当てを行ったユーザーとプロジェクト所有者が同じ場合、メール通知は送信されません。</p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>ユーザーは何かに割り当てられているので、これをオンにします。 </p> <p> 何かを割り当て、何かを共有し、何かへのアクセス権を取得しています。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL You're now the project owner of] &lt;Project Name&gt;</em></p> <p>メール通知の本文には、次のテキストが含まれます。<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;Your Name&gt;,<br></em><em>&lt;Name of the user who assigned you as the Project Owner&gt; [!UICONTROL made you the owner of] &lt;Project Name&gt;. [!UICONTROL As the Project Owner] は、プロジェクトアクティビティに関するメール通知を受信したり、プロジェクト時間数の承認を要求されたり、プロジェクト関連作業の承認に関与することがあります。全て自分の担当となります。</em> </p> <p> 日刊ダイジェスト通知の件名は次のとおりです。<em>[!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> <p> </p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>プロジェクト完了日<br>*プロジェクト名<br>*プロジェクト参照番号<br>*日刊ダイジェストの日付</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>担当プロジェクトのどれかでタスクのコミット日が変更される</strong> </p> <p>プロジェクト所有者には、コミット日を変更するユーザーがプロジェクト所有者本人である場合を除き、プロジェクトのタスクのコミット日が変更されると、メール通知が届きます。</p> <p>インスタント通知メールの件名は次のとおりです。<em>[!UICONTROL Commit date for] &lt;Task Name&gt; [!UICONTROL is now] &lt;New Commit Date&gt;</em></p> <p> 日刊ダイジェスト通知の件名は次のとおりです。<em> 所有するプロジェクトのダイジェスト &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>タスク名<br>プロジェクト名<br>タスク参照番号<br>コミット日を変更したユーザーの名前<br>新しいコミット日<br>タスク [!UICONTROL Planned Completion Date]<br>この変更によるプロジェクトタイムラインの影響に関する情報<br>割り当て先名<br>名前で入力<br>プロジェクト所有者<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*コミット日が変更されたタスクの合計数<br>*タスク名<br>*日刊ダイジェストの日付<br></p> </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>と [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>担当プロジェクトのいずれかでイシューのコミット日が変更される</strong> </p> <p>プロジェクト所有者には、コミット日を変更するユーザーがプロジェクト所有者本人である場合を除き、プロジェクトのイシューのコミット日が変更されると、メール通知が届きます。</p> <p>インスタント通知メールの件名は次のとおりです。<em>[!UICONTROL Commit date for] &lt;Issue Name&gt; [!UICONTROL is now] &lt;New Commit Date&gt;</em></p> <p> 日刊ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Projects You Own] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>イシュー名<br>プロジェクト名<br>イシュー参照番号<br>コミット日を変更したユーザーの名前<br>新しいコミット日<br>イシュー予定完了日<br>割り当て先名<br>名前で入力<br>プロジェクト所有者<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*コミット日が変更されたイシューの合計数<br>*イシュー名<br>*日刊ダイジェストの日付<br></p> </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>と [!UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
