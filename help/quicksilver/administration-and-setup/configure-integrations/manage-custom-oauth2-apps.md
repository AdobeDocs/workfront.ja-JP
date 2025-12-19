---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: カスタム OAuth2 アプリケーションの表示と管理
description: Adobe Workfront 管理者は、Workfront のインスタンス用の OAuth2 アプリケーションを表示および管理し、他のアプリケーションが Workfront にアクセスできるようにします。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 31e5f5e039e25fa25f3038c23ee579ba1f830bb7
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 80%

---

# カスタム OAuth2 アプリケーションの表示と管理

[!DNL Adobe Workfront] 管理者は、[!DNL Workfront] のインスタンス用の OAuth2 アプリケーションを表示および管理し、他のアプリケーションが [!UICONTROL Workfront] にアクセスできるようにします。

>[!NOTE]
>
>* OAuth2 のコンテキストで「Oauth2 アプリケーション」とは、アプリと [!DNL Workfront] などのサーバー間のこの種のアクセスリンクを指します。詳しくは、[ [!DNL Workfront]  統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。
>* 一度に最大 10 個の OAuth2 アプリケーションを持つことができます。

* カスタム OAuth2 アプリケーションの作成の詳細情報、手順および詳細については、[ 統合用の OAuth2 アプリケーションの作成  [!DNL Workfront]  を参照してください ](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* ユーザー資格情報を含む OAuth2 アプリケーション（認証コードフロー）の設定と使用に関する情報、手順、詳細については、[ 認証コードフローを使用した組織のカスタム OAuth 2 アプリケーションの設定と使用 ](../../wf-api/api/oauth-app-code-token-flow.md) を参照してください。
* サーバー認証（JWT フロー）を使用した OAuth2 アプリケーションの設定と使用に関する情報、手順、詳細については、[JWT フローを使用した組織のカスタム OAuth 2 アプリケーションの設定と使用 ](../../wf-api/api/oauth-app-jwt-flow.md) を参照してください。
* PKCE を使用して OAuth2 アプリケーションを設定および使用する手順については、[PKCE フローを使用した、組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-pkce-flow.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p> <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>Workfront 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

[!UICONTROL OAuth2] アプリケーションを表示または管理するには、組織でこのアプリケーションを作成する必要があります。

詳しくは、[ [!DNL Workfront]  統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

## カスタム OAuth2 アプリケーションの管理

* [カスタム OAuth2 アプリケーションの表示および編集](#view-and-edit-custom-oauth2-applications)
* [カスタム OAuth2 アプリケーションの削除](#delete-custom-oauth2-applications)

### カスタム OAuth2 アプリケーションの表示および編集 {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」をクリックして「**[!UICONTROL OAuth アプリケーション]**」を選択します。
1. 「**[!UICONTROL アプリ統合を作成]**」をクリックします。
1. アプリケーションの上にマウスポインターを置き、右端に表示されている **[!UICONTROL 編集]**![ 編集アイコン ](assets/edit-icon.png) をクリックします。
1. （オプション）アプリケーションの詳細を編集します。

   OAuth2 および JWT アプリに関連するフィールドについては、[ [!DNL Workfront]  統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

### カスタム OAuth2 アプリケーションの削除 {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」をクリックして「**[!UICONTROL OAuth アプリケーション]**」を選択します。
1. アプリケーションの上にマウスポインターを置き、右端に表示されたら **[!UICONTROL 削除]**![ 削除 ](assets/delete.png) をクリックします。

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

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」をクリックして「**[!UICONTROL OAuth アプリケーション]**」を選択します。
1. アプリケーションにマウスを移動して、右端に表示される&#x200B;**[!UICONTROL 編集]**&#x200B;アイコンをクリックします。
1. クライアントシークレットエリアで、次の詳細を表示します。

   * 作成日
   * 最終使用日
   * メモ

     クライアントシークレットにメモを追加するには、[クライアントシークレットのメモの追加と編集](#add-or-edit-notes-for-client-secret)を参照してください。

### クライアントシークレットのメモの追加または編集 {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」をクリックして「**[!UICONTROL OAuth アプリケーション]**」を選択します。
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

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、「**[!UICONTROL システム]**」をクリックして「**[!UICONTROL OAuth アプリケーション]**」を選択します。
1. 「**[!UICONTROL アプリ統合を作成]**」をクリックします。
1. アプリケーションにポインタを合わせて、右端に表示される&#x200B;**[!UICONTROL 編集]**&#x200B;アイコンをクリックします。
1. 削除するクライアントシークレットを見つけます。
1. クライアントシークレットの横にある **[!UICONTROL 削除]** アイコン ![ 削除 ](assets/delete.png) をクリックします。
