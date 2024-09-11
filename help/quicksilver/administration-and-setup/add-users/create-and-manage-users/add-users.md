---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: ユーザーの追加
description: Workfront 管理者または完全な管理アクセス権を持つユーザーとして、Workfront でユーザーを追加できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1132'
ht-degree: 95%

---

# ユーザーを追加

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>組織が Adobe Admin Console に登録されている場合は、Adobe Admin Console でシステム管理者を作成する必要があります。
>
>Adobe Admin Console でシステム管理者を作成する手順について詳しくは、[Adobe Admin Console でのシステム管理者の管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)を参照してください。
>
>Adobe Admin Console にオンボーディングされた組織のグループ管理者は、この手順を使用してユーザーを作成し、そのユーザーの承認依頼を管理者に送信できます。
>
>組織が Adobe Admin Console にオンボーディングされているかどうかに応じて異なる手順のリストについては、[プラットフォームベースの管理上の違い（Adobe Workfront／Adobe ビジネスプラットフォーム）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

Adobe Workfront でユーザーを追加するには、個々のユーザーを最初から作成するか、既存のユーザーをコピーします。

複数のユーザーを同時にインポートする方法について詳しくは、[ユーザーのインポート](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md)を参照してください。

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p><p>または</p><p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセス レベルです。 </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-in-access-levels.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>これら 2 つのオプションのうち、<b> ユーザー管理者（グループユーザー） </b> が有効になっている場合、ユーザーがメンバーになっているグループのグループ管理者である必要があります。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

ユーザーを追加する前に、以下に示すユーザーに関する情報を収集し、そのユーザーに関連付ける情報を決定します。

* ユーザーの個人情報。少なくとも、以下が必要です。

   * フルネーム
   * ユーザー名
   * デフォルトのパスワード
   * メールアドレス

  >[!NOTE]
  >
  >Workfront オブジェクトのアクセスレベルを指定する際に、ユーザービュー設定を微調整することで、ユーザーが他のユーザーの連絡先情報を表示できるかどうかを決定できます。詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

* 新しいユーザーの社内での役職な何ですか？このユーザーにはダイレクトレポート先がありますか？誰に報告しますか？
* どの担当業務に就いていますか？この担当業務は Workfront に存在しますか？この担当業務に就く人数に制限はありますか？担当業務の作成について詳しくは、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。
* ユーザーが持つアクセスレベルは何ですか？既に存在していますか？新しく作成する必要がありますか？詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。
* このユーザーはどのホームグループに所属すべきですか？このユーザーは複数のグループに所属する必要がありますか？グループについて詳しくは、[グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md)を参照してください。
* このユーザーはどのホームチームに所属すべきですか？このユーザーは複数のチームに所属する必要がありますか？チームについて詳しくは、[チームの概要](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)を参照してください。
* このユーザーに関連付ける必要があるカスタム情報は何ですか？

  ユーザーに関する情報を作成済みのカスタムフィールドに取り込む場合は、ユーザーの作成時にカスタムフォームを用意しておく必要があります。カスタムフォームについて詳しくは、「[ フォームデザイナーを使用したフォームのデザイン ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

## プロジェクトをゼロから作成

{{step-1-to-users}}

1. **新規ユーザー／新規ユーザー**&#x200B;をクリックして、Workfrontにまだ追加されていないユーザーを追加します。

   または

   **新規ユーザー／ユーザーのインポート**&#x200B;をクリックし、スプレッドシートのインポートファイルをアップロードしてユーザーを追加します。

   ユーザーをインポートする場合は、これらの手順を続ける必要はありません。詳しくは、[ユーザーのインポート](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md)を参照してください。

1. 表示される「**新規ユーザー**」ボックスで、「**詳細オプションを表示**」をクリックし、個人情報を入力するために利用可能なオプションを設定します。

   これらのオプションについては、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

1. 次のいずれかの操作を行います。

   * 「**このユーザーに招待状メールを送信**」を有効のままにしておきます。この場合、ユーザーにはメールが届き、Workfront 用の独自のパスワードを作成するためのリンクをたどることができます。メールの招待を受け入れずに Workfront のパスワードを作成したユーザーは、Workfront に「未登録」と表示されます。
   * 「**このユーザーに招待状メールを送信**」を無効にし、そのユーザーの「**パスワード**」を入力し、「**パスワードの確認**」ボックスでそれを確認します。このパスワードは、Workfront の外部のユーザーと共有する必要があります。

   >[!NOTE]
   >
   >* Workfront 管理者が Workfront との SSO 統合を有効にした場合、メールによる招待状を無効にすると、「&lt;SSO Configuration> 認証のみを許可」フィールドは非表示になります。「連合 ID」または「&lt;SSO Configuration> ユーザー名」フィールドは表示されたままです。
   >
   * 組織が Admin Console に既にオンボードされており、Workfront を介してユーザーを追加する場合は、メールの招待状を送信するオプションはありません。
   >
   既存のアドビユーザーの場合、Workfront が使用可能になっていることを知らせるメールがユーザーに届く場合と届かない場合があります。これは、製品のアドビ管理者が制御する環境設定です。

1. 「**このユーザーを追加**」をクリックします。

   または

   「**担当者ユーザーを追加して別のユーザーを開始**」をクリックして、新規ユーザーを保存し、別のユーザーを追加します。

   >[!NOTE]
   >
   Adobe Admin Console にオンボーディングされている組織にグループ管理者がユーザーを追加する場合、この手順には「**管理者の承認用にユーザーを送信**」と「**承認用に送信して次を開始**」のオプションがあります。ユーザーは「非アクティブ化済み」かつ「承認保留中」のステータスで作成されます。Workfront 管理者は、ユーザーを承認する必要があります。承認すると、Workfront でそのユーザーがアクティブ化され、Adobe Admin Consoleに追加されます。

## ユーザーのコピーによる新規ユーザーの作成

既存のユーザーをコピーして、ユーザーを作成できます。

>[!NOTE]
>
この方法でユーザーを作成する場合、次の場合を除き、元のユーザーから新しく作成されたユーザーにすべての情報がコピーされます。
>
* 「個人情報」セクションの情報。
* ログイン時に表示：このボックスでは、アクセスレベルのデフォルトのランディングタブが選択されています。
* 直属の部下
>

既存のユーザーをコピーして新規ユーザーを作成するには、次の手順に従います。

{{step-1-to-users}}

1. コピーするユーザーを選択して、コピーアイコン ![](assets/copy-icon.png) をクリックします。
1. 表示される「**ユーザーのコピー**」ボックスで、新規ユーザーに使用可能なフィールドを編集します。

   ユーザーに関連付けられているすべてのフィールドについて詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

1. 「**このユーザーを追加**」をクリックします。

   または

   「**担当者ユーザーを追加して別のユーザーを開始**」をクリックして、新規ユーザーを保存し、別のユーザーを追加します。

これにより、ユーザーの新しいアカウントが Workfront に作成されます。

ユーザーに招待状を送信するオプションを選択した場合、そのユーザーにはメールが届き、ユーザーはその中のリンクをたどって Workfront パスワードを作成できます。

>[!NOTE]
>
組織が Admin Console に既にオンボードされており、Workfront を介してユーザーを追加する場合は、メールの招待状を送信するオプションはありません。
>
既存のアドビユーザーの場合、Workfront が使用可能になっていることを知らせるメールがユーザーに届く場合と届かない場合があります。これは、製品のアドビ管理者が制御する環境設定です。
