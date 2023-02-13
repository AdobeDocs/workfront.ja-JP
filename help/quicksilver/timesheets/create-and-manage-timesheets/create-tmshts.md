---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 単一使用のタイムシートを作成する
description: 定期的でないタイムシートが必要な場合は、一時使用のタイムシートを手動で作成できます。 タイムシートの終了日に達し、より多くのタイムシートが必要になった場合は、新しいタイムシートを作成する必要があります。
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# 単一使用のタイムシートを作成する

定期的でないタイムシートが必要な場合は、一時使用のタイムシートを手動で作成できます。 タイムシートの終了日に達し、より多くのタイムシートが必要になった場合は、新しいタイムシートを作成する必要があります。

ユーザーからの追加の介入なしにユーザーの定期的なタイムシートを生成するタイムシートプロファイルの作成の詳細については、「 [タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* 単一使用のタイムシートは、グループに対して作成できません。

>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* 単一使用のタイムシートを作成する場合、タイムシートに含める特定の一般時間の種類を選択することはできません。 システムで有効化されたすべての一般的な時間タイプは、手動で作成されたタイムシートに表示されます。
>
>  タイムシートに表示する特定の一般時間タイプのみを選択する場合は、タイムシートプロファイルを使用します。 タイムシートプロファイルの詳細については、「 [タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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
   <td> <p>タイムシートに対する管理者アクセス権が必要です。 </p> <p>詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> <p><b> メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 単一使用のタイムシートを作成する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **タイムシート**. この **すべて** デフォルトでは「フィルター」が選択されています。 これにより、表示するアクセス権のあるすべてのタイムシートが表示されます。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （オプション）次のいずれかの操作を行って、タイムシートの一覧のフィルタを更新します。

   * 選択 **自分のタイムシート承認** ページの右上隅に、承認したタイムシートのみを表示する

      または

      選択 **マイタイムシート** タイムシートのみを表示する場合。

      これにより、[ 自分のタイムシートの承認 ] または [ 自分のタイムシート ] フィルタが、タイムシートの一覧に適用されます。

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * フィルターアイコンをクリックします。 ![](assets/filter-nwepng.png) 別のフィルターを適用するか、新しいフィルターを作成します。 フィルターの作成または更新について詳しくは、 [Adobe Workfrontでフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Workfront管理者またはグループ管理者が [ セットアップ ] 領域の [ リスト管理 ] または [ レイアウトテンプレート ] から [ 自分のタイムシート ] フィルタを削除した場合、[ 自分のタイムシート承認 ] および [ 自分のタイムシート ] オプションは、タイムシート一覧の先頭またはフィルタ一覧に表示されません。 詳しくは、次の記事を参照してください。
   > 
   >   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)



1. （オプション） **検索** アイコン ![](assets/search-icon.png) キーワードを入力し、特定のタイムシートを検索します。 たとえば、所有者名のタイムシート期間を検索できます。

1. （オプション） **表示** ![](assets/view-icon.png) または **グループ化** ![](assets/grouping.png) アイコンを使用して、別のビューやグループを適用するか、新しいビューやグループを作成します。

   フィルター、ビューまたはグループの作成について詳しくは、次の記事を参照してください。

   * [Adobe Workfrontでフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfrontでビューを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfrontでのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. クリック **新しいタイムシート** をタイムシートのリストの先頭に追加します。

   次の情報を指定します。

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>次のタイムシートを作成 :</strong> </td> 
      <td>タイムシートを作成するユーザー名、職務の役割、またはチームの入力を開始し、リストに表示されたら、それらをクリックします。</td> 
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
      <td role="rowheader"><strong>承認者</strong> </td> 
      <td>承認者は、タイムシートに関連付けられたユーザーのタイムシートを承認するユーザーです。 タイムシート管理権限を持つユーザーのみが承認者として設定できます。 タイムシート管理権限の詳細については、「 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.<br>タイムシート承認者の名前を入力し、一覧に表示されたら、その名前をクリックします。<br>1 つのタイムシートに複数の承認者を設定できます。 この場合、承認者の 1 人がタイムシートを承認すると、タイムシートは次のようにマークされます。 <strong>クローズ</strong> 残りのすべての承認者のタイムシート承認リストに表示されなくなります。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>時間を編集可能</strong> </td>

   <td> <p>承認者がタイムシートの時間を編集できるようにする場合は、このオプションを選択します。</p>

   このオプションは、 **タイムシートの編集を所有者と管理者に制限する** [ 設定 ] > [ タイムシートと時間 ] > [ 基本設定 ] 領域の設定 詳しくは、 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">タイムシートと時間の基本設定を構成する</a>.

   次のシナリオが存在します。

   <ul>
      <li>次の場合に <b>タイムシートの編集を所有者と管理者に制限する</b> オプションが有効：</li>
   <ul><li>承認者は、タイムシートの承認と拒否を実行できます。タイムシートの承認と拒否は、 <b>時間を編集可能</b> が有効かどうか。 </li>
   <li>タイムシート所有者のマネージャは、自分の直属のレポートのタイムシートのみを表示できます。</li></ul>
   <li>次の場合に <b>タイムシートの編集を所有者と管理者に制限する</b> オプションは無効です。</li>
   <ul><li>次の場合に <b>時間を編集可能</b> が有効になっている場合、承認者はタイムシートを送信、再度開く、または閉じて、時間を編集できます。</li>
   <li>次の場合に <b>時間を編集可能</b> が無効になっている場合、承認者はタイムシートを送信、再度開く、または閉じることができず、時間を編集できません。 承認者は、タイムシートの承認または拒否のみを行うことができます。 </li>
   <li>タイムシート所有者のマネージャは、自分の直属の部下のタイムシートを提出、取り消し、再度開き、編集することができます。</li></ul>
   </ul>

   <p><b>メモ</b>

   タイムシートを承認用に送信すると、時間を編集できなくなります。 提出されたタイムシートを編集可能な状態に戻すには、タイムシートを取り消すか、承認者にタイムシートを拒否させます。 詳しくは、 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">承認用のタイムシートを送信</a> および <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">タイムシートを承認</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">超過作業時間</span> </td> 
      <td>タイムシートの [ 超過作業時間 ] ボックスを非表示にすることもできます。 このオプションはデフォルトでは無効になっています。</td> 
      </tr> 
      </tbody> 
   </table>

1. クリック **タイムシートを作成**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## タスクと問題がユーザーのタイムシートに表示される場合

タスクまたはタスクが次の基準のいずれかに一致する場合、ユーザーに割り当てられたタスクまたはタスクは、ユーザーのタイムシートに自動的に表示されます。

* ユーザーがタスクまたは問題に何時間もログオンした
* タスクまたはタスクの予定日は、タイムシートの日付の範囲内に収まります
* タスクまたはタスクの開始日が実際の開始日です（タスクまたはタスクのステータスは「処理中」です）
* タスクまたは問題はタイムシートに固定されています
* 計画完了日は、タイムシートの日付範囲内で、状態は [ 進行中 ] です

この **タイムシートの事前入力…** 基本設定（[ タイムシートと時間 ] の基本設定）が選択されていない場合、タイムシートには、[ 進行中 ] の状態を持つ問題とタスクが表示されます。 タイムシートと時間の基本設定の詳細については、 [タイムシートと時間の基本設定を構成する](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
