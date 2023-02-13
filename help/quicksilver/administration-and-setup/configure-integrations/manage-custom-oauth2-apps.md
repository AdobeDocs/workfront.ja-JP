---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: カスタム OAuth2 アプリケーションの表示と管理
description: Adobe Workfront管理者は、Workfrontのインスタンスに関する OAuth2 アプリケーションを表示および管理できます。これにより、他のアプリケーションがWorkfrontにアクセスできるようになります。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# カスタム OAuth2 アプリケーションの表示と管理

As a [!DNL Adobe Workfront] 管理者は、 [!DNL Workfront]（他のアプリケーションがにアクセスできるようにする） [!UICONTROL Workfront].

>[!NOTE]
>
>OAuth2 のコンテキストでは、「Oauth2 アプリケーション」とは、次のようなアプリとサーバー間のこの種のアクセスリンクを指します。 [!DNL Workfront]. 詳しくは、 [用の OAuth2 アプリケーションの作成 [!DNL Workfront] 統合](../../administration-and-setup/configure-integrations/create-oauth-application.md)

* カスタム OAuth2 アプリケーションの作成について詳しくは、 [用の OAuth2 アプリケーションの作成 [!DNL Workfront] 統合](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* ユーザー資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、 [認証コードフローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-code-token-flow.md).
* サーバー認証（JWT フロー）を使用した OAuth2 アプリケーションの設定と使用の手順については、 [JWT フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-jwt-flow.md).
* PKCE を使用して OAuth2 アプリケーションを設定および使用する手順については、 [PKCE フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-pkce-flow.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> 次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 </p>
    <p>詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

次を作成する必要があります： [!UICONTROL OAuth2] アプリケーションを表示または管理する前に、組織のアプリケーションを使用してください。

詳しくは、 [用の OAuth2 アプリケーションの作成 [!DNL Workfront] 統合](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## カスタム OAuth2 アプリケーションの管理

* [カスタム OAuth2 アプリケーションの表示と編集](#view-and-edit-custom-oauth2-applications)
* [カスタム OAuth2 アプリケーションを削除します](#delete-custom-oauth2-applications)

### カスタム OAuth2 アプリケーションの表示と編集 {#view-and-edit-custom-oauth2-applications}

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth アプリケーション]**.
1. クリック **[!UICONTROL アプリ統合の作成]**.
1. アプリケーションの上にマウスポインターを置いて、「 **[!UICONTROL 編集]** ![](assets/edit-icon.png) 最も右側に現れる時
1. （オプション）アプリケーションの詳細を編集します。

   OAuth2 および JWT アプリに関連するフィールドについては、 [用の OAuth2 アプリケーションの作成 [!DNL Workfront] 統合](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### カスタム OAuth2 アプリケーションを削除します {#delete-custom-oauth2-applications}

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth アプリケーション]**.
1. クリック **  **.
1. アプリケーションの上にマウスポインターを置いて、「 **[!UICONTROL 削除]** ![](assets/delete.png) 最も右側に現れる時

## OAuth2 アプリケーションでのクライアントシークレットの管理

* [クライアントシークレットの詳細を表示](#view-client-secret-details)
* [クライアントシークレットのメモを追加または編集](#add-or-edit-notes-for-client-secret)
* [クライアント秘密鍵を削除](#delete-client-secret)

### クライアントシークレットの詳細を表示 {#view-client-secret-details}

>[!IMPORTANT]
>
>クライアントシークレット自体は表示できません。 クライアントシークレットを失った場合は、そのシークレットを削除して新しく作成する必要があります。
>
>* クライアントシークレットを削除するには、 [クライアント秘密鍵を削除](#delete-client-secret) 」を参照してください。
>* 新しいクライアントシークレットを作成するには、 [OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [用の OAuth2 アプリケーションの作成 [!DNL Workfront] 統合](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>




1. 次をクリック： *[!UICONTROL *メインメニュー]**アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth アプリケーション]**.
1. アプリケーションの上にマウスポインターを置いて、 **[!UICONTROL 編集]** アイコンが表示されます。
1. クライアントシークレット領域に詳細を表示します。

   * 作成日
   * 最終使用日
   * メモ

      クライアントシークレットにメモを追加するには、 [クライアントシークレットのメモを追加または編集](#add-or-edit-notes-for-client-secret).

### クライアントシークレットのメモを追加または編集 {#add-or-edit-notes-for-client-secret}

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth アプリケーション]**.
1. クリック **[!UICONTROL アプリ統合の作成]**.
1. アプリケーションの上にマウスポインターを置いて、 **[!UICONTROL 編集]** アイコンが表示されます。
1. メモを追加または編集するクライアント秘密鍵を探します。
1. クライアントシークレットの詳細を含むボックスをクリックします。

   注記テキストを追加したり、既存の注記テキストを編集したりできるようになりました。

   >[!NOTE]
   >
   >メモテキストには、最大 64 文字まで入力できます。

1. すぐに使用できるボタンをクリックするか、 **[!UICONTROL 入力]** をクリックしてメモテキストを保存します。

### クライアント秘密鍵を削除 {#delete-client-secret}

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth アプリケーション]**.
1. クリック **[!UICONTROL アプリ統合の作成]**.
1. アプリケーションの上にマウスポインターを置いて、 **[!UICONTROL 編集]** アイコンが表示されます。
1. 削除するクライアント秘密鍵を見つけます。
1. 次をクリック： **[!UICONTROL 削除]** アイコン ![](assets/delete.png) をクリックします。
