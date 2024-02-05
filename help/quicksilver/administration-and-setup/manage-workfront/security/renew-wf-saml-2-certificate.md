---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,セキュリティ,証明書,管理者,免除,設定,メタデータ
navigation-topic: security
title: Adobe Workfront SAML 2.0 メタデータ証明書の更新
description: Adobe Workfront サーバーでは、認証と承認に SAML 2.0 プロトコルを利用します。更新後、新しい証明書は 1 年間有効です。 ID プロバイダーで証明書を更新すると、この変更が必要であることを示す警告がWorkfrontに表示されます。 Workfront 管理者は、この変更をシステムレベルで管理できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: aec61210cf2c17775738db4975ae8d19223153cc
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 58%

---

# Adobe Workfront SAML 2.0 メタデータ証明書の更新

>[!IMPORTANT]
>
>このページで説明する手順は、Admin Console にまだ登録されていない組織にのみ適用されます。組織が Adobe Admin Console にオンボーディングされている場合、アクションは必要ありません。
>
>組織が Adobe Admin Console にオンボーディングされているかどうかに応じて異なる手順のリストについて詳しくは、[プラットフォームベースの管理上の違い（Adobe Workfront/Adobe Business Platform）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

Adobe Workfront サーバーでは、認証と承認に SAML 2.0 プロトコルを利用します。更新後、新しい証明書は 1 年間有効です。 ID プロバイダーで証明書を更新すると、この変更が必要であることを示す警告がWorkfrontに表示されます。 Workfront 管理者は、この変更をシステムレベルで管理できます。

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>組織の Workfront インスタンスが Adobe IMS によって有効化されている場合は使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。

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
  <td> <p>新規：標準 </p>
 <p>または</p> 
<p>現在：プラン </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Workfront 内で SAML 2.0 を設定

警告メッセージを精査し、ID プロバイダーでの SAML 2.0 メタデータの更新を確認するには、次の手順に従います。

1. Adobe Workfront の右上隅で、**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**設定** ![](assets/gear-icon-settings.png)」の順にクリックします。

1. **システム**／**シングル サインオン**&#x200B;をクリックします。

1. **タイプ**&#x200B;ドロップダウンメニューで、「**SAML 2.0**」を選択します。

1. 「**SAML 2.0 メタデータのダウンロード**」をクリックします。

   SAML 2.0 用に更新されたWorkfront証明書がダウンロードされます。この証明書には、サーバー用の正しいメタデータが含まれています。

1. ID プロバイダーで、現在のアサーションコンシューマーサービス (ACS) の URL（返信 URL とも呼ばれます）を安全な場所にコピーします。

   >[!CAUTION]
   >
   >手順 6 で Workfront メタデータをシングルサインオン（SSO）プロバイダーにアップロードする前に、現在のアサーション消費者サービス（ACS）の URL を安全な場所にコピーします。この URL（返信 URL とも呼ばれます）は、SSO プロバイダーの Workfront 設定ページにあります。
   >
   >
   >Workfront メタデータのアップロード後に ACS URL が変更された場合は、メタデータに含まれている ACS URL が正しくない可能性があります。シングルサインオンの接続が切断されないように、コピーしたものに戻す必要があります。この操作を行った後も、更新された証明書は正しいままです。

1. ID プロバイダーサーバーで、ダウンロードした新しい証明書を更新します。
1. （条件付き）アサーションコンシューマーサービス (ACS) の URL または返信 URL が ID プロバイダーで変更された場合は、手順 5 でコピーした URL に戻します。
1. Workfront の&#x200B;**シングルサインオン(SSO)** ページで、「**新しい Workfront 証明書がすでに ID プロバイダにアップロードされています**」というオプションが選択されていることを確認します。

   >[!NOTE]
   >
   >* このオプションは、次のすべてに該当する場合にのみ表示されます。
   >   * 組織は既に SAML 2.0 用に設定されています
   >   * 現在の証明書の有効期限が切れる準備が整いました
   >   * 新しい証明書が使用可能です
   >* このフィールドを選択すると、Workfront管理者は SSO 資格情報またはWorkfront資格情報を使用してWorkfrontにログインできます。

1. 「**保存**」をクリックします。

   ID プロバイダーのサーバーで SAML 2.0 証明書の更新を確認したので、警告メッセージが表示されなくなりました。

1. クリック **接続をテスト** 設定をテストするには、をクリックします。

   接続が成功したことを確認するメッセージが表示されます。

詳細情報やメタデータの手動設定に関するサポートについては、サポートチームにお問い合わせください ( [カスタマーサポートに連絡](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
