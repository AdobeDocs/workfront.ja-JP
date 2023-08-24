---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: ユーザーを追加
description: Workfront管理者または完全な管理アクセス権を持つユーザーとして、Workfrontでユーザーを追加できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 01b60a2fab1188c8510857490ea87f609897b0bb
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 1%

---

# ユーザーを追加

>[!IMPORTANT]
>
>このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織に適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、Adobe Admin Consoleを通じてこの操作を実行する必要があります。
>
>Adobe Admin Consoleにオンボーディングされた組織のグループ管理者は、この手順を使用して、ユーザーを作成し、管理者の承認を得るためにユーザーを送信できます。
>
>Adobe Admin Consoleでユーザーを追加する手順については、次の手順を実行します。
>
>* 詳しくは、 [Adobe Admin Consoleを使用したWorkfrontでのユーザー作成](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* この記事の「ユーザーの追加」の節を参照してください [ユーザーを個別に管理](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Adobe Admin Console管理者に問い合わせてください。
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfrontでユーザーを追加するには、個々のユーザーをゼロから作成するか、既存のユーザーをコピーします。

複数のユーザーを同時にインポートする方法について詳しくは、 [ユーザーの読み込み](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

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
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>. </p> </li> 
     <li> <p><b>ユーザー</b> 次のように設定されたアクセスレベルの設定： <b>編集</b> アクセス、 <b>作成</b> そして少なくとも 2 つのうち 1 つは <b>ユーザー管理者</b> 以下で有効になるオプション <b>設定を微調整する</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>この 2 つのオプションのうち、User <b>管理者（グループユーザー）</b> が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> <p>詳しくは、 <b>ユーザー</b> アクセスレベルでの設定については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 前提条件

ユーザーを追加する前に、以下に示すユーザーに関する情報を収集し、そのユーザーに関連付ける情報を決定します。

* ユーザーの個人情報は何ですか？ 少なくとも、以下が必要です。

   * 姓名
   * ユーザー名
   * デフォルトのパスワード
   * メールアドレス

  >[!NOTE]
  >
  >Workfrontオブジェクトのアクセスレベルを指定する際に、「ユーザービュー」設定を微調整することで、他のユーザーの連絡先情報を表示できるかどうかを指定できます。 詳しくは、 [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 会社内での新しいユーザーの位置は何ですか？ この人には直属の部下はありますか？ この人は誰に報告しますか？
* その人はどの職に就いていますか。 この職務はWorkfrontに存在しますか？ この職務に就く人数に制限はありますか？ ジョブの役割の作成について詳しくは、 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* ユーザーが持つアクセスレベルは何ですか？ 既に存在しているか、新しく作成する必要があるかを確認します。 詳しくは、 [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* このユーザーはどのホームグループに属すべきですか？ 担当者は複数のグループに属する必要がありますか？ グループについて詳しくは、 [グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* このユーザーはどのホームチームに所属すべきですか？ 担当者は複数のチームに所属する必要がありますか？ チームについて詳しくは、 [チームの概要](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* このユーザーに関連付ける必要があるカスタム情報は何ですか？

  ユーザーに関する情報が作成したカスタムフィールドに取り込まれる場合は、ユーザーの作成時にカスタムフォームを用意しておく必要があります。 カスタムフォームについて詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## ユーザーをゼロから作成する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).

1. クリック **新規ユーザ/新規ユーザ** をクリックして、Workfrontにまだ追加されていないユーザーを追加します。

   または

   クリック **新規ユーザ/ユーザの読み込み** をクリックして、スプレッドシートのインポートファイルをアップロードしてユーザーを追加します。

   ユーザーをインポートする場合は、これらの手順を続行する必要はありません。 詳しくは、 [ユーザーの読み込み](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. Adobe Analytics の **新しいユーザー** 表示されるボックスで、 **アドバンスオプションを表示**&#x200B;次に、利用可能なオプションを設定して、ユーザーの情報を入力します。

   これらのオプションについて詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 次のいずれかの操作を行います。

   * 終了 **この人に招待メールを送信する** 有効。 この場合、ユーザーは電子メールを受け取り、Workfront用の独自のパスワードを作成するためのリンクをたどることができます。 電子メールの招待を受け入れず、Workfrontのパスワードを作成したユーザーは、「Workfrontで未登録」と表示されます。
   * 無効にする **この人に招待メールを送信する**&#x200B;を入力し、 **パスワード** その人に対して、 **パスワードを確認** ボックス。 このパスワードは、Workfront以外のユーザーと共有する必要があります。

   >[!NOTE]
   >
   >Workfront管理者がWorkfrontとの SSO 統合を有効にした場合、「許可」 &lt;sso configuration=&quot;&quot;> 電子メールの招待状を無効にした場合、認証フィールドは非表示になります。 フェデレーション ID または &lt;sso configuration=&quot;&quot;> ユーザー名フィールドは表示されたままです。

   >[!NOTE]
   >
   組織がAdmin Consoleにオンボーディングされていて、Workfrontからユーザーを追加する場合は、電子メールで招待状を送信するオプションはありません。
   >
   新しいAdobeユーザーがAdmin Consoleに追加され、Admin Consoleが電子メールを配信して登録プロセスを完了するよう招待します。 すべてのユーザーが登録プロセスを完了して、任意のAdobe・システムにアクセスします。
   >
   既存のAdobeユーザーの場合、Workfrontが使用可能になっていることを知らせる電子メールをユーザーが受け取る場合と受け取らない場合があります。 これは、製品のAdobe管理者が制御するプリファレンスです。

1. クリック **このユーザーを追加**.

   または

   クリック **担当者ユーザーを追加して別のユーザーを開始** をクリックして、新しいユーザーを保存し、別のユーザーを追加します。

   >[!NOTE]
   >
   Adobe Admin Consoleにオンボーディングされている組織にユーザーを追加するグループ管理者の場合、この手順のオプションは次のとおりです **管理者の承認用にユーザーを送信** および **承認用に送信し、別の承認を開始**. ユーザーのステータスは、「非アクティブ化済み」および「承認待ち」です。 Workfrontの管理者は、ユーザーを承認する必要があります。承認すると、Workfrontでそのユーザーがアクティベートされ、Adobe Admin Consoleに追加されます。

## ユーザーをコピーして新しいユーザーを作成する

既存のユーザーをコピーして、ユーザーを作成できます。

>[!NOTE]
>
この方法でユーザーを作成する場合、次の場合を除き、すべての情報が元のユーザーから新しく作成されたユーザーにコピーされます。
>
* 個人情報セクションの情報。
* ログイン時に表示：このボックスでは、アクセスレベルのデフォルトのランディングタブが選択されています。
* 部下
>

既存のユーザーをコピーして新しいユーザーを作成するには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).
1. コピーするユーザーを選択し、コピーアイコンをクリックします。 ![](assets/copy-icon.png).
1. Adobe Analytics の **新しいユーザー** 表示されるボックスで、新しいユーザーが使用できるフィールドを編集します。

   ユーザーに関連付けられているすべてのフィールドについて詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. クリック **このユーザーを追加**.

   または

   クリック **担当者ユーザーを追加して別のユーザーを開始** をクリックして、新しいユーザーを保存し、別のユーザーを追加します。

これにより、Workfrontにユーザーの新しいアカウントが作成されます。

ユーザーに招待メールを送信するオプションを選択した場合は、Workfrontのパスワードを作成するためのリンクをたどってリンク先の電子メールがユーザーに送信されます。

>[!NOTE]
>
組織がAdmin Consoleにオンボーディングされていて、Workfrontからユーザーを追加する場合は、電子メールで招待状を送信するオプションはありません。
>
新しいAdobeユーザーがAdmin Consoleに追加され、Admin Consoleが電子メールを配信して登録プロセスを完了するよう招待します。 すべてのユーザーが登録プロセスを完了して、任意のAdobe・システムにアクセスします。
>
既存のAdobeユーザーの場合、Workfrontが使用可能になっていることを知らせる電子メールをユーザーが受け取る場合と受け取らない場合があります。 これは、製品のAdobe管理者が制御するプリファレンスです。
