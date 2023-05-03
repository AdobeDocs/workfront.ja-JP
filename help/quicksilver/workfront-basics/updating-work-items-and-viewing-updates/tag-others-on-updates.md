---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新時の他のユーザーへのタグ付け
description: Adobe Workfrontオブジェクトに更新コメントを付けると、プロジェクトのすべてのユーザーが、送信された情報を表示できます。 ただし、プロジェクトに参加していないユーザーがこの情報を表示する方がメリットが得られる場合があります。 これらのユーザーをプロジェクトに含める代わりに、更新時にタグ付けして、ユーザーと共有できます。 タグ付きユーザーは、イベント通知を受け取ります。
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 25625291f691f7858634d9961fccb4465008dc3c
workflow-type: tm+mt
source-wordcount: '1413'
ht-degree: 0%

---

# 更新時の他のユーザーへのタグ付け

<!--take "Beta" references out when we remove the beta-->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.-->

>[!NOTE]
>
>現在、Adobe Workfrontでのコメント作成エクスペリエンスの再設計中です。
>
>新しいコメントエクスペリエンスについて詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>次のオブジェクトの新しいエクスペリエンスにアクセスできます。
> * コメントベータ版を有効にする際の問題。
   >
   >     この機能は、問題の「更新」セクションでのみ使用でき、次の領域では使用できません。
   >
   >     * ホーム
   >     * リストの概要パネル
   >     * タイムシートの概要パネル
