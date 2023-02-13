---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 自動プロビジョニングされたユーザーのパスワードの変更
description: 多くの場合、新しいユーザーが一時パスワードを変更しようとすると、電子メールアドレスを入力して誤ったユーザー名のエラーを受け取ります。 システムが割り当てたユーザー名 (Globally Unique Identifier(GUID)) を入力する必要があります。 GUID を覚えて使用するのは困難なので、新しいユーザーのユーザー名をWorkfrontのメールアドレスに変更し、そのユーザーのパスワードを変更できるようにすることをお勧めします。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# 自動プロビジョニングされたユーザーのパスワードの変更

自動プロビジョニングを使用してユーザーを作成すると、Adobe Workfrontはユーザー名の GUID(Globally Unique Identifier) を割り当てます。 GUID は、乱数や文字の一意の文字列です。例： *5489cb430012526e1ea635e8c29f377f*.

多くの場合、新しいユーザーが一時的なパスワードを変更しようとすると、ユーザー名の電子メールアドレスを入力し、誤ったユーザー名のエラーを受け取ります。 ユーザーがパスワードを変更するには、システムに割り当てられたユーザー名 (GUID) を入力する必要があります。

GUID のユーザー名は使いにくい場合があるので、まずユーザー名をWorkfrontのメールアドレスに変更し、その後でパスワードを変更することをお勧めします。

>[!TIP]
>
>ユーザーの GUID は、次の方法で検索できます。
>
>* ユーザーのプロファイルに移動し、ブラウザーの URL から GUID をコピーします。
>
>  例：URL 内 `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`の場合は、数字と文字の文字列を最後の 2 つのスラッシュの間にコピーします。 `61941ab1000af22d7104628efa1c738b`.
>
>  詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* User > GUID 列を持つユーザーレポートを作成します。 詳しくは、 [レポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Workfront API に対するクエリ。
>


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
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自動プロビジョニングされたユーザーのパスワードの変更

1. 次の例に示すように、API リクエストを渡してユーザーの GUID ユーザー名を特定します。

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` ここで、 *`<domain>`* は会社のドメインで、 *`<ID of User>`* はユーザーのWorkfront ID です。

   次のような応答が返されます。

   ![](assets/get-guid.png)

   「username」の戻り値は、ユーザーの GUID です。

1. ユーザー名として GUID を使用して、ユーザーのパスワードを変更します。

   パスワードの変更について詳しくは、 [パスワードをリセット](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   組織で SSO システムを使用している場合、Workfrontシステム管理者のみがユーザーのパスワードを変更できます。 詳しくは、 [Adobe Workfrontでのシングルサインオンの概要](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. ユーザーがWorkfrontにログインした状態で、次の場所に移動します。

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. 内 **ログインメールアドレス** 」ボックスにユーザーの電子メールアドレスが正しいことを確認し、 **アカウントを更新**.

   ![](assets/guidusername-350x272.png)

   ユーザー名がWorkfrontの E メールアドレスに変更されます。

>[!TIP]
>
>ユーザーの ID を検索するには：
>
>1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).
>
>1. ユーザーを選択します。
>
>   ユーザーのプロファイルページが開き、URL にユーザー ID が表示されます。
