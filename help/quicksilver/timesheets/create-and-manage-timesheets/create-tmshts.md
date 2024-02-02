---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 単一のタイムシートの作成
description: 定期的でないタイムシートが必要な場合は、1 回限りのタイムシートを手動で作成できます。タイムシートの終了日に達し、より多くのタイムシートが必要になった場合は、新しいタイムシートを作成する必要があります。
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: ht
source-wordcount: '1090'
ht-degree: 100%

---

# 単一のタイムシートの作成

定期的でないタイムシートが必要な場合は、1 回限りのタイムシートを手動で作成できます。タイムシートの終了日に達し、より多くのタイムシートが必要になった場合は、新しいタイムシートを作成する必要があります。

ユーザーからの追加の介入なしに（推奨）、定期的なタイムシートを生成するタイムシートプロファイルの作成について詳しくは、[タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

>[!NOTE]
>
>* 1 回限りのタイムシートは、グループに対して作成できません。
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* 1 回限りのタイムシートを作成する場合、タイムシートに含める特定の一般的な時間タイプを選択することはできません。システムで有効化されたすべての一般的な時間タイプは、手動で作成されたタイムシートに表示されます。
>
>  タイムシートに表示する特定の一般的な時間タイプのみを選択する場合は、タイムシートプロファイルを使用します。タイムシートプロファイルについて詳しくは、[タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。
>

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タイムシートに対する管理アクセス権が必要です。 </p> <p>詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">ユーザーに対する特定の領域への管理アクセス権の付与</a>を参照してください。</p> <p><b> メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がユーザーのアクセスレベルを変更する方法については、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 単一のタイムシートの作成

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**タイムシート**」をクリックします。**すべて**&#x200B;のフィルターがデフォルトでは選択されています。これにより、表示するアクセス権のあるすべてのタイムシートが表示されます。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （オプション）次のいずれかの操作を行って、タイムシートリストのフィルターを更新します。

   * ページの右上隅にある「**マイタイムシート承認**」を選択して、承認するタイムシートのみを表示する。

     または

     「**マイタイムシート**」を選択して、自分のタイムシートのみを表示する。

     これにより、「マイタイムシート承認」フィルターまたは「マイタイムシート」フィルターが、タイムシートのリストに適用されます。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * フィルターアイコン ![](assets/filter-nwepng.png) をクリックして別のフィルターを適用するか、新しいフィルターを作成します。フィルターの作成または更新については、[Adobe Workfront でのフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者が、設定エリアのリスト制御またはレイアウトテンプレートから、「マイタイムシート承認」と「マイタイムシート」のフィルターを削除した場合、「マイタイムシート承認」と「マイタイムシート」のオプションは、タイムシート一覧の先頭にもフィルター一覧にも表示されません。詳しくは、次の記事を参照してください。
   > 
   >   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （オプション）**検索**&#x200B;アイコン ![](assets/search-icon.png) をクリックして、キーワードを入力し、特定のタイムシートを検索します。例えば、所有者名のタイムシート期間を検索できます。

1. （オプション）**表示** ![](assets/view-icon.png) アイコンまたは&#x200B;**グループ化** ![](assets/grouping.png) アイコンをクリックして、別のビューやグループを適用するか、新しいビューやグループを作成します。

   フィルター、ビューまたはグループ化の作成については、次の記事を参照してください。

   * [Adobe Workfront でのフィルターの作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront でビューの作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront でのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. タイムシートのリストの上部にある「**新規タイムシート**」をクリックします。

   次の情報を指定します。

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>次のタイムシートを作成 :</strong> </td> 
      <td>作成するタイムシートの対象となるユーザー、担当業務またはチームの名前を入力していき、リストに表示されたら名前をクリックします。</td> 
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
      <td role="rowheader"><strong>承認者</strong> </td> 
      <td>承認者とは、タイムシートに関連付けられたユーザーのタイムシートを承認するユーザーです。承認者として設定できるのは、タイムシートの管理権限を持つユーザーのみです。タイムシート管理権限について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理アクセス権をユーザーに付与</a>を参照してください。<br>タイムシート承認者の名前を入力していき、リストに表示されたら、その名前をクリックします。<br>1 つのタイムシートに複数の承認者を設定できます。この場合、承認者のうちの 1 人がタイムシートを承認すると、タイムシートは<strong>クローズ</strong>とマークされ、残りのすべての承認者のタイムシート承認リストに表示されなくなります。</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>時間を編集可能</strong> </td>

   <td> <p>承認者がタイムシートの時間を編集できるようにする場合は、このオプションを選択します。</p>

   このオプションは、設定／タイムシートと時間／環境設定エリアの「**タイムシートの編集を所有者と管理者に制限**」設定と連携して機能します。詳しくは、<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">タイムシートと時間の環境設定</a>を参照してください。

   次のシナリオが存在します。

   <ul>
      <li>「<b>タイムシートの編集を所有者と管理者に制限</b>」オプションが有効な場合は、次のようになります。</li>
   <ul><li>承認者は、「<b>時間を編集可能</b>」が有効か無効かにかかわらず、タイムシートの承認と拒否のみを行えます。 </li>
   <li>タイムシート所有者のマネージャーは、自分のダイレクトレポートのタイムシートのみを表示できます。</li></ul>
   <li>「<b>タイムシートの編集を所有者と管理者に制限</b>」オプションが無効な場合は、次のようになります。</li>
   <ul><li>「<b>時間を編集可能</b>」が有効になっている場合、承認者はタイムシートを送信、再度開くまたは閉じることができ、時間を編集できます。</li>
   <li>「<b>時間を編集可能</b>」が無効になっている場合、承認者はタイムシートを送信、再度開くまたは閉じることができず、時間を編集することもできません。承認者が行えるのは、タイムシートの承認または却下のみです。 </li>
   <li>タイムシート所有者のマネージャーは、ダイレクトレポートのタイムシートの提出、取り消し、リオープン、編集を行うことができます。</li></ul>
   </ul>

   <p><b>メモ</b>

   承認を受けるためにタイムシートを送信すると、時間を編集できなくなります。提出されたタイムシートを編集可能な状態に戻すには、タイムシートを取り消すか、承認者にタイムシートを却下させます。詳しくは、<a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">承認を受けるためのタイムシートの送信</a>と<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">タイムシートの承認</a>を参照してください。</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">超過作業時間</span> </td> 
      <td>タイムシートの「超過作業時間」ボックスを非表示にすることができます。このオプションはデフォルトでは無効になっています。</td> 
      </tr> 
      </tbody> 
   </table>

1. 「**タイムシートを作成**」をクリックします。

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## タスクとイシューがユーザーのタイムシートに表示される条件

タスクやイシューが次の条件のいずれかに一致する場合、ユーザーに割り当てられたタスクやイシューは、ユーザーのタイムシートに自動的に表示されます。

* ユーザーがタスクやイシューに費やした時間数を記録した
* タスクやイシューの予定日がタイムシートの日付範囲内に収まる
* タスクやイシューに実際の開始日がある（タスクやイシューのステータスは「処理中」）
* タスクやイシューがタイムシートにピン留めされている
* 予定完了日がタイムシートの日付範囲内に収まり、そのステータスが「処理中」になっている

**次以内の作業についてタイムシートを自動入力する**」環境設定（「タイムシートと時間」環境設定にある）が選択されていない場合、タイムシートには「処理中」のステータスを持つイシューとタスクが表示されます。「タイムシートと時間」環境設定について詳しくは、[タイムシートと時間の環境設定](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。
