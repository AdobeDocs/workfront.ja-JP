---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: タイムシートの作業週の開始日を修正
description: タイムシートの週の開始日が、私の期待する週単位の開始日と一致しません。
author: Lisa
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 5%

---

# タイムシートの週の作業開始日の修正

<!--Audited: 5/2025-->

## 問題

タイムシートの週の開始日が、私の期待する週単位の開始日と一致しません。

これは通常、タイムシート プロファイルに割り当てられていない場合や、タイムシートが手動で作成された場合に発生します。


## ソリューション

Workfront管理者は、[ タイムシート プロファイルの作成、編集、割り当て](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)の説明に従って、タイムシート プロファイルを作成し、全員をプロファイルに割り当てる必要があります。 Workfrontの管理者は、タイムシートの開始日を、予定される週次の開始日以外の日に定義することができます。 タイムシート プロファイルの開始日がタイムシートの開始日を確認します。

タイムシートが手動で作成された場合、タイムシートの週の開始日には、ユーザーのプロファイルで電子メールロケール設定が使用されます。詳しくは、[個人設定の設定](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)を参照してください。

例えば、メールロケールが英語（米国）に設定されている場合、タイムシートの週は日曜日から始まります。 または、メールロケールを英語（英国）に設定した場合、タイムシートの週は月曜日から始まります。


<!--
This is the old content for this article but I found this was not working this way at all, so I changed it to what it is today: 

## Problem

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solution

The start day of the week of a timesheet in Adobe Workfront uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser. 

For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.

This setting also affects the start day of the week in the pop-up calendars across the system.

The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always starts on Sunday.

Following are the directions for changing language and locale settings for various browsers that are supported with Workfront.

* **Chrome:** Copy and paste the following link into your Chrome browser: `chrome://settings/languages` then go to Languages.
* **Firefox:**Copy and paste the following link into your Firefox browser: `about:preferences#content` then go to Languages.
* **IE 11:** Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.

-->


