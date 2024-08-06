---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートのリストを書き出し
description: 管理職またはタイムシート承認者は、担当する従業員のタイムシートに関する情報をすばやく表示するために、タイムシートのリストをダウンロードする必要がある場合があります。これを行うには、タイムシートのリストを書き出します。
author: Alina
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 95%

---

# タイムシートのリストを書き出し

<!--Audited: 8/2024-->

管理職またはタイムシート承認者は、担当する従業員のタイムシートに関する情報をすばやく表示するために、タイムシートのリストをダウンロードする必要がある場合があります。これを行うには、タイムシートのリストを書き出します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：ライト以上 </p>
   <p>現在：レビュー以上 </p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクとイシューに対する表示またはそれ以上のアクセス権限 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タイムシートに対する表示以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old permissions:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to Tasks and Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the timesheets</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan or license type you have, contact your Workfront administrator.-->

## タイムシートのリストを書き出し

{{step1-to-timesheets}}

**タイムシート** エリアが開きます。


![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （オプション）**検索**&#x200B;アイコン ![](assets/search-icon.png) をクリックし、キーワードを入力して、特定のタイムシートを検索します。例えば、タイムシートの時間枠または所有者名を検索できます。

1. （オプション）次のいずれかの操作を行って、タイムシートリストのフィルターを更新します。

   * ページの右上隅にある「**マイタイムシート承認**」を選択して、承認するタイムシートのみを表示する

     または

     「**マイタイムシート**」を選択して、自分のタイムシートのみを表示する。

     これにより、「マイタイムシート承認」フィルターまたは「マイタイムシート」フィルターが、タイムシートリストに適用されます。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * フィルターアイコン ![](assets/filter-nwepng.png) をクリックして別のフィルターを適用するか、新しいフィルターを作成します。フィルターの作成または更新については、[Adobe Workfront でフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者が、設定領域の「リスト制御」またはレイアウトテンプレートから「マイタイムシート承認」フィルターと「マイタイムシート」フィルターを削除した場合、「マイタイムシート承認」オプションと「マイタイムシート」オプションは、タイムシートリストの上部またはフィルターリストには表示されません。詳しくは、次の記事を参照してください。
   >
   >   
   >   
   >   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （オプション）**表示**&#x200B;アイコン ![](assets/view-icon.png) または&#x200B;**グループ化**&#x200B;アイコン ![](assets/grouping.png) をクリックして、別のビューやグループ化を適用するか、新しいビューやグループ化を作成します。

   フィルター、ビューまたはグループ化の作成については、次の記事を参照してください。

   * [Adobe Workfront でフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront でビューを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront でのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 書き出すタイムシートを選択して、**書き出し**&#x200B;アイコン ![](assets/export-38x15.png) をクリックします。

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. タイムシートの一覧を書き出すファイルの種類を次のオプションから選択します。

   * PDF 横
   * PDF 縦
   * PDF のその他のサイズ
   * Excel
   * Excel（xlsx）
   * タブ区切り

   タイムシートのリストは、選択した形式でコンピューターにダウンロードされ、次のタイムシート情報が含まれます。

   * 日付範囲
   * 所有者名
   * 合計時間数
   * 超過作業時間
   * 承認者名
   * ステータス
