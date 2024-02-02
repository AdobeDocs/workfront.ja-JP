---
title: ユーザーの読み込み
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: ユーザーを Adobe Workfront サイトにインポートするには、ネットワークディレクトリサービス（Active Directory や他の LDAP ディレクトリなど）からユーザーを同期するか、スプレッドシートインポートファイルを使用してユーザーをインポートします。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: ht
source-wordcount: '599'
ht-degree: 100%

---

# ユーザーの読み込み

>[!IMPORTANT]
>
>このページで説明する手順は、Admin Console にまだ登録されていない組織にのみ適用されます。組織が Adobe Admin Console に登録されている場合は、Adobe Admin Console でこのアクションを実行してください。
>
>Adobe Admin Console でユーザーのプロファイルを編集する手順については、[ユーザーの一括アップロード](https://helpx.adobe.com/jp/enterprise/using/bulk-upload-users.html)の記事の「ユーザーを追加」の節を参照するか、Adobe Admin Console の管理者にお問い合わせください。
>
>組織が Adobe Admin Console にオンボーディングされているかどうかに応じて異なる手順のリストについては、[プラットフォームベースの管理上の違い（Adobe Workfront／Adobe Business Platform）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

スプレッドシートインポートファイルを使用して、ユーザーをインポートできます。

新しいユーザーを作成する前に、まず、そのユーザーに関連付けるすべてのオブジェクトが作成されていることを確認します。例えば、スケジュールを作成していない場合、新しいユーザーにスケジュールを割り当てることはできません。また、スケジュールを新しいユーザーに関連付けるために使用するフィールドは、新規ユーザー画面に表示されません。

## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。 </p> </li> 
     <li> <p>アクセスレベルの<b>ユーザー</b>設定が<b>編集</b>アクセスに設定されていて、<b>作成</b>と 2 つの<b>ユーザー管理者</b>オプションの少なくとも 1 つが、<b>設定の微調整</b> <img src="assets/gear-icon-in-access-levels.png"> で有効になっている。 </p> <p>この 2 つのオプションのうち、<b>ユーザー管理者（グループユーザー）</b>が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> <p>アクセスレベルの<b>ユーザー</b>設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## スプレッドシートインポートファイルを使用したユーザーのインポート

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**ユーザー** ![](assets/users-icon-in-main-menu.png) をクリックします。

1. **新規ユーザー**&#x200B;ドロップダウン矢印をクリックし、「**ユーザーのインポート**」をクリックします。

1. 表示される&#x200B;**ユーザーのインポート**&#x200B;ボックスで、サンプルファイルをダウンロードしてから、サンプルファイルを更新して、自分のユーザーの個人情報を含めます。

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
1. **ユーザーのインポート**&#x200B;ボックスの「**ファイルの選択**」をクリックします。

1. 保存したファイルに移動し、選択します。
1. （オプション）「**このユーザーに招待状メールを送信**」オプションを選択すると、ユーザーに招待メールが送信されて、Workfront アカウントが作成されたことが通知され、パスワードの設定が促されます。

   ユーザーのパスワードを設定する場合は、このオプションの選択を解除します。

1. 「**インポート**」をクリックします。

   ユーザーが正常にインポートされたことを示す確認メッセージが画面の上部に表示されます。
