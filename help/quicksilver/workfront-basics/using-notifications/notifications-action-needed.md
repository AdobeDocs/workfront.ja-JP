---
content-type: reference
navigation-topic: notifications
title: 「通知：アクションが必要」
description: 作業アイテムに対してアクションを実行する必要がある場合は、次の通知が表示されます。受信する通知の設定について詳しくは、「独自の電子メール通知を変更する」を参照してください。
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2442'
ht-degree: 98%

---

# 通知：[!UICONTROL アクションが必要]

作業アイテムに対してアクションを実行する必要がある場合は、次の通知が表示されます。受信する通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>私が新規作業リクエストを受けました</strong> </p> <p>作業アイテムの担当者は、リクエストを行うユーザーも担当者でない限り、メール通知を受け取ります。 </p> <p>タスクのステータスが[!UICONTROL Complete]か、イシューのステータスが[!UICONTROL Closed]の場合は通知は送信されません。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL New Work Request]: &lt;Request Name&gt;</em></p> <p>日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>タスク名</p> <p>[!UICONTROL Planned Completion Date]</p> <p>親</p> <p>割り当て元</p> <p>割り当て先</p> <p>[!UICONTROL Status]</p> <p>[!UICONTROL Description]</p> <p>[!UICONTROL View]ボタン<br>日刊ダイジェストに追加するオプション</p> <br> </td> 
   <td><strong>即時</strong>および<strong>日次</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がドキュメントを承認する必要があります</strong> </p> <p>ドキュメントの承認者は、承認者としてリストされると通知を受け取ります。</p> <p>インスタント通知メールの件名：<em>&lt;Name of the user who submitted the approval&gt; approval=""&gt; [!UICONTROL asked you to approve a document in [!DNL Adobe Workfront].]</em></p> <p>日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>承認を送信したユーザーの名前<br>ドキュメント名<br>ドキュメント参照番号<br>リクエストされた承認の日時<br>ドキュメントの詳細（形式、サイズ、バージョン番号）「<br><strong>[!UICONTROL Make Approval Decision]</strong>」ボタン<br>*保留中のドキュメント承認の合計数<br>*「<strong>[!UICONTROL Document Approvals</strong>*<strong>See All Approvals]</strong>」ボタン<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>即時および日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がプロジェクトを承認する必要があります</strong> </p> <p>担当業務の承認の場合、このイベントのメール通知を受け取るユーザーは、「[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]」が有効に設定されているかどうかによって異なります（<a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">グローバル承認設定を指定</a>を参照してください）。 </p> <p><strong>このオプションが有効な場合</strong>、承認に関連付けられた担当業務を持つ、システム内のすべてのユーザーにメール通知が送信されます。 </p> <p><strong>このオプションが無効な場合</strong>、承認プロセスに関連付けられた担当業務を持つプロジェクトチームメンバーのみがメール通知を受け取ります。</p> <p>承認がユーザーに関連付けられている場合、そのユーザーに通知が届きます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Project Pending Approval]: &lt;Project Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>承認を送信したユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>プロジェクトの優先度<br>承認ステップの承認待ち<br>承認待ちの決定の数<br>承認者の名前（ユーザーのみ）<br>[!UICONTROL Project Planned Completion Date]「<br><strong>[!UICONTROL Make Approval Decision]</strong>」ボタン<br>*保留中のプロジェクト承認の合計数<br>*「<strong>[!UICONTROL Project Approvals]</strong><br>*<strong>[!UICONTROL See All Approvals]</strong>」ボタンへのリンク<br>*日刊ダイジェストの日付</p> </td> 
   <td><strong>即時および日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がタスクを承認する必要があります</strong> </p> <p>担当業務の承認の場合、このイベントのメール通知を受け取るユーザーは、「[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]」が有効に設定されているかどうかによって異なります（<a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">グローバル承認設定を指定</a>を参照してください）。 </p> <p><strong>このオプションが有効な場合</strong>、承認に関連付けられた担当業務を持つ、システム内のすべてのユーザーにメール通知が送信されます。 </p> <p><strong>このオプションが無効な場合</strong>、承認プロセスに関連付けられた担当業務を持つプロジェクトチームメンバーのみがメール通知を受け取ります。</p> <p>承認がユーザーに関連付けられている場合、そのユーザーに通知が届きます。 </p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Task Pending Approval]: &lt;Task Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>タスク名<br>プロジェクト名<br>承認を送信したユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>タスクの優先度<br>承認ステージ名<br>承認者名<br>[!UICONTROL Task Planned Completion Date]「<br><strong>[!UICONTROL Make Approval Decision]</strong>」ボタン<br>*保留中のタスク承認の合計数<br>*「<strong>[!UICONTROL Task Approvals *See All Approvals]</strong>」ボタンへのリンク<strong></strong>*日刊ダイジェストの日付<br></p> </td> 
   <td><strong>今すぐおよび日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がタイムシートを承認する必要がある</strong> </p> <p>タイムシート承認者は、承認が必要なタイムシートが送信されたときにメール通知を受け取ります。ただし、タイムシート承認者がタイムシートを送信した場合、その承認者に通知は届きません。</p> <p>通知が送信されるのは、タイムシートのステータスが [!UICONTROL Submitted] の場合のみです。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Timesheet Submitted]：&lt;タイムシート所有者&gt;、&lt;タイムシートの開始日&gt; - &lt;タイムシートの終了日&gt;</em></p> <p> 日次ダイジェスト通知の件名：<em>[!UICONTROL Digest of Action Needed] &lt;日次ダイジェストの日付&gt;</em></p> </td> 
   <td> 承認を受けるためにタイムシートを送信したユーザーの名前<br>タイムシートの送信日時<br>タイムシートのステータス<br>タイムシートの開始日と終了日<br>タイムシートに記録された時間数<br>タイムシートに記録された超過時間数「<br><strong>[!UICONTROL Review]</strong>」および「<strong>[!UICONTROL Approve]</strong>」ボタン<br>*保留中のタイムシート承認の合計数<br>*<strong>[!UICONTROL Timesheet Approvals]</strong><br> へのリンク「<strong>[!UICONTROL *See All Approvals]</strong>」ボタン<br>*日次ダイジェストの日付 </td> 
   <td><strong>今すぐ</strong>および<strong>日次</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がイシューを承認する必要がある</strong> </p> <p>担当業務の承認の場合、このイベントのメール通知を受け取るユーザーは 「[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]」が有効になっているかどうかによって異なります（<a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL Configure global approval]</a> の設定を参照してください）。 </p> <p><strong>このオプションが有効な場合</strong>、承認に関連付けられた業務を担当するシステム内のすべてのユーザーにメール通知が送信されます。 </p> <p><strong>このオプションが無効な場合</strong>、承認プロセスに関連付けられた担当業務を持つプロジェクトチームメンバーのみがメール通知を受け取ります。</p> <p>承認がユーザーに関連付けられている場合、そのユーザーに通知が届きます。 </p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Issue Pending Approval]：&lt;イシューの名前&gt;</em></p> <p> 日次ダイジェスト通知の件名：<em> [!UICONTROL Digest of Action Needed] &lt;日次ダイジェストの日付&gt;</em></p> </td> 
   <td> イシュー名<br>プロジェクト名<br>イシューの参照番号<br>承認を受けるためにイシューを送信したユーザーの名前<br>承認待ちステータス<br>承認がリクエストされた日時<br>イシューの優先度<br>承認ステージ<br>承認者の名前<br>[!UICONTROL Issue Planned Completion Date]<br>[!UICONTROL Primary Contact]「<br><strong>[!UICONTROL Make Approval Decision]</strong>」ボタン<br>*保留中のイシュー承認数の合計<br>*<strong>[!UICONTROL Issue Approvals]</strong><br>へのリンク「<strong>[!UICONTROL *See All Approvals]</strong>」ボタン<br>*日次ダイジェストの日付 </td> 
   <td><strong>今すぐ</strong>および<strong>日次</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分に委任されたプロジェクトの承認について確認する必要がある</strong> </p> <p>プロジェクトの承認が委任されており、それについて確認する必要があります。</p> <p>即時通知メールの件名は次のとおりです。<em>[!UICONTROL Delegated Project Approval - Please Review] &lt;Project Name&gt;</em></p> <p><em>日次ダイジェスト通知の件名は次のとおりです。[!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em> </p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>承認をリクエストしたユーザーの名前<br>プロジェクトを承認するユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>プロジェクトの優先度<br>承認ステップ<br>承認者の名前<br>[!UICONTROL Project Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> ボタン<br>*保留中のプロジェクト承認の合計数<br>*リンク先 <strong>[!UICONTROL Project Approvals *See All Approvals]</strong> ボタン <br>*日次ダイジェストの日付 </td> 
   <td><strong>即時および日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分に委任されたタスクの承認について確認する必要がある</strong> </p> <p>タスクの承認が委任されたので、確認する必要があります。</p> <p>即時通知メールの件名は次のとおりです。<em>[!UICONTROL Delegated Task Approval - Please Review ]&lt;Task Name&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>承認をリクエストしたユーザーの名前<br>タスクを承認するユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>タスクの優先度<br>承認ステージ<br>承認者の名前<br>[!UICONTROL Task Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> ボタン <br>*保留中のタスク承認の合計数<br>*リンク先 <strong>[!UICONTROL Task Approvals *See All Approvals]</strong> ボタン<br>*日次ダイジェストの日付 </td> 
   <td><strong>即時および日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分に委任されたイシューの承認について確認する必要がある</strong> </p> <p>イシューの承認が委任されたので、確認する必要があります。</p> <p>即時通知メールの件名は次のとおりです。<em>[!UICONTROL Delegated Issue Approval - Please Review] &lt;Issue Name&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> イシュー名<br>プロジェクト名<br>イシューの参照番号<br>承認をリクエストしたユーザーの名前<br>イシューを承認するユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>イシューの優先度<br>承認ステージ<br>承認者の名前<br>イシュー予定完了日<br>プライマリ連絡先<br><strong>[!UICONTROL Make Approval Decision]</strong> ボタン<br>*保留中のイシューの承認数の合計<br>*リンク先 <strong>[!UICONTROL Issue Approval]</strong><br><strong>[!UICONTROL *See All Approvals]</strong> ボタン<br>*日次ダイジェストの日付<br></td> 
   <td><strong>即時および日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分にイシューが割り当てられている</strong> </p> <p>イシューの担当者がメール通知を受け取ります。イシューのステータスが [!UICONTROL Closed] の場合、またはそれと等しい場合、イシューの担当者はメールを受け取りません。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知メールの件名は次のとおりです。<em>[!UICONTROL New Work Request]: &lt;Issue Name&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>イシュー名<br>プロジェクト名<br>[!UICONTROL Issue Reference Number]<br>名前<br>イシューの期限（[!UICONTROL Planned Completion Date]）<br>イシューを割り当てたユーザーの名前<br><strong>[!UICONTROL Work On It]</strong> ボタン<br>*割り当ての合計数<br>*割り当てられたタスクとイシューの合計数<br>*リンク先 <strong>[!UICONTROL Work Requests]</strong><br>*日次ダイジェストの日付<br></p> </td> 
   <td><strong>即時および日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がタスクのプライマリ担当者に設定されている</strong> </p> <p>タスク担当者は、タスクのプライマリ担当者にされた場合、担当者が割り当てを行ったユーザーである場合を除き、メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] で、タスクが [!UICONTROL Complete] とマークされていない場合は、通知が送信されます。</p> <p>[!UICONTROL Review] または [!UICONTROL Requestor] のライセンスを持つユーザーには通知は届きません。</p> <p>即時通知メールの件名は次のとおりです。<em>[!UICONTROL New Work Request]: &lt;Task Name&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>名前<br>タスクの期限（[!UICONTROL Planned Completion Date]）<br>タスクを割り当てたユーザーの名前<br><strong>[!UICONTROL Work On It]</strong> ボタン<br>*割り当てられたタスクとイシューの合計数<br>*リンク先 <strong>[!UICONTROL Work Requests]</strong>*日次ダイジェストの日付 </td> 
   <td><strong>即時および日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私のチームが新規作業リクエストを受けました</strong> </p> <p>チームメンバーは、チームが新しい作業リクエストを受け取ると、メール通知を受け取ります。（リクエストを送信したユーザーは、チームのメンバーである場合は通知を受け取りません）。</p> <p>プロジェクトのステータスが [!UICONTROL Current] で、作業リクエストのステータスが [!UICONTROL New] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>即時通知メールの件名は次のとおりです。<em>[!UICONTROL New Work Request]: &lt;Request Name&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em>[!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p> イシュー名<br>プロジェクト名（リクエストキュー名）<br>イシューの参照番号<br>チーム名<br>イシュー期限（予定完了日）<br>リクエストを送信したユーザーの名前<br><strong>[!UICONTROL Work On It]</strong> ボタン<br>*チームに割り当てられたリクエストの合計数</p> <p>*作業リクエスト名</p> <p>[!UICONTROL *Planned Completion Date]</p> <p>*リクエストを送信したユーザーの名前<br>*リンク先 <strong>[!UICONTROL Team Requests]</strong><br>*日次ダイジェストの日付 </p> <p><span class="preview">*チームの割り当て</span> </p> </td> 
   <td><strong>即時および日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私のタイムシートが再開されました</strong> </p> <p>タイムシートの所有者は、タイムシートを再開したユーザーがタイムシートの所有者である場合を除き、タイムシートが再開されるとメール通知を受け取ります。</p> <p>メール通知は、タイムシートのステータスが [!UICONTROL Open] の場合にのみ送信されます。</p> <p>即時通知メールの件名は次のとおりです。<em>[!UICONTROL Timesheet Re-opened]: &lt;Timesheet Start Date&gt; - &lt;Timesheet End Date&gt;</em></p> <p>メモ：この通知を日刊ダイジェストメールに設定することはできません。</p> </td> 
   <td> タイムシートを再開したユーザーの名前<br>タイムシートが再開された日時<br>タイムシートのステータス（[!UICONTROL Re-opened]）<br>タイムシートに記録された合計時間数<br>タイムシートに記録された超過時間数<br><strong>[!UICONTROL Review]</strong> ボタン </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私のタイムシートが拒否されました</strong> </p> <p>タイムシートの所有者は、タイムシートを却下したユーザーが所有者である場合を除き、タイムシートが却下されるとメール通知を受け取ります。</p> <p>メール通知は、タイムシートのステータスが [!UICONTROL Rejected] の場合にのみ送信されます。</p> <p>即時通知メールの件名は次のとおりです。<em>[!UICONTROL Timesheet Rejected]:&lt;Start Date of the Timesheet&gt; - &lt;End Date of the Timesheet&gt;</em></p> <p>メモ：この通知を日刊ダイジェストメールに設定することはできません。</p> </td> 
   <td> タイムシートを却下したユーザーの名前<br>タイムシートのステータス（[!UICONTROL Rejected]）<br>タイムシートが却下された日時<br><strong>[!UICONTROL Review]</strong> ボタン </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが私からのアクセスをリクエストしています</strong> </p> <p>何かしてほしいというのでオンにしてください。</p> <p>プロジェクトを作成したユーザーがそのプロジェクトにアクセスできます。</p> <p>これにより、ユーザーがアクセスを要求したときに通知が受け取られます。</p> <p>即時通知メールの件名は次のとおりです。<em>&lt;Name of user who requested the access&gt; [!UICONTROL needs access to] &lt;Object Name&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Action Needed] &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> <p>オブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>アクセスをリクエストしたユーザーの名前<br>ユーザーがリクエストしているアクセスのタイプ<br><strong>[!UICONTROL Grant] &lt;Name of the access requested&gt; アクセス</strong>および <strong>[!UICONTROL Grant different access]</strong> ボタン<br>*保留中のアクセス要求の承認の合計数<br>*リンク先 <strong>[!UICONTROL Access Request]</strong> 承認<br>*日次ダイジェストの日付</p> </td> 
   <td><strong>即時および日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが私にドキュメントのアップロードをリクエストしています</strong> </p> <p>ドキュメントのアップロード要求をユーザーが受け取ると、ドキュメント要求にメール通知が送信されます。</p> <p>即時通知メールの件名は次のとおりです。<em>&lt;Name of the user requesting the document&gt; [!UICONTROL needs a document from you in [!DNL Workfront].]</em></p> <p> <p>メモ：この通知を日刊ダイジェストメールに設定することはできません。</p> </p> </td> 
   <td> ドキュメントを要求するユーザーの名前<br>ドキュメントをアップロードする必要があるオブジェクトの名前<br><strong>[!UICONTROL Attach it here]</strong> リンク </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
 </tbody> 
</table>
