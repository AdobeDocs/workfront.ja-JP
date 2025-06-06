---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Outlook からのコメントに返信
description: ' [!DNL Adobe Workfront]  のメール通知を Outlook の受信トレイで受信したとき、Outlook 内でその通知に返信するだけで、 [!DNL Workfront]  に簡単にコメントを投稿できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 36239da6-b5f2-423c-9e81-af78bc31bf26
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 68%

---

# [!DNL Outlook] からコメントに返信

>[!IMPORTANT]
>
>[Microsoftでは、従来の Exchange オンライン トークン ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートを無効にする処理を行っています。現在、このトークンは、Workfront Outlook アドインで認証に使用されています。 Microsoftによるこの変更は、既にお客様に影響を与え始めており、2025 年 10 月まで段階的に展開し続けます。
>
>* **Microsoftがこれらのトークンを完全に無効にすると、Microsoft Outlook 用Workfront統合は機能しなくなります。**
>
>この変更の一環として、Microsoftは、トークンを再度有効にする方法を変更することを決定しました。 **2025 年 6 月 30 日（PT）** 以降、管理者はトークン自体を再度有効にすることができなくなります。例外を付与できるのは、Microsoft サポートのみです。 **2025 年 10 月 1 日に、すべてのテナントに対してレガシートークンがオフになります。 例外は許可されません。**

[!DNL Adobe Workfront] のメール通知を [!DNL Outlook] の受信トレイで受信したとき、Outlook 内でその通知に返信するだけで、[!DNL Workfront] に簡単にコメントを投稿できます。


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

この統合を使用する前に、[!DNL Workfront] 管理者が、[!DNL Outlook for Office] を [!DNL Workfront] と併せて有効にする必要があります。

## [!DNL Outlook] からコメントに返信

1. 返信対象のコメントを含む [!DNL Workfront] メール通知を選択します。
1. メールメッセージの右上隅にある **[!DNL Workfront]** アイコンをクリックして、Workfront アドインを表示します。\
   [!DNL Workfront] アイコンにアクセスするには、メールの右上にある下向き矢印をクリックする必要がある場合があります。

1. **[!UICONTROL メニュー]**&#x200B;アイコン ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) をクリックして、使用可能な [!DNL Workfront] オプションのリストを表示します。


1. 「**[!UICONTROL コメントに返信]**」をクリックします。
1. 提供されたフィールドでコメントを指定します。
1. （オプション）「**[!UICONTROL 他者を含める]**」をクリックして、更新に含めるユーザーの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。\
   この手順を繰り返してさらにユーザーを追加し、「**[!UICONTROL 完了]**」をクリックします。\
   デフォルトでは、返信先のユーザーには、そのユーザーが含まれているかどうかに関係なく、通知が届きます。\

1. 「**[!UICONTROL コメント]**」をクリックします。