>
> * 目標

   >
   >   新しいコメントエクスペリエンスが目標のデフォルトです。 Workfront Goals にアクセスするには、追加のライセンスが必要です。 詳しくは、 [Workfront目標の使用要件](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    目標のコメントについて詳しくは、 [Adobe Workfront目標で目標コメントを管理](../../workfront-goals/goal-management/manage-goal-comments.md).



ユーザーが従わない可能性のあるオブジェクトに注意を向けたい場合は、オブジェクトの更新時にユーザーにタグを付けることができます。
これらのユーザーを割り当てたり、サブスクライブしたりして、オブジェクトに含めるのではなく、更新時にタグ付けしてユーザーと共有することができます。 タグ付きユーザーは、入力した更新に関する通知を受け取ります。

>[!NOTE]
>
>ユーザーが電子メール通知を受け取るには、プロファイルで個人通知を有効にする必要があります。 詳しくは、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

更新をWorkfrontオブジェクトに追加する方法について詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>イシューをプロジェクトまたはタスクに変換すると、更新内容は新しいプロジェクトまたはタスクにコピーされますが、タグ付けされたユーザーはコピーされません。 会話を続けるには、参加者に再度タグを付ける必要があります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>問題およびドキュメントの要求以上その他のすべてのオブジェクトを確認するか、それ以上の値を設定します</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>問題およびドキュメントの要求者以上他のすべてのオブジェクトのレビュー担当者以上</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>オブジェクトへのアクセスの表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 更新時の他のユーザーへのタグ付け

更新で他のユーザーにタグ付けする方法は、選択したエクスペリエンスとオブジェクトに応じて異なります。

### 現在の更新セクションの更新に関する他のユーザーへのタグ付け

1. 作業項目の更新を開始します。詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 内 **通知** フィールドに、含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   または

   @記号を **新しい更新を開始** 「 」領域で、更新に含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   >[!TIP]
   >
   >類似または同一の名前を持つユーザーがいる場合に正しいユーザーを識別するには、アバター、ユーザーのプライマリの役割、またはその電子メールアドレスに注目します。 更新でタグ付けしたユーザーを表示するには、少なくとも 1 つのジョブの役割に関連付ける必要があります。

   ![](assets/tag-users-in-update.png)

1. （オプション）更新を非公開にするには、 **私の会社に対してプライベート** をクリックします。 これにより、会社のユーザーだけが更新を表示できるようになります。 この **私の会社に対してプライベート** オプションは、会社がWorkfrontプロファイルで指定されている場合にのみ使用できます。

   >[!NOTE]
   >
   >会社外のタグ付きユーザーは、「更新」タブに非公開コメントが表示されなくても、アプリ内通知や電子メールを引き続き受け取ることができます。 情報を共有したくない場合は、更新時に外部ユーザーにタグ付けしないことをお勧めします。

1. （オプション）複数のユーザーおよびチームを追加するには、手順 2 を繰り返します。

   >[!NOTE]
   >
   >「通知」フィールドに一覧表示されるすべてのユーザーとチームメンバーは、更新のアプリ内通知を受け取り、電子メール通知の設定に応じて電子メールを受け取る場合があります。 コメントまたは返信でタグ付けしたユーザーは、そのコメントまたは返信に関する通知を受け取り、スレッドの残りの部分の「通知」フィールドに名前を表示できますが、タグ付けし直さない限り、別の通知を受け取りません。 詳しくは、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) および [システムの全員に対するイベント通知を設定する](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. クリック **更新**.\
   更新に含まれるユーザーには、オブジェクトに対する表示権限が自動的に付与され、オブジェクトに対する更新の表示と応答が可能になります。

   更新スレッドの上部で、各返信でタグ付けされたユーザーを確認できます。 これらのユーザーは、オブジェクトを購読しているユーザーと共に、オブジェクトに対して更新または返信がおこなわれるたびに通知を受け取ります。

   ![](assets/tagging-transparency-350x192.png)

   作業項目の更新時に使用できる追加機能について詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### コメントベータ版エクスペリエンスの更新に関する他のユーザーへのタグ付け

コメントベータ版のエクスペリエンスで、更新時に他のユーザーにタグ付けすることができます。 また、コメントの編集時に誤ってタグ付けされたユーザーを削除することもできます。

1. 作業項目の更新を開始します。詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 内 **担当者またはチームのタグ付け** フィールドに、含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   または

   @記号を **コメントを書く** 「 」領域で、更新に含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   >[!TIP]
   >
   >類似または同一の名前を持つユーザーがいる場合に正しいユーザーを識別するには、アバター、ユーザーのプライマリの役割、またはその電子メールアドレスに注目します。 更新でタグ付けしたユーザーを表示するには、少なくとも 1 つのジョブの役割に関連付ける必要があります。

   ![](assets/tag-others-unified-commenting.png)

1. （オプション）更新を非公開にするには、 **私の会社に対してプライベート** をクリックします。 これにより、会社のユーザーだけが更新を表示できるようになります。 この **私の会社に対してプライベート** オプションは、会社がWorkfrontプロファイルで指定されている場合にのみ使用できます。

   >[!NOTE]
   >
   >* このオプションは、ユーザーが会社に関連付けられている場合にのみ表示されます。
   >* 会社外のタグ付きユーザーは、「更新」タブに非公開コメントが表示されなくても、アプリ内通知や電子メールを引き続き受け取ることができます。 情報を共有したくない場合は、更新時に外部ユーザーにタグ付けしないことをお勧めします。


1. （オプション）複数のユーザーおよびチームを追加するには、手順 2 を繰り返します。 <!--insure this stays accurate-->

   >[!NOTE]
   >
   >「ユーザーまたはチームのタグ付け」フィールドに一覧表示されるすべてのユーザーおよびチームメンバーは、更新のアプリ内通知を受け取り、電子メール通知設定に応じて電子メールを受け取る場合があります。 コメントまたは返信で自分にタグを付けたユーザーは、そのコメントまたは返信に関する通知を受け取り、スレッドの残りの部分でスレッドのメンバーとして一覧表示できますが、タグを付け直さない限り、別の通知を受け取りません。 詳しくは、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) および [システムの全員に対するイベント通知を設定する](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. クリック **送信**.\
   更新に含まれるユーザーには、オブジェクトに対する表示権限が自動的に付与され、オブジェクトに対する更新の表示と応答が可能になります。

   「メンバー」領域で、更新のテキストの下に、各返信でタグ付けされたユーザーを確認できます。 これらのユーザーは、オブジェクトを購読しているユーザーと共に、オブジェクトに対して更新または返信がおこなわれるたびに通知を受け取ります。
1. （オプション） **メンバー** を更新に含めて、入力した更新が共有されているエンティティのリストを表示します。

   ![](assets/members-icons-expanded-unshimmed.png)

   作業項目の更新時に使用できる追加機能について詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. （オプション） **詳細** メニュー ![](assets/more-menu.png) 「いいね！」アイコンの右側にあるをクリックし、 **編集**. タグ付きユーザーを削除し、「 **送信**. コメントは、入力後 15 分以内に編集できます。 編集できるのは、自分が追加したコメントだけです。