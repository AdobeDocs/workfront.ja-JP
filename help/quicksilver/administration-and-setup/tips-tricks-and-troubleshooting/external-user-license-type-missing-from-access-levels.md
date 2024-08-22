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
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 87%

---

# 外部ユーザー指定ライセンスの種類がアクセスレベルにありません

## 問題

設定のアクセスレベルに外部ユーザー指定ライセンスの種類が表示されなくなりました。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!DNL Workfront] 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ソリューション

1. **[!UICONTROL 設定]**／**[!UICONTROL システム]**／**[!UICONTROL 環境設定]**&#x200B;に移動します。

1. 「**[!UICONTROL セキュリティ]**」セクションで、「**[!UICONTROL メールアドレスを使用して Workfront アカウントを持たないユーザーと共同作業]**」オプションが有効になっていることを確認します。

   このオプションが有効になっていない場合、外部ユーザーはアクセスレベル設定に表示されません。
