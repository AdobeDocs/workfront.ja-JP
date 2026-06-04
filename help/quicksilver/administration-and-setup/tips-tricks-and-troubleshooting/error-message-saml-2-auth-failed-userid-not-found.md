---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: エラーメッセージ：SAML 2.0認証に失敗しました：ユーザー識別子が見つかりません
description: SAML 2.0を使用している場合、「SAML 2.0 Authentication Failed-User Identifier Not Found」というエラーが発生すると、UIDまたはNAME IDがADFS要求ルールから渡されなくなります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
TQID: https://experienceleague.adobe.com/YxLEE1OvD-Wo3FSd5ewXMfijsTaCjjCjzAx-EWWlBPE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 225
ht-degree: 81%

---

# エラーメッセージ：SAML 2.0 認証失敗：ユーザーの識別子が見つかりません

## 問題

SAML 2.0 を使用すると、「SAML 2.0 認証に失敗しました：ユーザー識別子が見つかりません。」というエラーが表示されます。

## 原因

これは、**UID** または&#x200B;**名前 ID** が **ADFS 要求ルール** から渡されない場合に発生します。

ADFS では、**証明書利用者の信頼**&#x200B;には、**UID** または&#x200B;**名前 ID** 値を渡す&#x200B;**要求ルール**&#x200B;が必要です。 **[!DNL Workfront]テスト接続**&#x200B;を実行すると、成功した場合は、次のように表示されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ソリューション

1. **[!UICONTROL 証明書利用者の信頼]**／オブジェクトを選択／**[!UICONTROL 要求ルールを編集]**&#x200B;で **[!UICONTROL ADFS 情報]**&#x200B;を編集する場合。

1. **[!UICONTROL LDAP 属性]**（左の列）には、**[!UICONTROL メールアドレス]**（または任意の一意の識別子）が必要です。

1. **[!UICONTROL 発信する要求のタイプ]**（右列）は&#x200B;**[!UICONTROL 名前 ID]** である必要があります。

   >[!NOTE]
   >
   >LDAP 属性のメールアドレスを持つ必要はありません。 ユーザーを識別する任意の一意の識別子を使用できますが、それを&#x200B;**名前 ID** として [!DNL Adobe Workfront] に渡す必要があります。
