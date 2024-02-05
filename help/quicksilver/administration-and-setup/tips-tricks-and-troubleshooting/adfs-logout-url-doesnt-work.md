---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS ログアウト URL が機能しません
description: このページで説明する手順は、まだ Adobe Admin Console にオンボーディングされていない組織にのみ適用されます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: 4a9936b6bc034f2176167fc3939d647ee679a888
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 92%

---

# ADFS ログアウト URL が機能しません

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>このページで説明する手順は、まだ [!UICONTROL Adobe Admin Console] にオンボーディングされていない組織にのみ適用されます。
>
>組織が [!UICONTROL Adobe Admin Console] にオンボーディングされている場合は、[プラットフォームベースの管理上の違い（[!DNL Adobe Workfront]/[!DNL Adobe Business Platform]）](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

## 問題

ADFS ログアウト URL（https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0）を使用すると、次のエラーを含むメッセージページが表示されます。「サイトへのアクセス中に問題が発生しました。もう一度サイトを参照してみてください。」

問題が解決しない場合は、このサイトの管理者に問い合わせ、次の参照番号を入力して問題を特定してください。**57092dfc-751a-4915-8e6a-b4c5d413f8c6**

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
   <td role="rowheader">Adobe [!DNL Workfront] ライセンス</td> 
   <td> 
   <p>新規：標準</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## ソリューション

1. ADFS マネージャーサーバーで、次の順序で移動します。**[!UICONTROL 信頼関係]**／**[!UICONTROL 証明書利用者の信頼]**／`<your party trust>` プロパティ。

1. 「**[!UICONTROL エンドポイント]**」タブの下の、「**[!UICONTROL 追加]**」をクリックします。

1. **[!UICONTROL エンドポイントのタイプ]** = SAML Logout, Binding = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   別のページにリダイレクトする場合は、応答 URL を設定できます。ただし、ADFS サイトをお勧めします。これがログオフしていることを警告するためですが、それでもブラウザーを閉じる必要があります。
