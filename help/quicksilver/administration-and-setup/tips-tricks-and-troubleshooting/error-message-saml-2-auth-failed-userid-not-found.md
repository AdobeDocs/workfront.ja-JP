---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラーメッセージ：SAML 2.0 認証に失敗しました：ユーザー識別子が見つかりません」
description: SAML 2.0 を使用している場合、「SAML 2.0 Authentication Failed-User Identifier Not Found」というエラーは、UID ID または名前 ID が ADFS 要求規則から渡されないことを意味します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 80%

---

# エラーメッセージ：SAML 2.0 認証失敗：ユーザーの識別子が見つかりません

## 問題

SAML 2.0 を使用すると、「SAML 2.0 認証に失敗しました：ユーザー識別子が見つかりません。」というエラーが表示されます。

## 原因

これは、**UID** または&#x200B;**名前 ID** が **ADFS 要求ルール** から渡されない場合に発生します。

ADFS では、**証明書利用者の信頼**&#x200B;には、**UID** または&#x200B;**名前 ID** 値を渡す&#x200B;**要求ルール**&#x200B;が必要です。**[!DNL Workfront]テスト接続**&#x200B;を実行すると、成功した場合は、次のように表示されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!DNL Workfront] 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ソリューション

1. **[!UICONTROL 証明書利用者の信頼]**／オブジェクトを選択／**[!UICONTROL 要求ルールを編集]**&#x200B;で **[!UICONTROL ADFS 情報]**&#x200B;を編集する場合。

1. **[!UICONTROL LDAP 属性]**（左の列）には、**[!UICONTROL メールアドレス]**（または任意の一意の識別子）が必要です。

1. **[!UICONTROL 発信する要求のタイプ]**（右列）は&#x200B;**[!UICONTROL 名前 ID]** である必要があります。

   >[!NOTE]
   >
   >LDAP 属性のメールアドレスを持つ必要はありません。ユーザーを識別する任意の一意の識別子を使用できますが、それを&#x200B;**名前 ID** として [!DNL Adobe Workfront] に渡す必要があります。
