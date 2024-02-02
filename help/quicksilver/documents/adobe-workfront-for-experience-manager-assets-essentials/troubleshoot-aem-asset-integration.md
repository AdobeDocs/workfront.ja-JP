---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager 統合のトラブルシューティング
description: 「問題：アセットが Adobe Experience Manager に保存されない」
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a73ebfe8c735eb9e103b01a201a8f71d6ab7bda2
workflow-type: ht
source-wordcount: '241'
ht-degree: 100%

---

# Adobe Experience Manager 統合のトラブルシューティング

## 問題：アセットが Adobe Experience Manager に保存されない

ユーザーが Experience Manager Assets に書き出すアセットまたはフォルダーを選択して「選択」をクリックすると、セレクターウィンドウが閉じますが、アセットは Experience Manager Assets に保存されません。Workfront には、アセットが Experience Manager Assets に保存されなかったという表示はありません。

### 原因

これは、Adobe Cloud Manager の許可リストが原因で発生する場合があります。組織の Adobe Cloud Manager 許可リストに何もない場合、IP アドレスは制限されず、Workfront はAdobe Experience Manager 内の組織のフォルダーやアセットにアクセスできます。ただし、Cloud Manager 許可リストに IP アドレスが 1 つでも追加されている場合は、許可リストは、リストにない IP アドレスは許可されていないと見なします。したがって、Cloud Manager 許可リストに何らかの IP アドレスがある場合は、Workfront が Experience Manager Assets にアセットを送信できるように、Workfrontの IP アドレスも許可リストに追加する必要があります。

### 解決策：

Workfront の IP アドレスを Adobe Cloud Manager の許可リストに追加します。

* Adobe Cloud Manager に IP アドレスを追加する手順については、Adobe Experience Manager ドキュメントの [IP 許可リストの概要](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=ja)を参照してください。
* 許可リストに追加する Workfront の IP アドレスのリストについては、[ファイアウォールを設定](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。


