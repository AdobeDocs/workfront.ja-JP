---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: タイムシートの週の作業開始日の修正
description: タイムシートの週の開始日が、タイムシートプロファイルで構成された週の開始日と一致しません。
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 92%

---

# タイムシートの週の作業開始日の修正

## 問題

タイムシートの週の開始日が、タイムシートプロファイルで設定された週の開始日と一致しません（[タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照）。

## ソリューション

Adobe Workfront のタイムシートの週の開始日は、ブラウザーの言語とロケールの設定を使用して曜日を決定します。このため、ブラウザーの言語およびロケール設定を更新する必要があります。

例えば、ブラウザーの言語が英語に設定され、ロケールが米国に設定されている場合、週は日曜日に始まります。また、ブラウザーの言語が英語に設定され、ロケールが英国に設定されている場合、開始日は月曜日になります。

この設定は、システム全体のポップアップカレンダーの曜日にも影響します。

ロケールの変更は、リソースグリッド（またはリソースグリッド表示）の曜日には影響しません。週はいつも日曜日に始まる。

次に、Workfront でサポートされている様々なブラウザーの言語およびロケール設定を変更する方法を示します。

* **Chrome:** 次のリンクをコピーして、Chrome ブラウザーに貼り付けます：`chrome://settings/languages` 次に、[ 言語 ] に移動します。
* **Firefox：**&#x200B;Firefox ブラウザーにリンク「`about:preferences#content`」をコピー&amp;ペーストして、「言語」に移動します。
* **IE 11**：ツール／インターネットオプション／一般／言語
* **Safari**：Safari では、オペレーティングシステムの言語全体を変更しない限り、web 閲覧の言語を変更することはできません。クロムや Firefox など別のブラウザーをインストールする方が簡単です。


