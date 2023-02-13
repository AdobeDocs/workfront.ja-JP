---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 電子メールの設定を許可リスト行う
description: 組織で WorkfrontEnterprise プランを使用する場合は、Workfrontの電子メールドメインを作成し許可リストて、Workfrontからの電子メールを受け入れる電子メールドメインと、ユーザープロファイルで指定した電子メールアドレスに指定できる電子メールドメインを制御できます。 これは、組織のセキュリティポリシーで、Workfrontに保存されているデータを外部の電子メールアドレスに送信できないように制限されている場合に役立ちま許可リストす。社内ドメインのみをに含めて、このポリシーに従うことができます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 電子メールの設定を許可リスト行う

組織で WorkfrontEnterprise プランを使用している場合、Workfront電子メールを作成して、次の項目を制御できま許可リストす。

* Workfrontからの E メールを受け入れることが許可されている E メールドメイン。
* ユーザープロファイルでユーザーが指定した電子メールアドレスに含めることができる電子メールドメイン。

これは、組織のセキュリティポリシーで、Workfrontに保存されているデータを外部の電子メールアドレスに送信できないように制限されている場合に役立ちま許可リストす。社内ドメインのみを含めて、このポリシーに従うようにできます。

>[!IMPORTANT]
>
>IT チームは、次のメールが届くことを確認する必要があります： `notifications@my.workfront.com` が組織のシステムでブロックされていません。
>
>E メールの配信を成功させ、E メールのスプーフィングを防ぐために、Workfrontからのすべての E メールがそのアドレスから送信されます。 これには、自動アラートとユーザー間通信の両方が含まれます。
>
>例えば、Joan Harris という名前のユーザーから受け取ったWorkfront E メールの送信者行は次のようになります。
>
```
>Joan Harris <notifications@my.workfront.com>
>```

お使いの環境とAdobe Workfrontサーバー間の通信を開くための組織のファイアウォールの設定について詳しくは、 [ファイアウォールの設定を許可リスト行う](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

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
   <td> <p>Workfront管理者である。 詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## その他の許可リスト

企業向けプランがある場合は、Workfrontへのアクセスを指定した 45 個の IP アドレスまたは IP アドレスの範囲に制限するAdobe Workfront IP を設定できま許可リストす。 これにより、Workfrontアプリケーションのセキュリティレイヤーがさらに強化されます。 詳しくは、 [IP アドレスでAdobe Workfrontへのアクセスを制限する](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

また、特定のベンダーへのアクセスのみを許可するようにファイアウォールまたはメールサーバーが設定されている場合は、特定の IP アドレスをそのに追加する必要があり許可リストます。 これにより、環境とAdobe Workfrontサーバー間の通信が開始されます。 詳しくは、 [ファイアウォールの設定を許可リスト行う](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 電子メールの設定を許可リスト行う

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **顧客情報**.

1. 内 **メールの許可リスト** セクション、選択 **ドメインの有効化許可リスト**&#x200B;を選択し、「 **ドメインを追加**.
1. 表示されるボックスに、許可するドメイン（例： ）を入力します。 `ourcompany.com`を選択し、「 **ドメインを追加**.

1. 上記の手順を繰り返して、許可する他のドメインを追加します。
1. 完了したら、「 **保存**.
