---
product-area: requests
navigation-topic: create-requests
title: ユーザーが問題をリクエストキュープロジェクトに電子メールで送信できるようにします
description: ユーザーが問題をリクエストキュープロジェクトに電子メールで送信できるようにします
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: ca3c28174dca24f14a75869bdc209569d8d8d1a0
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# ユーザーが問題をリクエストキュープロジェクトに電子メールで送信できるようにします

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

ユーザーが電子メールでプロジェクトにイシューを追加できるようにプロジェクトを設定できます。 プロジェクトがリクエストキューとして指定されている場合にのみ、プロジェクトにイシューを電子メールで送信できます。 リクエストキュープロジェクトの作成について詳しくは、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>問題へのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

ユーザーが電子メールでプロジェクトにイシューを追加できるようにプロジェクトを設定するには、次の前提条件が必要です。

この機能を有効にする前に、次の条件を満たす必要があります。

* このアカウントに問題を電子メールで送信するユーザーは、Workfrontのライセンスを持つアクティブユーザーである必要があります。
* 外部ユーザーは、イシューを作成するアクセス権を持たないので、リクエストキューにイシューを電子メールで送信できません。
* このアカウントに問題を電子メールで送信するユーザーは、プロジェクトに対して問題の追加権限が必要です。
* アクティブなWorkfrontユーザーに関連付けられた電子メールアドレスからの電子メールは、プロジェクトに問題を送信できる電子メールのみです。
* プロジェクトはリクエストキューとして設定されます。
* プロジェクトに関連付けられた電子メールアカウントは、Workfrontユーザーアカウントにリンクされていません。

## Workfrontでのプロジェクトの設定

>[!NOTE]
>
>電子メールキューの設定を有効にする際は、次の点に注意してください。
>
>* Workfrontでは、すべてのクラスターにわたるリクエストキューごとに 1 つの一意の e メールを使用できます。 リクエストキューを無効にする場合、作成したメールアドレスが「インテークメールアドレス」ボックスに残っている限り、そのメールアドレスが保持されます。 取り込みメールの使用を中止する場合は、今後使用できるよう、取り込みメールフィールドから削除する必要があります。
>
>* リクエストキューに複数のキュートピックまたはトピックグループが含まれる場合、Workfrontは電子メールで送信されたリクエストの送信先キュートピックをランダムに選択し、電子メールで送信されたリクエストを管理しにくくします。
   >電子メールを通じて要求を受け取るように設定したプロジェクトには、複数のキュートピックを含めないことをお勧めします。 送信されたリクエストが異なるリソースやプロジェクトを対象としている場合は、送信後に手動でルーティングまたは移動する必要があります。


1. 電子メールでの問題の受信を有効にするプロジェクトに移動します。
1. クリック **キューの詳細** をクリックします。 クリックが必要になる場合があります **さらに表示** 1 つ目は
1. 内 **キュータイプ** 領域、選択 **ヘルプリクエストキューとして公開**.

1. 下にスクロールして **メールキュー設定** 「領域」、「 **メールによるリクエストインテークの有効化**.

1. 電子メールアドレスの先頭を **インテークメールアドレス** ボックス

   一意の電子メールアドレスを作成する必要があります。 インテークメールアドレスの一部に貴社の名前を使用することをお勧めします。

   >[!CAUTION]
   >
   >* 要求キューを含むプロジェクトが削除されている場合、この電子メールアドレスをごみ箱から復元することはできません。
   >
   >* この電子メールアドレスは一意である必要があるので、削除した場合は将来使用できなくなる可能性があります。

   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. （オプション） **電子メールでの送信に失敗した問題をすべて転送**&#x200B;をクリックし、下のボックスに転送メールアドレスを入力します。

   この電子メールアドレスは、プロジェクトへの送信に失敗した電子メールに関する情報を受け取ります。

1. 「**保存**」をクリックします。これで、アクティブなWorkfrontアカウントを持つユーザーがこの電子メールアドレスに電子メールを送信すると、Workfrontプロジェクトに問題が作成されます。

   >[!NOTE]
   >
   >電子メールで送信するには、ユーザーがプロジェクトでイシューを作成する権限を持っている必要があります。 このアクセス権を付与するには、[ 詳細設定 ] の [ 共有 ] ダイアログボックスを使用します。
   >
   >外部ユーザーは、イシューを作成するアクセス権を持たないので、リクエストキューにイシューを電子メールで送信できません。

## Workfrontで問題を受信

WorkfrontユーザーがWorkfrontに E メールを送信すると、次のことがおこなわれます。

* E メールの件名行が「Issue Name」になります。
* 電子メールの本文が「問題の説明」になります。
* E メールに添付されたドキュメントがある場合は、そのドキュメントがWorkfrontの問題に添付されます。
* E メールを送信するユーザーが、Workfrontの新しい問題のプライマリ連絡先になります。
* 電子メールの本文は 4,000 文字以内にする必要があります。
* 電子メールの添付ファイルの合計が 7 MB を超えてはなりません。
