---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラーメッセージ：SAML 2.0 認証失敗：ユーザーの識別子が見つかりません」
description: SAML 2.0 を使用している場合、「SAML 2.0 認証失敗：ユーザーの識別子が見つかりません」というエラーは、UID または名前 ID が ADFS 要求ルールから渡されないことを意味します。ADFS では、証明書利用者の信頼には、UID または名前 ID 値を渡す要求ルールが必要です。 [!DNL Workfront]  テスト接続を実行すると、成功した場合は、次のように表示されます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: ht
source-wordcount: '292'
ht-degree: 100%

---

# エラーメッセージ：SAML 2.0 認証失敗：ユーザーの識別子が見つかりません

## 問題

SAML 2.0 を使用すると、「SAML 2.0 認証に失敗しました：ユーザー識別子が見つかりません。」というエラーが表示されます。

## 原因

これは、**UID** または&#x200B;**名前 ID** が **ADFS 要求ルール** から渡されない場合に発生します。

ADFS では、**証明書利用者の信頼**&#x200B;には、**UID** または&#x200B;**名前 ID** 値を渡す&#x200B;**要求ルール**&#x200B;が必要です。**[!DNL Workfront]テスト接続**&#x200B;を実行すると、成功した場合は、次のように表示されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者であることが必要です。詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ソリューション

1. **[!UICONTROL 証明書利用者の信頼]**／オブジェクトを選択／**[!UICONTROL 要求ルールを編集]**&#x200B;で **[!UICONTROL ADFS 情報]**&#x200B;を編集する場合。

1. **[!UICONTROL LDAP 属性]**（左の列）には、**[!UICONTROL メールアドレス]**（または任意の一意の識別子）が必要です。

1. **[!UICONTROL 発信する要求のタイプ]**（右列）は&#x200B;**[!UICONTROL 名前 ID]** である必要があります。

   >[!NOTE]
   >
   >LDAP 属性のメールアドレスを持つ必要はありません。ユーザーを識別する任意の一意の識別子を使用できますが、それを&#x200B;**名前 ID** として [!DNL Adobe Workfront] に渡す必要があります。
