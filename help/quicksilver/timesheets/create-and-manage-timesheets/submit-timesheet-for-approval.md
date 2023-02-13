---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 承認用のタイムシートを送信
description: タイムシートを承認用に送信すると、管理者は作業時間を表示できます。 承認者は、記録されたすべての時間が正しい領域に割り当てられ、その期間に十分な時間数が記録されたことを確認できます。
author: Alina
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# 承認用のタイムシートを送信

タイムシートを承認用に送信すると、管理者は作業時間を表示できます。 承認者は、記録されたすべての時間が正しい領域に割り当てられ、その期間に十分な時間数が記録されたことを確認できます。

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
   <td> <p>タスクおよび問題に対する権限を表示または上限に設定する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 承認用のタイムシートを送信

* [承認用のタイムシートを送信](#submit-a-timesheet-for-approval)
* [提出されたタイムシートの状態の表示](#view-the-status-of-a-submitted-timesheet)

### 承認用のタイムシートを送信

タイムシート承認者が設定された後（「 」の節で説明） [タイムシート承認者を指定](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) 記事内 [タイムシートを承認](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md))、 **閉じる** タイムシートの下部にあるボタンが **承認用に送信** 」ボタンをクリックします。

タイムシートを承認用に発行するには、次の手順に従います。

1. 承認者を持つように構成されたタイムシートに移動します。
1. ログ時間 ( [ログ時間](../../timesheets/create-and-manage-timesheets/log-time.md).
1. クリック **承認用に送信** タイムシートの承認プロセスを開始します。

   ![](assets/submit-for-approval-button-on-timesheet-nwe.png)

   この **承認用に送信** ボタンが **承認**, **拒否**、および **再現率** ボタン タイムシートの状態が次の値に変わります： **送信済み**.

   タイムシートが承認用に送信されると、承認者は、 **承認** 領域 **ホーム** ページ。 次のことが起こる可能性があります。

   * ユーザーが承認した場合、 **再現率** ボタンの変更 **再度開く** タイムシートのステータスの更新先 **開く**.
   * もし彼らがそれを拒否すれば、 **承認用に送信** ボタン **再現率** ボタンとタイムシートのステータスの更新先 **却下**.

1. （オプション）「 **再現率** タイムシートを再度開き、時間を更新する必要がある場合。 詳しくは、 [タイムシートを取り消す](#recall-a-timesheet) 」の節を参照してください。

### 提出されたタイムシートの状態の表示 {#view-the-status-of-a-submitted-timesheet}

タイムシートを送信した後に、そのタイムシートの状態を表示できます。

Workfront管理者が [ ユーザーに対するタイムシートの承認 ] および [ ユーザーに対するタイムシートの却下 ] イベントハンドラを有効にした場合は、タイムシートが承認または却下された後に通知が表示されます。 イベント通知の有効化について詳しくは、 [Adobe Workfrontで使用可能なイベント通知](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

これらの通知を使用しない場合は、Workfrontの [ タイムシート ] 領域で、提出されたタイムシートの状態を確認できます。

タイムシートの状態を表示するには、次の手順に従います。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある
1. クリック **タイムシート**. この **すべて** デフォルトでは「フィルター」が選択されています。

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
   >   
   >   
   >   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （条件付き） **マイタイムシート**&#x200B;で、 **標準** ビューが適用され、 **ステータス** 列。

   タイムシートには次のステータスがあります。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">開く</td> 
      <td> <p>タイムシートは現在開いているので、時刻を記録できます。 </p> <p>取り消されたタイムシートは、ステータスが [ 開く ] になって表示されます。 詳しくは、 <a href="#recall-a-timesheet" class="MCXref xref">タイムシートを取り消す</a> 」の節を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">送信済み</td> 
      <td>タイムシートを承認用に提出しましたが、まだ承認されていません。 提出されたタイムシートを取り消して、編集を続行できます。 詳しくは、 <a href="#recall-a-timesheet" class="MCXref xref">タイムシートを取り消す</a> 」の節を参照してください。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">クローズ</td> 
      <td> <p>次のシナリオが存在します。</p> 
       <ul> 
        <li> <p>タイムシートに承認者がない場合は、時間を保存して終了しました。</p> </li> 
        <li> <p>タイムシートに承認者がある場合は、承認用に提出し、承認済みです。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">拒否</td> 
      <td>タイムシートを承認用に提出し、承認者が拒否しました。</td> 
     </tr> 
    </tbody> 
   </table>

## タイムシートを取り消す {#recall-a-timesheet}

既に承認用に提出されたタイムシートを取り消すことができます。 取り消し可能なのは、承認されていないタイムシートのみです。

タイムシートを取り消すには、次の手順に従います。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **タイムシート**.
1. クリック **マイタイムシート** 画面の右上隅にある、または **マイタイムシート** から **フィルター** ![](assets/filter-nwepng.png) ドロップダウンメニュー。
1. ステータスがのタイムシートの期間をクリックします **送信済み**.
1. クリック **再現率**.

   タイムシートが再び編集可能になり、ステータスが次のように変わります。 **開く**.
