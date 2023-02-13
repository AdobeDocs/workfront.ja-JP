---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'エラーメッセージ：SAML 2.0 認証失敗：ユーザー識別子が見つかりません'
description: SAML 2.0 を使用している場合、「SAML 2.0 Authentication Failed-User Identifier Not Found」というエラーは、UID または NAME ID が ADFS 要求ルールから渡されないことを意味します。 ADFS では、証明書利用者信頼には、UID または NAME ID 値を渡す要求規則が必要です。 実行時に [!DNL Workfront] 接続をテストする。成功した場合は、次のように表示されます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---

# エラーメッセージ：SAML 2.0 認証失敗：ユーザー識別子が見つかりません

## 問題

SAML 2.0 を使用すると次のエラーが表示されます。「SAML 2.0 認証に失敗しました：ユーザー識別子が見つかりません。」

## 原因

これは、 **UID** または **名前 ID** が **ADFS 要求ルール**.

ADFS では、 **証明書利用者信頼** を持つ必要がある **要求ルール** それは **UID** または **名前 ID** の値です。 実行時に **[!DNL Workfront]接続をテスト**&#x200B;成功した場合は、と表示されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決策

1. を編集する際に **[!UICONTROL ADFS 情報]**、 **[!UICONTROL 証明書利用者信託]** /オブジェクトを選択 >**[!UICONTROL 要求ルールの編集]**.

1. この **[!UICONTROL LDAP 属性]** （左の列）は、 **[!UICONTROL 電子メールアドレス]** （または一意の ID）。

1. この **[!UICONTROL 送信する要求の種類]** （右列） **[!UICONTROL 名前 ID]**.

   >[!NOTE]
   >
   >LDAP 属性の電子メールアドレスを指定する必要はありません。 ユーザーを識別する一意の識別子を使用できますが、に渡す必要があります。 [!DNL Adobe Workfront] を **名前 ID**.
