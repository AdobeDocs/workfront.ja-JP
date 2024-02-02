---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Workfront と SAML 2.0 での Outlook の使用を有効化
description: SAML 2.0 Authentication を有効にし、ユーザーが SAML 2.0 資格情報を使用して Microsoft Outlook から Workfront にログインできるようにする場合は、Office アドインで SAML 2.0 を有効にして認証を行う必要があります。
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: ht
source-wordcount: '294'
ht-degree: 100%

---

# Workfront と SAML 2.0 での Outlook の使用を有効化

SAML 2.0 Authentication を有効にし、ユーザーが SAML 2.0 資格情報を使用して Microsoft Outlook から Workfront にログインできるようにする場合は、Office アドインで SAML 2.0 を有効にして認証を行う必要があります。

>[!NOTE]
>
>組織の Workfront インスタンスがカスタム SSO Portal を使用している場合は使用できません。>
><!--
>or is enabled with Adobe IMS>
>-->
>詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。

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

## Workfront と SAML 2.0 での Outlook の使用を有効化

1. グローバルナビゲーションバーの Adobe Workfront の右上隅付近で「**設定**」をクリックします。
1. **システム**／**環境設定**&#x200B;をクリックします。

1. 「**セキュリティ**」セクションで、「**Office 365 アドインで SAML 2.0 Authentication を許可**」が有効になっていることを確認します。

   このオプションを使用すると、Office 365 アドインの Iframe でのみ Workfront の埋め込みを有効にすることができます。クリック可能なコンテンツが含まれていないので、クリックジャッキング侵害を起こしません。

   このオプションは、デフォルトで有効になっています。

   >[!NOTE]
   >
   >「**iframe への Workfront の埋め込みを許可**」オプションを有効にする場合、「**Office 365 アドインで SAML 2.0 Authentication を許可**」オプションはグレー表示になり、有効になります。
   >
   >![](assets/if-you-enable.png)
   >

1. 「**保存**」をクリックします。

   ここで保存した変更内容は、Workfront のすべてのユーザーのエクスペリエンスに影響します。
