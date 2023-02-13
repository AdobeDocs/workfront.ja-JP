---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートを承認
description: タイムシートの承認プロセスにより、管理者は直属の部下の作業時間を表示できます。 承認者は、記録されたすべての時間が正しい領域に割り当てられ、その期間に対して十分な時間数が記録されたことを確認できます。
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# タイムシートを承認

タイムシートの承認プロセスにより、管理者は直属の部下の作業時間を表示できます。 承認者は、記録されたすべての時間が正しい領域に割り当てられ、その期間に対して十分な時間数が記録されたことを確認できます。

Adobe Workfrontでは、この領域でサポートするタイムシートの承認を構成できます。

タイムシートの送信の詳細については、 [承認用のタイムシートを送信](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
 </tbody> 
</table>

*保有しているプランやライセンスの種類を確認するには、Workfront管理者にお問い合わせください。

## タイムシート承認者を指定

通常、タイムシートは、機能マネージャまたは人事担当者によって承認されます。 （タイムシートは、通常、プロジェクトマネージャによって承認されていません。）

タイムシートの承認者は、タイムシートプロファイルの作成時に定義されます。 承認者に指定するには、プランライセンスが必要です。

タイムシート承認者の指定の詳細については、「 [タイムシートプロファイルを作成または編集する](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) 記事内 [タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## タイムシートを承認

承認者として指定された、提出済みのタイムシートを承認できます。 タイムシートを承認用に提出すると、タイムシートは **承認** の **ホーム**  ページ。 詳しくは、 [作業の承認](../../review-and-approve-work/manage-approvals/approving-work.md).

Workfront管理者が [ ユーザーに対するタイムシートの承認 ] および [ ユーザーに対するタイムシートの却下 ] イベントハンドラを有効にした場合は、タイムシートが承認または却下された後に通知が表示されます。 イベント通知の有効化について詳しくは、 [Adobe Workfrontで使用可能なイベント通知](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

タイムシートを承認するには、次の手順に従います。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある
1. クリック **タイムシート**.
1. を選択します。 **自分のタイムシート承認** ページの右上隅に、承認したタイムシートのみを表示する

   または

   を選択します。 **自分のタイムシート承認** タイムシートリストの一番上でフィルタを設定します。

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >[ 自分のタイムシートの承認 ] オプションは、Workfront管理者またはグループ管理者が [ 設定 ] 領域の [ リスト管理 ] または [ レイアウトテンプレート ] から [ 自分のタイムシートの承認 ] フィルタを削除した場合は、タイムシート一覧の上部またはフィルタ一覧に表示されません。 詳しくは、次の記事を参照してください。
   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. （オプション） **検索** アイコン ![](assets/search-icon.png) をタイムシートリストの先頭に表示し、キーワードを入力して特定のタイムシートを検索します。 期間、または所有者または承認者の名前を検索できます。
1. 承認するタイムシートの期間をクリックします。 タイムシートが開きます。

   >[!TIP]
   承認待ちタイムシートのステータスは [!UICONTROL 送信済み].


1. クリック **承認**

   または

   タイムシートを却下する場合は、[ ] をクリックします。 **拒否** タイムシートの左下隅に表示されます。

   承認済みの場合、タイムシートのステータスは次のように変わります。 **クローズ**.

   却下された場合、タイムシートのステータスは「 」に変わります。 **却下**.
