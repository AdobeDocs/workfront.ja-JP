---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: メール許可リストの設定
description: 組織が Workfront エンタープライズプランを使用する場合は、Workfront メール許可リストを作成して、どのメールドメインが Workfront からのメールの受け入れを許可するか、そしてユーザーがユーザープロファイルで指定するメールアドレスにどのメールドメインを含めることができるかを制御できます。これは、組織のセキュリティポリシーにより、ユーザーが Workfront に保存されているデータを外部のメールアドレスに送信できないように制限されている場合に便利です。会社の内部ドメインのみを許可リストに含めることにより、このポリシーが確実に遵守されます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '510'
ht-degree: 100%

---

# メール許可リストの設定

組織で Workfront エンタープライズプランを使用している場合、Workfront メール許可リストを作成すると、以下の項目を制御できます。

* Workfront からのメールを受け入れることが許可されているメールドメイン。
* ユーザープロファイルでユーザーが指定したメールアドレスに含めることができるメールドメイン。

これは、組織のセキュリティポリシーにより、ユーザーが Workfront に保存されているデータを外部のメールアドレスに送信できないように制限されている場合に便利です。会社の内部ドメインのみを許可リストに含めることにより、このポリシーが確実に遵守されます。

>[!IMPORTANT]
>
>IT チームは、`notifications@my.workfront.com` から送信されるメールが組織のシステムでブロックされていないことを確認する必要があります。
>
>Workfront からのメールは、メール配信の成功率を高め、メールのなりすましを排除するために、すべてそのアドレスから送信されます。これには、自動アラートとユーザー間通信の両方が含まれます。
>
>例えば、Joan Harris という名前のユーザーから受け取った Workfront メールの送信者行は次のようになります。
>```
>Joan Harris <notifications@my.workfront.com>
>```

ご使用の環境と Adobe Workfront サーバー間の通信を開くための組織のファイアウォールの設定について詳しくは、[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

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
   <td> <p>Workfront 管理者である必要があります。詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## その他の許可リスト

組織にエンタープライズプランがある場合は、Adobe Workfront IP 許可リストを設定して、Workfront へのアクセスを 45 個の IP アドレス、または指定した IP アドレスの範囲に制限することができます。これにより、Workfront アプリケーションのセキュリティレイヤーがさらに強化されます。詳しくは、[IP アドレスによる Adobe Workfront へのアクセスの制限](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md)を参照してください。

またファイアウォールやメールサーバーが、特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをそのに許可リストに追加する必要があります。これにより、環境と Adobe Workfront サーバー間の通信が開始されます。詳しくは、[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

## メール許可リストの設定

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. **システム**／**顧客情報**&#x200B;をクリックします。

1. 「**メールの許可リスト**」セクションで、「**ドメインの許可リストを有効にする**」を選択し、次に「**ドメインを追加**」をクリックします。
1. 表示されるボックスに、許可するドメイン（例：`ourcompany.com`）を入力し、次に「**ドメインを追加**」をクリックします。

1. 上記の手順を繰り返して、許可する他のドメインを追加します。
1. 完了したら、「**保存**」をクリックします。
