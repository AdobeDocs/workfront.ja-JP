---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: 融合
navigation-topic: fusion-release-activity
title: '''Workfront Fusion リリースアクティビティ：2020 年 11 月 30 日の週'
description: このページでは、2020 年 11 月 30 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 9621683b-735d-40a6-8d7c-b5bd167cbdd2
hidefromtoc: true
source-git-commit: e18b23e7d58aced4c95c5df51769a6e959fa3d57
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Workfront Fusion リリースアクティビティ：2020 年 11 月 30 日の週

このページでは、2020 年 11 月 30 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。

最近のすべての変更の一覧については、 [Adobe Workfront Fusion リリースアクティビティ](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Workfront Fusion の最近のバグ修正の一覧については、 [Workfrontメンテナンスの更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) ページを開き、 Workfront Fusion メンテナンスアップデートというラベルの付いたアップデートがないか確認します。

## Workfront Fusion 2.0 Web フックのレート制限。

Workfront Fusion 2.0 に新しいパフォーマンスガードレールが導入されました。Web フックのレート制限は 1 秒あたり 100 個です。 この制限に達すると、Workfront Fusion 2.0 は 429(Too Many Requests) ステータスを送信します。

以前は、Webhook のリクエストに制限はありませんでした。

詳しくは、 [Adobe Workfront Fusion パフォーマンスガードレール](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md).

## Workfront Fusion 2.0 のWorkfrontオブジェクトにカスタムフォームを追加する

カスタムフォームをWorkfront Fusion 2.0 でオブジェクトに追加できるように、 Workfront /その他に AssignCategories アクションを追加しました。 アクションモジュール。

以前は、Workfront Fusion 2.0 モジュールを使用してWorkfrontのオブジェクトにカスタムフォームを追加することはできませんでした。

詳しくは、 Workfront /その他を参照してください。 アクションモジュール ( [Adobe Workfrontモジュール](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Jira Server connector and modules now available</h2>
<p>We've added a Jira Server connector to Workfront Fusion. The Jira Server connector offers the same functionality as the current Jira Cloud connector. </p>
<p>With Jira Server modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, modified, or deleted</p> </li>
<li> <p>Create, read, update, or delete a record</p> </li>
<li> <p>List or search records</p> </li>
<li> <p>Download an attachment</p> </li>
<li> <p>Add an issue to a sprint</p> </li>
<li> <p>Make a custom API call</p> </li>
</ul>
<p>Previously, Jira modules were available only for Jira Cloud.</p>
<p>For more information on available Jira modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref" xrefformat="{para}">Jira Software modules</a>.</p>
<h2>Azure DevOps connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Azure DevOps applications. With the Azure DevOps modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when a record is added, updated, or deleted.</p> </li>
<li> <p>Create or update records.</p> </li>
<li> <p>Get data from existing records.</p> </li>
<li> <p>Download or upload attachments.</p> </li>
<li> <p>Link work items together.</p> </li>
<li> <p>Retrieve a list of work items.</p> </li>
<li> <p>Perform a custom API call.</p> </li>
</ul>
<p>For more information see <a href="../../../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref" xrefformat="{para}">Azure DevOps modules</a>.</p>
<h2>Microsoft Dynamics 365 connector and modules now available</h2>
<p>You can now use Workfront Fusion to connect to your Microsoft Dynamics 365 account. With the Microsoft Dynamics 365 modules, you can:</p>
<ul>
<li> <p>Trigger a scenario when records are added or updated in Microsoft Dynamics 365</p> </li>
<li> <p>Create, read, update, or delete a Microsoft Dynamics 365record</p> </li>
<li> <p>Perform a custom API call</p> </li>
</ul>
<p>For information about available Microsoft Dynamics 365 modules, see <a href="../../../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref" xrefformat="{para}">Microsoft Dynamics 365 modules</a>.</p>
</div>
-->
