---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: タイムシートの作業週の開始日を修正する
description: タイムシートの週の開始日が、タイムシートプロファイルで構成された週の開始日と一致しません。
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# タイムシートの作業週の開始日を修正する

## 問題

タイムシートの週の開始日が、タイムシートプロファイルで設定された週の開始日と一致しません ( 詳しくは、 [タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## 解決策

Adobe Workfrontのタイムシートの週の開始日は、ブラウザの言語とロケールの設定を使用して曜日を決定します。 このため、ブラウザーの言語およびロケール設定を更新する必要があります。 

例えば、ブラウザーの言語が英語に設定され、ロケールが米国に設定されている場合、週は日曜日に始まります。 また、ブラウザーの言語が英語に設定され、ロケールが英国に設定されている場合、開始日は月曜日になります。

この設定は、システム全体のポップアップカレンダーの曜日にも影響します。

ロケールの変更は、リソースグリッド（またはリソースグリッド表示）の曜日には影響しません。 週は常に日曜日に始まります。

次に、Workfrontでサポートされている様々なブラウザーの言語およびロケール設定を変更する方法を示します。

* **クロム：** 次のリンクを Chrome ブラウザーにコピー&amp;ペーストします。 `chrome://settings/languages` 次に、言語に移動します。
* **Firefox:**次のリンクを Firefox ブラウザーにコピー&amp;ペーストします。 `about:preferences#content` 次に、言語に移動します。
* **IE 11:** ツール/インターネットオプション/一般/言語
* **Safari:** 残念ながら、Safari では、オペレーティングシステムの言語全体を変更しない限り、Web 閲覧の言語を変更することはできません。 Chrome や Firefox など別のブラウザーをインストールする方が簡単です。

 
