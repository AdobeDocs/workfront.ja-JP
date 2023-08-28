---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新時の他のユーザーへのタグ付け
description: Adobe Workfrontオブジェクトに更新コメントを付けると、プロジェクトのすべてのユーザーが、送信された情報を表示できます。 ただし、プロジェクトに参加していないユーザーがこの情報を表示する方がメリットが得られる場合があります。 これらのユーザーをプロジェクトに含める代わりに、更新時にタグ付けして、ユーザーと共有できます。 タグ付きユーザーは、イベント通知を受け取ります。
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 0%

---

# 更新時の他のユーザーへのタグ付け

<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<!--take new commenting and legacy commenting out when we remove the legacy commenting and the new one is the only experience-->

<span class="preview">このページで強調表示されている情報は、まだ一般に利用できない機能を示しています。 この機能は、すべての顧客のプレビュー環境でのみ使用できます。 実稼動環境では、毎月のリリース以降、高速リリースを有効にしたお客様も同じ機能を実稼動環境で使用できます。 </span>\
<span class="preview">高速リリースについて詳しくは、 [組織の高速リリースを有効または無効にします](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>

<span class="preview">現在のリリーススケジュールについて詳しくは、 [2023 年第 4 四半期リリースの概要](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span>

>[!IMPORTANT]
>
>現在、Adobe Workfrontでのコメント作成エクスペリエンスの再設計中です。
>どの環境から、およびどのオブジェクトからコメントエクスペリエンスにアクセスしたかに応じて、「更新」セクションに異なる機能が表示される場合があります。
>
>新しいコメントエクスペリエンスとその可用性について詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>新しいコメントエクスペリエンスは、「更新」セクションでのみ使用でき、次の領域では使用できません。
>
> * ホーム
> * リスト内の概要パネル
> * タイムシートの [ 概要 ] パネル


<!--old note before August 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).

-->

ユーザーが従わない可能性のあるオブジェクトに注意を向けたい場合は、オブジェクトの更新時にユーザーにタグを付けることができます。
これらのユーザーを割り当てたり、サブスクライブしたりして、オブジェクトに含めるのではなく、更新時にタグ付けしてユーザーと共有することができます。 タグ付きユーザーは、入力した更新に関する通知を受け取ります。

>[!NOTE]
>
>ユーザーが電子メール通知を受け取るには、プロファイルで個人通知を有効にする必要があります。 詳しくは、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>

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
   <td> <p>問題およびドキュメントに対する要求以上、その他のすべてのオブジェクトに対する確認以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>問題およびドキュメントに対して要求者以上、その他すべてのオブジェクトに対してレビュー担当者以上</p> 
   <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクトの権限</strong></td> 
   <td> <p>オブジェクトへのアクセスの表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 更新時の他のユーザーへのタグ付け

更新で他のユーザーにタグ付けする方法は、選択したエクスペリエンスとオブジェクトに応じて異なります。

### 現在の更新セクションの更新に関する他のユーザーへのタグ付け

<!--change "current" to "legacy" at the October 26, 2023 release-->

現在の更新セクションでは、ユーザーに手動でタグ付けできます。

1. 作業項目の更新を開始します。詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Adobe Analytics の **通知** フィールドに、含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   または

   @記号を **新しい更新を開始** 「 」領域で、更新に含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   >[!TIP]
   >
   >類似または同一の名前を持つユーザーがいる場合に正しいユーザーを識別するには、アバター、ユーザーのプライマリの役割、またはその電子メールアドレスに注目します。
   >
   >更新でタグ付けしたユーザーを表示するには、少なくとも 1 つのジョブの役割に関連付ける必要があります。
   >
   >ユーザーがユーザーの電子メールを表示するには、アクセスレベルで [ 連絡先情報の表示 ] 設定を有効にしておく必要があります。 詳しくは、 [ユーザーへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. （オプション）更新を非公開にするには、 **私の会社に対してプライベート** をクリックします。 これにより、会社のユーザーだけが更新を表示できるようになります。 The **私の会社に対してプライベート** オプションは、会社がWorkfrontプロファイルで指定されている場合にのみ使用できます。

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

### 新しいコメントエクスペリエンスの更新時に他のユーザーにタグ付けする

新しいコメントエクスペリエンスでの更新に関して、他のユーザーにタグを付けるには、次の方法があります。

* **自動**：ユーザーがスレッドを開始したり、コメントを追加したり、返信を追加したりすると、自動的にタグ付けされ、コメントボックスの「ユーザーにタグ付け」領域または「チームに追加」領域に追加されます。 <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

  >[!TIP]
  >
  >従来のコメント作成エクスペリエンスでスレッドが開始した場合、スレッド参加者は自動的にタグ付けされません。

* **手動**：ユーザーを手動でコメントボックスの「ユーザーにタグを付ける」領域に追加する場合。

また、コメントを編集または返信する際に、誤ってタグ付けされたユーザーを削除することもできます。

1. 作業項目の更新を開始します。詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). コメントの所有者は、自動的にタグ付けされ、コメントボックスの「担当者またはチームにタグ付け」領域に追加されます。

   >[!TIP]
   >
   >コメントの所有者は、コメントボックスの「ユーザーまたはチームにタグ付け」領域で自分の名前を表示できません。

1. Adobe Analytics の **担当者またはチームのタグ付け** フィールドに、含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   または

   @記号を **コメントを書く** 「 」領域で、更新に含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   >[!TIP]
   > 
   >類似または同一の名前を持つユーザーがいる場合に正しいユーザーを識別するには、アバター、ユーザーのプライマリの役割、またはその電子メールアドレスに注目します。
   > 
   >更新でタグ付けしたユーザーを表示するには、少なくとも 1 つのジョブの役割に関連付ける必要があります。
   > 
   >ユーザーがユーザーの電子メールを表示するには、アクセスレベルで [ 連絡先情報の表示 ] 設定を有効にしておく必要があります。 詳しくは、 [ユーザーへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-others-unified-commenting.png)

1. （オプション）更新を非公開にするには、 **私の会社に対してプライベート** をクリックします。 これにより、会社のユーザーだけが更新を表示できるようになります。 The **私の会社に対してプライベート** オプションは、会社がWorkfrontプロファイルで指定されている場合にのみ使用できます。

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

   <span class="preview">タグ付きエンティティの名前は、アバターの横に、最大 2 つのエンティティまで表示されます。 3 つ以上のエンティティがタグ付けされている場合、最初のエンティティの名前が表示され、さらにタグ付けされたエンティティの数も表示されます。</span>

   ![](assets/members-icons-expanded-unshimmed.png)

   作業項目の更新時に使用できる追加機能について詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. （オプション） **その他** メニュー ![](assets/more-menu.png) <span class="preview">コメントの右上隅に</span>を選択し、次に **編集**. タグ付きユーザーを削除し、「 **送信**. コメントは、入力後 15 分以内に編集できます。 編集できるのは、自分が追加したコメントだけです。

   >[!TIP]
   >
   >従来のコメント作成機能を使用してコメントや返信を追加する場合、特にタグ付けされていないコメントの所有者は、新しいコメント作成機能を使用するユーザーによって手動で削除することはできません。



