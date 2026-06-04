---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: メール許可リストを設定
description: 組織が Workfront エンタープライズプランを使用する場合は、Workfront メール許可リストを作成して、どのメールドメインが Workfront からのメールの受け入れを許可するか、そしてユーザーがユーザープロファイルで指定するメールアドレスにどのメールドメインを含めることができるかを制御できます。 これは、組織のセキュリティポリシーにより、ユーザーが Workfront に保存されているデータを外部のメールアドレスに送信できないように制限されている場合に便利です。会社の内部ドメインのみを許可リストに含めることにより、このポリシーが確実に遵守されます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
TQID: https://experienceleague.adobe.com/a8hcTFpx3LmuGpQM8Wk8BpLDCFUVJWLAcP-YV5ogK0U
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 403
ht-degree: 89%

---

# メール許可リストの設定

組織でWorkfront Enterprise プランを使用している場合は、Workfrontのメール許可リストに加えるを作成して制御できます。

* Workfront からのメールを受け入れることが許可されているメールドメイン。
* ユーザープロファイルでユーザーが指定したメールアドレスに含めることができるメールドメイン。

これは、組織のセキュリティポリシーにより、ユーザーが Workfront に保存されているデータを外部のメールアドレスに送信できないように制限されている場合に便利です。会社の内部ドメインのみを許可リストに含めることにより、このポリシーが確実に遵守されます。

>[!IMPORTANT]
>
>IT チームは、`notifications@my.workfront.com` から送信されるメールが組織のシステムでブロックされていないことを確認する必要があります。
>
>Workfront からのメールは、メール配信の成功率を高め、メールのなりすましを排除するために、すべてそのアドレスから送信されます。 これには、自動アラートとユーザー間通信の両方が含まれます。
>
>例えば、Joan Harrisという名前のユーザーから受け取ったWorkfrontの電子メールの「差出人」行は、次のようになります。
>`Joan Harris <notifications@my.workfront.com>`

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

ファイアウォールやメールサーバーが、特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の IP アドレスをその許可リストに追加する必要があります。 これにより、環境と Adobe Workfront サーバー間の通信が開始されます。 詳しくは、[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

## メール許可リストの設定

{{step-1-to-setup}}

1. **システム**／**顧客情報**&#x200B;をクリックします。
1. 「**メールの許可リスト**」セクションで、「**ドメインの許可リストを有効にする**」を選択し、次に「**ドメインを追加**」をクリックします。
1. 表示されるボックスに、許可するドメイン（例：`ourcompany.com`）を入力し、次に「**ドメインを追加**」をクリックします。
1. 上記の手順を繰り返して、許可する他のドメインを追加します。
1. 完了したら、「**保存**」をクリックします。
