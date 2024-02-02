---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: カスタム OAuth2 アプリケーションの表示と管理
description: Adobe Workfront 管理者は、Workfront のインスタンス用の OAuth2 アプリケーションを表示および管理し、他のアプリケーションが Workfront にアクセスできるようにします。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: ht
source-wordcount: '702'
ht-degree: 100%

---

# カスタム OAuth2 アプリケーションの表示と管理

[!DNL Adobe Workfront] 管理者は、[!DNL Workfront] のインスタンス用の OAuth2 アプリケーションを表示および管理し、他のアプリケーションが [!UICONTROL Workfront] にアクセスできるようにします。

>[!NOTE]
>
>OAuth2 のコンテキストで「Oauth2 アプリケーション」とは、アプリと [!DNL Workfront] などのサーバー間のこの種のアクセスリンクを指します。詳しくは、[ [!DNL Workfront]  統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

* カスタム OAuth2 アプリケーションの作成について詳しくは、[ [!DNL Workfront]  統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。
* ユーザーの資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、[認証コードフローを使用した、組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-code-token-flow.md)を参照してください。
* サーバー認証（JWT フロー）を使用した OAuth2 アプリケーションの設定と使用の手順については、[JWT フローを使用した、組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-jwt-flow.md)を参照してください。
* PKCE を使用して OAuth2 アプリケーションを設定および使用する手順については、[PKCE フローを使用した、組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-pkce-flow.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> [!DNL Workfront] 管理者であることが必要です。 </p>
    <p>[!DNL Workfront] 管理者について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに対する完全な管理アクセス権の付与</a>を参照してください。</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

[!UICONTROL OAuth2] アプリケーションを表示または管理するには、組織でこのアプリケーションを作成する必要があります。

詳しくは、[ [!DNL Workfront]  統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

## カスタム OAuth2 アプリケーションの管理

* [カスタム OAuth2 アプリケーションの表示および編集](#view-and-edit-custom-oauth2-applications)
* [カスタム OAuth2 アプリケーションの削除](#delete-custom-oauth2-applications)

### カスタム OAuth2 アプリケーションの表示および編集 {#view-and-edit-custom-oauth2-applications}

1. [!DNL Adobe Workfront] の右上にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン（![](assets/main-menu-icon.png)）をクリックし、**[!UICONTROL 設定]**&#x200B;アイコン（![](assets/gear-icon-settings.png)）をクリックします。

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」をクリックして「**[!UICONTROL OAuth アプリケーション]**」を選択します。
1. 「**[!UICONTROL アプリ統合を作成]**」をクリックします。
1. アプリケーションにマウスを移動して、右端に表示される&#x200B;**[!UICONTROL 編集]**&#x200B;アイコン（![](assets/edit-icon.png)）をクリックします。
1. （オプション）アプリケーションの詳細を編集します。

   OAuth2 および JWT アプリに関連するフィールドについては、[ [!DNL Workfront]  統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

### カスタム OAuth2 アプリケーションの削除 {#delete-custom-oauth2-applications}

1. [!DNL Adobe Workfront] の右上にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン（![](assets/main-menu-icon.png)）をクリックし、**[!UICONTROL 設定]**&#x200B;アイコン（![](assets/gear-icon-settings.png)）をクリックします。

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」をクリックして「**[!UICONTROL OAuth アプリケーション]**」を選択します。
1. **  ** をクリックします。
1. アプリケーションにマウスを移動して、右端に表示される&#x200B;**[!UICONTROL 削除]**&#x200B;アイコン（![](assets/delete.png)）をクリックします。

## OAuth2 アプリケーションでのクライアントシークレットの管理

* [クライアントシークレットの詳細の表示](#view-client-secret-details)
* [クライアントシークレットのメモの追加または編集](#add-or-edit-notes-for-client-secret)
* [クライアントシークレットの削除](#delete-client-secret)

### クライアントシークレットの詳細の表示 {#view-client-secret-details}

>[!IMPORTANT]
>
>クライアントシークレット自体は表示できません。クライアントシークレットがわからなくなった場合は、そのシークレットを削除して新しく作成する必要があります。
>
>* クライアントシークレットを削除するには、この記事の[クライアントシークレットの削除](#delete-client-secret)を参照してください。
>* 新しいクライアントシークレットを作成するには、[ [!DNL Workfront]  統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)の [OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md#create)を参照してください。
>



1. [!DNL Adobe Workfront] の右上にある **[!UICONTROL メインメニュー]** アイコン（![](assets/main-menu-icon.png)）、**[!UICONTROL 設定]**&#x200B;アイコン（![](assets/gear-icon-settings.png)）の順にをクリックします。

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」をクリックして「**[!UICONTROL OAuth アプリケーション]**」を選択します。
1. アプリケーションにマウスを移動して、右端に表示される&#x200B;**[!UICONTROL 編集]**&#x200B;アイコンをクリックします。
1. クライアントシークレットエリアで、次の詳細を表示します。

   * 作成日
   * 最終使用日
   * メモ

     クライアントシークレットにメモを追加するには、[クライアントシークレットのメモの追加と編集](#add-or-edit-notes-for-client-secret)を参照してください。

### クライアントシークレットのメモの追加または編集 {#add-or-edit-notes-for-client-secret}

1. [!DNL Adobe Workfront] の右上隅で&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」、「**[!UICONTROL OAuth アプリケーション]**」の順に選択します。
1. 「**[!UICONTROL アプリ統合を作成]**」をクリックします。
1. アプリケーションにポインタを合わせて、右端に表示される&#x200B;**[!UICONTROL 編集]**&#x200B;アイコンをクリックします。
1. メモを追加または編集するクライアントシークレットを見つけます。
1. クライアントシークレットの詳細を含むボックスをクリックします。

   メモテキストを追加したり、既存のメモのテキストを編集したりできるようになりました。

   >[!NOTE]
   >
   >メモテキストには、最大 64 文字まで入力できます。

1. すぐに使用できるボタンをクリックするか、**[!UICONTROL Enter]** キーをクリックしてメモテキストを保存します。

### クライアントシークレットの削除 {#delete-client-secret}

1. [!DNL Adobe Workfront]の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」、「**[!UICONTROL OAuth アプリケーション]**」を選択します。
1. 「**[!UICONTROL アプリ統合を作成]**」をクリックします。
1. アプリケーションにポインタを合わせて、右端に表示される&#x200B;**[!UICONTROL 編集]**&#x200B;アイコンをクリックします。
1. 削除するクライアントシークレットを見つけます。
1. クライアントシークレットの横にある&#x200B;**[!UICONTROL 削除]**&#x200B;アイコン ![](assets/delete.png) をクリックします。
