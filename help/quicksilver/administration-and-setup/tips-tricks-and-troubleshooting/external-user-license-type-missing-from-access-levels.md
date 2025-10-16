---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 外部ユーザーのライセンスの種類がアクセス レベルにありません
description: 設定のアクセスレベルに外部ユーザー指定ライセンスの種類が表示されなくなりました。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 83%

---

# 外部ユーザー指定ライセンスの種類がアクセスレベルにありません

## 問題

設定のアクセスレベルに外部ユーザー指定ライセンスの種類が表示されなくなりました。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ソリューション

1. **[!UICONTROL 設定]**／**[!UICONTROL システム]**／**[!UICONTROL 環境設定]**&#x200B;に移動します。

1. 「**[!UICONTROL セキュリティ]**」セクションで、「**[!UICONTROL メールアドレスを使用して Workfront アカウントを持たないユーザーと共同作業]**」オプションが有効になっていることを確認します。

   このオプションが有効になっていない場合、外部ユーザーはアクセスレベル設定に表示されません。
