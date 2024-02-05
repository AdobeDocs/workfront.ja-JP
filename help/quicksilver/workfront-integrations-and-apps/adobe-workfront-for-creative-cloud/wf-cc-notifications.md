---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Adobe Creative Cloud で  [!DNL Adobe Workfront]  通知を表示および管理
description: 承認が必要なアイテム、与えられた割り当て、または関連付けられているアイテムに対するコメントや変更に関する  [!DNL Adobe Workfront]  からの通知を、Adobe Creative Cloud で受け取ることができます。
author: Courtney,Becky
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: b07474c0-ba41-4382-8374-040f633a47ed
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 96%

---

# [!DNL Adobe Creative Cloud] から [!DNL Adobe Workfront] 通知を表示および管理

承認が必要なアイテム、与えられた割り当て、または関連付けられているアイテムに対するコメントや変更に関する [!DNL Adobe Workfront] からの通知を、Adobe Creative Cloud で受け取ることができます。

これらの通知には、Adobe Creative Cloud から移動せずに実行できる [!DNL Workfront] アクションが含まれています。

通知は、次の Adobe Creative Cloud アプリで使用できます。

{{cc-app-list}}

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <!--<td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">製品</td> 
   <td>[!DNL Workfront] ライセンスに加えて [!DNL Adobe Creative Cloud] ライセンスが必要です。</td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

{{cc-install-prereq}}

* [!DNL Workfront] でインスタント通知を有効にしている。インスタント通知の有効化について詳しくは、 [独自の電子メール通知を変更する](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Adobe Creative Cloud で [!DNL Workfront] 通知を表示および管理

1. プラグインパネルの上部付近にある&#x200B;**[!UICONTROL 通知]**&#x200B;アイコン ![通知アイコン](assets/cc-plugin-notifications-icon.png) をクリックします。アイコン上の青い点は、未読の通知があることを示します。
1. （オプション）すべての通知を既読としてマークするには、「**[!UICONTROL すべてを既読とマーク]**」をクリックします。

   これにより、プラグインと Workfront で、通知が既読としてマークされます。既読の通知は、プラグインの通知のリストに表示されなくなります。

1. 通知で言及されている作業項目に移動するには、通知をクリックします。

## Adobe Creative Cloud プラグインで使用可能な Workfront 通知

プラグインでは、次の通知を使用できます。


* 自分が更新を受信する対象者として追加された
* チームが更新を受信する対象者として追加された（@teamname）
* 自分のユーザープロファイルに誰かがコメントした
* 自分が含まれている更新に対して誰かがコメントした
* 自分の作業項目または自分がしたことに対して誰かがコメントした
* 自分のドキュメントが承認、変更して承認、または却下された
