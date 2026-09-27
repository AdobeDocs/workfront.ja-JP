---
title: ドキュメント統合を無効にする
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: '[!DNL anAdobe] [!DNL Workfront]管理者は、Workfrontとサードパーティのドキュメントプロバイダーとの間の接続を無効にできます。'
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
TQID: 'https://experienceleague.adobe.com/3tfxxth82eJEjEmdVD3AJFxl6B1m3EVKMQP9Gy4LC24'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 91%
---
# ドキュメント統合の無効化

[!DNL Adobe] [!DNL Workfront] 管理者は、[!DNL Workfront] とサードパーティのドキュメントプロバイダーとの接続を無効にすることができます。

[!DNL Workfront] とドキュメントプロバイダーの間の接続を無効にすると、ドキュメントへのリンクが [!DNL Workfront] で非表示になります。 ユーザーはリンクされたドキュメントを表示できなくなり、[!DNL Workfront] リンクを使用してドキュメントに変更を加えることはできず、そのプロバイダーに他のドキュメントを追加することもできません。

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
