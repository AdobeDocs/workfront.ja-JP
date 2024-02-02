---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 自動プロビジョニングされたユーザーのパスワードを変更
description: 新しいユーザーが一時パスワードを変更しようとする際、メールアドレスを入力すると、ユーザー名が間違っているというエラーが表示されることがよくあります。システムによって割り当てられたユーザー名（グローバル一意識別子（GUID））を入力する必要があります。GUID を記憶するのは困難なので、新しいユーザーのユーザー名を Workfront のメールアドレスに変更し、ユーザーが各自パスワードを変更できるようにすることをお勧めします。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: ht
source-wordcount: '532'
ht-degree: 100%

---

# 自動プロビジョニングされたユーザーのパスワードを変更

自動プロビジョニングを使用してユーザーを作成すると、Adobe Workfront はユーザー名の GUID（グローバル一意識別子）を割り当てます。GUID は、乱数や文字の一意の文字列です。例：*5489cb430012526e1ea635e8c29f377f*

新規ユーザーが一時パスワードを変更しようとする際、ユーザー名にメールアドレスを入力すると、ユーザー名が正しくないというエラーが表示されることがよくあります。ユーザーがパスワードを変更するには、システムによって割り当てられたユーザー名（GUID）を入力する必要があります。

GUID のユーザー名は使いにくい場合があるので、まずユーザーのユーザー名を Workfront のメールアドレスに変更し、その後ユーザーが各自パスワードの変更を行うことができるようにするをお勧めします。

>[!TIP]
>
>ユーザーの GUID は、次の方法で検索できます。
>
>* ユーザーのプロファイルに移動し、ブラウザーの URL から GUID をコピーします。
>
>  例えば、URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details` の場合は、数字と文字の文字列を最後の 2 つのスラッシュの間 `61941ab1000af22d7104628efa1c738b` をコピーします。
>
>  詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。
>
>* ユーザー／GUID 列で、ユーザーレポートを作成します。詳しくは、[レポートを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)を参照してください。
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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自動プロビジョニングされたユーザーのパスワードを変更

1. 次の例に示すように、API リクエストを渡してユーザーの GUID ユーザー名を決定します。

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` ここで、*`<domain>`* は会社のドメインで、*`<ID of User>`* は、ユーザーの Workfront ID です。

   次のような応答が返されます。

   ![](assets/get-guid.png)

   「ユーザー名」の戻り値は、ユーザーの GUID です。

1. ユーザー名として GUID を使用して、ユーザーのパスワードを変更します。

   パスワードの変更について詳しくは、[パスワードをリセット](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md)を参照してください。

   組織で SSO システムを使用している場合、Workfront システム管理者のみがユーザーのパスワードを変更できます。詳しくは、[Adobe Workfront でのシングルサインオンの概要](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)を参照してください。

1. ユーザーが Workfront にログインした状態で、次の場所に移動します。

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. 「**ログインメールアドレス**」ボックスにユーザーのメールアドレスが正しいことを確認し、「**アカウントを更新**」をクリックします。

   ![](assets/guidusername-350x272.png)

   ユーザーのユーザー名が Workfront のメールアドレスに変更されます。

>[!TIP]
>
>ユーザーの ID を検索するには、次の手順に従います。
>
>1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**ユーザー** ![](assets/users-icon-in-main-menu.png) の順にクリックします。
>
>1. ユーザーを選択します。
>
>   ユーザーのプロファイルページが開き、URL にユーザー ID が表示されます。
>
