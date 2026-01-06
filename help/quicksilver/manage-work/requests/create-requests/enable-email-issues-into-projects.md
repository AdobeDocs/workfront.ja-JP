---
product-area: requests
navigation-topic: create-requests
title: ユーザーが問題をリクエストキュープロジェクトにメールで送信できるようにする
description: ユーザーがメールでイシューをプロジェクトに追加できるように、プロジェクトを設定できます。
author: Becky
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 82%

---

# ユーザーが問題をリクエストキュープロジェクトにメールで送信できるようにする

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

ユーザーがメールでプロジェクトにイシューを追加できるようにプロジェクトを設定できます。プロジェクトがリクエストキューとして指定されている場合にのみ、イシューをプロジェクトにメールで送信できます。 リクエストキュープロジェクトの作成について詳しくは、[リクエストキューを作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>投稿者以上</p>
   <p>リクエスト以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 製品</td> 
   <td> <ul><li>Adobe Workfront</li><li>計画リクエストまたはリクエストフォームを表示するには、Adobe Workfront Planning が必要です。</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

ユーザーがメールでイシューをプロジェクトに追加できるようにプロジェクトを設定するには、次の条件が必要です。

* このアカウントにイシューをメールで送信するユーザーは、Workfront のライセンスを持つアクティブユーザーである必要があります。
* このアカウントにイシューをメールで送信するユーザーは、プロジェクトに対してイシューの追加権限が必要です。
* 外部ユーザーは、イシューを作成するアクセス権を持たないので、リクエストキューにイシューをメールで送信できません。
* アクティブな Workfront ユーザーに関連付けられたメールアドレスからのメールのみが、プロジェクトにイシューを送信できます。元の送信者のメールアドレスをアクティブな Workfront アカウントに関連付ける必要があるので、Workfront アカウントに関連付けられていないメールからアクティブな Workfront ユーザーのメールに転送されるメールでは、プロジェクトでイシューを作成できません。
* プロジェクトはリクエストキューとして設定されます。
* プロジェクトに関連付けられたメールアカウントは、Workfront ユーザーアカウントにリンクされていません。

## Workfront でのプロジェクトの設定

>[!NOTE]
>
>メールキューの設定を有効にする際は、次の点に注意してください。
>
>* Workfront では、すべてのクラスターにわたるリクエストキューごとに 1 つの一意のメールを使用できます。リクエストキューを無効にする場合、作成したメールアドレスが取り込みメールアドレスボックスに残っている限り、そのメールアドレスが保持されます。取り込みメールの使用を中止する場合は、今後使用できるよう、取り込みメールフィールドから削除する必要があります。
>
>* リクエストキューに複数のキュートピックまたはトピックグループがある場合、Workfrontはメールでリクエストを送信するキュートピックをランダムに選択するので、メールでリクエストを管理するのが困難になります。
>メールを通じてリクエストを受け取るように設定したプロジェクトには、複数のキュートピックを含めないことをお勧めします。送信されたリクエストが異なるリソースやプロジェクトを対象としている場合は、送信後に手動でルーティングまたは移動する必要があります。

1. メールでのイシューの受信を有効にするプロジェクトに移動します。
1. 左側のパネルで **キューの詳細** をクリックします。
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
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in Workfront. Only emails created from this email address are added as issues.
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

  >[!NOTE]
  >
  > MSG ファイルはサポートされていないので、Workfrontの問題には添付されません。

* メールを送信するユーザーが、Workfront の新しいイシューのプライマリ連絡先になります。
* メールの本文は 4,000 文字以内にする必要があります。
* メールの添付ファイルの合計が 7 MB を超えてはなりません。
