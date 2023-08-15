---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新に返信する
description: 作業オブジェクトの更新に対して、誰かが追加または返信すると、その返信がそのオブジェクトの [ 更新 ] セクションの通信スレッドに表示されます。 オブジェクトに対するビューアクセス権を持っている場合は、更新に返信を追加したり、「いいね！」をクリックしたりできます。
author: Lisa and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: d93d42322d62ff5eb927ca13febcb763cbec3f13
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%

---

# 更新に返信する

<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<!--after August 17: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/enable-fast-release-process.html?lang=en ). </span>  
<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>-->

<!--replace the note below with this at August 17: 
>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>Depending on what environment and what objects you access the commenting experience from, you might see different functionality in the Updates section. 
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>The new commenting experience is available only for the Updates section, and it is not available for the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets

-->

>[!NOTE]
>
>現在、Adobe Workfrontでのコメント作成エクスペリエンスの再設計中です。
>
>新しいコメントエクスペリエンスについて詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>次のオブジェクトの新しいエクスペリエンスにアクセスできます。
> * イシュー、プロジェクト、タスク、およびドキュメント。
>
>     これは、コメント作成ベータ版のエクスペリエンスを有効にした場合に使用できます。
>
>     この機能は、「更新」セクションでのみ使用でき、次の領域では使用できません。
>
>     * ホーム
>     * リスト内の概要パネル
>     * タイムシートの [ 概要 ] パネル
>
> * 目標、ボード領域のカード
>
>   新しいコメントエクスペリエンスは、目標とカードの唯一のエクスペリエンスです。 Workfront Goals にアクセスするには、追加のライセンスが必要です。 詳しくは、 [Workfront目標の使用要件](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     カードの「コメント」セクションと「システムアクティビティ」セクションを有効にすると、「ボード」領域でカードの更新を追加し、表示することができます。 詳しくは、 [ボードへのアドホックカードの追加](../../agile/get-started-with-boards/add-card-to-board.md).


誰かが作業オブジェクトのコメントやシステムの更新に返信すると、その返信がそのオブジェクトの [ 更新 ] セクションの通信スレッドに表示されます。

>[!IMPORTANT]
>
>新しいコメントエクスペリエンスでは、システムの更新に返信できません。 詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>問題およびドキュメントに対して要求者以上、その他すべてのオブジェクトに対してレビュー担当者以上</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクトの権限</strong></td> 
   <td> <p>オブジェクトへのアクセスの表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## Workfrontでの更新または返信に対する返信

表示できるオブジェクトのスレッド内のコメントに返信したり、Workfrontまたはグループ管理者としてログインし、別のユーザーの代わりにコメントに返信したりできます。 詳しくは、 [別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

コメントまたは返信への返信は、選択したエクスペリエンスとオブジェクトに応じて異なります。

### 現在の更新セクションの更新または返信に返信します

1. 返信を追加するオブジェクトに移動します。
1. 次の日： **更新** タブで、返信先の更新または返信を探します。

1. （オプション）既存の更新で画像を表示するには、次のいずれかの操作をおこないます。

   * 次をクリック： **プレビュー** アイコン ![](assets/previewimageicon-31x31.png) 画像のサムネールで、フルサイズの画像を新しいブラウザータブで開きます。
   * 次をクリック： **ダウンロード** アイコン ![](assets/downloadimageicon.png) を画像のサムネールにドラッグして、画像をダウンロードします。

1. クリック **返信** 更新時に、表示されるボックスに返信を入力します。

   会話に積極的に関わっているユーザーや、各返信にタグ付けされているユーザーが、その更新スレッドの上部に表示されます。 これらのユーザーは、オブジェクトを購読しているユーザーと共に、オブジェクトに対して更新または返信がおこなわれるたびに通知を受け取ります。 さらに多くのユーザーにタグを付けて、返信に含めることもできます。  さらに多くのユーザーにタグを付けるには、 [更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. （オプション）返信に以前の更新のテキストを含めるには、 **その他** 見積もりを行う更新または返信の横のメニューから、 **見積もりの返信**. 前の更新のテキストが入力領域に表示され、縦の灰色の線が付きます。
1. （オプション）記事の「Workfrontの更新でのリッチテキストの使用」の節で説明されているように、書式、絵文字、リンク、画像を使用します。 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. クリック **返信** をクリックして返信を保存します。

### 新しいコメントエクスペリエンスを使用する際にコメントに返信

新しいコメント作成エクスペリエンスで使用可能な機能とオブジェクトについて詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. 返信を追加するオブジェクトに移動します。
1. クリック **更新**」、「 **コメント** タブをクリックし、返信先のコメントまたは返信を探します。
1. （オプション）返信に以前の更新のテキストを含めるには、 **その他** 見積もりを行う更新または返信の横のメニュー <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>-->を選択し、次に **見積もりの返信**. 前の更新のテキストが入力領域に表示され、縦の灰色の線が付きます。
1. クリック **返信**.

   会話に積極的に関与しているユーザーがの下部に表示されます。 **新しいコメント** 」ボックスに追加して、不要なものを追加したり、削除したりできます。 これらのユーザーは、オブジェクトを購読しているユーザーと共に、オブジェクトに対して更新または返信がおこなわれるたびに通知を受け取ります。 さらに多くのユーザーにタグを付けて、返信に含めることもできます。  さらに多くのユーザーにタグを付けるには、 [更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. 返信の入力を開始し、リッチテキストツールバーの追加のオプションを使用します。 リッチテキストなどの更新機能の使用について詳しくは、 [作業を更新](../updating-work-items-and-viewing-updates/update-work.md).

1. クリック **送信** をクリックして返信を保存します。

1. （オプション） **その他** メニュー ![](assets/more-menu.png) 更新の横 <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>--> 返信を管理するその他のオプションを参照してください。 詳しくは、 [作業を更新](../updating-work-items-and-viewing-updates/update-work.md).


## 電子メール通知から更新に返信

電子メール通知の設定によっては、アクセス権のある特定のオブジェクトに対して更新が行われた際に電子メール通知を受け取る場合があります。

電子メール通知から更新に返信する方法は次のとおりです。

* 受信した電子メールに返信します。 返信メールは、元のコメントに対するWorkfrontの返信として追加されます。
* E メール内の「コメント」ボタンを使用して、Workfrontに戻り、「更新」領域の更新に返信します。

以下は、タスクの「更新」タブでの更新の結果としてトリガーされる電子メール通知の例です。

![email.png](assets/email-350x202.png)

詳しくは、 [電子メール通知に返信](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






