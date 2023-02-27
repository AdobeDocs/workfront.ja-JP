---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Workfront Fusion リリースアクティビティ：2021 年 5 月 3 日の週'
description: このページでは、2021 年 5 月 3 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Workfront Fusion リリースアクティビティ： 2021 年 5 月 3 日の週

このページでは、2021 年 5 月 3 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。

最近のすべての変更の一覧については、 [Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Workfront Fusion の最近のバグ修正の一覧については、 [Workfrontメンテナンスの更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) ページを開き、 Workfront Fusion メンテナンスアップデートというラベルの付いたアップデートがないか確認します。

## Salesforce コネクタで SOQL を使用した検索が可能に

Salesforce /レコードの検索モジュールに、SOQL(Salesforce Object Query Language) を使用して検索するオプションが追加されました。 また、以前利用可能なオプション（SOSL および単純検索）を使用して検索することもできます。

詳しくは、 [Salesforce モジュール](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Azure DevOps コネクタの新しい接続タイプに必要なスコープの数が少なくなりました

セキュリティを強化するために、Workfront Fusion Azure DevOps コネクタに新しいコネクタタイプが追加されました。 Azure DevOps モジュールで接続を作成する際に、次の 2 種類の接続から選択できます。

* Azure DevOps

   この新しい接続タイプでは、スコープはWorkfront Fusion で特に必要なスコープに制限されます。

* Azure DevOps （すべてのスコープをリクエスト）

   これはレガシーの接続タイプで、Azure DevOps への接続で使用可能なすべてのスコープをリクエストします。

Azure DevOps を使用するすべての新しいシナリオで、Azure DevOps 接続タイプを使用することをお勧めします。 また、既存のシナリオで Azure DevOps モジュールを変更して、新しい接続タイプを使用することをお勧めします。 レガシー Azure DevOps （すべてのスコープをリクエスト）接続タイプは、近い将来非推奨となります。

詳しくは、 [Azure DevOps モジュール](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
