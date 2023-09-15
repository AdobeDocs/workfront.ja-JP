---
content-type: reference
navigation-topic: notifications
title: "通知：自分のプロジェクトに関する情報"
description: 次の通知は、作業中のプロジェクトでのアクティビティの発生に関して警告します。
author: Lisa
feature: Get Started with Workfront
exl-id: c4cf84eb-8911-4bff-a548-7f0e6d8aa7b5
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 6%

---

# 通知：自分が取り組んでいるプロジェクトに関する情報

次の通知は、作業中のプロジェクトでのアクティビティの発生に関して警告します。

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
   <td> <p><strong>私が担当しているプロジェクトにドキュメントが追加されました</strong> </p> <p>プロジェクトチームのメンバーは、ドキュメントを追加したユーザーを除き、ドキュメントがプロジェクトに追加されると電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] で、ドキュメントがプライベートでない場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL ドキュメントが ] に追加されました &lt;project name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。 <em>[!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>ドキュメント参照番号<br>ドキュメントを追加したユーザーの名前<br>ドキュメント名<br>追加日<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br>ドキュメントのサムネール<br><strong>[!UICONTROL プレビュー ]</strong> および <strong>[!UICONTROL ダウンロード ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加されたドキュメントの合計数<br>*ドキュメント名<br>*ドキュメントをアップロードしたユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私が担当しているプロジェクトでマイルストーンタスクが完了しました</strong> </p> <p>プロジェクトチームのメンバーは、プロジェクトのマイルストーンタスクが完了すると通知を受け取ります。 個人用タスクが完了した場合、通知は送信されません。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt; オン &lt;project name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前<br>タスクステータス<br>タスクが完了した日時<br>前のタスクのステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン <br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加するプロジェクトの状況がアクティブになった</strong> </p> <p>プロジェクトチームのメンバーは、プロジェクトのステータスが [!UICONTROL Current] に設定されると、電子メール通知を受け取ります。</p> <p>注意：プロジェクトのステータスが [!UICONTROL Current] に設定された場合に通知を受け取るには、ユーザーがプロジェクトの「スタッフ」タブにリストされている必要があります。 プロジェクトチームにユーザーを追加する方法については、 <a href="../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">プロジェクトチームを管理</a>.</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;project name=""&gt; [!UICONTROL は現在です — プロジェクトに移動して、タスクを確認してください。]</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクトのステータス<br>プロジェクト [!UICONTROL 予定完了日 ]<br>プロジェクト所有者<br>自分に割り当てられたタスクのリスト、自分の職務の役割の 1 つ、または自分のチームの 1 つに割り当てられたタスクのリスト<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトのステータス<br>*1 日のダイジェストの日付</p> </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>私のチームが参加しているプロジェクトがアクティブになりました</strong> <p>プロジェクトがアクティブになると、チームのメンバーに電子メール通知が届きます。 通知を受け取るには、チームを少なくとも 1 つのタスクに割り当てる必要があります。</p><p>個々のユーザーとチームの両方がプロジェクトのタスクに割り当てられている場合。 チームは通知を受け取りません。</p><p>即時通知 E メールの件名は次のとおりです。 <i>&lt;project name=""&gt; [!UICONTROL がアクティブです — プロジェクトに移動して、タスクを確認してください。]</i></p><p>日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p></td> 
   <td>プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクトのステータス<br>プロジェクト [!UICONTROL 予定完了日 ]<br>プロジェクト所有者<br>チームに割り当てられたタスクのリスト<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトのステータス<br>*1 日のダイジェストの日付</td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私が担当しているプロジェクトが完了しました</strong> </p> <p>プロジェクトチームのメンバーは、プロジェクトのステータスが [!UICONTROL 完了 ] になると電子メール通知を受け取ります。</p> <p>ヒント：プロジェクトが定期的に完了している場合、このオプションを有効にすると、多くのプロジェクトでのタスク数が限られているユーザー向けに多数の電子メールを作成できます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL プロジェクトステータスの変更 ]: &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクトを完了したユーザーの名前<br>プロジェクトのステータス<br>プロジェクトが完了した日時<br>前のプロジェクトのステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトのステータス<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私が担当しているプロジェクトでタスクが完了しました</strong> </p> <p>プロジェクトチームのメンバーは、プロジェクトでタスクが完了すると電子メール通知を受け取ります。 <br>プロジェクトチームの詳細については、 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a>.</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;task name=""&gt; オン &lt;project name=""&gt;</em></p> <p> <p>注意：タスクがステータス（[!UICONTROL 完了 ]）に変更されても、電子メールの件名には「[!UICONTROL 完了 ]」と表示されます。</p> </p> <p><em> 日次ダイジェスト通知の件名は [!UICONTROL 現在表示中のプロジェクトのダイジェスト ] です。 &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> <p>タスク名<br>プロジェクト名<br>タスク参照番号<br>タスクを完了したユーザーの名前<br>タスクステータス<br>タスクのステータスが変更された日時<br>前のタスクのステータス<br><strong>詳細を見る</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したタスクの合計数<br>*タスク名<br>*タスクを完了したユーザーの名前<br>*日別ダイジェストの日付<br></p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私が担当しているプロジェクトに問題が追加されました</strong> </p> <p>プロジェクトチームのメンバーは、問題がプロジェクトに追加されると、電子メール通知を受け取ります。</p> <p>通知は、プロジェクトのステータスが「現在」の場合にのみ送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 問題の追加先 ] &lt;project name=""&gt;</em></p> <p> </p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>問題の参照番号<br>イシューを追加したユーザーの名前<br>問題のタイプ<br>問題名<br>入力日<br>問題の優先度<br>割り当て先名 <br>問題ステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトに追加された問題の合計数<br>*問題名<br>*問題に割り当てられたユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私が担当しているプロジェクトに関する問題が完了しました</strong> </p> <p>プロジェクトチームのメンバーは、プロジェクトで問題が完了すると、電子メール通知を受け取ります。<br>プロジェクトチームの詳細については、 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a>.</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 完了 ] : &lt;issue name=""&gt; オン &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名<br>プロジェクト名<br>問題を完了したユーザーの名前<br>問題ステータス<br>問題が完了した日時<br>以前の問題のステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了した問題の総数<br>*問題名<br>*問題に割り当てられたユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私が担当しているプロジェクトに未割り当ての問題が追加されました</strong> </p> <p>未割り当ての問題がプロジェクトに追加されると、プロジェクトチームのメンバーに電子メール通知が送信されます。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL この新しいイシューに割り当てるユーザー ] &lt;project name=""&gt;?</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>問題の参照番号<br>イシューを追加したユーザーの名前<br>問題名<br>問題のタイプ<br>入力日<br>問題の優先度<br>割り当て先名（空） <br>問題ステータス<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加された問題の総数<br>*問題名<br>*イシューを追加したユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がプロジェクトに追加されました</strong> </p> <p>プロジェクトに追加されたユーザーは、自分がプロジェクトに追加しない限り、追加されたときに電子メール通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL プロジェクトに追加されました ] &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクトに追加したユーザーの名前<br>プロジェクト [!UICONTROL 予定開始日 ]<br>プロジェクト [!UICONTROL 予定完了日 ]<br>プロジェクトの完了率<br>プロジェクト上の他のユーザーの名前 <br>プロジェクト所有者<br><strong>詳細を見る</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*1 日のダイジェストの日付</p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私が担当しているプロジェクトでステータスが変更されました</strong> </p> <p>プロジェクトチームのメンバーは、プロジェクトのステータスが変更されると、電子メール通知を受け取ります。 <br>プロジェクトチームの詳細については、 <a href="../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a>.</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL プロジェクトステータスの変更 ]: &lt;project name=""&gt;</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。 <em> [!UICONTROL 現在利用中のプロジェクトのダイジェスト ] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクトのステータスを変更したユーザーの名前<br>新規プロジェクトステータス<br>プロジェクトのステータスが変更された日時<br>前のプロジェクトのステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトのステータス<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
 </tbody> 
</table>
