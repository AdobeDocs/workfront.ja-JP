---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Workfrontおよび SAML 2.0 での Outlook の使用を有効にする
description: SAML 2.0 認証を有効にし、ユーザーが SAML 2.0 資格情報を使用してMicrosoft Outlook からWorkfrontにログインできるようにする場合は、Office アドインで SAML 2.0 を有効にして認証を行う必要があります。
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# Workfrontおよび SAML 2.0 での Outlook の使用を有効にする

SAML 2.0 認証を有効にし、ユーザーが SAML 2.0 資格情報を使用してMicrosoft Outlook からWorkfrontにログインできるようにする場合は、Office アドインで SAML 2.0 を有効にして認証を行う必要があります。

>[!NOTE]
>
>組織のWorkfrontインスタンスがカスタム SSO ポータルを使用している場合は使用できません。>
><!--
>or is enabled with Adobe IMS>
>-->
>詳細については、ネットワークまたは IT 管理者にお問い合わせください。

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

## Workfrontおよび SAML 2.0 での Outlook の使用を有効にする

1. クリック **設定** グローバルナビゲーションバーのAdobe Workfrontの右上隅付近
1. クリック **システム** > **環境設定**.

1. 内 **セキュリティ** セクションで、 **Office 365 アドインで SAML 2.0 認証を許可する**&#x200B;が有効になっている。

   このオプションを使用すると、Office 365 アドインの Iframe でのみWorkfrontの埋め込みを有効にできます。 クリック可能なコンテンツが含まれていないので、クリックジャッキング違反は発生しません。

   このオプションは、デフォルトで有効になっています。

   >[!NOTE]
   >
   >このオプションを有効にした場合 **iframe へのWorkfrontの埋め込みを許可**、オプション **Office 365 アドインで SAML 2.0 認証を許可する** はグレー表示になり、有効になります。
   >
   >![](assets/if-you-enable.png)

1. 「**保存**」をクリックします。

   ここで保存した変更は、Workfrontのすべてのユーザーのエクスペリエンスに影響します。
