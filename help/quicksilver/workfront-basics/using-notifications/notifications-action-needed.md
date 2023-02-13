---
content-type: reference
navigation-topic: notifications
title: '通知：必要なアクション'
description: 作業項目に対してアクションを実行する必要がある場合は、次の通知が表示されます。 受信する通知の設定については、「独自のイベント通知をアクティブ化または非アクティブ化する」を参照してください。
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '2446'
ht-degree: 4%

---

# 通知： [!UICONTROL 必要なアクション]

作業項目に対してアクションを実行する必要がある場合は、次の通知が表示されます。 受信する通知の設定については、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>新規作業要求を受けた</strong> </p> <p>作業項目の担当者は、リクエストを行うユーザーも担当者でない限り、電子メール通知を受け取ります。 </p> <p>タスクのステータスが [!UICONTROL 完了 ] か、問題のステータスが [!UICONTROL クローズ済み ] の場合は通知は送信されません。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 新しい作業リクエスト ]: &lt;request name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。 <em>[!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>タスク名</p> <p>[!UICONTROL 計画完了日 ]</p> <p>親</p> <p>割り当て元</p> <p>割り当て先</p> <p>[!UICONTROL ステータス ]</p> <p>[!UICONTROL 説明 ]</p> <p>[!UICONTROL 表示 ] ボタン<br>日別ダイジェストに追加するオプション</p> <br> </td> 
   <td><strong>即時および</strong> <strong>毎日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がドキュメントを承認する必要がある</strong> </p> <p>ドキュメントの承認者は、承認者としてリストされると通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;name of="" the="" user="" who="" submitted="" the="" approval=""&gt; [!UICONTROL により、 [!DNL Adobe Workfront].]</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>承認を送信したユーザーの名前<br>ドキュメント名<br>ドキュメント参照番号<br>リクエストされた承認の日時<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br><strong>[!UICONTROL 承認を決定 ]</strong> ボタン<br>*保留中のドキュメント承認の合計数<br>*リンク先 <strong>[!UICONTROL ドキュメントの承認</strong>*<strong>すべての承認を見る ]</strong> ボタン<br>*日別ダイジェストの日付<br></td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がプロジェクトを承認する必要がある</strong> </p> <p>ジョブの役割の承認の場合、このイベントの電子メール通知を受け取るユーザーは、「[!UICONTROL 承認者がプロジェクトチームに属している必要がない（役割を含む承認プロセスの場合）]」設定が有効かどうかによって異なります ( <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">グローバル承認設定の指定</a>) をクリックします。 </p> <p><strong>このオプションが有効な場合</strong>承認済みの場合、ジョブの役割が関連付けられている、システム内のすべてのユーザーに電子メール通知が送信されます。 </p> <p><strong>このオプションが無効な場合</strong>承認プロセスに関連付けられたジョブロールを持つプロジェクトチームメンバーのみが電子メール通知を受け取ります。</p> <p>承認がユーザーに関連付けられている場合、そのユーザーに通知が届きます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL プロジェクト承認待ち ]: &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>承認を送信したユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>プロジェクトの優先度<br>承認ステップ承認待ち<br>承認待ちの決定数<br>承認者名（ユーザーのみ）<br>[!UICONTROL プロジェクト予定完了日 ] <br><strong>[!UICONTROL 承認を決定 ]</strong> ボタン<br>*保留中のプロジェクト承認の合計数 <br>*リンク先 <strong>[!UICONTROL プロジェクトの承認 ]</strong><br>*<strong>[!UICONTROL すべての承認を表示 ]</strong> ボタン<br>*日別ダイジェストの日付</p> </td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がタスクを承認する必要がある</strong> </p> <p>ジョブの役割の承認の場合、このイベントの電子メール通知を受け取るユーザーは、「[!UICONTROL 承認者がプロジェクトチームに属している必要がない（役割を含む承認プロセスの場合）]」設定が有効かどうかによって異なります ( <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">グローバル承認設定の指定</a>) をクリックします。 </p> <p><strong>このオプションが有効な場合</strong>承認済みの場合、ジョブの役割が関連付けられている、システム内のすべてのユーザーに電子メール通知が送信されます。 </p> <p><strong>このオプションが無効な場合</strong>承認プロセスに関連付けられたジョブロールを持つプロジェクトチームメンバーのみが電子メール通知を受け取ります。</p> <p>承認がユーザーに関連付けられている場合、そのユーザーに通知が届きます。 </p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL タスク承認待ち ]: &lt;task name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>タスク名<br>プロジェクト名<br>承認を送信したユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>タスクの優先度<br>承認ステージ名<br>承認者名<br>[!UICONTROL タスクの予定完了日 ]<br><strong>[!UICONTROL 承認を決定 ]</strong> ボタン<br>*保留中のタスク承認の合計数<br>*リンク先<strong>[!UICONTROL タスク承認*すべての承認を表示 ]</strong> ボタン<strong></strong>*日別ダイジェストの日付<br></p> </td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がタイムシートを承認する必要がある</strong> </p> <p>タイムシート承認者は、承認が必要なタイムシートが提出されたときに電子メール通知を受け取ります。ただし、タイムシートを提出したユーザーがタイムシート承認者でもある場合を除きます。</p> <p>タイムシートのステータスが [!UICONTROL 送信済み ] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL タイムシートが提出されました ]: &lt;timesheet owner=""&gt;, &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 承認のためにタイムシートを提出したユーザーの名前<br>タイムシートが提出された日時<br>タイムシートの状態<br>タイムシートの開始日と終了日<br>タイムシートに記録された時間数<br>タイムシートに記録された超過時間数<br><strong>[!UICONTROL レビュー ]</strong> および <strong>[!UICONTROL 承認 ]</strong> ボタン<br>*保留中のタイムシート承認の合計数<br>*リンク先 <strong>[!UICONTROL タイムシートの承認 ]</strong><br><strong>[!UICONTROL *すべての承認を表示 ]</strong> ボタン<br>*日別ダイジェストの日付 </td> 
   <td><strong>即時および</strong> <strong>毎日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が問題を承認する必要がある</strong> </p> <p>ジョブの役割の承認の場合、このイベントの電子メール通知を受け取るユーザーは、「[!UICONTROL 承認者がプロジェクトチームに属している必要がない（役割を含む承認プロセスの場合）]」設定が有効かどうかによって異なります ( <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL グローバル承認を設定 ]</a>) をクリックします。 </p> <p><strong>このオプションが有効な場合</strong>承認済みの場合、ジョブの役割が関連付けられている、システム内のすべてのユーザーに電子メール通知が送信されます。 </p> <p><strong>このオプションが無効な場合</strong>承認プロセスに関連付けられたジョブロールを持つプロジェクトチームメンバーのみが電子メール通知を受け取ります。</p> <p>承認がユーザーに関連付けられている場合、そのユーザーに通知が届きます。 </p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 承認待ちの問題 ]: &lt;issue name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名<br>プロジェクト名<br>問題の参照番号<br>承認のために問題を送信したユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>問題の優先度<br>承認ステージ<br>承認者の名前<br>[!UICONTROL 発行予定完了日 ]<br>[!UICONTROLプライマリ連絡先 ]<br><strong>[!UICONTROL 承認を決定 ]</strong> ボタン<br>*保留中の問題の承認数の合計です<br>*リンク先 <strong>[!UICONTROL 問題の承認 ]</strong><br><strong>[!UICONTROL *すべての承認を表示 ]</strong> ボタン<br>*日別ダイジェストの日付 </td> 
   <td><strong>即時および</strong> <strong>毎日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が委任されたプロジェクトの承認について確認する必要がある</strong> </p> <p>プロジェクトの承認が委任されたので、確認する必要があります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 委任されたプロジェクトの承認 — 確認してください ] &lt;project name=""&gt;</em></p> <p><em>日次ダイジェスト通知の件名は次のとおりです。[!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em> </p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>承認をリクエストしたユーザーの名前<br>プロジェクトを承認するユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>プロジェクトの優先度<br>承認ステップ<br>承認者の名前<br>[!UICONTROL プロジェクト予定完了日 ]<br><strong>[!UICONTROL 承認を決定 ]</strong> ボタン<br>*保留中のプロジェクト承認の合計数<br>*リンク先 <strong>[!UICONTROL プロジェクト承認*すべての承認を表示 ]</strong> ボタン <br>*日別ダイジェストの日付 </td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が委任されたタスクの承認について確認する必要がある</strong> </p> <p>タスクの承認が委任されたので、確認する必要があります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 委任タスクの承認 — 確認してください ]&lt;task name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>承認をリクエストしたユーザーの名前<br>タスクを承認するユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>タスクの優先度<br>承認ステージ<br>承認者の名前<br>[!UICONTROL タスクの予定完了日 ]<br><strong>[!UICONTROL 承認を決定 ]</strong> ボタン <br>*保留中のタスク承認の合計数<br>*リンク先 <strong>[!UICONTROL タスク承認*すべての承認を表示 ]</strong> ボタン<br>*日別ダイジェストの日付 </td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が委任された問題の承認について確認する必要がある</strong> </p> <p>問題の承認が委任されたので、確認する必要があります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 委任された問題の承認 — 確認してください ] &lt;issue name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 問題名<br>プロジェクト名<br>問題の参照番号<br>承認をリクエストしたユーザーの名前<br>問題を承認するユーザーの名前<br>承認待ちステータス<br>リクエストされた承認の日時<br>問題の優先度<br>承認ステージ<br>承認者の名前<br>発行計画完了日<br>プライマリ連絡先<br><strong>[!UICONTROL 承認を決定 ]</strong> ボタン<br>*保留中の問題の承認の合計数<br>*リンク先 <strong>[!UICONTROL 問題の承認 ]</strong><br><strong>[!UICONTROL *すべての承認を表示 ]</strong> ボタン<br>*日別ダイジェストの日付<br></td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分に問題が割り当てられた</strong> </p> <p>問題の担当者が電子メール通知を受け取ります。 問題のステータスが [!UICONTROL クローズ済み ] の場合、またはそれと等しい場合、問題の担当者は電子メールを受け取りません。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 新しい作業リクエスト ]: &lt;issue name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>問題名<br>プロジェクト名<br>[!UICONTROL 問題参照番号 ]<br>名前<br>問題の期限（[!UICONTROL 予定完了日 ]）<br>イシューを割り当てたユーザーの名前<br><strong>[!UICONTROL 操作 ]</strong> ボタン<br>*割り当ての合計数<br>*割り当てられたタスクとタスクの合計数<br>*リンク先 <strong>[!UICONTROL Work Requests]</strong><br>*日別ダイジェストの日付<br></p> </td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がタスクのプライマリ割り当てに設定された</strong> </p> <p>タスクの担当者がタスクの主な担当者になった場合は、タスクの担当者が割り当てをおこなったユーザーでない限り、タスクの主な担当者になった場合に電子メール通知が送信されます。</p> <p>プロジェクトのステータスが [!UICONTROL 現在 ] で、タスクが [!UICONTROL 完了 ] とマークされていない場合は、通知が送信されます。</p> <p>[!UICONTROL レビュー ] または [!UICONTROL リクエスト元 ] のライセンスを持つユーザーには通知が届きません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 新しい作業リクエスト ]: &lt;task name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>名前<br>タスクの期限（[!UICONTROL 予定完了日 ]）<br>タスクを割り当てたユーザーの名前<br><strong>[!UICONTROL 操作 ]</strong> ボタン<br>*割り当てられたタスクとタスクの合計数<br>*リンク先 <strong>[!UICONTROL Work Requests]</strong>*日別ダイジェストの日付 </td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>担当チームが新しい作業要求を受けた</strong> </p> <p>チームメンバーは、チームが新しい作業リクエストを受け取ると、電子メール通知を受け取ります。 （リクエストを送信したユーザーは、チームのメンバーである場合は通知を受け取りません）。</p> <p>プロジェクトのステータスが [!UICONTROL Current] で、作業リクエストのステータスが [!UICONTROL New] の場合にのみ通知が送信されます。</p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 新しい作業リクエスト ]: &lt;request name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。 <em>[!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p> 問題名<br>プロジェクト名（リクエストキュー名）<br>問題の参照番号<br>チーム名<br>発行期限（計画完了日）<br>リクエストを送信したユーザーの名前<br><strong>[!UICONTROL 操作 ]</strong> ボタン<br>*チームに割り当てられたリクエストの合計数</p> <p>*作業依頼名</p> <p>[!UICONTROL *計画完了日 ]</p> <p>*リクエストを送信したユーザーの名前<br>*リンク先 <strong>[!UICONTROL チームリクエスト ]</strong><br>*日別ダイジェストの日付 </p> <p><span class="preview">*チーム割り当て</span> </p> </td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分のタイムシートが再開された</strong> </p> <p>タイムシートの所有者は、タイムシートを再開したユーザーがタイムシートの所有者でもない限り、タイムシートが再開されると電子メール通知を受け取ります。</p> <p>電子メール通知は、タイムシートのステータスが [!UICONTROL 開く ] の場合にのみ送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL タイムシートが再開されました ]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p>注意：この通知は、毎日のダイジェスト電子メールには設定できません。</p> </td> 
   <td> タイムシートを再開したユーザーの名前<br>タイムシートが再開された日時<br>タイムシートのステータス（[!UICONTROL 再開済み ]）<br>タイムシートに記録された合計時間数<br>タイムシートに記録された超過時間数<br><strong>[!UICONTROL レビュー ]</strong> ボタン </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分のタイムシートが拒否された</strong> </p> <p>タイムシートの所有者は、タイムシートを拒否したユーザーが所有者でもない限り、タイムシートが拒否されると電子メール通知を受け取ります。</p> <p>電子メール通知は、タイムシートのステータスが [!UICONTROL 却下 ] の場合にのみ送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL タイムシート却下 ] :&lt;start date="" of="" the="" timesheet=""&gt; - &lt;end date="" of="" the="" timesheet=""&gt;</em></p> <p>注意：この通知は、毎日のダイジェスト電子メールには設定できません。</p> </td> 
   <td> タイムシートを却下したユーザーの名前<br>タイムシートのステータス（[!UICONTROL 却下 ]）<br>タイムシートが却下された日時<br><strong>[!UICONTROL レビュー ]</strong> ボタン </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが私からのアクセスを要求しています</strong> </p> <p>私に何かをするように頼むので、それをオンにします。</p> <p>プロジェクトを作成したユーザーがそのプロジェクトにアクセスできます。</p> <p>これにより、ユーザーがアクセスを要求したときに通知が受け取られます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;name of="" user="" who="" requested="" the="" access=""&gt; [!UICONTROL は ] へのアクセス権が必要です &lt;object name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 必要なアクションのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>オブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>アクセスをリクエストしたユーザーの名前<br>ユーザーがリクエストしているアクセスのタイプ<br><strong>[!UICONTROL 付与 ] &lt;name of="" the="" access="" requested=""&gt; アクセス</strong> および <strong>[!UICONTROL 別のアクセス権を付与 ]</strong> ボタン<br>*保留中のアクセス要求の承認の合計数<br>*リンク先 <strong>[!UICONTROL アクセスリクエスト ]</strong> 承認<br>*1 日のダイジェストの日付</p> </td> 
   <td><strong>即時および毎日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ドキュメントのアップロードを要求している人がいます</strong> </p> <p>ドキュメントのアップロード要求をユーザーが受け取ると、ドキュメント要求に電子メール通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;name of="" the="" user="" requesting="" the="" document=""&gt; [!UICONTROL には [!DNL Workfront].]</em></p> <p> <p>注意：この通知は、毎日のダイジェスト電子メールには設定できません。</p> </p> </td> 
   <td> ドキュメントを要求するユーザーの名前<br>ドキュメントをアップロードするオブジェクトの名前<br><strong>[!UICONTROL ここに添付 ]</strong> リンク </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
 </tbody> 
</table>
