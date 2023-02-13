---
content-type: reference
navigation-topic: notifications
title: '通知：その他の情報'
description: 次の通知は、スポンサーとしているプロジェクトでのアクティビティの発生に関して警告します。
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 8%

---

# 通知：その他の情報

次の通知は、スポンサーとしているプロジェクトでのアクティビティの発生に関して警告します。

受信する通知の設定については、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

関連トピック [イベント通知](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>毎日の通知を有効または無効にすることはできません。また、このカテゴリのイベントに関する日々のダイジェスト電子メールを受信することもできません。 以下に対する個々のインスタント通知を有効または無効にできます： [!UICONTROL その他] カテゴリ。

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
   <td> <p><strong>メッセージが [!UICONTROL アナウンスセンター ] に送信されます</strong> </p> <p>新しいメッセージが [!UICONTROL アナウンスセンター ] に送信されると、電子メール通知が届きます。 </p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL [!DNL Adobe Workfront] お知らせ ] : &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> 発表の対象<br>お知らせに含まれるメッセージのテキスト<br>添付されたドキュメント<br>お知らせを送信したユーザーの名前<br>お知らせが送信された日時 </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>タスク割り当てへの変更により自分のユーザーの一人に影響が出た</strong> </p> <p>管理者として指定されたユーザーの直属のレポートの 1 つが新しいタスクに割り当てられると、管理者は、その割り当てに関する電子メールを受け取ります。 </p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL タスクリソース割り当て ]: &lt;task name=""&gt;</em></p> </td> 
   <td>プロジェクト名<br>タスク名<br>タスクが作成された日時<br>タスクを作成したユーザーの名前<br>割り当て名<br>期限（計画完了日）<br>タスクステータス<br></td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ドキュメントのアップロード要求の受信後、要求がキャンセルされました</strong> </p> <p>ドキュメントリクエストがキャンセルされると、ドキュメントリクエストは電子メール通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; ドキュメントリクエストがキャンセルされました。 </em></p> <p>電子メール通知の本文には、次のテキストが含まれます。</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL では、以前のリクエストに関する情報をアップロードする必要はなくなりました。 私たちはちょうどあなたに知らせたかった。]</em> </p> </td> 
   <td>リクエストをキャンセルしたユーザーの名前<br>元のドキュメントのアップロードリクエストのテキスト<br>元のドキュメントリクエストに対する「[!UICONTROL CANCELLED]」バナー<br>元のドキュメントリクエストの日時<br></td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が確認すべきエラーが見つかりました</strong> </p> <p>電子メールでコメントに返信するユーザーは、返信が配信されなかった場合に電子メール通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL での処理に失敗しました ] &lt;subject of="" original="" message=""&gt;</em></p> <p>電子メールを使用してコメントに返信する方法については、を参照してください。<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>問題の割り当て変更により自分のユーザーが影響を受けた</strong> </p> <p>イシューに割り当てられたユーザーのマネージャーは、そのユーザーがイシューから削除されたり、イシューに割り当てられたりすると、電子メール通知を受け取ります。 </p> <p>通知は、プロジェクトのステータスが「現在」または「計画」の場合にのみ送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>問題の割り当て： &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>問題名<br>プロジェクト名<br>問題の参照番号<br>割り当てをおこなったユーザーの名前<br>問題のタイプ<br>イシューに割り当てられたユーザーの名前<br>発行日が入力されました<br>問題の優先度<br>プライマリ連絡先<br>問題 [!UICONTROL 計画完了日 ]<br>問題ステータス<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン</p> </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分のユーザー 1 名がプロジェクトに追加された</strong> </p> <p>管理者は、ユーザーの 1 人がプロジェクトに追加されると、電子メール通知を受け取ります。 この通知は、プロジェクトのステータスに関係なく送信されます。 </p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>E メールの件名は次のとおりです。 <em>プロジェクト割り当て： &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>プロジェクト名<br>Portfolio名<br>プロジェクト参照番号<br>プロジェクトに人物を追加したユーザーの名前<br>プロジェクトに追加されたユーザーの名前<br>プロジェクト [!UICONTROL 予定開始日 ]<br>プロジェクト [!UICONTROL 予定完了日 ]<br>プロジェクト完了率<br>プロジェクト上の他のユーザーの名前<br>プロジェクトステータス<br>プロジェクト所有者<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br><br><br></p> </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するポートフォリオまたはプログラムに誰かがプロジェクトを追加した</strong> </p> <p>ポートフォリオまたはプログラムに新しいプロジェクトが追加されると、ポートフォリオまたはプログラム所有者に通知が届きます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL プロジェクトがに追加されました ] &lt;portfolio name=""&gt;[ プロジェクト GUID]</em></p> </td> 
   <td> Portfolio名<br>プロジェクト参照番号<br>ポートフォリオ/プログラムにプロジェクトを追加したユーザーの名前<br><br></td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが自分とオブジェクトを共有する</strong> </p> <p>オブジェクトに対する権限の [!UICONTROL Sharing] リストにユーザーが追加されると、電子メール通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL アクセスの許可 ] : &lt;object name=""&gt;</em></p> <p>通知は、プロジェクトのステータスが [!UICONTROL Current] の場合にのみ送信されます。</p> </td> 
   <td> オブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>オブジェクトへのオリジナルのアクセス<br>オブジェクトに対する新しいアクセスが許可されました<br>アクセスが許可された日時 <br>アクセス権を付与したユーザーの名前 </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かがマイ チームとオブジェクトを共有する</strong> </p> <p>オブジェクトに対する権限の共有リストにチームを追加すると、電子メール通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL アクセスの許可 ] : &lt;object name=""&gt; [ アクセス規則 GUID]</em></p> </td> 
   <td> オブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>古いアクセス<br>新しいアクセス<br>アクセスが許可された日時<br>チームの名前<br>アクセス権を付与したユーザーの名前 </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>購読しているタスク、イシューまたはプロジェクトを更新します</strong> </p> <p>購読している項目に対して誰かがコメントをすると、電子メール通知が送信されます。</p> <p>購読 E メールの件名は次のとおりです。 <em>[!UICONTROL] が更新されました &lt;object type=""&gt; 購読している場所： &lt;object name=""&gt;</em></p> </td> 
   <td> オブジェクト名<br> オブジェクト参照番号<br> 購読項目に対してコメントを行ったユーザーの名前<br> コメントが行われた日付<br> 購読項目に追加されたコメント  </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
 </tbody> 
</table>
