---
title: ' [!DNL Adobe Workfront]  を有効化（Outlook 用）'
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: ユーザーが Outlook 用  [!DNL Adobe Workfront]  の使用を開始するには、まずシステムでそれを有効にする必要があります。
author: Lisa, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: be523b27-191f-46ca-9a87-d512f9a15a1e
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 60%

---

# [!DNL Adobe Workfront for Outlook] を有効にする

>[!IMPORTANT]
>
>[Microsoftでは、従来の Exchange オンライン トークン ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートを無効にする処理を行っています。現在、このトークンは、Workfront Outlook アドインで認証に使用されています。 Microsoftによるこの変更は、既にお客様に影響を与え始めており、2025 年 10 月まで段階的に展開し続けます。
>
>* **Microsoftがこれらのトークンを完全に無効にすると、Microsoft Outlook 用Workfront統合は機能しなくなります。**
>
>この変更の一環として、Microsoftは、トークンを再度有効にする方法を変更することを決定しました。 **2025 年 6 月 30 日（PT）** 以降、管理者はトークン自体を再度有効にすることができなくなります。例外を付与できるのは、Microsoft サポートのみです。 **2025 年 10 月 1 日に、すべてのテナントに対してレガシートークンがオフになります。 例外は許可されません。**


ユーザーが Outlook 用 [!DNL Adobe Workfront for Outlook] の使用を開始するには、まずシステムでそれを有効にする必要があります。

[!DNL Workfront for Outlook] を有効にした後の使用方法について詳しくは、[[!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/workfront-for-outlook.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>[!DNL Workfront] の管理者である必要があります。[!DNL Workfront] 管理者については、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

+++

## [!DNL Workfront] [!DNL Outlook] アドインを有効化

1. [!DNL Workfront] に管理者としてログインします。

{{step-1-to-setup}}

1. **[!UICONTROL システム]**&#x200B;を展開し、続いて「**[!UICONTROL 環境設定]**」をクリックします。

1. 「**[!UICONTROL ユーザーが Workfront のモバイルアプリケーションと [!DNL Workfront] [!DNL Outlook] アドイン]** が使用できるようにする」が選択されていることを確認します。\
   この設定では、[!DNL Workfront] モバイルアプリケーションの使用を許可するだけでなく、[!DNL Workfront] [!DNL Outlook] アドインの使用も許可します。

   このオプションは、デフォルトで有効になっています。

1. 「**[!UICONTROL 保存]**」をクリックします。

## [!DNL Workfront] [!DNL Outlook] アドインのインストール

[!DNL Outlook] 用に [!DNL Workfront] アドインを使用するためのシステム要件について詳しくは、「[ [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md) 用に Adobe Workfront を設定」にある[システム要件](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#system-requirements-and-prerequisites)を参照してください。

[!DNL Outlook] 用の [!DNL Workfront] アドインをインストールする方法について詳しくは、[設定 [!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)にある[アドインのインストール](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#downloading-and-installing-the-add-in)を参照してください。
