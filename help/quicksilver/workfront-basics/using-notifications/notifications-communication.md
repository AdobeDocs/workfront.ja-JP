---
content-type: reference
navigation-topic: notifications
title: 「通知：コミュニケーション」
description: 以下の通知は、自分が関係する作業項目に対する更新コメントなど、コミュニケーションに関することを知らせるものです。受信する通知の設定について詳しくは、「独自の電子メール通知を変更する」を参照してください。
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 98%

---

# 通知：コミュニケーション

以下の通知は、自分が関係する作業項目に対する更新コメントなど、コミュニケーションに関することを知らせるものです。受信する通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>これらの通知は、特定の項目に投稿されたすべてのコメントに関することを知らせるものです。このため、日刊ダイジェストメールで配信するには、すべての通知を同時に選択または選択解除する必要があります。特定のコメントが発生したときにのみ通知を受け取りたい場合は、個々の通知を即時配信に指定することができます。

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
   <td> <p><strong>自分が更新を受信する対象者として追加された</strong> </p> <p>対象者として更新を受信するのは、<a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL Tag others on] 更新</a>で説明されているように、あるユーザーが更新に別のユーザーを明確に追加した場合です。</p> <p>この場合、更新を受信する対象者に追加されたユーザーは、更新に関するメール通知を受け取ります。</p> <p>このメール通知は、ユーザーがオブジェクトに対するアクセス権を持っている場合にのみ送信されます。</p> <p>即時通知メールの件名：<em>&lt;Name of the user who included you in the update&gt; [!UICONTROL wanted you to know]</em></p> <p>日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> 更新が行われたオブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>対象者指定更新に追加されたすべてのユーザーおよびチームの名前<br>更新が行われた日時<br>対象者指定更新のテキスト<br><strong>「[!UICONTROL Comment]」</strong>ボタン<br>*受け取ったコメントの総数<br>*オブジェクトごとの受け取ったコメント数<br>*「<strong>[!UICONTROL See All Notifications]</strong>」ボタン<br>*日刊ダイジェストの日付<br></td> 
   <td> <p><strong>即時</strong> </p> <p><strong>および日刊</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが自分の要求に返信した</strong> </p> <p>ユーザーが作業リクエストを送信し、別のユーザーが作業リクエストに返信すると、そのリクエストを送信したユーザーはメール通知を受け取ります。</p> <p>次の場合、メール通知は送信されません。</p> 
    <ul> 
     <li> <p>返信するユーザーがリクエストを出したユーザーと同じ</p> </li> 
     <li> <p>ユーザーにその内容を表示するアクセス権がない</p> </li> 
    </ul><strong>即時通知メールの件名：<em>[!UICONTROL Comment on] &lt;Project Name&gt; の &lt;Request Name&gt; (参照番号 &lt;Request Reference Number&gt;)</em></strong>日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></td> 
   <td> リクエスト名<br>プロジェクト名<br>参照番号<br>リクエストに返信したユーザーの名前<br>コメントが付けられた日時<br>リクエストに対して付けられたコメントのテキスト<br>*受け取ったコメントの総数<br>*リクエストごとの受け取ったコメントの数<br>*「<strong>[!UICONTROL See All Notifications]</strong>」ボタン<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分のリクエストに関するコメントが投稿されました</strong> </p> <p>コメントを投稿したユーザーがイシューのプライマリ連絡先でもある場合を除き、[!UICONTROL Help Desk] リクエストにコメントが投稿されると、イシューのプライマリ連絡先はメール通知を受け取ります。</p> <p>コメントに直接含まれるユーザーにもメール通知が送信されます。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。</p> <p>即時通知メールの件名：<em>[!UICONTROL Comment on] &lt;Project Name&gt; の &lt;Request Name&gt; (参照番号 &lt;Request Reference Number&gt;)</em></p> <p>日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> リクエスト名<br>プロジェクト名<br>参照番号<br>リクエストに返信したユーザーの名前<br>コメントが付けられた日時<br>リクエストに対して付けられたコメントのテキスト<br>*受け取ったコメントの総数<br>*リクエストごとの受け取ったコメントの数<br>*プロジェクト名<br>*「<strong>[!UICONTROL See All Notifications]</strong>」ボタン<br>*日刊ダイジェストの日付<br></td> 
   <td> <p><strong>即時</strong> </p> <p><strong>および日刊</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分のドキュメントにコメントが追加されました</strong> </p> <p>[!DNL Adobe Workfront] 内のドキュメントの所有者は、ドキュメントにコメントが投稿されると、コメントを投稿したユーザーがドキュメントの所有者である場合を除き、メール通知を受け取ります。</p> <p>コメントに直接含まれるユーザーにもメール通知が送信されます。</p> <p>プロジェクトのステータスが [!UICONTROL Current] の場合にのみ通知が送信されます。 </p> <p>即時通知メールの件名：<em>[!UICONTROL Comment on] &lt;Project Name&gt; の &lt;Request Name&gt; (参照番号 &lt;Request Reference Number&gt;)</em></p> <p> 日刊ダイジェスト通知の件名：<em>[!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td>ドキュメント名<br>プロジェクト名、タスク名またはイシュー名<br>参照番号<br>リクエストに返信したユーザーの名前<br>コメントが付けられた日時<br>ドキュメントに対して付けられたコメントのテキスト</td> 
   <td> <p><strong>即時</strong> </p> <p><strong>および日刊</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分が参加中のスレッドに対して誰かがコメントした</strong> </p> <p>スレッドの参加者と、ダイレクトメッセージに含まれるユーザーは、いずれかのユーザーがスレッドにコメントを作成すると電子メール通知を受け取ります。</p> <p>ユーザーが通知を受け取るには、[!UICONTROL View] アクセス権が必要です。</p> <p>次のユーザーは通知を受け取りません。</p> 
    <ul> 
     <li>ダイレクトメッセージに含まれるチーム</li> 
     <li>メモの所有者</li> 
     <li>プライマリ連絡先</li> 
    </ul> <p><strong>インスタント通知メールの件名は次のとおりです。<em>[!UICONTROL RE: Comment on] &lt;Object Name&gt;&lt;Object Type&gt; on &lt;Project Name&gt;(ref# &lt;Object Reference Number&gt;</em>)</strong> </p> <p><strong>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></strong> </p> </td> 
   <td> オブジェクト名<br>親オブジェクト名<br>スレッドにコメントしたユーザーの名前<br>スレッド上で作成されたコメントのテキスト<br>コメントが作成された日時<br>*受け取ったコメントの合計数<br>*オブジェクトごとの受け取ったコメント数<br>*プロジェクト名<br>*「<strong>[!UICONTROL See All Notifications]</strong>」ボタン<br>*日次ダイジェストの日付 </td> 
   <td><strong>[!UICONTROL Daily]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>誰かが自分の作業アイテムのいずれかに対してコメントした</strong> </p> <p>ユーザーが作業項目に更新を追加するたびに、作業項目の担当者はメール通知を受け取ります。ただし、更新を追加するユーザーが担当者でもある場合を除きます。 </p> <p>リクエストにコメントが投稿されたら、イシューのプライマリ連絡先に電子メールを送信します。</p> <p>リクエストにコメントが投稿されると、イシューのプライマリ連絡先はメール通知を受け取ります。ただし、コメントを投稿したユーザーがイシューのプライマリ連絡先でもある場合を除きます。</p> <p>コメントに直接含まれるユーザーにもメール通知が送信されます。</p> <p>インスタント通知メールの件名は次のとおりです。<em>[!UICONTROL Comment on] &lt;Work Item Name&gt; on &lt;Project Name (ref# &lt;Work Item Reference Number&gt;)</em></p> <p> 日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> 作業項目名<br>プロジェクト名<br>作業項目の参照番号<br>作業項目にコメントしたユーザーの名前<br>作業項目に対して作成されたコメントのテキスト<br>コメントが作成された日時<br>*受け取ったコメントの合計数<br>*オブジェクトごとの受け取ったコメント数<br>*プロジェクト名<br>*「<strong>[!UICONTROL See All Notifications]</strong>」ボタン<br>*日次ダイジェストの日付 </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分チームが更新を受信する対象として追加された</strong> </p> <p>対象指定更新とは、特定のユーザーが別のユーザーを特定して更新に含める場合です。詳しくは、<a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">更新時の他のユーザーへのタグ付け</a>を参照してください。</p> <p>この場合、対象指定更新に含まれるチームのメンバーが、更新に関するメール通知を受け取ります。</p> <p>メール通知は、オブジェクトへのアクセス権を持つユーザーにのみ送信されます。</p> <p>対象指定更新を送信するユーザーが、含まれるチームのメンバーである場合、更新を送信するユーザーはメール通知を受け取りません。</p> <p>インスタント通知メールの件名は次のとおりです。[!UICONTROL Comment on] &lt;Object name&gt; on &lt;Parent Object Name&gt; (ref# &lt;Object Reference Number&gt;)</p> <p> 日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>オブジェクト名<br>親オブジェクト名<br>オブジェクト参照番号<br>対象指定更新を行ったユーザーの名前<br>対象指定更新に含まれるすべてのチームおよびユーザーの名前<br>対象指定更新が行われた日時<br>対象指定更新のテキスト「<br><strong>[!UICONTROL Comment]</strong>」ボタン<br>*受け取ったコメントの合計数<br>*オブジェクトごとの受け取ったコメント数<br>*プロジェクト名<br>*「<strong>[!UICONTROL See All Notifications]</strong>」ボタン<br>*日次ダイジェストの日付 </p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ユーザーに関するコメントが追加されたとき</strong> </p> <p>ユーザーオブジェクトの「[!UICONTROL Updates]」タブで、ユーザーに対してコメントを作成できます。また、ユーザーの設定の編集中に、ユーザーに対してコメントを作成することもできます。コメントが作成されたユーザーは、このコメントを通知するメールを受け取ります。 </p> <p>ユーザーの「[!UICONTROL Updates]」タブで更新を入力するには、少なくともそのユーザーに対する [!UICONTROL View] 権限が必要です。ユーザーの設定を編集するには、そのユーザーに対する [!UICONTROL Edit] 権限が必要です。 </p> <p>「更新」タブでユーザーにコメントを付ける方法について詳しくは、<a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業を更新</a>を参照してください。</p> <p>ユーザーの設定を編集する際にユーザーにコメントを入力する方法について詳しくは、<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">環境設定</a>を参照してください。</p> <p>インスタント通知メールの件名は次のとおりです。<em>&lt;User Name&gt; [!UICONTROL wanted you to know]</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL Digest of Communication] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> ユーザー名<br>コメントを追加したユーザーの名前<br>コメントのテキスト<br>コメントが作成され日時<br>*受け取ったコメントの合計数<br>*オブジェクトごとの受け取ったコメント数<br>*「<strong>[!UICONTROL See All Notifications]</strong>」ボタン<br>*日次ダイジェストの日付 </td> 
   <td> <p><strong>今すぐ</strong> </p> <p><strong>および日次</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
