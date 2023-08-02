---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager統合のトラブルシューティング
description: 「問題：アセットがAdobe Experience Managerに保存されない」
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a73ebfe8c735eb9e103b01a201a8f71d6ab7bda2
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# Adobe Experience Manager統合のトラブルシューティング

## 問題：アセットがAdobe Experience Managerに保存されない

ユーザーがExperience Manager Assetsに書き出すアセットまたはフォルダーを選択して「選択」をクリックすると、セレクターウィンドウが閉じますが、アセットはExperience Manager Assetsに保存されません。 Workfrontで、アセットがExperience Manager Assetsに保存されなかったことを示すものはありません。

### 原因

これは、Cloud Manager でのAdobeが原因許可リストに加えるで発生する場合があります。 組織の Cloud ManagerAdobeが空の場合許可リストに加えるは、IP アドレスは制限されず、WorkfrontはAdobe Experience Manager内の組織のフォルダーやアセットにアクセスできます。 ただし、Cloud Manager に 1 つの IP アドレスも追加されている場合許可リストに加えるは、リストにない IP アドレスは許可されていないと想定されま許可リストに加えるす。 したがって、Cloud Manager に任意の IP アドレスが含まれている場合許可リストに加えるは、WorkfrontがExperience Manager Assetsにアセットを送信できるように、Workfrontの IP アドレスもに追加する必要がありま許可リストに加えるす。

### 解決策：

Workfront IP アドレスを Cloud ManagerAdobeに追加しま許可リストに加えるす。

* Cloud Manager に IP アドレスを追加する手順については、次を参照してください。Adobe: [IP許可リストの概要](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) (Adobe Experience Managerドキュメント ) を参照してください。
* Workfrontに追加する IP アドレスのリストについては、 [ファイアウォールを設定する](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).


