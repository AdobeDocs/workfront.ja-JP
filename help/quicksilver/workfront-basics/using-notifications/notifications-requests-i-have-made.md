---
content-type: reference
navigation-topic: notifications
title: '通知：私が行ったリクエスト'
description: 次の通知で、Adobe Workfrontでおこなったリクエストを通知します。
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 6%

---

# 通知：自分が行ったリクエスト

次の通知で、でのリクエストについて知らせます。 [!DNL Adobe Workfront].

受信する通知の設定については、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

関連トピック [イベント通知](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>行った要求</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ドキュメント承認要求が完了した</strong> </p> <p>ドキュメントの承認を要求したユーザーは、ドキュメントの承認要求が完了すると、電子メール通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。<em> &lt;approver name=""&gt; 次に該当 &lt;approval decision="" uicontrol="" approved="" uicontrol="" approved="" with="" changes="" uicontrol="" rejected=""&gt; このドキュメント。</em></p> <p>注意：この通知は、毎日のダイジェスト電子メールには設定できません。</p> </td> 
   <td> ドキュメント名<br>承認者名 </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がプライマリ連絡先となっている問題に関するドキュメントが、変更またはアップロードされた</strong> </p> <p>問題の主要連絡先は、問題に関するドキュメントがアップロードまたは変更されたときに電子メール通知を受け取ります。ただし、ドキュメントをアップロードまたは変更したユーザーが主要連絡先でもある場合は除きます。</p> <p>通知は、プロジェクトが [!UICONTROL ヘルプリクエストキュー ] として設定されている場合にのみ送信されます ( <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL リクエストキューの作成 ]</a>) をクリックします。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>に追加されたドキュメント &lt;issue name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。 <em>要求のダイジェスト &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> ドキュメントがアップロードされたオブジェクト名<br>親オブジェクト名<br>ドキュメント参照番号<br>ドキュメントをアップロードしたユーザーの名前<br>ドキュメント名<br>追加日<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br>ドキュメントのサムネール<br><strong>[!UICONTROL プレビュー ]</strong> および <strong>[!UICONTROL ダウンロード ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*アップロードされたドキュメントの合計数<br>*ドキュメント名<br>*親オブジェクト名<br>*ドキュメントを追加したユーザーの名前<br>*日別ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ドキュメントのアップロード要求が果たされました</strong> </p> <p>ドキュメント要求者は、ドキュメントのアップロード要求が満たされると、電子メール通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL ドキュメントリクエスト元 ] &lt;user name=""&gt; が満たされた</em></p> <p>注意：この通知は、毎日のダイジェスト電子メールには設定できません。</p> </td> 
   <td> <p>ドキュメントをアップロードしたユーザーの名前<br>ドキュメントがアップロードされたオブジェクト名<br>ドキュメント名<br><br></p> </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かに割り当てたパーソナル タスクが完了しました</strong> </p> <p>アドホックタスクを割り当てたユーザーに対し、そのタスクの完了時に通知が送信されます。 </p> <p>アドホックタスクについて詳しくは、 <a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">[!UICONTROL Home] 領域から作業項目を作成する</a>.</p> <p>即時通知 E メールの件名は次のとおりです。 <em>タスク完了： &lt;task name=""&gt;</em></p> <p> <p>注意：この通知は、毎日のダイジェスト電子メールには設定できません。</p> </p> </td> 
   <td> タスク名<br>デフォルトのプロジェクト名（個人用タスクを受け取ったユーザーの個人用プロジェクト）<br>タスク参照番号<br>タスク所有者名<br>新規タスクステータス<br>タスクが完了した日時<br>前のタスクステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br><br><br></td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がプライマリ連絡先である問題が完了した</strong> </p> <p>問題の主要連絡先は、問題が完了したときに通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 問題の完了 ]: &lt;issue name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> 要求のダイジェスト &lt;date of="" the="" daily="" digest=""&gt;</em></p> <p> </p> </td> 
   <td> 問題名<br>プロジェクト名<br>問題の参照番号<br>問題を完了したユーザーの名前<br>新しいステータス<br>問題が完了した日時<br>以前の問題のステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン <br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了した問題の総数<br>*問題名<br>*問題を完了したユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がプロジェクトに問題を追加した</strong> </p> <p>問題の主な連絡先は、プロジェクトに問題を追加したときに通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] または [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 問題が送信されました ]: &lt;issue name=""&gt; オン &lt;project name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> 要求のダイジェスト &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> プロジェクト名<br>Portfolio名<br>問題の参照番号<br>名前<br>問題名<br>入力日<br>問題の優先度<br>問題ステータス<br>割り当て先名<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加された問題の総数<br>*問題名<br>*1 日のダイジェストの日付 </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が要求を送信した（確認）</strong> </p> <p>問題のプライマリ連絡先は、問題を送信すると電子メール通知を受け取ります。</p> <p>通知は、プロジェクトのステータスが [!UICONTROL Current] で、プロジェクトが [!UICONTROL Help Request Queue] として設定されている場合 ( <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL リクエストキューの作成 ]</a>) をクリックします。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL リクエストが送信されました ]: &lt;request name=""&gt; オン &lt;project request="" queue="" name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> 要求のダイジェスト &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>プロジェクト名（リクエストキュー名）<br>Portfolio名<br>問題の参照番号<br>問題名<br>入力日<br>問題の優先度<br>問題ステータス<br>割り当て先名<br>プライマリ連絡先<br>*プロジェクト参照番号<br>*プロジェクト名<br>*送信されたリクエストの合計数<br>*リクエスト名<br>*リクエストの優先度<br>*1 日のダイジェストの日付</p> </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分の要求がクローズされた（確認）</strong> </p> <p>リクエストが閉じられると、問題のプライマリー連絡先に電子メール通知が届きます。</p> <p>通知は、プロジェクトのステータスが「現在」で、プロジェクトが [!UICONTROL ヘルプリクエストキュー ] として設定されている場合 ( <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>) をクリックします。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL リクエストは閉じられました ]:"&lt;request name=""&gt;"</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL リクエストのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> リクエスト名<br>プロジェクト名<br>リクエストの参照番号<br>リクエストを閉じたユーザーの名前<br>問題ステータス<br>リクエストが閉じられた日時<br>前のリクエストのステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト参照番号<br>*プロジェクト名<br>*クローズされたリクエストの合計数<br>*リクエスト名<br>*リクエストを閉じたユーザーの名前<br>*1 日のダイジェストの日付 </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分の要求に誰かが割り当てられた</strong> </p> <p>主要連絡先と割り当てられたユーザーが同じユーザーでない限り、ユーザーが問題に割り当てられると、問題の主要連絡先に電子メール通知が届きます。</p> <p>通知は、プロジェクトのステータスが「現在」で、プロジェクトが [!UICONTROL ヘルプリクエストキュー ] として設定されている場合 ( <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL リクエストキューの作成 ]</a>) をクリックします。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;name of="" the="" user="" who="" is="" assigned="" to="" your="" request=""&gt; [!UICONTROL がリクエストに割り当てられました ]:"&lt;request name=""&gt;"</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL リクエストのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>問題名<br>プロジェクト名<br>問題の参照番号<br>リクエスト名<br>リクエストタイプ<br>入力日<br>問題の優先度<br>プライマリ連絡先<br>計画完了日<br>問題ステータス<br><strong>詳細を表示</strong> ボタン <br>*プロジェクト名<br>*プロジェクト参照番号<br>*割り当てられたリクエストの合計数<br>*リクエスト名<br>*名前に割り当て済み<br>*1 日のダイジェストの日付</p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が作成したプロジェクトの状態が変更した</strong> </p> <p>プロジェクトを作成したユーザーは、プロジェクトのステータスが変更されると、電子メール通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL プロジェクトステータスの変更 ]: &lt;project name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL リクエストのダイジェスト ] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>ステータスを変更したユーザーの名前<br>新しいステータス<br>プロジェクトステータスが変更された日時<br>前のプロジェクトステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*プロジェクトの新規ステータス<br>*プロジェクトステータスを変更したユーザーの名前<br>*1 日のダイジェストの日付</p> </td> 
   <td> <p><strong>今すぐ</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分の要求の状態が変更した</strong> </p> <p>ステータスを変更したユーザーが主要連絡先でもない限り、問題のステータスが変更されると、問題の主要連絡先に電子メール通知が届きます。</p> <p>通知は、プロジェクトのステータスが「現在」で、プロジェクトが [!UICONTROL ヘルプリクエストキュー ] として設定されている場合にのみ送信されます ( <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL リクエストキューの作成 ]</a>) をクリックします。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;request name=""&gt; が &lt;new status=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> 要求のダイジェスト &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> リクエスト名<br>プロジェクト名<br>リクエストの参照番号<br>リクエストのステータスを変更したユーザーの名前<br>新しいステータス<br>リクエストのステータスが変更された日時<br>前のリクエストのステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*ステータスが変更されたリクエストの合計数<br>*リクエスト名<br>*前のリクエストのステータス<br>*新規リクエストステータス<br>*ステータスを変更したユーザーの名前<br>*日別ダイジェストの日付<br></td> 
   <td> <p><strong>日次</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
