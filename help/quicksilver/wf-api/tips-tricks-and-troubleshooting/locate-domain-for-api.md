---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API 呼び出しのドメイン形式
description: Adobe Workfront API で使用するドメインを見つけます。
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 100%

---

# Adobe Workfront API 呼び出しのドメイン形式

Workfront API に対して API 呼び出しを行う場合は、呼び出しで組織のドメインを使用します。このドメイン URL の形式は、組織が Adobe Unified Shell にオンボーディングされているかどうかによって異なります。

組織が Adobe Unified Shell にオンボーディングされているかどうかを確認するには、Workfront ページを表示しているときに表示される URL を調べます。

| Workfront URL は、次で始まります。 | API 呼び出し用の URL： |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

ドメインを見つけるには、次の手順に従います。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL 設定]**」![設定アイコン](/help/_includes/assets/gear-icon-setup.png)の順にクリックします。
1. 「**システム**」を選択して、「**顧客情報**」を選択します。

   ドメインが画面の右側に表示されます。

   ![ドメイン](assets/domain.png)

