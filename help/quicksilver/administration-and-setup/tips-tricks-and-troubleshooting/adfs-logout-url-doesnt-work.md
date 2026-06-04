---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS ログアウト URLが機能しない
description: このページで説明する手順は、まだ Adobe Admin Console にオンボーディングされていない組織にのみ適用されます。
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
TQID: https://experienceleague.adobe.com/RRaLL70JcSBcvoS6EUFuWj5Ejwljekt4QuQ3kXDx-44
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 250
ht-degree: 80%

---

# ADFS ログアウト URL が機能しません

<!-- Audited: 1/2024 -->

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>このページに記載されている手順は、[!UICONTROL Adobe Admin Console]にまだオンボーディングされていない組織にのみ適用されます。
>
>現在すべての組織がAdobe Admin Consoleに登録されているため、この記事は近い将来に削除されます。
>
>組織が [!UICONTROL Adobe Admin Console] にオンボーディングされている場合は、[プラットフォームベースの管理上の違い（[!DNL Adobe Workfront]/[!DNL Adobe Business Platform]）](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

## 問題

ADFS ログアウト URL（https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0）を使用すると、次のエラーを含むメッセージページが表示されます。「サイトへのアクセス中に問題が発生しました。 もう一度サイトを参照してみてください。」

問題が解決しない場合は、このサイトの管理者に問い合わせ、次の参照番号を入力して問題を特定してください。**57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] ライセンス</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>  
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ソリューション

1. ADFS マネージャーサーバーで、次の順序で移動します。**[!UICONTROL 信頼関係]**／**[!UICONTROL 証明書利用者の信頼]**／`<your party trust>` プロパティ。

1. 「**[!UICONTROL エンドポイント]**」タブの下の、「**[!UICONTROL 追加]**」をクリックします。

1. **[!UICONTROL エンドポイントのタイプ]** = SAML Logout, Binding = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   別のページにリダイレクトする場合は、応答 URL を設定できます。 ただし、ADFS サイトをお勧めします。これがログオフしていることを警告するためですが、それでもブラウザーを閉じる必要があります。
