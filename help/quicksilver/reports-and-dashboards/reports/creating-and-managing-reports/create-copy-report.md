---
product-area: reporting;user-management
keywords: 保存, 新規, レポート, コピー
navigation-topic: create-and-manage-reports
title: レポートのコピーを作成
description: アクセス権のある任意のレポートのコピーを作成できます。カスタムレポートの正確なコピーを作成するか、デフォルトレポートの新しいバージョンを保存することができます。レポートをコピーすると、コピーしたレポートの所有者になり、マイレポートセクションに表示されます。
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 74%

---

# レポートのコピーを作成

<!-- Audited: 11/2024 -->

アクセス権のある任意のレポートのコピーを作成できます。カスタムレポートの正確なコピーを作成するか、デフォルトレポートの新しいバージョンを保存することができます。レポートをコピーすると、コピーしたレポートの所有者になり、マイレポートセクションに表示されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループ化へのアクセスの編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限*</td> 
   <td><p>レポートに対する権限を表示</p></td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## レポートの正確なコピーを作成

カスタムレポートのコピーを作成する場合は、次の操作を行います。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL レポート]**」の順にクリックします。

1. **すべてのレポート** をクリックして、レポートを開きます。

1. 「**レポートのアクション**」、「**コピー**」の順にクリックします。

   >[!TIP]
   >
   >レポートがデフォルトのレポートの場合、コピーオプションはレポートのアクションメニューに表示されません。\
   >デフォルトのレポートのコピーを作成する方法について詳しくは、[レポートの新しいバージョンを作成](#create-a-new-version-of-a-report)を参照してください。

   ![レポートをコピー](assets/unshimmed-report-actions-copy.png)

   元のレポートのコピーが、デフォルト名 _[元のレポートの名前 ] （コピー）_ で作成されます。 例えば、レポートの「Q4 Completed Tasks」のコピーは、「Q4 Completed Tasks （Copy）」という名前になります。

1. （任意）レポートの名前を変更するには、**レポートアクション**&#x200B;**編集** の順にクリックします。 左上隅のテキストボックスに新しい名前を入力し、完了したら「**保存して閉じる** をクリックします。

1. （オプション）新しいバージョンのレポートを他のユーザーと共有するには、「**レポートのアクション**」をクリックして、次に「**共有**」をクリックします。

   >[!NOTE]
   >
   >共有情報は、元のバージョンからコピーしたレポートには転送されません。\
   >以前のレポートの共有先の確認方法について詳しくは、[レポートアクティビティに関するレポートを作成](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify)を参照してください。

1. （オプション）元のレポートに対する管理権限を持っていて、元のレポートが不要になった場合は、元のレポートを削除して、Workfront 内の不要な重複レポートを削除できます。

   元のレポートを削除するには、以下のように行います。

   1. レポートに移動します。

   1. 「**レポートのアクション**」、「**削除**」の順にクリックします。

   1. 「**はい、削除します**」をクリックして、レポートの削除を確認します。

## レポートの新しいバージョンを作成 {#create-a-new-version-of-a-report}

組み込みレポートのコピーを作成する場合は、次の操作を行います。

1. Adobe Workfrontの右上隅にある **メインメニュー** アイコン ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png) をクリックします。

1. **レポート** をクリックし、**すべてのレポート** をクリックします。
1. ビルトインレポートの名前をクリックして開きます。
1. 「**レポートのアクション**」、「**編集**」の順にクリックします。

   ![レポートを編集](assets/unshimmed-report-actions-default-report.png)

1. レポートの以下のタブで、必要に応じて変更を加えます。

   * **列（表示）**：表示のカスタマイズに関して詳しくは、[Adobe Workfront の表示の概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)を参照してください。
   * **グループ化**：グループ化のカスタマイズに関して詳しくは、[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。
   * **フィルター**：フィルターのカスタマイズについて詳しくは、[フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)の記事を参照してください。
   * **チャート**：レポートチャートのカスタマイズについて詳しくは、[レポートにチャートを追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

1. 右上隅の「**レポート設定**」をクリックします。
1. 「**レポートタイトル**」フィールドで、レポートに新しい名前を付けます。
1. 「**完了**」をクリックします。
1. 「**新規レポートとして保存**」をクリックします。

   ![&#x200B; 新規報告書として保存 &#x200B;](assets/unshimmed-save-as-new-report.png)

1. （オプション）新しいバージョンのレポートを他のユーザーと共有するには、「**レポートアクション**」、「**共有**」の順にクリックします。
