---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API 呼び出しのドメイン形式
description: Adobe Workfront API で使用するドメインを見つけます。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 1f45298f6bff0b633ce2cd5f3bedd098904eba9d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 22%

---


# Adobe Workfront API 呼び出しのドメイン形式

Workfront API への API 呼び出しをおこなう場合は、呼び出しで組織のドメインを使用します。 このドメイン URL の形式は、組織が統合シェルにオンボードされているかどうかに応じて異なります。Adobe

組織がAdobe統合シェル上にあるかどうかを知るには、Workfrontページを表示する際に表示される URL を調べます。

| Workfront URL は次の語句で始まります。 | API 呼び出しの URL: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

ドメインを見つけるには、次の手順に従います。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. 選択 **システム**&#x200B;を選択し、「 **顧客情報**.

   ドメインが画面の右側に表示されます。

   ![ドメイン](assets/domain.png)

