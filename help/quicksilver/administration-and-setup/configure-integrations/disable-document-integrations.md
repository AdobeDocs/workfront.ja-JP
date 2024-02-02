---
title: ドキュメント統合の無効化
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: ' [!DNL anAdobe] [!DNL Workfront] 管理者は、Workfront とサードパーティのドキュメントプロバイダーとの接続を無効にすることができます。'
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: ht
source-wordcount: '325'
ht-degree: 100%

---

# ドキュメント統合の無効化

[!DNL Adobe] [!DNL Workfront] 管理者は、[!DNL Workfront] とサードパーティのドキュメントプロバイダーとの接続を無効にすることができます。

[!DNL Workfront] とドキュメントプロバイダーの間の接続を無効にすると、ドキュメントへのリンクが [!DNL Workfront] で非表示になります。ユーザーはリンクされたドキュメントを表示できなくなり、[!DNL Workfront] リンクを使用してドキュメントに変更を加えることはできず、そのプロバイダーに他のドキュメントを追加することもできません。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。[!DNL Workfront] 管理者について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## クラウドプロバイダー統合を無効にする

[!UICONTROL Workfront DAM]、[!DNL Box]、[!DNL Dropbox]、[!DNL Google Drive]、[!DNL Microsoft OneDrive]、[!DNL WebDAM] のドキュメント統合を無効にするには：

1. [!DNL Workfront] 管理者として [!DNL Workfront] にログインします。
1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) をクリックします。

1. **[!UICONTROL ドキュメント]**／**[!UICONTROL クラウドプロバイダー]**&#x200B;をクリックします。

1. [!DNL Workfront] から切断するクラウドプロバイダーの選択を解除します。
1. 「**[!UICONTROL 保存]**」をクリックします。

   ユーザーは、無効にした特定のクラウドプロバイダーに接続できず、そのクラウドプロバイダーから Workfront にドキュメントをリンクできなくなりました。

## [!DNL SharePoint] 統合を無効にする

1. [!DNL Workfront] 管理者として [!DNL Workfront] にログインします。
1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) をクリックします。

1. 「**[!UICONTROL ドキュメント]**」を展開し、「**[!UICONTROL [!DNL SharePoint]統合]**」をクリックします。
1. 無効にする [!DNL SharePoint] 統合を選択します。
1. 「**[!UICONTROL 無効にする]**」をクリックします。\
   ユーザーは、無効にした [!DNL SharePoint] サイトに接続できず、[!DNL SharePoint] から [!DNL Workfront] にドキュメントをリンクできなくなりました。

## カスタム統合を無効にする

1. [!DNL Workfront] に管理者としてログインします。
1. [!DNL Adobe Workfront] の右上にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン（![](assets/main-menu-icon.png)）、**[!UICONTROL 設定]**&#x200B;アイコン（![](assets/gear-icon-settings.png)）の順にクリックします。

1. **[!UICONTROL ドキュメント]**／**[!UICONTROL カスタム統合]**&#x200B;をクリックします。
1. 無効にするカスタム統合を選択します。
1. 「**[!UICONTROL 無効にする]**」をクリックします。

   ユーザーは、無効にしたサードパーティのドキュメントプロバイダーに接続できず、そのクラウドプロバイダーから [!DNL Workfront] にドキュメントをリンクできなくなりました。
