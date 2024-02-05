---
content-type: reference
navigation-topic: notifications
title: 「通知：その他の情報」
description: 次の通知は、自分がスポンサーしているプロジェクトで発生するアクティビティについて警告します。
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 298b74c2d228a76c02d34470fa8298028605cab4
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 97%

---

# 通知：その他の情報

次の通知は、自分がスポンサーしているプロジェクトで発生するアクティビティについて警告します。

受信する通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

[イベント通知](../../workfront-basics/using-notifications/event-notifications.md)も参照してください。

>[!NOTE]
>
>毎日の通知を有効または無効にすることはできません。また、このカテゴリのイベントに関する日々のダイジェストメールを受信することもできません。[!UICONTROL その他]カテゴリのインスタント通知を個別に有効または無効にできます。

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
   <td> <p><strong>[!UICONTROL Announcement Center] にメッセージが送信されました</strong> </p> <p>新しいメッセージが [!UICONTROL Announcement Center] に送信されると、メール通知が届きます。 </p> <p>即時通知メールの件名は次のとおりです：<em>[!UICONTROL [!DNL Adobe Workfront] Announcement]：&lt;お知らせの件名&gt;</em></p> </td> 
   <td> お知らせの件名<br>お知らせに含まれるメッセージのテキスト<br>添付されたドキュメント<br>お知らせを送信したユーザーの名前<br>お知らせが送信された日時 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>タスク割り当てへの変更により、自分のユーザー 1 人に影響があります</strong> </p> <p>管理者として指定されたユーザーのダイレクトレポートの 1 つが新しいタスクに割り当てられると、管理者は、その割り当てに関するメールを受け取ります。 </p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知メールの件名は次のとおりです：<em>[!UICONTROL Task Resource Assignment]：&lt;タスク名&gt;</em></p> </td> 
   <td>プロジェクト名<br>タスク名<br>タスクが作成された日時<br>タスクを作成したユーザーの名前<br>割り当て名<br>期限（予定完了日）<br>タスクステータス<br></td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ドキュメントのアップロードリクエストを受信後、リクエストがキャンセルされました</strong> </p> <p>ドキュメントリクエストがキャンセルされると、ドキュメントのリクエスト先はメール通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; ドキュメントリクエストがキャンセルされました。 </em></p> <p>メール通知の本文には、次のテキストが含まれます。</p> <p><em>[!UICONTROL Hi] &lt;名前&gt;、<br><br>&lt;リクエストをキャンセルしたユーザーの名前&gt;[!UICONTROL no longer needs you to upload anything regarding the request you got earlier. We just wanted to let you know.]</em> </p> </td> 
   <td>リクエストをキャンセルしたユーザーの名前<br>元のドキュメントのアップロードリクエストのテキスト<br>元のドキュメントリクエストに対する「[!UICONTROL CANCELED]」バナー<br>元のドキュメントリクエストの日時<br></td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が確認すべきエラーが見つかりました</strong> </p> <p>メールでコメントに返信するユーザーは、返信が配信されなかった場合にメール通知を受け取ります。</p> <p>即時通知メールの件名は次のとおりです：<em>[!UICONTROL Failed to Process on] &lt;元のメッセージの件名&gt;</em></p> <p>電子メールを使用してコメントに返信する方法について詳しくは、 <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">電子メール通知に返信</a>.</p> </td>
   <td> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>イシューの割り当て変更により、自分のユーザー 1 人に影響があります</strong> </p> <p>イシューに割り当てられたユーザーのマネージャーは、そのユーザーがイシューから削除されたり、イシューに割り当てられたりすると、メール通知を受け取ります。 </p> <p>通知は、プロジェクトのステータスが「現在」または「計画」の場合にのみ送信されます。</p> <p>即時通知メールの件名は次のとおりです。<em>イシューの割り当て：&lt;イシュー名&gt;</em></p> </td> 
   <td> <p>イシュー名<br>プロジェクト名<br>イシューの参照番号<br>割り当てを行ったユーザーの名前<br>イシューのタイプ<br>イシューに割り当てられたユーザーの名前<br>入力されたイシューの日付<br>イシューの優先度<br>プライマリ連絡先<br>イシュー [!UICONTROL Planned Completion Date]<br>イシューステータス<br><strong>[!UICONTROL See More Details]</strong> ボタン</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分のユーザー 1 名がプロジェクトに追加されました</strong> </p> <p>マネージャーは、ユーザーの 1 人がプロジェクトに追加されると、メール通知を受け取ります。この通知は、プロジェクトのステータスに関係なく送信されます。 </p> <p>[!UICONTROL Review] ライセンスを持つユーザーには通知が送信されません。</p> <p>メールの件名は次のとおりです。<em>プロジェクトの割り当て：&lt;ユーザー名&gt;[&lt;プロジェクト GUID&gt;_ &lt;ユーザー GUID&gt;]</em></p> </td> 
   <td> <p>プロジェクト名<br>ポートフォリオ名<br>プロジェクト参照番号<br>プロジェクトに人物を追加したユーザーの名前<br>プロジェクトに追加されたユーザーの名前<br>プロジェクト [!UICONTROL Planned Start Date]<br>プロジェクト [!UICONTROL Planned Completion Date]<br>プロジェクトの完了率<br>プロジェクト上の他のユーザーの名前<br>プロジェクトのステータス<br>プロジェクト所有者<br><strong>[!UICONTROL See More Details]</strong> ボタン<br><br><br></p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が所有するポートフォリオまたはプログラムに誰かがプロジェクトを追加しました</strong> </p> <p>ポートフォリオまたはプログラムに新しいプロジェクトが追加されると、ポートフォリオおよび／またはプログラム所有者に通知が届きます。</p> <p>即時通知メールの件名は次のとおりです。<em>[!UICONTROL Project added to] &lt;ポートフォリオ名&gt;[プロジェクト GUID]</em></p> </td> 
   <td> ポートフォリオ名<br>プロジェクト参照番号<br>ポートフォリオ／プログラムにプロジェクトを追加したユーザーの名前<br><br></td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが自分とオブジェクトを共有しています</strong> </p> <p>オブジェクトに対する権限の [!UICONTROL Sharing] リストにユーザーが追加されると、メール通知が送信されます。</p> <p>インスタント通知メールの件名は次のとおりです。<em>[!UICONTROL Access Granted]：&lt;Object Name&gt;</em></p> <p>通知は、プロジェクトのステータスが [!UICONTROL Current] の場合にのみ送信されます。</p> </td> 
   <td> オブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>オブジェクトへの元のアクセス<br>オブジェクトに付与された新しいアクセス<br>アクセスが付与された日時 <br>アクセス権を付与したユーザーの名前 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが自分のチームとオブジェクトを共有しています</strong> </p> <p>オブジェクトに対する権限の共有リストに誰かがチームを追加すると、メール通知が送信されます。</p> <p>インスタント通知メールの件名は次のとおりです。<em>[!UICONTROL Access Granted]: &lt;Object Name&gt; [アクセスルール GUID]</em></p> </td> 
   <td> オブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>古いアクセス<br>新しいアクセス<br>アクセスが付与された日時<br>チームの名前<br>アクセス権を付与したユーザーの名前 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>登録しているタスク、イシュー、またはプロジェクトが更新されました</strong> </p> <p>登録している項目に対して誰かがコメントをすると、メール通知が届きます。</p> <p>サブスクリプションメールの件名は次のとおりです。<em>[!UICONTROL An update was made to the] &lt;Object Type&gt; 登録しているユーザー：&lt;Object Name&gt;</em></p> </td> 
   <td> オブジェクト名<br> オブジェクト参照番号<br> 登録項目に対してコメントを行ったユーザーの名前<br> コメントが行われた日付<br> 登録項目に追加されたコメント </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
 </tbody> 
</table>
