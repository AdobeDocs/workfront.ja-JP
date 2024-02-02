---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 「Workfront Fusion リリースアクティビティ：2021年5月3日（PT）の週」
description: このページでは、2021年5月3日（PT）の週に Adobe Workfront Fusion で行われたすべての機能強化について説明します。
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: ht
source-wordcount: '270'
ht-degree: 100%

---

# Workfront Fusion リリースアクティビティ：2021年5月3日（PT）の週

このページでは、2021年5月3日（PT）の週に Adobe Workfront Fusion で行われたすべての機能強化について説明します。

最近のすべての変更内容のリストについては、[Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)を参照してください。

Workfront Fusion での最近のバグ修正のリストについては、[Workfront メンテナンスアップデート](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ja)ページで、Workfront Fusion メンテナンスアップデートというラベルが付いたアップデートがあるか確認してください。

## Salesforce コネクターで SOQL を使用した検索が可能に

Salesforce／レコードを検索モジュールに、SOQL（Salesforce Object Query Language）を使用して検索するオプションが追加されました。また、以前利用可能なオプション（SOSL および単純検索）を使用して検索することもできます。

詳しくは、[Salesforce モジュール](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md)を参照してください。

## Azure DevOps コネクタの新しい接続タイプに必要なスコープの数が減少

セキュリティを強化するために、Workfront Fusion Azure DevOps コネクタに新しいコネクタータイプが追加されました。Azure DevOps モジュールで接続を作成する際に、次の 2 種類の接続から選択できます。

* Azure DevOps

  この新しい接続タイプでは、スコープは Workfront Fusion で特に必要なスコープに制限されます。

* Azure DevOps（すべてのスコープをリクエスト）

  これはレガシーの接続タイプで、Azure DevOps への接続で使用可能なすべてのスコープをリクエストします。

Azure DevOps を使用するすべての新しいシナリオで、Azure DevOps 接続タイプを使用することをお勧めします。また、既存のシナリオで Azure DevOps モジュールを変更して、新しい接続タイプを使用することをお勧めします。レガシー Azure DevOps（すべてのスコープをリクエスト）接続タイプは、近い将来非推奨となります。

詳しくは、[Azure DevOps モジュール](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md)を参照してください。
