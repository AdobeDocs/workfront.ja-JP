---
content-type: reference
navigation-topic: notifications
title: '通知：通信'
description: 次の通知は、関係する作業項目に対する更新コメントなど、通信に関する警告を表示します。 受信する通知の設定については、「独自のイベント通知をアクティブ化または非アクティブ化する」を参照してください。
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: 2af2a1f7d1a4d0b06cf4e7bfd2b9997ff8b9a6bf
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 通知：通信

次の通知は、関係する作業項目に対する更新コメントなど、通信に関する警告を表示します。 受信する通知の設定については、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>これらの通知は、特定の項目に投稿されたすべてのコメントに関して警告します。 このため、毎日のダイジェスト電子メールで配信するには、すべての通知を同時に選択または選択解除する必要があります。 特定のコメントが発生したときにのみ通知を受け取る場合は、個々の通知を指定して即時配信を行うことができます。

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
   <td> <p><strong>自分が更新を受信する対象者として追加された</strong> </p> <p>有向更新とは、ユーザーが更新に別のユーザーを特別に含める場合です。詳しくは、 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL 他のユーザーに [!UICONTROL Tag on] アップデートをタグ付け</a>.</p> <p>この場合、有効な更新に含まれるユーザーは、更新に関する電子メール通知を受け取ります。</p> <p>電子メール通知は、ユーザーがオブジェクトに対するアクセス権を持っている場合にのみ送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL で知りたかった操作 ]</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。 <em>[!UICONTROL 通信のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 更新が行われたオブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>ダイレクト更新に含まれるすべてのユーザーおよびチームの名前<br>更新が行われた日時<br>直接更新のテキスト<br><strong>[!UICONTROL コメント ]</strong> ボタン<br>*受け取ったコメントの総数<br>*各オブジェクトに対して受け取ったコメント数<br>*<strong>[!UICONTROL すべての通知を表示 ]</strong> ボタン<br>*日別ダイジェストの日付<br></td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが自分の要求に返信した</strong> </p> <p>ユーザが作業要求を送信し、別のユーザが作業要求に返信した後、その要求を送信したユーザは電子メール通知を受け取る。</p> <p>次の場合、E メール通知は送信されません。</p> 
    <ul> 
     <li> <p>返信するユーザーは、要求を行ったユーザーと同じです</p> </li> 
     <li> <p>ユーザーはメモを表示するアクセス権を持っていません</p> </li> 
    </ul><strong>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL コメント先 ] &lt;request name=""&gt; オン &lt;project name=""&gt; ( 参照# &lt;request reference="" number=""&gt;)</em></strong> 日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 通信のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> リクエスト名<br>プロジェクト名<br>参照番号<br>リクエストに返信したユーザーの名前<br>コメントが行われた日時<br>リクエストに対して行われたコメントのテキスト<br>*受け取ったコメントの総数<br>*リクエストごとに受け取ったコメント数<br>*<strong>[!UICONTROL すべての通知を表示 ]</strong> ボタン<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分の要求に対するコメントが投稿されました</strong> </p> <p>コメントを投稿したユーザーが問題の主要連絡先でもある場合を除き、問題の主要連絡先は、[!UICONTROL ヘルプデスク ] リクエストにコメントが投稿されたときに電子メール通知を受け取ります。</p> <p>コメントに直接含まれるユーザーにも電子メール通知が送信されます。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL コメント先 ] &lt;request name=""&gt; オン &lt;project name=""&gt; ( 参照# &lt;request reference="" number=""&gt;)</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 通信のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> リクエスト名<br>プロジェクト名<br>参照番号<br>リクエストに返信したユーザーの名前<br>コメントが行われた日時<br>リクエストに対して行われたコメントのテキスト<br>*受け取ったコメントの総数<br>*リクエストごとに受け取ったコメント数<br>*プロジェクト名<br>*<strong>[!UICONTROL すべての通知を表示 ]</strong> ボタン<br>*日別ダイジェストの日付<br></td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分のドキュメントにコメントが追加されました</strong> </p> <p>内のドキュメントの所有者 [!DNL Adobe Workfront] コメントを投稿したユーザーがドキュメント所有者でもない限り、ドキュメントにコメントが投稿されると電子メール通知を受け取ります。</p> <p>コメントに直接含まれるユーザーにも電子メール通知が送信されます。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。 </p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL コメント先 ] &lt;request name=""&gt; オン &lt;project name=""&gt; ( 参照# &lt;request reference="" number=""&gt;)</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 通信のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>ドキュメント名<br>プロジェクト名、タスク名またはタスク名<br>参照番号<br>リクエストに返信したユーザーの名前<br>コメントが行われた日時<br>ドキュメントに対するコメントのテキスト</td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加中のスレッドに対して誰かがコメントした</strong> </p> <p>スレッドの参加者と、ダイレクトメッセージに含まれるユーザーは、ユーザーがスレッドにコメントを入れると電子メール通知を受け取ります。</p> <p>ユーザーが通知を受け取るには、[!UICONTROL 表示 ] へのアクセス権が必要です。</p> <p>次のユーザーは通知を受け取りません。</p> 
    <ul> 
     <li>ダイレクトメッセージに含まれるチーム</li> 
     <li>メモの所有者</li> 
     <li>プライマリ連絡先</li> 
    </ul> <p><strong>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL RE:コメント ] &lt;object name=""&gt;&lt;object type=""&gt; オン &lt;project name=""&gt;( 参照# &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> 日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 通信のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> オブジェクト名<br>親オブジェクト名<br>スレッドにコメントしたユーザーの名前<br>スレッド上で行われたコメントのテキスト<br>コメントが行われた日時<br>*受け取ったコメントの総数<br>*各オブジェクトに対して受け取ったコメント数<br>*プロジェクト名<br>*<strong>[!UICONTROL すべての通知を表示 ]</strong> ボタン<br>*1 日のダイジェストの日付 </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが自分の作業アイテムのいずれかに対してコメントした</strong> </p> <p>作業項目の担当者は、更新を追加したユーザーが担当者でもない限り、ユーザーが作業項目に更新を追加するたびに電子メール通知を受け取ります。 </p> <p>リクエストにコメントが投稿されたら、問題の主要連絡先に電子メールを送信します。</p> <p>コメントを投稿したユーザーがイシューの主要連絡先でもある場合を除き、イシューの主要連絡先は、リクエストに対してコメントが投稿されると電子メール通知を受け取ります。</p> <p>コメントに直接含まれるユーザーにも電子メール通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL コメント先 ] &lt;work item="" name=""&gt; オン &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 通信のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 作業項目名<br>プロジェクト名<br>作業項目の参照番号<br>作業項目にコメントしたユーザーの名前<br>作業項目に対して行われたコメントのテキスト<br>コメントが行われた日時<br>*受け取ったコメントの総数<br>*各オブジェクトに対して受け取ったコメント数<br>*プロジェクト名<br>*<strong>[!UICONTROL すべての通知を表示 ]</strong> ボタン<br>*1 日のダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分チームが更新を受信する対象として追加された</strong> </p> <p>有向更新とは、ユーザーが更新に別のユーザーを特別に含める場合です。詳しくは、 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">更新時の他のユーザーへのタグ付け</a>.</p> <p>この場合、ダイレクト更新に含まれるチームのメンバーは、更新に関する電子メール通知を受け取ります。</p> <p>電子メール通知は、オブジェクトへのアクセス権を持つユーザーにのみ送信されます。</p> <p>有向更新を送信するユーザーが、含まれるチームのメンバーである場合、更新を送信するユーザーは電子メール通知を受け取りません。</p> <p>即時通知 E メールの件名は次のとおりです。[!UICONTROL コメント先 ] &lt;object name=""&gt; オン &lt;parent object="" name=""&gt; ( 参照# &lt;object reference="" number=""&gt;)</p> <p> 日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 通信のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>オブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>ダイレクト更新を行ったユーザーの名前<br>ダイレクト更新に含まれるすべてのチームおよびユーザーの名前<br>ダイレクト更新がおこなわれた日時<br>ダイレクト更新のテキスト<br><strong>[!UICONTROL コメント ]</strong> ボタン<br>*受け取ったコメントの総数<br>*各オブジェクトに対して受け取ったコメント数<br>*プロジェクト名<br>*<strong>[!UICONTROL すべての通知を表示 ]</strong> ボタン<br>*1 日のダイジェストの日付 </p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ユーザーに関するコメントが追加されたとき</strong> </p> <p>ユーザーオブジェクトの「[!UICONTROL 更新 ]」タブで、ユーザーにコメントを追加できます。 また、ユーザーの設定の編集中に、ユーザーにコメントを付けることもできます。 コメントを作成したユーザーには、このコメントを通知する電子メールが送信されます。 </p> <p>ユーザーの [!UICONTROL 更新 ] タブで更新を入力するには、少なくともユーザーの [!UICONTROL 表示 ] 権限が必要です。 ユーザーの設定を編集するには、ユーザーの [!UICONTROL 編集 ] 権限が必要です。 </p> <p>「更新」タブでユーザーにコメントを付ける方法について詳しくは、 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業を更新</a>.</p> <p>ユーザーの設定を編集する際にユーザーにコメントを入力する方法について詳しくは、 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">設定を行う</a>.</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;user name=""&gt; [!UICONTROL で知りたかった操作 ]</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 通信のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> ユーザー名<br>コメントを追加したユーザーの名前<br>コメントのテキスト<br>コメントが行われた日時<br>*受け取ったコメントの総数<br>*各オブジェクトに対して受け取ったコメント数<br>*<strong>[!UICONTROL すべての通知を表示 ]</strong> ボタン<br>*1 日のダイジェストの日付 </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日別</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
