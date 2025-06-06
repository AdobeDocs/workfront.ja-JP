---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Outlook メールから  [!DNL Adobe Workfront]  リクエストを作成
description: Outlook メールから  [!DNL Adobe Workfront]  リクエストを作成できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 77%

---

# [!UICONTROL Outlook] メールから [!DNL Adobe Workfront] リクエストを作成

>[!IMPORTANT]
>
>[Microsoftでは、従来の Exchange オンライン トークン ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートを無効にする処理を行っています。現在、このトークンは、Workfront Outlook アドインで認証に使用されています。 Microsoftによるこの変更は、既にお客様に影響を与え始めており、2025 年 10 月まで段階的に展開し続けます。
>
>* **Microsoftがこれらのトークンを完全に無効にすると、Microsoft Outlook 用Workfront統合は機能しなくなります。**
>
>この変更の一環として、Microsoftは、トークンを再度有効にする方法を変更することを決定しました。 **2025 年 6 月 30 日（PT）** 以降、管理者はトークン自体を再度有効にすることができなくなります。例外を付与できるのは、Microsoft サポートのみです。 **2025 年 10 月 1 日に、すべてのテナントに対してレガシートークンがオフになります。 例外は許可されません。**


Outlook メールから [!DNL Adobe Workfront] リクエストを作成できます。

メールに基づいて [!DNL Workfront] リクエストを作成する際は、メールのコンテンツ（件名と本文を含む）がデフォルトでリクエストに含まれます。

>[!NOTE]
>
>[!DNL Workfront]共有 [!UICONTROL Outlook] メールボックスからリクエストを作成することはできません。

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

担当の [!DNL Workfront] 管理者はこの統合を使用する前に [!DNL Workfront] で [!DNL Outlook for Office] を有効にする必要があります。

## [!DNL Outlook] メールからリクエストを作成

[!DNL Outlook] から [!DNL Workfront] リクエストを作成するには：

1. [!DNL Workfront] リクエストに含める情報を含むメールを選択します。
1. メールメッセージの右上隅にある **[!DNL Workfront]** アイコンをクリックして、Workfront アドインを表示します。\
   メールの右上にある下向き矢印をクリックして [!DNL Workfront] アイコンにアクセスする場合もあります。

1. **[!UICONTROL メニュー]**&#x200B;アイコン ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png) をクリックして使用可能な [!DNL Workfront] オプションのリストを表示します。

1. 「**[!UICONTROL リクエストを送信]**」をクリックします
1. 「**[!UICONTROL リクエストタイプを選択]**」フィールドで、リクエストを送信するリクエストキューを選択します。

1. 次の情報を指定します。\
   リクエストキューの設定方法に応じて、使用可能なフィールドは異なる場合があります。使用可能なフィールドの完全なリストと説明については、[ [!DNL Adobe Workfront] リクエストの作成と送信](../../manage-work/requests/create-requests/create-submit-requests.md)の記事を参照してください。

   * **[!UICONTROL 件名]：**&#x200B;リクエストの件名を指定します。デフォルトでは、メールの件名が使用されます。
   * **[!UICONTROL 説明]：**&#x200B;リクエストの説明を指定します。デフォルトでは、メールの本文が使用されます。
   * **[!UICONTROL ドキュメント]：**&#x200B;リクエストに含めるドキュメントを添付します。ドラッグ&amp;ドロップするか、「**[!UICONTROL ファイルを選択]**」をクリックし、ドキュメントを参照して選択します。

     デフォルトでは、メールに添付されたドキュメントがリクエストに含まれます。

1. 「**[!UICONTROL リクエストを送信]**」をクリックします。\
   リクエストは、指定されたリクエストキューの [!DNL Workfront] に送信されました。

1. （オプション）[!DNL Outlook] に戻り、元のメールを選択します。\
   [!DNL Workfront] アドインパネルの上部に、メールがリクエストとして Workfront に追加されたことを示すリンクが表示され、確認が行われます。リンクには、変換された日付が含まれます。
