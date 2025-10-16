---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: メールの設定許可リスト
description: 組織が Workfront エンタープライズプランを使用する場合は、Workfront メール許可リストを作成して、どのメールドメインが Workfront からのメールの受け入れを許可するか、そしてユーザーがユーザープロファイルで指定するメールアドレスにどのメールドメインを含めることができるかを制御できます。これは、組織のセキュリティポリシーにより、ユーザーが Workfront に保存されているデータを外部のメールアドレスに送信できないように制限されている場合に便利です。会社の内部ドメインのみを許可リストに含めることにより、このポリシーが確実に遵守されます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: 15ea03bf586054f7ef421f8cacede6f42835a6e4
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 91%

---

# メール許可リストの設定

Workfront エンタープライズプランを使用している場合は、以下を管理するWorkfront メール許可リストを作成できます。

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
>&#x200B;>`Joan Harris <notifications@my.workfront.com>`

ご使用の環境と Adobe Workfront サーバー間の通信を開くための組織のファイアウォールの設定について詳しくは、[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p> <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>Workfront 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## その他の許可リスト

ファイアウォールやメールサーバーが、特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをその許可リストに追加する必要があります。これにより、環境と Adobe Workfront サーバー間の通信が開始されます。詳しくは、[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

## メール許可リストの設定

{{step-1-to-setup}}

1. **システム**／**顧客情報**&#x200B;をクリックします。
1. 「**メールの許可リスト**」セクションで、「**ドメインの許可リストを有効にする**」を選択し、次に「**ドメインを追加**」をクリックします。
1. 表示されるボックスに、許可するドメイン（例：`ourcompany.com`）を入力し、次に「**ドメインを追加**」をクリックします。
1. 上記の手順を繰り返して、許可する他のドメインを追加します。
1. 完了したら、「**保存**」をクリックします。
