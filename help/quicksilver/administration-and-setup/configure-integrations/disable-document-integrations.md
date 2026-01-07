---
title: ドキュメント統合の無効化
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: ' [!DNL anAdobe] [!DNL Workfront] 管理者は、Workfront とサードパーティのドキュメントプロバイダーとの接続を無効にすることができます。'
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 97%

---

# ドキュメント統合の無効化

[!DNL Adobe] [!DNL Workfront] 管理者は、[!DNL Workfront] とサードパーティのドキュメントプロバイダーとの接続を無効にすることができます。

[!DNL Workfront] とドキュメントプロバイダーの間の接続を無効にすると、ドキュメントへのリンクが [!DNL Workfront] で非表示になります。ユーザーはリンクされたドキュメントを表示できなくなり、[!DNL Workfront] リンクを使用してドキュメントに変更を加えることはできず、そのプロバイダーに他のドキュメントを追加することもできません。

## アクセス要件

+++展開すると、この記事の機能のアクセス要件が表示されます。

<table>
  <tr>
   <td>Adobe Workfront パッケージ
   </td>
   <td> <p>PrimeまたはUltimate</p>
    <p>ワークフロー Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Adobe Workfront ライセンス
   </td>
   <td><p>標準</p>
   <p>プラン</p>
   </td>
  </tr>
   <tr>
   <td>アクセスレベル設定
   </td>
   <td>[!DNL Workfront] 管理者である必要があります。
   </td>
  </tr>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## クラウドプロバイダー統合を無効にする

[!UICONTROL Workfront DAM]、[!DNL Box]、[!DNL Dropbox]、[!DNL Google Drive]、[!DNL Microsoft OneDrive]、[!DNL WebDAM] のドキュメント統合を無効にするには：

1. [!DNL Workfront] 管理者として [!DNL Workfront] にログインします。

{{step-1-to-setup}}

1. **[!UICONTROL ドキュメント]**／**[!UICONTROL クラウドプロバイダー]**&#x200B;をクリックします。

1. [!DNL Workfront] から切断するクラウドプロバイダーの選択を解除します。
1. 「**[!UICONTROL 保存]**」をクリックします。

   ユーザーは、無効にした特定のクラウドプロバイダーに接続できず、そのクラウドプロバイダーから Workfront にドキュメントをリンクできなくなりました。

## [!DNL SharePoint] 統合を無効にする

1. [!DNL Workfront] 管理者として [!DNL Workfront] にログインします。

{{step-1-to-setup}}

1. 「**[!UICONTROL ドキュメント]**」を展開し、「**[!UICONTROL [!DNL SharePoint]統合]**」をクリックします。
1. 無効にする [!DNL SharePoint] 統合を選択します。
1. 「**[!UICONTROL 無効にする]**」をクリックします。\
   ユーザーは、無効にした [!DNL SharePoint] サイトに接続できず、[!DNL SharePoint] から [!DNL Workfront] にドキュメントをリンクできなくなりました。

## カスタム統合を無効にする

1. [!DNL Workfront] に管理者としてログインします。

{{step-1-to-setup}}

1. **[!UICONTROL ドキュメント]**／**[!UICONTROL カスタム統合]**&#x200B;をクリックします。
1. 無効にするカスタム統合を選択します。
1. 「**[!UICONTROL 無効にする]**」をクリックします。

   ユーザーは、無効にしたサードパーティのドキュメントプロバイダーに接続できず、そのクラウドプロバイダーから [!DNL Workfront] にドキュメントをリンクできなくなりました。
