---
product-area: reporting
navigation-topic: create-and-manage-reports
title: レポートの実行
description: 表示にアクセスできる任意のレポートを実行できます。
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---


# レポートの実行

表示にアクセスできる任意のレポートを実行できます。

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの表示</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## レポートの実行

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **レポート**.

1. 次のオプションから選択します。

   * **マイレポート：** 作成したレポート。
   * **自分と共有：** 他のユーザーが自分と共有したレポート。
   * **すべてのレポート：** アクセス権のあるシステム内のすべてのレポート。

1. 実行するレポートの名前をクリックします。\
   または\
   プロンプトを使用してレポートを作成した場合は、ドロップダウンメニューから適切な情報を選択し、 **レポートを実行**.\
   プロンプトの詳細については、「 [レポートにプロンプトを追加する](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   レポートの内容には、レポートの右上隅にタイムスタンプが表示されます。このタイムスタンプには、レポートを実行したユーザーのコンテキストからレポートを実行した日時、タイムゾーンが含まれます。

1. （オプション） **再読み込みアイコン** ![](assets/qs-report-refresh-icon.png) ：レポートがしばらくブラウザーに表示されている場合に、レポートの結果を更新します。

1. （条件付き）レポートでフィルターまたはプロンプトが使用される場合、 **フィルタとプロンプトを表示** 表示中のレポートで使用されているフィルタとプロンプトのリストを表示します。 レポートにフィルタのみが含まれる場合、またはプロンプトのみが含まれる場合は、 **フィルターを表示** または **プロンプトを表示** が表示されます。

   ![フィルターとプロンプトを表示](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   情報は、ページの左側のレポート名の下に表示されます。 プロンプトの場合は、手順 4 に従って、レポートの実行時に行われたプロンプトの選択に関する情報です。

1. [ カスタムプロンプト ] を使用している場合は、表示されません。 システムプロンプトのみが表示されます。 カスタムフィルターは常に表示されます。

## キャッシュされたレポートの表示

しばらくブラウザーに表示されているレポートは、キャッシュに保存される場合があります。 次のいずれかの操作を実行するときに、キャッシュされたレポートを強制的に再読み込みすることができます。

* レポート設定を編集し、レポートを保存します。
* [ 表示 ]、[ グループ ]、または [ フィルタ ] を変更します。
* 次をクリック： **再読み込みアイコン**
このオプションは、レポートが保存された時間を示すメッセージボックス内でページの右上隅に表示されます。または、レポートが配置されているダッシュボードの右上隅に表示されます。 ダッシュボードの再読み込みの詳細については、この記事の「ダッシュボードの表示」の節を参照してください [ダッシュボードの概要](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

* 「概要」、「マトリックス」または「グラフ」の各タブに移動して、最初のページ以外のレポートのページにアクセスします。
