---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager 統合のトラブルシューティング
description: 問題：アセットが Adobe Experience Manager に保存されない
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
TQID: https://experienceleague.adobe.com/VaiQnZXQe39sYlnJOblWoea9UwOaujEU3ME-jh7-0EI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 247
ht-degree: 93%

---

# Adobe Experience Manager 統合のトラブルシューティング

## 問題：アセットが Adobe Experience Manager に保存されない

ユーザーが Experience Manager Assets に書き出すアセットまたはフォルダーを選択して「選択」をクリックすると、セレクターウィンドウが閉じますが、アセットは Experience Manager Assets に保存されません。 Workfront には、アセットが Experience Manager Assets に保存されなかったという表示はありません。

### 原因

これは、Adobe Cloud Manager の許可リストが原因で発生する場合があります。 組織の Adobe Cloud Manager 許可リストに何もない場合、IP アドレスは制限されず、Workfront はAdobe Experience Manager 内の組織のフォルダーやアセットにアクセスできます。 ただし、Cloud Manager 許可リストに IP アドレスが 1 つでも追加されている場合は、許可リストは、リストにない IP アドレスは許可されていないと見なします。 したがって、Cloud Manager 許可リストに何らかの IP アドレスがある場合は、Workfront が Experience Manager Assets にアセットを送信できるように、Workfrontの IP アドレスも許可リストに追加する必要があります。

### 解決策：

Workfront の IP アドレスを Adobe Cloud Manager の許可リストに追加します。

* Adobe Cloud Manager に IP アドレスを追加する手順については、Adobe Experience Manager ドキュメントの [IP 許可リストの概要](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction)を参照してください。
* 許可リストに追加する Workfront の IP アドレスのリストについては、[ファイアウォールを設定](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。
