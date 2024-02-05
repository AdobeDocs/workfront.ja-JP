---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートの承認
description: 管理者はタイムシートの承認プロセスで、直属の部下の作業時間を表示できます。承認者は、記録されたすべての時間が正しいエリアに割り当てられ、その期間に対して十分な時間数が記録されていることを確認できます。
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: ht
source-wordcount: '520'
ht-degree: 100%

---

# タイムシートの承認

管理者はタイムシートの承認プロセスで、直属の部下の作業時間を表示できます。承認者は、記録されたすべての時間が正しいエリアに割り当てられ、その期間に対して十分な時間数が記録されていることを確認できます。

これに対応できるよう、Adobe Workfront ではタイムシートの承認を設定する機能が提供されています。

タイムシートの送信について詳しくは、[承認用のタイムシートの送信](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
 </tbody> 
</table>

*ご利用のプランやライセンスタイプは、Workfront 管理者にお問い合わせください。

## タイムシートの承認者の指定

通常、タイムシートは、部門マネージャーまたは人事担当者によって承認されます（通常はプロジェクトマネージャーによって承認されません）。

タイムシートの承認者は、タイムシートプロファイルの作成時に定義されます。承認者に指定されるには、プランライセンスが必要です。

タイムシートの承認者の指定について詳しくは、[タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)の[タイムシートプロファイルの作成または編集](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create)を参照してください。

## タイムシートの承認

承認者は、自分を承認者として指定して提出されたタイムシートを承認できます。承認に向けて提出されたタイムシートは、「**ホーム**」ページの&#x200B;**承認**」にリストされます。詳しくは、[作業の承認](../../review-and-approve-work/manage-approvals/approving-work.md)を参照してください。

Workfront 管理者がユーザーに対するタイムシートの承認およびユーザーイベントハンドラーに対するタイムシートの却下を有効にしている場合は、タイムシートが承認または却下された後に通知が表示されます。イベント通知の有効化について詳しくは、[Adobe Workfront で使用可能なイベント通知](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)を参照してください。

タイムシートを承認するには：

1. Adobe Workfrontの右上にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。
1. 「**タイムシート**」をクリックします。
1. ページの右上にある「**マイタイムシート承認**」を選択し、承認するタイムシートを表示します。

   または

   タイムシートのリストの一番上で「**マイタイムシート承認**」フィルターを選択します。

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者が、「設定」エリアの「リスト制御」または「レイアウトテンプレート」から「マイタイムシート承認」フィルターを削除した場合、タイムシートリストの上部またはフィルターリストに「マイタイムシート承認」オプションが表示されません。詳しくは、次の記事を参照してください。
   >
   >   
   >   
   >* [レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （オプション）タイムシートのリストの上部で&#x200B;**検索**&#x200B;アイコン ![](assets/search-icon.png) をクリックし、キーワードを入力して特定のタイムシートを検索します。時間枠のほか、所有者や承認者の名前を検索できます。
1. 承認するタイムシートの時間枠をクリックします。タイムシートが開きます。

   >[!TIP]
   >
   >承認待ちタイムシートのステータスは「[!UICONTROL 提出済み]」です。


1. 「**承認**」をクリックします。

   または

   タイムシートを却下する場合は、タイムシートの左下にある「**拒否**」をクリックします。

   タイムシートが承認されると、タイムシートのステータスが「**クローズ**」に変わります。

   却下された場合は、ステータスが「**拒否**」に変わります。
