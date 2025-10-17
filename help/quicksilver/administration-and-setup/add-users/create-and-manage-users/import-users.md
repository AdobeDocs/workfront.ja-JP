---
title: ユーザーの読み込み
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: ユーザーを Adobe Workfront サイトにインポートするには、ネットワークディレクトリサービス（Active Directory や他の LDAP ディレクトリなど）からユーザーを同期するか、スプレッドシートインポートファイルを使用してユーザーをインポートします。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 69%

---

# ユーザーの読み込み

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/jp/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

スプレッドシートインポートファイルを使用して、ユーザーをインポートできます。

新しいユーザーを作成する前に、まず、そのユーザーに関連付けるすべてのオブジェクトが作成されていることを確認します。例えば、スケジュールを作成していない場合、新しいユーザーにスケジュールを割り当てることはできません。また、スケジュールを新しいユーザーに関連付けるために使用するフィールドは、新規ユーザー画面に表示されません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p><p>プラン</p></td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセス レベルです。 </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-in-access-levels.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>これら 2 つのオプションのうち、<b> ユーザー管理者（グループユーザー） </b> が有効になっている場合、ユーザーがメンバーになっているグループのグループ管理者である必要があります。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## スプレッドシートインポートファイルを使用したユーザーのインポート

{{step-1-to-users}}

1. **新規ユーザー**&#x200B;ドロップダウン矢印をクリックし、「**ユーザーのインポート**」をクリックします。

1. 表示された **ユーザーのインポート** ボックスで、サンプルファイルをダウンロードした後、サンプルファイルを更新して独自のユーザーの個人情報を含めます。

   各行には、次のフィールドが含まれます。

   * **名**
   * **姓**
   * **メールアドレス**

     メールアドレスは一意である必要があります。

   * **アクセス レベル**

     アクセスレベルでは大文字と小文字が区別されます。

   * **SSO ログイン ID**

     このフィールドは、システムで SSO が有効になっている場合にのみ含まれます。各ユーザーのこのフィールドに連合 ID を追加する必要があります。「ユーザー」タブからユーザーを作成する際に、ユーザーが SSO を使用せずにログインできるようにする場合は、ユーザーのパスワードを設定できます。ただし、インポート機能では「SSO ログイン ID」を空白のままにすることはできません。

   * ユーザーのメールアドレスの前後に余分なスペースが存在しないことを確認します。

   行の入力が完了すると、次のようになります。

   ![importing-new-users.png](assets/importing-new-users.png)

1. ファイルをワークステーション上の場所に保存します。
1. **ユーザーをインポート** ボックスの **ファイルを選択** をクリックします。

1. 保存したファイルに移動し、選択します。

<!--
1. (Optional) Select the **Send an invite email to this user** option to send an email invitation to the user, notifying them that a Workfront account has been created and prompting them to set their password.

   Deselect this option if you want to set the password for the user.

-->

1. 「**インポート**」をクリックします。

   ユーザーが正常に読み込まれたことを示す確認メッセージが画面の上部に表示されます。

>[!NOTE]
>
>ユーザーは、「ディアクティベート済み」および「承認待ち」のステータスで作成されます。
> 
>ユーザーのステータスが数分以内にディアクティベートおよび承認待ちから変わらず、画面を更新しても承認待ちバッジが削除されない場合は、ユーザーのバッチをAdobe Admin Consoleに直接追加できます。
>
>手順については、アドビドキュメントの[複数ユーザーの管理 | CSV の一括アップロード](https://helpx.adobe.com/jp/enterprise/using/bulk-upload-users.html)を参照してください。
