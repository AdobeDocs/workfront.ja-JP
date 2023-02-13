---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0，セキュリティ，証明書，管理者，免除，設定，メタデータ
navigation-topic: security
title: Adobe Workfront SAML 2.0 メタデータ証明書を更新します
description: このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、Adobe Admin Consoleを通じてこの操作を実行する必要があります。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Adobe Workfront SAML 2.0 メタデータ証明書を更新します

>[!IMPORTANT]
>
>このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、操作は必要ありません。
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfrontサーバーは、認証と承認に SAML 2.0 プロトコルを使用します。 更新後、新しい証明書は 1 年間有効です。 ID プロバイダーで証明書を更新すると、この変更が必要であることを示す警告がWorkfrontに表示されます。 Workfront管理者は、この変更をシステムレベルで管理できます。

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>組織のWorkfrontインスタンスで「Adobe IMS」が有効になっている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。

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

## Workfront内での SAML 2.0 の設定

警告メッセージを確認し、ID プロバイダーで SAML 2.0 メタデータの更新を確認するには、次の手順を実行します。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **シングルサインオン**.

1. 内 **タイプ** ドロップダウンメニューで、「 **SAML 2.0**.

1. クリック **SAML 2.0 メタデータのダウンロード**.

   SAML 2.0 用に更新されたWorkfront証明書がダウンロードされます。この証明書には、サーバー用の正しいメタデータが含まれています。

   >[!CAUTION]
   >
   >手順 5 でWorkfrontメタデータをシングルサインオン (SSO) プロバイダーにアップロードする前に、現在のアサーションコンシューマーサービス (ACS) の URL を安全な場所にコピーします。 この URL（返信 URL とも呼ばれます）は、SSO プロバイダーのWorkfront設定ページにあります。
   >
   >
   >Workfrontメタデータのアップロード後に ACS URL が変更された場合は、メタデータに正しくない ACS URL が含まれている可能性があります。 シングルサインオンの接続が壊れないように、コピーしたに変更する必要があります。 この操作を行った後も、更新された証明書は正しく保持されます。

1. ID プロバイダーサーバーに移動し、ダウンロードした新しい証明書を更新します。
1. Workfrontで、 **シングルサインオン (SSO) ページ**&#x200B;で、次のオプションが選択されていることを確認します。 **新しいWorkfront証明書は既に ID プロバイダーにアップロードされています**.

   このフィールドを選択すると、Workfront管理者は SSO 資格情報またはWorkfront資格情報を使用してWorkfrontにログインできます。

1. 「**保存**」をクリックします。

   ID プロバイダーのサーバーで SAML 2.0 証明書の更新を確認したので、警告メッセージが表示されなくなりました。

1. クリック **接続をテスト** 設定をテストする場合。

   接続が成功したことを確認するメッセージが表示されます。

詳細情報やメタデータの手動設定に関するサポートについては、サポートチームにお問い合わせください ( [カスタマーサポートに連絡](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
