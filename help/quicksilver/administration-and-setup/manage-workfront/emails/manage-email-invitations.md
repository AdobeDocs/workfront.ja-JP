---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 新規ユーザーへのメール招待を管理
description: Adobe Workfront管理者は、E メールの招待状を使用して、Workfrontにユーザーを追加し、追加されたことをユーザーに通知できます。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# 新規ユーザーへのメール招待を管理

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、Adobe Admin Consoleを通じてこの操作を実行する必要があります。
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfront管理者は、E メールの招待状を使用して、Workfrontにユーザーを追加し、追加されたことをユーザーに通知できます。

電子メールの招待状を使用すると、新しいユーザーはリンクをたどってWorkfrontアカウントのパスワードを選択できます。 その後、アカウントの設定を完了できます。

新しいアカウントのセキュリティを確保するために、新しいユーザーは自分のパスワードを選択できるよう、E メールの招待状を使用することをお勧めします。 また、新しいユーザーのアカウント作成時に、そのユーザーのパスワードを選択することもできます。 Workfrontに新しいユーザーを追加する方法について詳しくは、 [ユーザーを追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

次の新しいユーザー電子メールを設定できます。

* Workfrontに追加された新規ユーザー
* 要求者のライセンスを持つユーザーがWorkfrontに追加された

電子メールの招待状が送信されると、すべての新規ユーザーに同じ電子メールが表示されます。

E メールの招待状の受け取りについて詳しくは、 [E メールの招待状を受け取り、Adobe Workfront用のパスワードを作成します](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者</p> </td> 
  </tr> 
 </tbody> 
</table>

## E メールの招待状を生成 {#generate-email-invitations}

E メールの招待状は、次のシナリオで生成されます。

* 新しいユーザーを作成し、 **この人に招待メールを送信** の **新しいユーザー** フォーム。 新しいユーザーの作成について詳しくは、 [ユーザーを追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* 複数の新しいユーザーをインポートし、 **これらの担当者に招待メールを送信** オプション。 複数の新しいユーザーのインポートについて詳しくは、 [ユーザーの読み込み](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* ユーザーを作成した後は、Workfrontにまだアカウントを登録しておらず、Workfrontのパスワードを設定していないユーザーへの招待を手動で生成できます。\
   アカウントを作成済みだが、まだ登録していないユーザーは、 **登録解除** Workfront

   >[!NOTE]
   >
   >この **この人に招待メールを送信** 」ボックスに入力すると、電子メールの招待状を手動で生成することはできません。 E メールの招待状を手動で再送信できるのは、アカウントの作成時に元の E メールの招待状を送信したユーザーのみです。 新しいユーザーの作成について詳しくは、 [ユーザーを追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

既存の未登録ユーザーへの E メール招待状を手動で生成するには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).
1. 次を表示するユーザーを選択します： **登録解除** 名前の後にラベルを付けます。

   ![](assets/unreg-user-qs-350x221.png)

1. その他アイコンをクリックします。 ![](assets/more-icon.png)を選択し、「 **ユーザーに登録を促す**.

   新しいユーザーに、Workfrontのパスワードを作成するために使用できる新しいリンクが記載された招待メールが送信されます。

   >[!NOTE]
   >
   >組織がAdmin Consoleにオンボーディングされ、Workfrontを通じてユーザーを追加する場合、新しいユーザーに電子メール招待メールを送信するオプションはありません。
   >
   >新しいAdobeユーザーがAdmin Consoleに追加され、Admin Consoleが電子メールを配信して登録プロセスを完了するよう招待します。 すべてのユーザーが登録プロセスを完了して、任意のAdobe・システムにアクセスします。
   >
   >既存のAdobeユーザーの場合、Workfrontが使用可能になっていることを知らせる電子メールをユーザーが受け取る場合と受け取らない場合があります。 これは、製品のAdobe管理者が制御するプリファレンスです。

## E メールの招待状の設定 {#configure-email-invitations}

Workfront管理者は、新しいユーザーへの E メールの招待状に含めるメッセージを設定できます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のリストで、 **電子メール** > **招待**.

1. 内 **一般オプション** セクションで、次のいずれかの変更をおこないます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>...日後に招待リンクを非アクティブ化</strong> </td> 
      <td> <p>E メールの招待状にWorkfrontへの有効なリンクが含まれなくなるまでの時間を選択します。 デフォルトの日数は 45 日です。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>メッセージやサービス期間を含める</strong> </td> 
      <td> <p>Workfrontに追加されたすべての新規ユーザーの電子メール招待状を変更する場合は、このオプションを選択します。 これには、要求者のライセンスを持つユーザーは含まれません。</p> 
       <ul> 
        <li><strong>メッセージ</strong>:すべての新規ユーザーの電子メールの招待状を変更する場合は、電子メールの本文として電子メールの招待状に含めるテキストを指定します。</li> 
        <li><strong>利用条件</strong>:すべての新規ユーザーに対する電子メールの招待状を変更する場合は、電子メールの招待状に含めるテキストを利用条件として指定します。<br></li> 
        <li><strong>ヘルプデスクユーザー向けのメッセージやサービス期間を含める</strong>:要求者のライセンスを持つWorkfrontに追加されたすべての新規ユーザーに対して電子メールの招待状を変更する場合は、このオプションを選択します。</li> 
        <li><strong>メッセージ</strong>:要求者のライセンスを持つすべての新規ユーザーに対して電子メールの招待状を変更する場合は、電子メールの本文として電子メールの招待状に含めるテキストを指定します。</li> 
        <li><strong>利用条件</strong>:依頼者のライセンスを持つすべての新規ユーザーに対して電子メールの招待状を変更する場合は、電子メールの招待状に含めるテキストを利用条件として指定します。<br></li> 
        <li> <p>内 <strong>招待のプレビュー</strong> 「 」セクションに、電子メールの招待状のプレビューを表示できます。 電子メールの招待状にカスタマイズしたメッセージを含めることを選択した場合は、カスタマイズしたメッセージがこの領域に表示されます。</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
