---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシート情報を編集する
description: タイムシートに管理アクセス権を持つユーザーは、Adobe Workfrontで既存のタイムシートに関する情報を編集できます。 例えば、所有者、承認者、またはタイムシートの期間を編集できます。
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 92%

---

# タイムシート情報を編集する

タイムシートに管理アクセス権を持つユーザーは、Adobe Workfrontで既存のタイムシートに関する情報を編集できます。 例えば、所有者、承認者、またはタイムシートの期間を編集できます。

1 つのタイムシートの情報を編集することも、複数のタイムシートを一括編集することもできます。

>[!IMPORTANT]
>
>ユーザーがタイムシートプロファイルに関連付けられ、タイムシートが自動的に生成される場合、既存のタイムシートに対して行った変更は、将来の日付に対して生成されるタイムシートには反映されません。自動的に生成されるすべてのタイムシートには、タイムシートプロファイルで確立された設定が含まれます。詳しくは、[タイムシートプロファイルを作成](../create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td><p>タイムシートへの管理アクセス</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タイムシートを編集する

1. Adobe Workfront の右上隅で&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**タイムシート**」をクリックします。

   「**すべて**」のフィルターはデフォルトで選択されており、表示できるアクセス権のあるすべてのタイムシートが表示されます。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （オプション）**検索**&#x200B;アイコン ![](assets/search-icon.png) をクリックし、キーワードを入力して、特定のタイムシートを検索します。例えば、タイムシートの期間または所有者名を検索できます。

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
   >   * [レイアウトテンプレートを使用したフィルター、ビュー、およびグループ化をカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （オプション）**表示**&#x200B;アイコン ![](assets/view-icon.png) または&#x200B;**グループ化**&#x200B;アイコン ![](assets/grouping.png) をクリックして、別のビューやグループを適用するか、新しいビューやグループを作成します。

   フィルター、ビューまたはグループ化の作成については、次の記事を参照してください。

   * [Adobe Workfront でフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront でビューを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront でのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 1 つまたは複数のタイムシートを選択し、タイムシートリストの一番上にある&#x200B;**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。
1. 次の情報を表示または指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>所有者</strong> </td> 
      <td> <p>これは、タイムシートが作成されたユーザーの名前です。このフィールドは編集できません。 </p> <p>複数のタイムシートを選択した場合、このフィールドは表示されません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>開始日</strong> </td> 
      <td>これは、タイムシートの開始日です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>終了日</strong> </td> 
      <td> これは、タイムシートの終了日です。</td> 
     </tr>
<tr> 
      <td role="rowheader"><strong>ステータス</strong> </td> 
      <td> これがタイムシートのステータスです。
タイムシートのステータスについて、次のオプションがあります。 
      <ul><li><b>オープン</b>：タイムシートを開いて、時間エントリを編集できます。</li>
      <li><b>送信済み</b>：指定された承認者にタイムシートが承認用に送信されます。</li>
      <li><b>却下</b>：タイムシートは承認者によって承認されず、ユーザーが時間エントリを編集できるようになりました。</li>
      <li><b>クローズ</b>：タイムシートは、ユーザーがクローズしたか、承認者が承認したためクローズされました。クローズされたタイムシートに時間を追加することはできません。</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>承認者</strong> </td> 
      <td> <p>承認者は、タイムシートに関連付けられたユーザーのタイムシートを承認するユーザーです。承認者として設定できるのは、タイムシートへの管理者アクセス権を持つユーザーだけです。 </p> <p>タイムシート管理権限について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理アクセス権をユーザーに付与</a>を参照してください。</p> <p>タイムシート承認者の名前の入力を開始し、リストに表示されたら、その名前を選択します。</p> <p>1 つのタイムシートに複数の承認者を設定できます。この場合、承認者の 1 人がタイムシートを承認すると、タイムシートは<strong>クローズ</strong>とマークされ、残りのすべての承認者のタイムシート承認リストから消えます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>時間の編集が可能</strong> </td> 
      <td> <p>承認者がタイムシートの時間を編集できるようにする場合は、このオプションを選択します。</p> <p>複数のタイムシートを選択した場合は、このオプションは使用できません。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">超過作業時間</span> </td> 
      <td> <p>タイムシートの「超過作業時間」ボックスを非表示にすることができます。</p> <p>このオプションはデフォルトでは無効になっています。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
