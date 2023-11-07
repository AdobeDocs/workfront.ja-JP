---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 9 の新機能（続き）
description: このリストは、大きいリストの後半部分です。 前半は、API バージョン 9 の新機能です。 バージョン 9 のアップデートの一覧については、 API バージョン 9 のアップデートを参照してください。
author: Becky
feature: Workfront API
role: Developer
exl-id: 0af97c16-e6a7-4796-92e0-4c2d9751c845
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 20%

---

# API バージョン 9 の新機能（続き）

このリストは、大きいリストの後半部分です。 前半は、 [API バージョン 9 の新機能](../../wf-api/api/new-api-version-9.md). バージョン 9 の更新のリストは、次の場所にあります。 [API バージョン 9 の更新](../../wf-api/api/new-api-version-9-updates.md).

## PortalSection

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
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

{style="table-layout:auto"}

## PortalSectionLastViewer

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| creationDate | `customer` |  |  |  |  | `COUNT` |
| `customerID` | `report` |  |  |  |  | `GET` |
| `ID` | `viewer` |  |  |  |  | `REPORT` |
| `reportID` |  |  |  |  |  | `SEARCH` |
| viewerID |   |   |   |   |   |   |

{style="table-layout:auto"}

## PortalSectionStatisticInfo

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
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

{style="table-layout:auto"}

## PortalTab

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
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

{style="table-layout:auto"}

## PortalTabSection

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
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

{style="table-layout:auto"}

## ReportFolder

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| customerID | `customer` |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style="table-layout:auto"}

## ScheduleReport

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
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
