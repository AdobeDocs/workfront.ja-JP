---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 9 の新機能（続き）
description: このリストは、大きいリストの後半部分です。 前半は、API バージョン 9 の新機能です。 バージョン 9 のアップデートのリストについては、 API バージョン 9 のアップデートを参照してください。
author: Becky
feature: Workfront API
exl-id: 0af97c16-e6a7-4796-92e0-4c2d9751c845
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 29%

---

# API バージョン 9 の新機能（続き）

このリストは、大きいリストの後半部分です。 前半は、 [API バージョン 9 の新機能](../../wf-api/api/new-api-version-9.md). バージョン 9 の更新のリストは、次の場所にあります。 [API バージョン 9 の更新](../../wf-api/api/new-api-version-9-updates.md).

## PortalSection

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `accessorIDs` | `customer` | `accessRules` | `accessLevelMM` | `exportFusionChartToPDF` |  | `ADD` |
| `appGlobalID` | `enteredBy` | `lastViewers` | `displayDescription` | `getPK` |  | `COPY` |
| `controllerClass` | `filter` | `linkedRoles` | `displayName` | `getReportFromCache` |  | `COUNT` |
| `currency` | `groupBy` | `linkedTeams` | `groupIDs` | `isReportFilterable` |  | `DELETE` |
| `customerID` | `lastUpdatedBy` | `linkedUsers` | `linkedCustomersMM` | `linkCustomer` |  | `EDIT` |
| `dashboards` | `publicRunAsUser` | `portalTabSections` | `linkedPortalTabsMM` | `migratePortalSectionsPPMToAnaconda` |  | `GET` |
| `defaultTab` | `reportFolder` | `scheduledReports` | `linkedRoleIDs` | `unlinkCustomer` |  | `REPORT` |
| `definition` | `runAsUser` |  | `linkedTeamIDs` |  |  | `SEARCH` |
| `description` | `scheduledReport` |  | `linkedUsersMM` |   |   |   |
| `descriptionKey` | `statisticInfo` |  | `portalTabsMM`  |   |   |   |
| `enablePromptSecurity` | `view` |  | `scheduledReportsOM`  |   |   |   |
| `enteredByID`  |   |   |   |   |   |   |
| `extRefID`  |   |   |   |   |   |   |
| `filterControl`  |   |   |   |   |   |   |
| `filterID`  |   |   |   |   |   |   |
| `folderName`  |   |   |   |   |   |   |
| `forceLoad`  |   |   |   |   |   |   |
| `ganttOpen`  |   |   |   |   |   |   |
| `globalUIKey`  |   |   |   |   |   |   |
| `groupByID`  |   |   |   |   |   |   |
| `groupControl`  |   |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| `isAppGlobalCopiable`  |   |   |   |   |   |   |
| `isAppGlobalEditable`  |   |   |   |   |   |   |
| `isNewFormat` |   |   |   |   |   |   |
| `isPublic`  |   |   |   |   |   |   |
| `isReport`  |   |   |   |   |   |   |
| `isStandalone`  |   |   |   |   |   |   |
| `lastUpdateDate`  |   |   |   |   |   |   |
| `lastUpdatedByID`  |   |   |   |   |   |   |
| `maxResults`  |   |   |   |   |   |   |
| `methodName`  |   |   |   |   |   |   |
| `modDate`  |   |   |   |   |   |   |
| `name` |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `objID`  |   |   |   |   |   |   |
| `objInterface` |   |   |   |   |   |   |
| `objObjCode` |   |   |   |   |   |   |
| `preferenceID` |   |   |   |   |   |   |
| `publicRunAsUserID` |   |   |   |   |   |   |
| `publicToken` |   |   |   |   |   |   |
| `reportFolderID`  |   |   |   |   |   |   |
| `reportType` |   |   |   |   |   |   |
| `runAsUserID`  |   |   |   |   |   |   |
| `scheduledReportID`  |   |   |   |   |   |   |
| `securityAncestorsDisabled`  |   |   |   |   |   |   |
| `securityRootID`  |   |   |   |   |   |   |
| `securityRootObjCode`  |   |   |   |   |   |   |
| `showPrompts`  |   |   |   |   |   |   |
| `sortBy`  |   |   |   |   |   |   |
| `sortBy2` |   |   |   |   |   |   |
| `sortBy3`  |   |   |   |   |   |   |
| `sortType`  |   |   |   |   |   |   |
| `sortType2` |   |   |   |   |   |   |
| `sortType3` |   |   |   |   |   |   |
| `specialView` |   |   |   |   |   |   |
| `toolBar` |   |   |   |   |   |   |
| `uiObjCode`  |   |   |   |   |   |   |
| `viewControl` |   |   |   |   |   |   |
| `viewID` |   |   |   |   |   |   |
| `width` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## PortalSectionLastViewer

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| creationDate | `customer` |  |  |  |  | `COUNT` |
| `customerID` | `report` |  |  |  |  | `GET` |
| `ID` | `viewer` |  |  |  |  | `REPORT` |
| `reportID` |  |  |  |  |  | `SEARCH` |
| viewerID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## PortalSectionStatisticInfo

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `allViews` | `customer` |  |  |  |  | `COUNT` |
| `customerID` | `report` |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `lastUpdatedDate` |  |  |  |  |  | `SEARCH` |
| `reportID`  |   |   |   |   |   |   |
| `viewsLastMonth`  |   |   |   |   |   |   |
| `viewsLastQuarter` |   |   |   |   |   |   |
| `viewsLastYear` |   |   |   |   |   |   |
| `viewsThisMonth`  |   |   |   |   |   |   |
| `viewsThisQuarter`  |   |   |   |   |   |   |
| `viewsThisYear`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## PortalTab

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `accessorIDs` | `customer` | `accessRules` | `linkedRoleIDs` | `advancedCopy` |  | `ADD` |
| `customerID` | `lastUpdatedBy` | `linkedRoles` | `linkedTeamIDs` | `exportDashboard` |  | `COPY` |
| `description` | `user` | `linkedTeams` | `linkedUsersMM` | `migrateCustomTabUserPrefs` |  | `COUNT` |
| `displayOrder` |  | `linkedUsers` |  |  |  | `DELETE` |
| `docID` |  | `portalTabSections` |  |  |  | `EDIT` |
| `extRefID` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isPublic` |  |  |  |  |  | `SEARCH` |
| `lastUpdateDate`  |   |   |   |   |   |   |
| `lastUpdatedByID`  |   |   |   |   |   |   |
| `name` |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `portalProfileID`  |   |   |   |   |   |   |
| `tabname` |   |   |   |   |   |   |
| `userID`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## PortalTabSection

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `area` | `calendarPortalSection`  |   |   |   |   |   |
| `calendarPortalSectionID` | `customer`  |   |   |   |   |   |
| `customerID` | `externalSection`  |   |   |   |   |   |
| `displayOrder` | `internalSection`  |   |   |   |   |   |
| `externalSectionID` | `portalTab` |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| `internalSectionID` |   |   |   |   |   |   |
| `portalSectionObjCode`  |   |   |   |   |   |   |
| `portalSectionObjID`  |   |   |   |   |   |   |
| `portalTabID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## ReportFolder

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| customerID | `customer` |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## ScheduleReport

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `customerID` | `customer` | `groups` | `accessLevelMM` | `sendReportDeliveryNow` |  | `ADD` |
| `description` | `enteredBy` | `roles` |  |  |  | `COPY` |
| `enteredByID` | `portalSection` | `teams` |  |  |  | `COUNT` |
| `externalEmails` | `runAsUser` | `users` |  |  |  | `DELETE` |
| `format` |  |  |  |  |  | `EDIT` |
| `groupIDs` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isExcelHyperlinksEnabled` |  |  |  |  |  | `SEARCH` |
| `lastRuntimeMilliseconds` |   |   |   |   |   |   |
| `lastSentDate` |   |   |   |   |   |   |
| `name`  |   |   |   |   |   |   |
| `pageSize`  |   |   |   |   |   |   |
| `portalSectionID`  |   |   |   |   |   |   |
| `recipients`  |   |   |   |   |   |   |
| `recurrenceRule` |   |   |   |   |   |   |
| `roleIDs` |   |   |   |   |   |   |
| `runAsUserID` |   |   |   |   |   |   |
| `runAsUserTypeAhead` |   |   |   |   |   |   |
| `schedTime`  |   |   |   |   |   |   |
| `schedule` |   |   |   |   |   |   |
| `scheduleStart`  |   |   |   |   |   |   |
| `startDate`  |   |   |   |   |   |   |
| `teamIDs` |   |   |   |   |   |   |
| `uiObjCode`  |   |   |   |   |   |   |
| `uiObjID`  |   |   |   |   |   |   |
| `userIDs`  |   |   |   |   |   |   |
