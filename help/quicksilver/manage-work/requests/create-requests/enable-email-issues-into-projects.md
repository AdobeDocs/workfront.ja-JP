---
product-area: requests
navigation-topic: create-requests
title: ユーザーが問題をリクエストキュープロジェクトにメールで送信できるようにする
description: ユーザーが問題をリクエストキュープロジェクトにメールで送信できるようにする
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: dad055b0901cfa8114f7f6b13b6f689d70b31205
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 92%

---

# ユーザーが問題をリクエストキュープロジェクトにメールで送信できるようにする

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

ユーザーがメールでプロジェクトにイシューを追加できるようにプロジェクトを設定できます。プロジェクトがリクエストキューとして指定されている場合にのみ、プロジェクトにイシューをメールで送信できます。リクエストキュープロジェクトの作成について詳しくは、[リクエストキューを作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

ユーザーがメールでプロジェクトにイシューを追加できるようにプロジェクトを設定するには、次の前提条件が必要です。

この機能を有効にする前に、次の条件を満たす必要があります。

* このアカウントにイシューをメールで送信するユーザーは、Workfront のライセンスを持つアクティブユーザーである必要があります。
* このアカウントにイシューをメールで送信するユーザーは、プロジェクトに対してイシューの追加権限が必要です。
* 外部ユーザーは、イシューを作成するアクセス権を持たないので、リクエストキューにイシューをメールで送信できません。
* アクティブなWorkfrontユーザーに関連付けられた電子メールアドレスからの電子メールのみが、問題をプロジェクトに送信できます。 元の送信者の E メールアドレスをアクティブなWorkfrontアカウントに関連付ける必要があるので、Workfrontアカウントに関連付けられていない E メールからアクティブなWorkfrontユーザー E メールに転送される E メールは、プロジェクトに問題を作成できません。
* プロジェクトはリクエストキューとして設定されます。
* プロジェクトに関連付けられたメールアカウントは、Workfront ユーザーアカウントにリンクされていません。

## Workfront でのプロジェクトの設定

>[!NOTE]
>
>メールキューの設定を有効にする際は、次の点に注意してください。
>
>* Workfront では、すべてのクラスターにわたるリクエストキューごとに 1 つの一意のメールを使用できます。リクエストキューを無効にする場合、作成したメールアドレスが取り込みメールアドレスボックスに残っている限り、そのメールアドレスが保持されます。取り込みメールの使用を中止する場合は、今後使用できるよう、取り込みメールフィールドから削除する必要があります。
>
>* リクエストキューに複数のキュートピックまたはトピックグループが含まれる場合、Workfront はメールで送信されたリクエストが送信されるキュートピックをランダムに選択するため、メールで送信されたリクエストの管理が困難になります。
>メールを通じてリクエストを受け取るように設定したプロジェクトには、複数のキュートピックを含めないことをお勧めします。送信されたリクエストが異なるリソースやプロジェクトを対象としている場合は、送信後に手動でルーティングまたは移動する必要があります。

1. メールでのイシューの受信を有効にするプロジェクトに移動します。
1. 左側のパネルで「**キューの詳細**」をクリックします。まず「**さらに表示**」をクリックする必要がある場合もあります。
1. **キュータイプ**&#x200B;エリアで、「**ヘルプリクエストキューとして発行**」を選択します。

1. **E メールキューの設定**&#x200B;エリアまで下にスクロールし、「**E メール経由で要求取り込みを有効にする**」を選択します。

1. **取り込み E メールアドレス**&#x200B;ボックスにメールアドレスの先頭を入力します。

   一意のメールアドレスを作成する必要があります。取り込みメールアドレスの一部に会社名を使用することをお勧めします。

   >[!CAUTION]
   >
   >* リクエストキューを含むプロジェクトが削除されている場合、このメールアドレスをごみ箱から復元することはできません。
   >
   >* このメールアドレスは一意である必要があるので、削除した場合は将来使用できなくなる可能性があります。
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. （オプション）「**E メールで送信に失敗した問題のすべてを転送する**」を選択し、下のボックスに転送メールアドレスを入力します。

   このメールアドレスは、プロジェクトへの送信に失敗したメールに関する情報を受け取ります。

1. 「**保存**」をクリックします。これで、アクティブな Workfront アカウントを持つユーザーがこのメールアドレスにメールを送信すると、Workfront プロジェクトにイシューが作成されます。

   >[!NOTE]
   >
   >メールで送信するには、ユーザーがプロジェクトでイシューを作成する権限を持っている必要があります。このアクセス権は、「詳細設定」の「共有」ダイアログボックスで付与できます。
   >
   >外部ユーザーは、イシューを作成するアクセス権を持たないので、リクエストキューにイシューをメールで送信できません。

## Workfront でイシューを受信する

Workfront ユーザーが Workfront にメールを送信すると、次のことが行われます。

* メールの件名行が「イシュー名」になります。
* メールの本文が「イシューの説明」になります。
* メールに添付されたドキュメントがある場合は、そのドキュメントが Workfront のイシューに添付されます。
* メールを送信するユーザーが、Workfront の新しいイシューのプライマリ連絡先になります。
* メールの本文は 4,000 文字以内にする必要があります。
* メールの添付ファイルの合計が 7 MB を超えてはなりません。
