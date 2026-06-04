---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 プルーフの機能強化
description: このページでは、本番環境に対する 2020.2 リリースで行われたすべてのプルーフの機能強化について説明します。 これらの機能強化は、2020年5月11日（PT）の週に本番環境で利用できるようになりました。
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
TQID: https://experienceleague.adobe.com/Z86GWBBVdj1DPENzHS7wKI1ViRGFzov8L3sNtss4iJU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 100%

---

# 2020.2 プルーフの機能強化

このページでは、本番環境に対する 2020.2 リリースで行われたすべてのプルーフの機能強化について説明します。 これらの機能強化は、2020年5月11日（PT）の週に本番環境で利用できるようになりました。

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
