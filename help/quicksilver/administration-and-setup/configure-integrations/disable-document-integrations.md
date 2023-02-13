---
title: ドキュメント統合の無効化
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: 形式 [!DNL anAdobe] [!DNL Workfront] 管理者は、Workfrontとサードパーティのドキュメントプロバイダーとの接続を無効にすることができます。
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 1%

---

# ドキュメント統合の無効化

As a [!DNL Adobe] [!DNL Workfront] 管理者は、 [!DNL Workfront] およびサードパーティのドキュメントプロバイダー

次の間の接続を無効にした場合： [!DNL Workfront] また、ドキュメントプロバイダーがドキュメントへのリンクを [!DNL Workfront]. ユーザーはリンクされたドキュメントを表示できなくなり、 [!DNL Workfront] リンクを作成し、そのプロバイダーに他のドキュメントを追加することはできません。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

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
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## クラウドプロバイダー統合を無効にする

次のドキュメント統合を無効にするには： [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. にログインします。 [!DNL Workfront] as a [!DNL Workfront] 管理者。
1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL ドキュメント]** > **[!UICONTROL クラウドプロバイダー]**.

1. 連携を解除するクラウドプロバイダーの選択を解除します [!DNL Workfront].
1. 「**[!UICONTROL 保存]**」をクリックします。

   無効にした特定のクラウドプロバイダーに接続できず、そのクラウドプロバイダーからWorkfrontにドキュメントをリンクできなくなりました。

## を無効にします。 [!DNL SharePoint] 統合

1. にログインします。 [!DNL Workfront] as a [!DNL Workfront] 管理者。
1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 展開 **[!UICONTROL ドキュメント]**&#x200B;を選択し、「 **[!UICONTROL [!DNL SharePoint]統合]**.
1. を選択します。 [!DNL SharePoint] 統合を無効にします。
1. クリック **[!UICONTROL 無効にする]**.\
   ユーザーが [!DNL SharePoint] サイトを無効にし、ドキュメントをリンクできなくなりました。 [!DNL SharePoint] から [!DNL Workfront].

## カスタム統合の無効化

1. にログインします。 [!DNL Workfront] 管理者として。
1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL ドキュメント]** > **[!UICONTROL カスタム統合]**.
1. 無効にするカスタム統合を選択します。
1. クリック **[!UICONTROL 無効にする]**.

   無効にしたサードパーティのドキュメントプロバイダにユーザーが接続できず、そのクラウドプロバイダから次にドキュメントをリンクできなくなりました： [!DNL Workfront].
