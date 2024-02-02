---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Outlook メールからの既存オブジェクトの更新
description: Outlook メールからの情報で、既存のプロジェクト、タスクまたはイシューを更新できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: 16acba0f1981b75ca141a36d096fb6f5d37c40d1
workflow-type: ht
source-wordcount: '451'
ht-degree: 100%

---

# [!DNL Outlook] メールからの既存オブジェクトの更新

[!DNL Outlook] メールからの情報で、既存のプロジェクト、タスクまたはイシューを更新できます。

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

&#42;ご利用のプラン、ライセンスタイプ、アクセスを確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

この統合を使用するには、まず [!DNL Workfront] 管理者が [!DNL Workfront] で [!DNL Outlook for Office] を有効にする必要があります。

## [!DNL Outlook] メールからの既存オブジェクトの更新

1. [!DNL Outlook] で、[!DNL Adobe Workfront update]に組み込む情報を含んだメールを選択します。
1. メールメッセージの右上隅にある **[!DNL Workfront]** アイコンをクリックして、Workfront アドインを表示します。\
   [!DNL Workfront] アイコンにアクセスするには、メールの右上にある下向き矢印をクリックする必要がある場合があります。

1. **[!UICONTROL メニュー]**&#x200B;アイコン ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) をクリックして、使用可能な [!DNL Workfront] オプションのリストを表示します。


1. Workfront で「**[!UICONTROL 更新]」をクリックします**。\
   タスクとして保存する前に、メールからの次の情報を更新できます。

   * **[!UICONTROL タイプ]**：更新するオブジェクトのタイプを選択します。**[!UICONTROL プロジェクト]**、**[!UICONTROL タスク]**&#x200B;または&#x200B;**[!UICONTROL イシュー]**&#x200B;を選択できます。選択したオブジェクトによって、以下の「**[!UICONTROL 名前]**」フィールドに表示される結果が決まります。オブジェクトのタイプが不明な場合は、「**[!UICONTROL すべて]**」を選択して、プロジェクト、タスクおよびイシューを同時に検索します。

   * **[!UICONTROL 名前]**：更新するプロジェクト、タスクまたはイシューの名前を入力していきます。名前がドロップダウンリストに表示されたら、クリックします。
   * **[!UICONTROL 更新]**：デフォルトでは、更新はメールの本文と同じです。必要に応じて更新を変更できます。

     この[!UICONTROL 更新]は、Workfront で更新ステータスとして表示されます。

   * **[!UICONTROL 添付ファイル]**：メールの添付ファイルは、タスクの[!UICONTROL ドキュメント]エリアに保存されます。更新を送信する前に、添付ファイルを削除することができます。

1. （オプション）「**[!UICONTROL この更新に他者を含める]**」をクリックして、更新に含めるユーザーの名前を入力していき、ドロップダウンリストに名前が表示されたらクリックします。\
   この手順を繰り返してさらにユーザーを追加し、「**[!UICONTROL 完了]**」をクリックします。\
   デフォルトでは、返信先のユーザーには、そのユーザーが含まれているかどうかに関係なく、通知が届きます。\

1. （オプション）**[!UICONTROL ロック]**&#x200B;アイコンをクリックして、この更新を社内のユーザーのみに制限します。更新がロックされている場合、社外のユーザーは更新を表示できません。

   * **[!UICONTROL ロック解除]：**&#x200B;更新のあるプロジェクト、タスクまたはイシューに対するアクセス権を持つユーザーは誰でも更新を表示できます。

     デフォルトでは、更新はロック解除されています。\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL ロック済み]：**&#x200B;更新を表示できるのは、社内のユーザーのみです。

     ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. 「**[!UICONTROL 更新]**」をクリックします。
1. （オプション）「**[!UICONTROL Workfront で表示]**」をクリックして、[!UICONTROL Outlook] 内の [!DNL Workfront] 統合で更新された項目を表示します。
