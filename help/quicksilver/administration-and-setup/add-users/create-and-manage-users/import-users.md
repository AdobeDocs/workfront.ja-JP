---
title: ユーザーの読み込み
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: ユーザーをAdobe Workfrontサイトにインポートするには、ネットワークディレクトリサービス（Active Directory や他の LDAP ディレクトリなど）からユーザーを同期するか、スプレッドシートインポートファイルを使用してユーザーをインポートします。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

# ユーザーの読み込み

>[!IMPORTANT]
>
>このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、Adobe Admin Consoleを通じてこの操作を実行する必要があります。
>
>Adobe Admin Consoleでユーザーのプロファイルを編集する手順については、この記事の「ユーザーの追加」の節を参照してください [ユーザーの一括アップロード](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) または、Adobe Admin Console管理者に問い合わせてください。
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

ユーザーは、スプレッドシートインポートファイルを使用してインポートできます。

新しいユーザーを作成する前に、まず、そのユーザーに関連付けるすべてのオブジェクトが作成されていることを確認します。 例えば、スケジュールを作成していない場合、新しいユーザーにスケジュールを割り当てることはできません。また、スケジュールを新しいユーザーに関連付けるために使用するフィールドは、[ 新しいユーザー ] 画面に表示されません。

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
     <li> <p><b>ユーザー</b> 設定を <b>編集</b> アクセス、 <b>作成</b> そして少なくとも 2 つのうち 1 つは <b>ユーザー管理者</b> 以下で有効になるオプション <b>設定を微調整する</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>この 2 つのオプションのうち、ユーザー <b>管理者（グループユーザー）</b> が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> <p>詳しくは、 <b>ユーザー</b> アクセスレベルでの設定については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## スプレッドシートのインポートファイルを使用したユーザーのインポート

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).

1. 次をクリック： **新しいユーザー** ドロップダウン矢印をクリックし、 **ユーザーの読み込み**.

1. 内 **ユーザーの読み込み** 表示されるボックスに、サンプルファイルをダウンロードしてから、サンプルファイルを更新して、独自のユーザーの個人情報を含めます。

   各行には、次のフィールドが含まれます。

   * **名**
   * **姓**
   * **E メール アドレス**

      電子メールアドレスは一意である必要があります。

   * **アクセスレベル**

      アクセスレベルでは大文字と小文字が区別されます。

   * **SSO ログイン ID**

      このフィールドは、システムで SSO が有効になっている場合にのみ含まれます。 各ユーザーのこのフィールドにフェデレーション ID を追加する必要があります。 「ユーザー」タブからユーザーを作成する場合、SSO を使用せずにユーザーがログインできるようにするには、ユーザーのパスワードを設定できます。 ただし、インポート機能では SSO ログイン ID を空白のままにすることはできません。

   * ユーザーの E メールアドレスの前後に余分なスペースが存在しないようにします。

   行の作成が完了すると、次のようになります。

   ![importing-new-users.png](assets/importing-new-users.png)

1. ファイルをワークステーション上の場所に保存します。
1. クリック **ファイルを選択** 内 **ユーザーの読み込み** ボックス

1. に移動し、保存したファイルを選択します。
1. （オプション） **このユーザーに招待メールを送信** 電子メールの招待状をユーザーに送信するオプション。Workfrontアカウントが作成されたことを通知し、パスワードの設定を促すメッセージを表示します。

   ユーザーのパスワードを設定する場合は、このオプションの選択を解除します。

1. クリック **インポート**.

   ユーザーが正常に読み込まれたことを示す確認メッセージが画面上部に表示されます。
