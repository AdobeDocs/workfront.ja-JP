---
product-area: reporting
navigation-topic: create-and-manage-reports
title: レポートを実行する
description: 表示するアクセス権のあるすべてのレポートを実行できます。
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 81%

---


# レポートを実行する

表示するアクセス権のあるすべてのレポートを実行できます。

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
      <td> 
      <p>新規：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>プラン</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーの表示アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を表示</p></td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## レポートを実行する

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL レポート]**」の順にクリックします。

1. 次のオプションから選択します。

   * **マイレポート：**&#x200B;作成したレポート。
   * **自分と共有：**&#x200B;他のユーザーが自分と共有したレポート。
   * **すべてのレポート：**&#x200B;システム内のアクセスできるすべてのレポート。

1. 実行するレポートの名前をクリックします。\
   または\
   プロンプトを使用してレポートを作成した場合は、ドロップダウンメニューから適切な情報を選択し、「**レポートを実行**」をクリックします。\
   プロンプトについて詳しくは、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)を参照してください。\
   レポートの内容は、右上隅のタイムスタンプとともに表示されます。このタイムスタンプには、レポートを実行したユーザーのコンテキストにある、レポートを実行した日時とタイムゾーンが含まれます。

1. （任意） **再読み込みアイコン** 再読み込みアイコン ![](assets/unshimmed-report-refresh-icon.png) をクリックして、レポートがしばらくの間ブラウザーに表示された場合に、レポートの結果を更新します。

1. （条件付き）レポートでフィルターまたはプロンプトを使用する場合は、「**フィルターとプロンプトを表示**」をクリックして、表示中のレポートで使用されているフィルターとプロンプトのリストを表示します。レポートにフィルターのみが含まれる場合、またはプロンプトのみが含まれる場合は、「**フィルターを表示**」または「**プロンプトを表示**」が表示されます。

   ![フィルターとプロンプトを表示](assets/unshimmed-show-filters-and-prompts.png)

   情報は、ページの左側のレポート名の下に表示されます。プロンプトの場合は、手順 3 に従ってレポートの実行時に選択したプロンプトに関する情報が表示されます。

1. カスタムプロンプトを使用している場合は、表示されません。システムプロンプトのみが表示されます。カスタムフィルターは常に表示されます。

## キャッシュされたレポートを表示

しばらくの間ブラウザーに表示しているレポートがキャッシュされる場合があります。キャッシュされたレポートを強制的に再読み込みするには、次のいずれかの操作を実行します。

* レポート設定を編集し、レポートを保存します。
* ビュー、グループまたはフィルターを変更します。
* **再読み込みアイコン**![ 再読み込みアイコン ](assets/unshimmed-report-refresh-icon.png) をクリックします
このオプションは、レポートが保存された時刻を示すメッセージ ボックス内のページの右上隅か、レポートが配置されているダッシュボードの右上隅にあります。 ダッシュボードの再読み込みについて詳しくは、[ダッシュボードの概要](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)の記事の「ダッシュボードを表示」の節を参照してください。

* 「概要」タブ、「マトリックス」タブまたは「グラフ」タブに移動して、最初のページ以外のレポートのページにアクセスします。
