---
content-type: reference
navigation-topic: notifications
title: 「通知：私が行ったリクエスト」
description: 次の通知で、Adobe Workfront で行われたリクエストについて通知します。
author: Lisa
feature: Get Started with Workfront
exl-id: 42771f71-dbf8-4e73-9a0e-8efea612af4a
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 99%

---

# 通知：私が行ったリクエスト

次の通知では、[!DNL Adobe Workfront] で行われたリクエストについて知らせます。

受信する通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

[イベント通知](../../workfront-basics/using-notifications/event-notifications.md)も参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td colspan="3"><strong>私が行ったリクエスト</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ドキュメント承認要求が完了しました</strong> </p> <p>ドキュメントの承認を要求したユーザーは、ドキュメントの承認要求が完了すると、メール通知を受け取ります。</p> <p>インスタント通知メールの件名：<em> &lt;Approver Name&gt; 様、このドキュメントが &lt;Approval Decision([!UICONTROL Approved], [!UICONTROL Approved with Changes], [!UICONTROL Rejected])&gt;されました。</em></p> <p>メモ：この通知を日刊ダイジェストメールに設定することはできません。</p> </td> 
   <td> ドキュメント名<br>承認者名 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がプライマリ連絡先となっているイシューに関するドキュメントが、変更またはアップロードされました</strong> </p> <p>イシューの主要連絡先は、イシューに関するドキュメントがアップロードまたは変更されたときにメール通知を受け取ります。ただし、ドキュメントをアップロードまたは変更したユーザーが主要連絡先でもある場合は除きます。</p> <p>通知は、（<a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a> で説明されているように）プロジェクトが [!UICONTROL Help Request Queue] として設定されている場合にのみ送信されます。</p> <p>インスタント通知メールの件名：<em>ドキュメントが &lt;Issue Name&gt; に追加されました</em></p> <p>日刊ダイジェスト通知の件名は次のとおりです。<em>リクエストのダイジェスト &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> ドキュメントがアップロードされたオブジェクト名<br>親オブジェクト名<br>ドキュメント参照番号<br>ドキュメントをアップロードしたユーザーの名前<br>ドキュメント名<br>追加した日<br>ドキュメントの詳細（形式、サイズ、バージョン番号）<br>ドキュメントのサムネール「<br><strong>[!UICONTROL Preview]</strong>」ボタンおよび「<strong>[!UICONTROL Download]</strong>」ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*アップロードされたドキュメントの合計数<br>*ドキュメント名<br>*親オブジェクト名<br>*ドキュメントを追加したユーザーの名前<br>*日刊ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ドキュメントのアップロードリクエストが実行されました</strong> </p> <p>ドキュメント依頼者は、ドキュメントのアップロードリクエストが満たされると、メール通知を受け取ります。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Your document request from] &lt;User Name&gt; が満たされました</em></p> <p>メモ：この通知を日刊ダイジェストメールに設定することはできません。</p> </td> 
   <td> <p>ドキュメントをアップロードしたユーザーの名前<br>ドキュメントがアップロードされたオブジェクト名<br>ドキュメント名<br><br></p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かに割り当てたパーソナルタスクが完了しました</strong> </p> <p>アドホックタスクを他の誰かに割り当てたユーザーに対し、そのタスクの完了時に通知が送信されます。 </p> <p>アドホックタスクに関して詳しくは、<a href="../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md" class="MCXref xref">[!UICONTROL Home] エリアから作業アイテムを作成する</a>を参照してください。</p> <p>インスタント通知メールの件名：<em>タスク完了：&lt;Task Name&gt;</em></p> <p> <p>メモ：この通知を日刊ダイジェストメールに設定することはできません。</p> </p> </td> 
   <td> タスク名<br>デフォルトのプロジェクト名（個人用タスクを受け取ったユーザーの個人用プロジェクト）<br>タスク参照番号<br>タスク所有者名<br>新規タスクステータス<br>タスクが完了した日時<br>タスクの前のステータス「<br><strong>[!UICONTROL See More Details]</strong>」ボタン<br><br><br></td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分がプライマリ連絡先であるイシューが完了した</strong> </p> <p>イシューのプライマリ連絡先は、イシューが完了したときに通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Issue Completion]：&lt;Issue Name&gt;</em></p> <p>日刊ダイジェスト通知の件名は次のとおりです。<em>リクエストのダイジェスト &lt;Date of the daily digest&gt;</em></p> <p> </p> </td> 
   <td> イシュー名<br>プロジェクト名<br>イシューの参照番号<br>イシューを完了したユーザーの名前<br>新しいステータス<br>イシューが完了した日時<br>以前のイシューのステータス「<br><strong>[!UICONTROL See More Details]</strong>」ボタン<br>*プロジェクト名<br>*プロジェクト参照番号<br>*完了したイシューの総数<br>*イシュー名<br>*イシューを完了したユーザーの名前<br>*日刊ダイジェストの日付 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がプロジェクトにイシューを追加しました</strong> </p> <p>イシューのプライマリ連絡先は、プロジェクトにイシューを追加したときに通知を受け取ります。</p> <p>プロジェクトのステータスが [!UICONTROL Current] か [!UICONTROL Planning] の場合にのみ通知が送信されます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Issue submitted]：&lt;Project Name&gt; の &lt;Issue Name&gt;</em></p> <p>日刊ダイジェスト通知の件名：<em>リクエストのダイジェスト &lt;Date of the daily digest&gt;</em></p> </td> 
   <td> プロジェクト名<br>ポートフォリオ名<br>イシューの参照番号<br>ご自身の名前<br>イシュー名<br>入力した日付<br>イシューの優先度<br>イシューのステータス<br>割り当て先名<br>プライマリ連絡先<br>*プロジェクト名<br>*プロジェクト参照番号<br>*追加されたイシューの総数<br>*イシュー名<br>*日刊ダイジェストの日付 </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>および日次</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私がリクエストを送信します (確認)</strong> </p> <p>イシューのプライマリ連絡先には、イシューの送信時にメール通知が届きます。</p> <p>通知は、（<a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>で説明されているように）プロジェクトのステータスが [!UICONTROL Current] で、プロジェクトが [!UICONTROL Help Request Queue] として設定されている場合にのみ送信されます。</p> <p>インスタント通知メールの件名は <em>[!UICONTROL Request Submitted]: &lt;Project (Request Queue) Name&gt; の &lt;Request Name&gt;</em> です。</p> <p>日刊ダイジェスト通知の件名は、<em>自分の要求のダイジェスト &lt;Date of the daily digest&gt;</em> です</p> </td> 
   <td> <p>プロジェクト名（リクエストキュー名）<br>ポートフォリオ名<br>イシューの参照番号<br>イシュー名<br>入力日<br>イシューの優先度<br>イシューのステータス<br>割り当て先名<br>プライマリ連絡先<br>*プロジェクトの参照番号<br>*プロジェクト名<br>*送信されたリクエストの合計数<br>*リクエスト名<br>*リクエストの優先度<br>*日刊ダイジェストの日付</p> </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>および日次</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私のリクエストがクローズされます (確認)</strong> </p> <p>リクエストがクローズされると、イシューのプライマリ連絡先にメール通知が届きます。</p> <p>通知は、（<a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>で説明されているように）プロジェクトのステータスが進行中で、プロジェクトが [!UICONTROL Help Request Queue] として設定されている場合にのみ送信されます。</p> <p>インスタント通知メールの件名は、<em>[!UICONTROL Your request has been closed]:"&lt;Request Name&gt;"</em> です</p> <p>日刊ダイジェスト通知の件名は、<em> [!UICONTROL Digest of your Requests] &lt;Date of the daily digest&gt;</em> です</p> </td> 
   <td> リクエスト名<br>プロジェクト名<br>リクエストの参照番号<br>リクエストをクローズしたユーザーの名前<br>イシューのステータス<br>リクエストがクローズされた日時<br>前のリクエストのステータス<br><strong>「[!UICONTROL See More Details]</strong>」ボタン<br>*プロジェクトの参照番号<br>*プロジェクト名<br>*クローズされたリクエストの合計数<br>*リクエスト名<br>*リクエストをクローズしたユーザーの名前<br>*日刊ダイジェストの日付 </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私のリクエストに誰かが割り当てられています</strong> </p> <p>ユーザーがイシューに割り当てられると、イシューのプライマリ連絡先にはメール通知が届きます。ただし、プライマリ連絡先が割り当てユーザーでもある場合を除きます。</p> <p>通知は、（<a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>で説明されているように）プロジェクトのステータスが進行中で、プロジェクトが [!UICONTROL Help Request Queue] として設定されている場合のみ送信されます。</p> <p>インスタント通知メールの件名は、<em>&lt;Name of the user who is assigned to your request&gt; [!UICONTROL has been assigned to your request]: "&lt;Request Name&gt;"</em> です</p> <p>日刊ダイジェスト通知の件名は、<em>[!UICONTROL Digest of your Requests] &lt;Date of the daily digest&gt;</em> です</p> </td> 
   <td> <p>イシュー名<br>プロジェクト名<br>イシューの参照番号<br>リクエスト名<br>リクエストタイプ<br>入力日<br>イシューの優先度<br>プライマリ連絡先<br>予定完了日<br>イシューのステータス<br><strong>「詳細を表示」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*割り当てられたリクエストの合計数<br>*リクエスト名<br>*割り当て先名<br>*日刊ダイジェストの日付</p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私が作成したプロジェクトでステータスが変更されました</strong> </p> <p>プロジェクトを作成したユーザーには、プロジェクトステータスの変更時にメール通知が届きます。</p> <p>インスタント通知メールの件名は、<em>[!UICONTROL Project Status Change] : &lt;Project Name&gt;</em> です</p> <p>日刊ダイジェスト通知の件名は、<em>[!UICONTROL Digest of your Requests] &lt;Date of the daily digest&gt;</em> です</p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>プロジェクトの参照番号<br>ステータスを変更したユーザーの名前<br>新しいステータス<br>プロジェクトステータスが変更された日時<br>前のプロジェクトのステータス<br><strong>「[!UICONTROL See More Details]」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*プロジェクトの新しいステータス<br>*プロジェクトステータスを変更したユーザーの名前<br>*日刊ダイジェストの日付</p> </td> 
   <td> <p><strong>今すぐ</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私のリクエストでステータスが変更されました</strong> </p> <p>イシューのステータスが変更されると、イシューのプライマリ連絡先にメール通知が届きます。ただし、ステータスを変更したユーザーがプライマリ連絡先と同じ場合を除きます。</p> <p>通知は、（<a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">[!UICONTROL Create a Request Queue]</a>で説明されているように）プロジェクトのステータスが進行中で、プロジェクトが [!UICONTROL Help Request Queue] として設定されている場合にのみ送信されます。</p> <p>インスタント通知メールの件名は、<em>&lt;Request Name&gt; は &lt;New Status&gt; です</em>です</p> <p>日刊ダイジェスト通知の件名は、<em>自分の要求のダイジェスト &lt;Date of the daily digest&gt;</em> です</p> </td> 
   <td> リクエスト名<br>プロジェクト名<br>リクエストの参照番号<br>リクエストのステータスを変更したユーザーの名前<br>新しいステータス<br>リクエストのステータスが変更された日時<br>前のリクエストのステータス<br><strong>「[!UICONTROL See More Details]」</strong>ボタン<br>*プロジェクト名<br>*プロジェクトの参照番号<br>*ステータスが変更されたリクエストの合計数<br>*リクエスト名<br>*前のリクエストのステータス<br>*新しいリクエストステータス<br>*ステータスを変更したユーザーの名前<br>*日刊ダイジェストの日付<br></td> 
   <td> <p><strong>日次</strong> </p> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>
