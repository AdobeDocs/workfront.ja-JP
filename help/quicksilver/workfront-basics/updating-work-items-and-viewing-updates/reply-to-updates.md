---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新に返信する
description: 作業オブジェクトの更新に対して、誰かが追加または返信すると、その返信がそのオブジェクトの「更新」セクションの通信スレッドに表示されます。オブジェクトに対する表示アクセス権を持っている場合は、更新に返信を追加したり、「いいね！」をクリックしたりできます。
author: Nolan and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: 7ef4d6c852328ff30e8b8c21398100f2f73e0dea
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 72%

---

# 更新に返信する

<!-- Audited: April 2024-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span> 
-->

作業オブジェクトに関するコメントまたはシステム更新に対してユーザーが返信すると、その返信が通信スレッドのオブジェクトの「コメント」セクションと「すべての」タブに表示されます。

>[!IMPORTANT]
>
>「システムアクティビティ」タブでシステムの更新に返信することはできません。 2024 年 4 月 11 日（PT）より前の従来のコメントエクスペリエンスで行われたシステム更新への返信は、読み取り専用として表示されます。

この記事では、Workfront内のほとんどのオブジェクトからのコメントに返信する方法を説明します。 様々なオブジェクトの更新セクションの違いについては、[ 更新セクションの概要 ](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>新規：イシューとドキュメントにはコントリビューター以上、その他のすべてのオブジェクトにはライト以上</p> 
   <p>現在：イシューとドキュメントについてはリクエスト以上、その他のすべてのオブジェクトについてはレビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>更新先のオブジェクトに対する表示または編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>オブジェクトに対する表示アクセス権</p> </td> 
  </tr> 
 </tbody> 
</table>

*ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront での更新または返信に対する返信

表示できるオブジェクトのスレッド内のコメントに返信したり、Workfront 管理者またはグループ管理者としてログインし、別のユーザーの代わりにコメントに返信したりできます。詳しくは、[別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)を参照してください。

### コメントに返信する

オブジェクトの「更新」セクションのコメントへの返信は、Workfrontのほとんどのオブジェクトで同様です。

1. 返信を追加するオブジェクトに移動します。
1. 「**更新**」、オブジェクトの「**コメント**」タブの順にクリックし、返信するコメントまたは返信を探します。

   または

   [**すべて**] タブをクリックし、[**コメントで返信**] をクリックして、[ コメント ] タブでコメントを開き、返信します。 「すべて」タブでは返信できません。

1. （オプション）以前の更新のテキストを返信に含めるには、返信したいコメントの右上隅にある&#x200B;**その他**&#x200B;メニューをクリックしたあと、「**引用返信**」をクリックします。以前の更新のテキストが入力エリアに表示され、灰色の縦線が付きます。
1. 「**返信**」をクリックします。

   ![ 「返信して更新」空のボックス ](assets/reply-to-update-empty-box.png)

   会話に積極的に参加しているユーザーが「**返信を追加...**」ボックスの下部に表示されます。さらに追加したり、関係なくなったものを削除したりできます。これらのユーザー、およびオブジェクトを購読しているユーザーは、オブジェクトに対して更新や返信が行われるたびに通知を受け取ります。さらに多くのユーザーをタグ付けして、返信に含めることもできます。さらに多くのユーザーをタグ付けするには、[更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。

   >[!TIP]
   >
   >   既存の返信にさらに返信を追加するには、「**返信を追加...**」ボックスに入力していくか、元のコメントで「**返信**」をクリックします。返信はスレッドの最後に追加されます。

1. 返信の入力を開始し、リッチテキストツールバーの追加のオプションを使用します。リッチテキストなどの更新機能の使用について詳しくは、[作業を更新](../updating-work-items-and-viewing-updates/update-work.md)を参照してください。

1. 「**送信**」をクリックして返信を保存します。

1. （オプション）返信を管理するその他のオプションについては、返信するコメントの右上隅にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックします。 詳しくは、[作業の更新](../updating-work-items-and-viewing-updates/update-work.md)を参照してください。

<!--
### Reply to an update or reply in the legacy Updates section

1. Go to the object to which you want to add a reply.
1. On the **Updates** tab for the object, find the update or reply to which you want to reply.

1. (Optional) To view an image in the existing update do one of the following:

   * Click the **Preview** icon ![](assets/previewimageicon-31x31.png) on the image thumbnail to open the full-size image in a new browser tab.
   * Click the **Download** icon ![](assets/downloadimageicon.png) on the image thumbnail to download the image.

1. Click **Reply** on the update, then type a reply in the box that appears.

   You can see the users who are actively engaged in the conversation or tagged in each reply at the top of that update thread. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object. You can also tag more users to include them in your reply.  To tag more users, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)
   
1. (Optional) To include text from a previous update in your reply, click the **More** menu next to the update or reply you want to quote, then click **Quote Reply**. Text from the previous update appears in the input area, marked with a vertical gray line.
1. (Optional) Use formatting, emojis, include links, or images as explained in the section "Use Rich Text in a Workfront update" in the article [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Click **Reply** to save the reply.

-->

## メール通知から更新に返信

メール通知の設定によっては、アクセス権のある特定のオブジェクトに対して更新が行われた際にメール通知を受信する場合があります。

メール通知から更新に返信する方法は次のとおりです。

* 受信したメールに返信します。返信メールは、元のコメントに対する Workfront の返信として追加されます。
* メール内の「コメント」ボタンを使用して、Workfront に戻り、アップデートエリアの更新に返信します。

以下は、タスクの「更新」タブでの更新の結果としてトリガーされるメール通知の例です。

![email.png](assets/email-350x202.png)

詳しくは、[メール通知に返信](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md)を参照してください。






