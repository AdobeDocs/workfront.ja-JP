---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Outlook メールをタスクとして作業リストに追加
description: ' [!DNL Outlook]  メールを  [!DNL Adobe Workfront]  タスクに変換することができます。メールが変換されると、そのタスクはホームエリアの作業用リストに表示されます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 76%

---

# [!DNL Outlook] メールをタスクとして作業リストに追加

>[!IMPORTANT]
>
>[Microsoftでは、従来の Exchange オンライン トークン ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートを無効にする処理を行っています。現在、このトークンは、Workfront Outlook アドインで認証に使用されています。 Microsoftによるこの変更は、既にお客様に影響を与え始めており、2025 年 10 月まで段階的に展開し続けます。
>
>* **Microsoftがこれらのトークンを完全に無効にすると、Microsoft Outlook 用Workfront統合は機能しなくなります。**
>
>この変更の一環として、Microsoftは、トークンを再度有効にする方法を変更することを決定しました。 **2025 年 6 月 30 日（PT）** 以降、管理者はトークン自体を再度有効にすることができなくなります。例外を付与できるのは、Microsoft サポートのみです。 **2025 年 10 月 1 日に、すべてのテナントに対してレガシートークンがオフになります。 例外は許可されません。**


[!DNL Outlook] メールを [!DNL Adobe Workfront] タスクに変換することができます。メールが変換されると、そのタスクは[!UICONTROL ホーム]エリアの[!UICONTROL 作業]リストに表示されます。

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

## [!DNL Outlook] メールをタスクとして作業リストに追加

1. タスクに変換する [!DNL Outlook] 内のメールを選択します。
1. メールメッセージの右上隅にある **[!DNL Workfront]** アイコンをクリックして [!DNL Workfront] アドインを表示します。\
   メールの右上にある下向き矢印をクリックして [!DNL Workfront] アイコンにアクセスする場合もあります。

1. **[!UICONTROL メニュー]**![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png)アイコンをクリックして、使用可能な [!DNL Workfront] オプションのリストを表示します。


1. 「**[!UICONTROL 作業に追加]**」をクリックします。

1. 「**[!UICONTROL プロジェクトに追加]**」フィールドの選択を解除します。
1. （オプション）メールをタスクとして保存する前に、次の情報を更新できます。

   * **[!UICONTROL タスク名]：**&#x200B;デフォルトでは、タスク名はメールの件名と同じです。必要に応じてタスク名を変更できます。
   * **[!UICONTROL 説明]：**&#x200B;デフォルトでは、説明はメール本文と同じです。必要に応じて説明を変更できます。
   * **[!UICONTROL 添付ファイル]：**&#x200B;メールの添付ファイルは、タスクの[!UICONTROL ドキュメント]エリアに保存されます。メールをタスクとして保存する前に、任意の添付ファイルを削除することができます。

1. 「**[!UICONTROL 追加]**」をクリックします。\
   タスクはホームエリアの[!UICONTROL 作業リスト]に、コミット日なしで追加されます。

1. （オプション）新しいタブの [!DNL Workfront] アプリケーションで **[!UICONTROL Workfront で表示]** タスクをクリックします。

1. （オプション）[!DNL Outlook] に戻り、元のメールを選択します。\
   [!DNL Workfront] アドインパネルの上部に、メールが Workfront に追加されたことを示すリンクが表示され、確認が行われます。リンクには、変換された日付が含まれます。
