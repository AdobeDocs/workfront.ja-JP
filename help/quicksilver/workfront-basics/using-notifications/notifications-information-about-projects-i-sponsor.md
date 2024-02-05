---
content-type: reference
navigation-topic: notifications
title: 「通知：スポンサーしているプロジェクトに関する情報」
description: 次の通知は、自分がスポンサーしているプロジェクトで発生するアクティビティについて警告します。
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 98%

---

# 通知：スポンサーしているプロジェクトに関する情報

次の通知は、自分がスポンサーしているプロジェクトで発生するアクティビティについて警告します。

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
   <td> <p><strong>自分がスポンサーしているプロジェクトにドキュメントが追加されました</strong> </p> <p>プロジェクトスポンサーは、ドキュメントがプロジェクトに追加されるとメール通知を受け取ります。</p> <p>プロジェクトのステータスが[!UICONTROL Current]で、ドキュメントが[!UICONTROL Private]でない場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Document added to] &lt;Project Name&gt;</em></p> <p>日次ダイジェスト通知の件名：<em>[!UICONTROL Digest of Projects You Sponsor] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>ドキュメントの参照番号<br>ドキュメントを追加したユーザーの名前<br>ドキュメント名<br>追加した日付<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br>ドキュメントのサムネール<br><strong>[!UICONTROL Preview]</strong>および<strong>[!UICONTROL Download]</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*追加されたドキュメントの合計数<br>*ドキュメント名<br>*ドキュメントを追加したユーザーの名前<br>*日次ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がスポンサーしているプロジェクトのマイルストーンタスクが完了した</strong> </p> <p>プロジェクトスポンサーは、スポンサーしているプロジェクトでマイルストーンタスクが完了すると、メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]: &lt;Project Name&gt; の &lt;Task Name&gt;</em></p> <p>注意：タスクが [!UICONTROL Complete] と同等のステータスに変更された場合も、メールの件名には [!UICONTROL Complete] と表示されます。<br></p> <p>日次ダイジェスト通知の件名：<em>スポンサーするプロジェクトのダイジェスト &lt;Date of daily digest&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前<br>新規タスクステータス<br>タスクが完了した日時<br>前のタスクのステータス<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日次ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がスポンサーしているプロジェクトに遅延が発生した</strong> </p> <p>プロジェクトがスケジュールより遅れると、プロジェクトスポンサーにメール通知が届きます。進捗状況ステータスが「[!UICONTROL At Risk]」または「[!UICONTROL In Trouble]」の場合、プロジェクトはスケジュールより遅れています。</p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Project Progress Change]: &lt;Project Name&gt;</em></p> <p>日次ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>プロジェクトの進捗ステータス<br>プロジェクトの[!UICONTROL Planned Start Date]<br>プロジェクトの[!UICONTROL Planned Completion Date]<br>プロジェクトの[!UICONTROL Projected Start Date]<br>プロジェクトの[!UICONTROL Projected Completion Date]<br>プロジェクトの完了率<br>プロジェクトのステータス<br>プロジェクト所有者<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトの進捗ステータス<br>*日次ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がスポンサーしているプロジェクトのタスクが完了した</strong> </p> <p>プロジェクトスポンサーがメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]: &lt;Project Name&gt; の &lt;Task Name&gt;</em></p> <p> <p>注意：タスクが [!UICONTROL Complete] と同等のステータスに変更された場合も、メールの件名には [!UICONTROL Complete] と表示されます。</p> </p> <p>日次ダイジェスト通知の件名：<em>スポンサーするプロジェクトのダイジェスト &lt;Date of daily digest&gt; </em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスクの参照番号<br>タスクを完了したユーザーの名前<br>タスクのステータス<br>タスクのステータスが変更された日時<br>タスクの以前のステータス<br><strong>詳細を見る</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日次ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がスポンサーしているプロジェクトのタスクに遅延が発生した</strong> </p> <p>プロジェクトのタスクがスケジュールより遅れると、プロジェクトスポンサーにメール通知が届きます。進捗ステータスが [!UICONTROL At Risk]、[!UICONTROL Behind]、[!UICONTROL Late] の場合、タスクはスケジュールより遅れています。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Task Progress Change]: &lt;Task Name&gt;</em></p> <p>日次ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>新規タスク進捗ステータス<br>タスクの[!UICONTROL Planned Start Date]<br>タスクの[!UICONTROL Planned Completion Date]<br>タスクの[!UICONTROL Projected Start Date]<br>タスクの[!UICONTROL Projected Completion Date]<br>タスクの完了率<br>タスクステータス<br>割り当て先名<br>名前で入力<br>*プロジェクト名<br>*プロジェクト参照番号<br>*スケジュールより遅れているタスクの合計数<br>*タスク名<br>*タスクを入力したユーザーの名前<br>*日次ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がスポンサーするプロジェクトに問題が追加された</strong> </p> <p>プロジェクトスポンサーは、イシューがプロジェクトに追加されるとメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Issue added to] &lt;Project Name&gt;</em></p> <p>日次ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>イシューの参照番号<br>イシューを追加したユーザーの名前<br>イシュー名<br>イシュータイプ<br>入力した日付<br>イシューの優先度<br>割り当て先の名前 <br>イシューのステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*プロジェクトに追加されたイシューの合計数<br>*イシュー名<br>*イシューの割り当て先のユーザーの名前<br>*日次ダイジェストの日付<br><br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がスポンサーするプロジェクトの問題が完了した</strong> </p> <p>プロジェクトスポンサーがメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Complete]: &lt;Project Name&gt; の &lt;Issue Name&gt;</em></p> <p>日次ダイジェスト通知の件名：<em>スポンサーするプロジェクトのダイジェスト &lt;Date of daily digest&gt; </em></p> </td> 
   <td> イシュー名<br>プロジェクト名<br>イシューの参照番号<br>イシューを完了したユーザーの名前<br>イシューステータス<br>イシューが完了した日時<br>以前のイシューステータス<br><strong>詳細を表示</strong>ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したイシューの総数<br>*イシュー名<br>*イシューに割り当てられたユーザーの名前<br>*日次ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がスポンサーしているプロジェクトに未割り当ての問題が追加された</strong> </p> <p>プロジェクトスポンサーは、未割り当てのイシューがプロジェクトに追加されるとメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Who should be assigned to this new issue on] &lt;Project Name&gt;?</em></p> <p>日次ダイジェスト通知の件名：<em> [!UICONTROL Digest of Projects You Sponsor] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>イシューの参照番号<br>イシューを追加したユーザーの名前<br>イシュー名<br>イシューのタイプ<br>入力日<br>イシューの優先度<br>割り当て先名（空）<br>イシューステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加されたイシューの総数<br>*イシュー名<br>*イシューを追加したユーザーの名前<br>*日次ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がプロジェクトのスポンサーに設定された</strong> </p> <p>プロジェクトスポンサーがプロジェクトのスポンサーとして設定されると、メール通知が送信されます。<br></p> <p>インスタント通知メールの件名は次のとおりです。<em>[!UICONTROL Project Sponsor]: &lt;Project Name&gt;</em></p> <p>メール通知の本文には、次のテキストが含まれます。</p> <p><em>[!UICONTROL Hi] &lt;Your Name&gt;、</em> </p> <p><em>&lt;Name of the user who assigned you as the Project Sponsor&gt; [!UICONTROL made you the sponsor of] &lt;Project Name&gt;. [!UICONTROL As the Project Sponsor, you might receive additional email notifications about project activity or be involved in approving work related to the project. Enjoy.]</em> </p> <p>日次ダイジェスト通知の件名：<em>スポンサーするプロジェクトのダイジェスト &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>プロジェクト予定完了日<br>*プロジェクト名<br>*プロジェクト参照番号<br>*日刊ダイジェストの日付</p> </td> 
   <td><strong>インスタント</strong> </td> 
  </tr> 
 </tbody> 
</table>
