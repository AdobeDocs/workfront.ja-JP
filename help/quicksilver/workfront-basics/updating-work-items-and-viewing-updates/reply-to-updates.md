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
source-git-commit: ee957e319941fe5eabb9144eed184372e5402197
workflow-type: tm+mt
source-wordcount: '1190'
ht-degree: 90%

---

# 更新に返信する

<!--remove legacy and new experience references when we remove the legacy updates in the UI - Jan 2024???-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 

-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのユーザーの場合はプレビュー環境で、迅速なリリースを有効にしているユーザーの場合は実稼動環境でのみ使用できます。 </span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview">現在のリリーススケジュールについて詳しくは、[2024年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md)を参照してください。</span>

>[!IMPORTANT]
>
>現在アドビでは、Adobe Workfront のコメントエクスペリエンスを再設計しているところです。
>
>コメントエクスペリエンスにアクセスする目的のオブジェクトに応じて、「更新」セクションに次の機能が表示される場合があります。
>* 新しいエクスペリエンス
>* 従来のエクスペリエンス
>* 新しいエクスペリエンスと従来のエクスペリエンス
>
>新しいコメントエクスペリエンスとその可用性について詳しくは、[新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md)を参照してください。
>
><Span class="preview"> プレビュー環境で、従来のコメント機能がプロジェクト、タスク、イシュー、ドキュメントから削除されました。 </span>
>
>新しいコメントエクスペリエンスは、Workfront オブジェクトの「更新」セクションでのみ使用できます。次のエリアから更新にアクセスする場合は使用できません。
>
> * ホーム
> * リストの概要パネル
> * タイムシートの概要パネル
> * ワークロードバランサーの概要パネル
>
><span class="preview">迅速なリリースプロセスを選択した顧客の場合、プレビュー環境のリスト、タイムシート、ワークロードバランサーの概要パネルと実稼動環境に新しいコメントエクスペリエンスが表示されます。 </span>

誰かが作業オブジェクトのコメントやシステムの更新に返信すると、その返信がそのオブジェクトの「更新」セクションの通信スレッドに表示されます。

>[!IMPORTANT]
>
>新しいコメントエクスペリエンスでは、システム更新に返信できません。詳しくは、[新しいコメント機能エクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md)を参照してください。

<!--adjust the sentence before the second IMPORTANT and remove this important note when we remove legacy from the system-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront ライセンス*</strong></td> 
   <td> <p>イシューとドキュメントについてはリクエスト以上、その他のすべてのオブジェクトについてはレビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>イシューおよびドキュメントに対して要求者以上、その他すべてのオブジェクトに対してレビュアー以上</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>オブジェクトに対する表示アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;自分のプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## Workfront での更新または返信に対する返信

表示できるオブジェクトのスレッド内のコメントに返信したり、Workfront 管理者またはグループ管理者としてログインし、別のユーザーの代わりにコメントに返信したりできます。詳しくは、[別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)を参照してください。

コメントまたは返信への返信は、選択したエクスペリエンスとオブジェクトに応じて異なります。

### 新しいコメントエクスペリエンスを使用する際のコメントへの返信

新しいコメントエクスペリエンスで使用できる機能とオブジェクトについて詳しくは、[新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md)を参照してください。

1. 返信を追加するオブジェクトに移動します。
1. クリック **更新**&#x200B;を選択し、 **コメント** オブジェクトの Tab キーを押して、返信先のコメントまたは返信を検索します

   または

   <span class="preview">「」をクリックします **すべて** tab キーを押してから、 **コメントで返信** 「コメント」タブでコメントを開いて返信します。 「すべて」タブでは返信できません。</span>

1. （オプション）以前の更新のテキストを返信に含めるには、返信するコメントの右上隅にある&#x200B;**その他**&#x200B;メニューをクリックし、「**引用返信**」をクリックします。以前の更新のテキストが入力エリアに表示され、灰色の縦線が付きます。
1. 「**返信**」をクリックします。

   ![](assets/reply-to-update-empty-box.png)

   会話に積極的に参加しているユーザーが「**返信を追加...**」ボックスの下部に表示されます。さらにユーザーを追加したり、関係なくなったユーザーを削除したりできます。これらのユーザー、およびオブジェクトを購読しているユーザーは、オブジェクトに対して更新や返信が行われるたびに通知を受け取ります。さらに多くのユーザーをタグ付けして、返信に含めることもできます。さらに多くのユーザーをタグ付けするには、[更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。

   >[!TIP]
   >
   >   既存の返信にさらに返信を追加するには、「**返信を追加...**」ボックスに入力するか、元のコメントで「**返信**」をクリックします。返信はスレッドの最後に追加されます。

1. 返信の入力を開始し、リッチテキストツールバーの追加のオプションを使用します。リッチテキストなどの更新機能の使用について詳しくは、[作業を更新](../updating-work-items-and-viewing-updates/update-work.md)を参照してください。

1. 「**送信**」をクリックして返信を保存します。

1. （オプション）返信するコメントの右上隅にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックすると、返信を管理するオプションがさらに表示されます。詳しくは、[作業の更新](../updating-work-items-and-viewing-updates/update-work.md)を参照してください。

### 従来の「更新」セクションでの更新または返信に対する返信

1. 返信を追加するオブジェクトに移動します。
1. オブジェクトの「**更新**」タブで、返信する更新または返信を探します。

1. （オプション）既存の更新で画像を表示するには、次のいずれかの操作を実行します。

   * 画像のサムネールで&#x200B;**プレビュー**&#x200B;アイコン ![](assets/previewimageicon-31x31.png) をクリックして、フルサイズの画像を新しいブラウザータブで開きます。
   * 画像のサムネールで&#x200B;**ダウンロード**&#x200B;アイコン ![](assets/downloadimageicon.png) をクリックして、画像をダウンロードします。

1. 更新で「**返信**」をクリックして、表示されるボックスに返信を入力します。

   会話に積極的に参加しているユーザーや各返信にタグ付けされているユーザーが、その更新スレッドの上部に表示されます。これらのユーザー、およびオブジェクトを購読しているユーザーは、オブジェクトに対して更新や返信が行われるたびに通知を受け取ります。さらに多くのユーザーをタグ付けして、返信に含めることもできます。さらに多くのユーザーをタグ付けするには、[更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。

   ![](assets/tagging-transparency-350x192.png)

1. （オプション）返信に以前の更新のテキストを含めるには、引用を行う更新または返信の横にある&#x200B;**その他**&#x200B;メニュー、「**引用返信**」の順にクリックします。以前の更新のテキストが入力エリアに表示され、灰色の縦線が付きます。
1. （オプション）[作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)記事内「Workfront の更新でのリッチテキストの使用」の節で説明されているように、リンクまたは画像を含む書式、絵文字を使用します。
1. 「**返信**」をクリックして、返信を保存します。

## メール通知から更新に返信

メール通知の設定によっては、アクセス権のある特定のオブジェクトに対して更新が行われた際にメール通知を受信する場合があります。

メール通知から更新に返信する方法は次のとおりです。

* 受信したメールに返信します。返信メールは、元のコメントに対する Workfront の返信として追加されます。
* メール内の「コメント」ボタンを使用して、Workfront に戻り、アップデートエリアの更新に返信します。

以下は、タスクの「更新」タブでの更新の結果としてトリガーされるメール通知の例です。

![email.png](assets/email-350x202.png)

詳しくは、[メール通知に返信](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md)を参照してください。






