---
product-area: reporting;user-management
keywords: 保存、新規、レポート、コピー
navigation-topic: create-and-manage-reports
title: レポートのコピーの作成
description: アクセス権のある任意のレポートのコピーを作成できます。 カスタムレポートの正確なコピーを作成するか、新しいバージョンのデフォルトレポートを保存することができます。 レポートをコピーすると、コピーしたレポートの所有者になり、「マイレポート」セクションに表示されます。
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# レポートのコピーの作成

アクセス権のある任意のレポートのコピーを作成できます。 カスタムレポートの正確なコピーを作成するか、新しいバージョンのデフォルトレポートを保存することができます。 レポートをコピーすると、コピーしたレポートの所有者になり、「マイレポート」セクションに表示されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## レポートの正確なコピーの作成

所有者となるレポートのコピーを作成する場合は、次の手順を実行します。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **レポート**&#x200B;を、**すべてのレポート**.
1. レポートを開きます。
1. クリック **レポートのアクション**&#x200B;を、 **コピー**.

   >[!TIP]
   >
   >レポートがデフォルトのレポートの場合、コピーオプションはレポートのアクションメニューに表示されません。\
   >デフォルトのレポートのコピーを作成する方法について詳しくは、 [レポートの新しいバージョンの作成](#create-a-new-version-of-a-report).

   ![レポートのコピー](assets/nwe-fulllistofreportactions-2022.png)

   元のレポートのコピーが作成され、デフォルトの名前が *のコピー [元のレポートの名前]*. 例えば、「Q4 Completed Tasks」というレポートの名前には、「Copy of Q4 Completed Tasks」と表示されます。

1. （オプション）レポートの名前を変更するには、新しい名前を入力します。

   >[!TIP]
   >
   >新しい名前を入力する前にタイトルの選択を解除した場合は、レポートタイトルを選択し、名前を削除してから、新しい名前を入力します。

1. （オプション）新しいバージョンのレポートを他のユーザーと共有するには、 **レポートのアクション**&#x200B;を、 **共有**.

   >[!NOTE]
   >
   >共有情報は、元のバージョンからコピーしたレポートには転送されません。\
   >以前のレポートの共有先の確認方法について詳しくは、 [レポートアクティビティに関するレポートの作成](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. （オプション）元のレポートに対する管理権限を持っていて、元のレポートが不要になった場合は、元のレポートを削除して、Workfrontで不要な重複レポートを削除できます。

   元のレポートを削除するには、次の手順を実行します。

   1. レポートに移動します。
   1. クリック **レポートのアクション**&#x200B;を、 **削除**.

   1. クリック **はい、削除します** をクリックして、レポートの削除を確認します。

## レポートの新しいバージョンの作成 {#create-a-new-version-of-a-report}

デフォルトのレポートのコピーを作成する場合は、次の手順を実行します。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **レポート**&#x200B;を、**すべてのレポート**.
1. デフォルトのレポート名をクリックして開きます。
1. クリック **レポートのアクション**&#x200B;を、 **編集**.

   ![レポートの編集](assets/nwe-reportactionsfordefaultreport-2022.png)

1. レポートの次のタブで、必要に応じて変更を加えます。

   * **列（表示）**:ビューのカスタマイズの詳細については、「 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **グループ化**:グループ化のカスタマイズについて詳しくは、「 [Adobe Workfrontでのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **フィルター**:フィルターのカスタマイズについて詳しくは、 [Adobe Workfrontのフィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **グラフ**:レポートグラフのカスタマイズの詳細については、「 [レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. 右上隅で、 **レポート設定**.
1. 内 **レポートタイトル** フィールドに新しい名前を付けます。
1. クリック **完了**.
1. クリック **新しいレポートとして保存**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. （オプション）新しいバージョンのレポートを他のユーザーと共有するには、 **レポートのアクション**&#x200B;を、 **共有**.
