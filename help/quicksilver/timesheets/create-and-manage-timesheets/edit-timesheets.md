---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシート情報の編集
description: タイムシートへの管理者アクセス権を持つユーザーは、 Adobe Workfrontの既存のタイムシートに関する情報を編集できます。 たとえば、所有者、承認者、またはタイムシートの期間を編集できます。
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 2%

---

# タイムシート情報の編集

タイムシートへの管理者アクセス権を持つユーザーは、 Adobe Workfrontの既存のタイムシートに関する情報を編集できます。 たとえば、所有者、承認者、またはタイムシートの期間を編集できます。

1 つのタイムシートの情報を編集することも、複数のタイムシートを一括編集することもできます。

>[!IMPORTANT]
>
>ユーザーがタイムシートプロファイルに関連付けられ、タイムシートが自動的に生成される場合、既存のタイムシートに対して行った変更は、将来の日付に対して生成されるタイムシートには反映されません。 自動的に生成されるすべてのタイムシートには、タイムシートプロファイルで設定された設定が含まれます。 詳しくは、 [タイムシートプロファイルを作成](../create-and-manage-timesheets/create-timesheet-profiles.md)


## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タイムシートに対する管理者アクセス権が必要です。 </p> <p>詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タイムシートを編集

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **タイムシート**.

   The **すべて** 既定では [ フィルタ ] が選択され、表示するアクセス権のあるすべてのタイムシートが表示されます。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （オプション） **検索** アイコン ![](assets/search-icon.png) キーワードを入力し、特定のタイムシートを検索します。 たとえば、タイムシートの期間または所有者名を検索できます。

1. （オプション）次のいずれかの操作を行って、タイムシートの一覧のフィルタを更新します。

   * 選択 **自分のタイムシート承認** ページの右上隅に、承認したタイムシートのみを表示する

     または

     選択 **マイタイムシート** をクリックして、タイムシートのみを表示します。

     これにより、[ 自分のタイムシートの承認 ] または [ 自分のタイムシート ] フィルタが、タイムシートの一覧に適用されます。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * フィルターアイコンをクリックします。 ![](assets/filter-nwepng.png) 別のフィルターを適用するか、新しいフィルターを作成します。 フィルターの作成または更新について詳しくは、 [Adobe Workfrontでフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Workfront管理者またはグループ管理者が [ セットアップ ] 領域の [ リスト管理 ] または [ レイアウトテンプレート ] から [ 自分のタイムシート ] フィルタを削除した場合、[ 自分のタイムシート承認 ] と [ 自分のタイムシート ] オプションは、タイムシート一覧の先頭またはフィルタ一覧に表示されません。 詳しくは、次の記事を参照してください。
   >
   >   
   >   
   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （オプション）**表示** ![](assets/view-icon.png) または **グループ化** ![](assets/grouping.png) アイコンを使用して、別のビューやグループを適用するか、新しいビューやグループを作成します。

   フィルター、ビューまたはグループの作成について詳しくは、次の記事を参照してください。

   * [Adobe Workfrontでフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfrontでビューを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfrontでのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 1 つまたは複数のタイムシートを選択し、 **編集** アイコン ![](assets/edit-icon.png) をタイムシートリストの先頭に表示します。
1. 次の情報を表示または指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>所有者</strong> </td> 
      <td> <p>これは、タイムシートが作成されたユーザーの名前です。 このフィールドは編集できません。 </p> <p>複数のタイムシートを選択した場合、このフィールドは表示されません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>開始日</strong> </td> 
      <td>タイムシートの開始日です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>終了日</strong> </td> 
      <td> タイムシートの終了日です。</td> 
     </tr>
<tr> 
      <td role="rowheader"><strong>ステータス</strong> </td> 
      <td> これはタイムシートの状態です。
      タイムシートの状態に関するオプションとして、次のものが考えられます。 
      <ul><li><b>開く</b>：タイムシートは開封済みで、時間エントリは編集できます。</li>
      <li><b>送信済み</b>：指定された承認者にタイムシートが承認用に送信されます。</li>
      <li><b>却下</b>：タイムシートは承認者によって承認されず、ユーザーが時間エントリを編集できるようになりました。</li>
      <li><b>閉じる</b>：タイムシートは、ユーザーによって閉じられているか、承認者によって承認されているため、閉じられました。 クローズ済みのタイムシートに時間を追加することはできません。</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>承認者</strong> </td> 
      <td> <p>承認者は、タイムシートに関連付けられたユーザーのタイムシートを承認するユーザーです。 承認者として設定できるのは、タイムシートへの管理者アクセス権を持つユーザーだけです。 </p> <p>タイムシート管理権限の詳細については、「 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> <p>タイムシート承認者の名前を入力し、一覧に表示されたら、その名前を選択します。</p> <p>1 つのタイムシートに複数の承認者を設定できます。 この場合、承認者の 1 人がタイムシートを承認すると、タイムシートは次のようにマークされます。 <strong>閉じる</strong> 残りのすべての承認者のタイムシート承認リストに表示されなくなります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>時間を編集可能</strong> </td> 
      <td> <p>承認者がタイムシートの時間を編集できるようにする場合は、このオプションを選択します。</p> <p>複数のタイムシートを選択した場合は、このオプションは使用できません。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">超過作業時間</span> </td> 
      <td> <p>タイムシートの [ 超過作業時間 ] ボックスを非表示にすることもできます。</p> <p>このオプションはデフォルトでは無効になっています。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
