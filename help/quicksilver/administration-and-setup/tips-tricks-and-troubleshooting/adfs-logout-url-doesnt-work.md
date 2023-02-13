---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS ログアウト URL が機能しません
description: このページで説明する手順は、まだAdobe Admin Consoleにオンボーディングされていない組織にのみ適用されます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# ADFS ログアウト URL が機能しません

>[!IMPORTANT]
>
>このページで説明する手順は、まだ [!UICONTROL Adobe Admin Console].
>
>組織が [!UICONTROL Adobe Admin Console]を参照してください。 [プラットフォームベースの管理上の違い ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## 問題

ADFS ログアウト URL(https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0) を使用すると、次のエラーを含むメッセージページが表示されます。「サイトへのアクセス中に問題が発生しました。 もう一度サイトを参照してみてください。」

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
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決策

1. ADFS マネージャーサーバーで、に移動します。 **[!UICONTROL 信頼関係]** > **[!UICONTROL 証明書利用者信託]** > `<your party trust>` プロパティ。

1. 以下 **[!UICONTROL エンドポイント]** タブ、クリック **[!UICONTROL 追加]**.

1. **[!UICONTROL エンドポイントのタイプ]** = SAML ログアウト、バインディング=POST、URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   別のページにリダイレクトする場合は、応答 URL を設定できます。 ただし、ADFS サイトは、ログオフしたと警告するので、お勧めします。ただし、ブラウザーは閉じる必要があります。
