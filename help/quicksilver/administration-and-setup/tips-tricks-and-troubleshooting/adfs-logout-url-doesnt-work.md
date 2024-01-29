---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS ログアウト URL が機能しません
description: このページで説明する手順は、まだAdobe Admin Consoleにオンボーディングされていない組織にのみ適用されます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: 4a9936b6bc034f2176167fc3939d647ee679a888
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# ADFS ログアウト URL が機能しません

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>このページで説明する手順は、まだ [!UICONTROL Adobe Admin Console].
>
>組織が [!UICONTROL Adobe Admin Console]を参照してください。 [プラットフォームベースの管理上の違い ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## 問題

ADFS ログアウト URL(https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0) を使用すると、「サイトへのアクセス中に問題が発生しました。 もう一度サイトを参照してみてください。」

問題が解決しない場合は、このサイトの管理者に問い合わせ、次の参照番号を入力して問題を特定してください。 **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

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
   <td role="rowheader">Adobe [!DNL Workfront] ライセンス</td> 
   <td> 
   <p>新規：標準</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 解決策

1. ADFS マネージャーサーバーで、に移動します。 **[!UICONTROL 信頼関係]** > **[!UICONTROL 証明書利用者信託]** > `<your party trust>` プロパティ。

1. の下 **[!UICONTROL エンドポイント]** タブ、クリック **[!UICONTROL 追加]**.

1. **[!UICONTROL エンドポイントのタイプ]** = SAML ログアウト、バインディング=POST、URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   別のページにリダイレクトする場合は、応答 URL を設定できます。 ただし、ADFS サイトは、ログオフしたと警告するので、お勧めします。ただし、ブラウザーは閉じる必要があります。
