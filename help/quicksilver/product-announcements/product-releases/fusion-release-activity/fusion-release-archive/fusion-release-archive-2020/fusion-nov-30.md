---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
keywords: Fusion
navigation-topic: fusion-release-activity
title: 'Workfront Fusion リリースアクティビティ：2020年11月30日（PT）の週'
description: このページでは、2020年11月30日（PT）の週に Adobe Workfront Fusion で行われたすべての機能強化について説明します。
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 9621683b-735d-40a6-8d7c-b5bd167cbdd2
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: ht
source-wordcount: '213'
ht-degree: 100%

---

# Workfront Fusion リリースアクティビティ：2020年11月30日（PT）の週

このページでは、2020年11月30日（PT）の週に Adobe Workfront Fusion で行われたすべての機能強化について説明します。

最近のすべての変更内容のリストについては、[Adobe Workfront Fusion リリースアクティビティ](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)を参照してください。

Workfront Fusion での最近のバグ修正のリストについては、[Workfront メンテナンスアップデート](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=ja)ページで、Workfront Fusion メンテナンスアップデートというラベルが付いたアップデートがあるか確認してください。

## Workfront Fusion 2.0 web フックのレート制限。

Workfront Fusion 2.0 に新しいパフォーマンスガードレールが導入されました。現在、web フックには、1 秒あたりリクエスト 100 個のレート制限があります。この制限に達すると、Workfront Fusion 2.0 は 429（リクエストが多すぎます）ステータスを送信します。

以前は、web フックのリクエストに制限はありませんでした。

詳しくは、[Adobe Workfront Fusion のパフォーマンスガードレール](../../../../../workfront-fusion/get-started/fusion-performance-guardrails.md)を参照してください。

## Workfront Fusion 2.0 で Workfront オブジェクトにカスタムフォームを追加

Workfront Fusion 2.0 でオブジェクトにカスタムフォームを追加できるよう、Workfront／その他のアクションモジュールに AssignCategories アクションを追加しました。

以前は、Workfront Fusion 2.0 モジュールを使用して Workfront でオブジェクトにカスタムフォームを追加することはできませんでした。

Workfront／その他のアクションモジュールについて詳しくは、[Adobe Workfront モジュール](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md)を参照してください。

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
