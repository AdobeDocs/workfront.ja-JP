---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 プルーフの機能強化
description: このページでは、実稼動環境に対する 2020.2 リリースで行われたすべてのプルーフの機能強化について説明します。これらの機能強化は、2020年5月11日（PT）の週に実稼動環境で利用できるようになりました。
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 100%

---

# 2020.2 プルーフの機能強化

このページでは、実稼動環境に対する 2020.2 リリースで行われたすべてのプルーフの機能強化について説明します。これらの機能強化は、2020年5月11日（PT）の週に実稼動環境で利用できるようになりました。

2020.2 リリースで利用可能なすべての変更点の一覧については、[2020.2 リリースの概要](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md)を参照してください。

## プルーフのドメインが proofhq.com から workfront.com に変わります。

>[!NOTE]
>
>この機能は元々 2020.1 リリースの一部として伝えられていましたが、実稼動環境へのリリース前にリリースから削除されていました。

ファイアウォールやメールサーバーで特定のベンダーへのみアクセスできるように設定されている場合は、次の URL を許可リストに追加する必要があります。これにより、組織のユーザーがブラウザープルーフビューアーとデスクトッププルーフビューアーの両方で、Workfront 内のプルーフを表示できるようになります。

&#42;.workfront.com

&#42;proofhq.com URL も引き続き必要です。

許可リストの更新について詳しくは、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

この更新は、Workfront 内のプルーフにのみ適用されます。Workfront Proof アプリケーションをスタンドアロンで使用する場合は適用されません。

## ゲストによるプルーフコメントを更新領域で表示

プルーフの共同作業を効率化するために、ゲストによるコメントが更新領域に表示されます。

以前は、ゲストによるプルーフのコメントはプルーフでのみ利用できました。
