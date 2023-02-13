---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートのリストをエクスポートする
description: 人物マネージャまたはタイムシートの承認者は、担当者のタイムシートに関する情報をすばやく表示するには、タイムシートの一覧をダウンロードする必要がある場合があります。 これを行うには、タイムシートのリストを書き出します。
author: Alina
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 2%

---

# タイムシートのリストをエクスポートする

人物マネージャまたはタイムシートの承認者は、担当者のタイムシートに関する情報をすばやく表示するには、タイムシートの一覧をダウンロードする必要がある場合があります。 これを行うには、タイムシートのリストを書き出します。

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
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよび問題へのアクセス権以上の表示</p> <p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タイムシートに対するアクセス許可を表示するか、それ以上に設定します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有しているプランやライセンスの種類を確認するには、Workfront管理者にお問い合わせください。

## タイムシートのリストをエクスポートする

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **タイムシート**. この **すべて** デフォルトでは「フィルター」が選択されています。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （オプション） **検索** アイコン ![](assets/search-icon.png) キーワードを入力し、特定のタイムシートを検索します。 例えば、タイムセットの時間枠や所有者名を検索できます。

1. （オプション）次のいずれかの操作を行って、タイムシートの一覧のフィルタを更新します。

   * 選択 **自分のタイムシート承認** ページの右上隅に、承認したタイムシートのみを表示する

      または

      選択 **マイタイムシート** タイムシートのみを表示する場合。

      これにより、[ 自分のタイムシートの承認 ] または [ 自分のタイムシート ] フィルタが、タイムシートの一覧に適用されます。

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * フィルターアイコンをクリックします。 ![](assets/filter-nwepng.png) 別のフィルターを適用するか、新しいフィルターを作成します。 フィルターの作成または更新について詳しくは、 [Adobe Workfrontでフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Workfront管理者またはグループ管理者が [ セットアップ ] 領域の [ リスト管理 ] または [ レイアウトテンプレート ] から [ 自分のタイムシート ] フィルタを削除した場合、[ 自分のタイムシート承認 ] および [ 自分のタイムシート ] オプションは、タイムシート一覧の先頭またはフィルタ一覧に表示されません。 詳しくは、次の記事を参照してください。
   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （オプション） **表示** ![](assets/view-icon.png) または **グループ化** ![](assets/grouping.png) アイコンを使用して、別のビューやグループを適用するか、新しいビューやグループを作成します。

   フィルター、ビューまたはグループの作成について詳しくは、次の記事を参照してください。

   * [Adobe Workfrontでフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfrontでビューを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfrontでのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. エクスポートするタイムシートを選択し、 **書き出し**  ![](assets/export-38x15.png) アイコン

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. タイムシートの一覧を書き出すファイルの種類を次のオプションから選択します。

   * PDFLadscape
   * PDF縦
   * PDFのその他のサイズ
   * Excel
   * Excel (xlsx)
   * タブ区切り

   タイムシートの一覧は、選択した形式でコンピュータにダウンロードされ、次のタイムシート情報が含まれます。

   * 日付範囲
   * 所有者名
   * 合計時間数
   * 超過金額
   * 承認者名
   * ステータス
