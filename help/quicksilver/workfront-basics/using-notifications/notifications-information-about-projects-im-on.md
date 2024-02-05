---
content-type: reference
navigation-topic: notifications
title: 「通知：自分が参加しているプロジェクトに関する情報」
description: 次の通知は、作業中のプロジェクトで発生するアクティビティについて警告します。
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 99%

---

# 通知：自分が参加しているプロジェクトに関する情報

次の通知は、作業中のプロジェクトで発生するアクティビティについて警告します。

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
   <td> <p><strong>自分が参加しているプロジェクトにドキュメントが追加された</strong> </p> <p>ドキュメントがプロジェクトに追加されると、プロジェクトチームのメンバー（ドキュメントを追加したユーザーを除く）はメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] で、ドキュメントがプライベートでない場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名は次の通りです：<em>[!UICONTROL Document added to] &lt;Project Name&gt;</em></p> <p>日次ダイジェスト通知の件名は次の通りです：<em>[!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>ドキュメントの参照番号<br>ドキュメントを追加したユーザーの名前<br>ドキュメント名<br>追加した日付<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br>ドキュメントのサムネール<br><strong>[!UICONTROL Preview]</strong> と <strong>[!UICONTROL Download]</strong> ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*追加されたドキュメントの合計数<br>*ドキュメント名<br>*ドキュメントをアップロードしたユーザーの名前<br>*日次ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加しているプロジェクトのマイルストーンタスクが完了した</strong> </p> <p>プロジェクトのマイルストーンタスクが完了すると、プロジェクトチームのメンバーは通知を受け取ります。個人のタスクが完了しても、通知は送信されません。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>件名は次の通りです：<em>[!UICONTROL Complete]: &lt;Task Name&gt; on &lt;Project Name&gt;</em></p> <p>日次ダイジェスト通知の件名は次の通りです：<em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスクの参照番号<br>タスクを完了したユーザーの名前<br>タスクのステータス<br>タスクが完了した日時<br>タスクの以前のステータス<br><strong>[!UICONTROL See More Details]</strong> ボタン <br>*プロジェクト名<br>*プロジェクトの参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日次ダイジェストの日付<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加するプロジェクトの状況がアクティブになった</strong> </p> <p>プロジェクトのステータスが [!UICONTROL Current] に設定されると、プロジェクトチームのメンバーはメール通知を受け取ります。</p> <p>メモ：プロジェクトのステータスが [!UICONTROL Current] に設定されている場合に通知を受け取るには、ユーザーがプロジェクトの「スタッフ」タブにリストされている必要があります。プロジェクトチームにユーザーを追加する方法については、<a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">プロジェクトチームを管理</a>を参照してください。</p> <p>インスタント通知メールの件名は次の通りです：<em>&lt;Project Name&gt; [!UICONTROL is Current - Go to your project and see your tasks!]</em></p> <p> 日次ダイジェスト通知の件名は次の通りです：<em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>プロジェクトのステータス<br>プロジェクト [!UICONTROL Planned Completion Date]<br>プロジェクト所有者<br>自分、自分の職務の役割の 1 つ、または自分のチームの 1 つに割り当てられたタスクのリスト<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトのステータス<br>*日次ダイジェストの日付</p> </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>自分のチームが参加するプロジェクトがアクティブになった</strong> <p>プロジェクトがアクティブになると、チームのメンバーはメール通知を受け取ります。通知を受け取るには、チームを 1 つ以上のタスクに割り当てる必要があります。</p><p>個々のユーザーとチームの両方がプロジェクトのタスクに割り当てられている場合。チームは通知を受け取りません。</p><p>インスタント通知メールの件名は次の通りです：<i>&lt;Project Name&gt; [!UICONTROL is Active - Go to your project and see your tasks!]</i></p><p>日次ダイジェスト通知の件名は次の通りです：<em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p></td> 
   <td>プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>プロジェクトのステータス<br>プロジェクト [!UICONTROL Planned Completion Date]<br>プロジェクト所有者<br>自分、自分の職務の役割の 1 つ、または自分のチームの 1 つに割り当てられたタスクのリスト<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトのステータス<br>*日次ダイジェストの日付</td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加しているプロジェクトが完了した</strong> </p> <p>プロジェクトのステータスが [!UICONTROL Complete] になると、プロジェクトチームのメンバーはメール通知を受け取ります。</p> <p>ヒント：プロジェクトが定期的に完了する場合、このオプションを有効にすると、多くのプロジェクトでタスク数が限られているユーザー向けに大量のメールを作成できます。</p> <p>インスタント通知メールの件名は次の通りです：<em>[!UICONTROL Project Status Change]: &lt;Project Name&gt;</em></p> <p> 日刊ダイジェスト通知の件名は次の通りです：<em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>プロジェクトの参照番号<br>プロジェクトを完了したユーザーの名前<br>プロジェクトのステータス<br>プロジェクトが完了した日時<br>プロジェクトの以前のステータス<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*プロジェクトのステータス<br>*日次ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加しているプロジェクトのタスクが完了した</strong> </p> <p>プロジェクトでタスクが完了すると、プロジェクトチームのメンバーはメール通知を受け取ります。<br>プロジェクトチームについて詳しくは、<a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a>を参照してください。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名は次の通りです：<em>[!UICONTROL Complete]: &lt;Task Name&gt; on &lt;Project Name&gt;</em></p> <p> <p>注意：タスクが [!UICONTROL Complete] と同等のステータスに変更された場合も、メールの件名には [!UICONTROL Complete] と表示されます。</p> </p> <p><em> 日次ダイジェスト通知の件名は次の通りです：[!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em> </p> </td> 
   <td> <p>タスク名<br>プロジェクト名<br>タスクの参照番号<br>タスクを完了したユーザーの名前<br>タスクのステータス<br>タスクのステータスが変更された日時<br>タスクの以前のステータス<br><strong>詳細を見る</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日次ダイジェストの日付<br></p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加しているプロジェクトに問題が追加された</strong> </p> <p>イシューがプロジェクトに追加されると、プロジェクトチームのメンバーはメール通知を受け取ります。</p> <p>プロジェクトのステータスが「進行中」の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名は次の通りです：<em>[!UICONTROL Issue added to] &lt;Project Name&gt;</em></p> <p> </p> <p> 日次ダイジェスト通知の件名は次の通りです：<em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>イシューの参照番号<br>イシューを追加したユーザーの名前<br>イシュータイプ<br>イシュー名<br>入力した日付<br>イシューの優先度<br>割り当て先の名前 <br>イシューのステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*プロジェクトに追加されたイシューの合計数<br>*イシュー名<br>*イシューの割り当て先のユーザーの名前<br>*日次ダイジェストの日付 </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日次</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加しているプロジェクトの問題が完了した</strong> </p> <p>プロジェクトでイシューが完了すると、プロジェクトチームのメンバーはメール通知を受け取ります。<br>プロジェクトチームについて詳しくは、<a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a>を参照してください。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名は次の通りです：<em>[!UICONTROL Complete]: &lt;Issue Name&gt; on &lt;Project name&gt;</em></p> <p> 日次ダイジェスト通知の件名は次の通りです：<em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> イシュー名<br>プロジェクト名<br>イシューを完了したユーザーの名前<br>イシューのステータス<br>イシューが完了した日時<br>イシューの以前のステータス<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*完了したイシューの合計数<br>*イシュー名<br>*イシューの割り当て先のユーザーの名前<br>*日次ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加しているプロジェクトに未割り当ての問題が追加された</strong> </p> <p>未割り当てのイシューがプロジェクトに追加されると、プロジェクトチームのメンバーはメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名は次の通りです：<em>[!UICONTROL Who should be assigned to this new issue on] &lt;Project Name&gt;?</em></p> <p> 日次ダイジェスト通知の件名は次の通りです：<em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>イシューの参照番号<br>イシューを追加したユーザーの名前<br>イシュー名<br>イシュータイプ<br>入力した日付<br>イシューの優先度<br>割り当て先の名前（空欄）<br>イシューのステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*追加されたイシューの合計数<br>*イシュー名<br>*イシューを追加したユーザーの名前<br>*日次ダイジェストの日付<br></td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日次</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がプロジェクトに追加された</strong> </p> <p>ユーザーがプロジェクトに追加されると、自分自身をプロジェクトに追加した場合を除き、追加されたユーザーはメール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名は次の通りです：<em>[!UICONTROL You've been added to the project] &lt;Project Name&gt;</em></p> <p> 日次ダイジェスト通知の件名は次の通りです：<em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>プロジェクトの参照番号<br>プロジェクトに追加したユーザーの名前<br>プロジェクトの [!UICONTROL Planned Start Date]<br>プロジェクトの [!UICONTROL Planned Completion Date]<br>プロジェクトの完了率<br>プロジェクトの他のユーザーの名前<br>プロジェクト所有者<br><strong>詳細を見る</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*日次ダイジェストの日付</p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加しているプロジェクトの状態が変更した</strong> </p> <p>プロジェクトのステータスが変更されると、プロジェクトチームのメンバーはメール通知を受け取ります。<br>プロジェクトチームについて詳しくは、<a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a>を参照してください。</p> <p>インスタント通知メールの件名は次の通りです：<em>[!UICONTROL Project Status Change]: &lt;Project Name&gt;</em></p> <p> 日次ダイジェスト通知の件名は次の通りです：<em> [!UICONTROL Digest of Projects You're On] &lt;Date of daily digest&gt; </em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>プロジェクトの参照番号<br>プロジェクトのステータスを変更したユーザーの名前<br>プロジェクトの新しいステータス<br>プロジェクトのステータスが変更された日時<br>プロジェクトの以前のステータス<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*プロジェクトのステータス<br>*日次ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
 </tbody> 
</table>
