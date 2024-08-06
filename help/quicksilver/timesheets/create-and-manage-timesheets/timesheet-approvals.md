---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートの承認
description: 管理者はタイムシートの承認プロセスで、直属の部下の作業時間を表示できます。承認者は、記録されたすべての時間が正しいエリアに割り当てられ、その期間に対して十分な時間数が記録されていることを確認できます。
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 76%

---

# タイムシートの承認

<!--Audited: 8/2024-->

管理者はタイムシートの承認プロセスで、直属の部下の作業時間を表示できます。承認者は、記録されたすべての時間が正しいエリアに割り当てられ、その期間に対して十分な時間数が記録されていることを確認できます。

これに対応できるよう、Adobe Workfront ではタイムシートの承認を設定する機能が提供されています。

タイムシートの送信について詳しくは、[承認用のタイムシートの送信](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> <p>新規：標準</p>
   <p>現在：プラン </p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## タイムシートの承認者の指定

通常、タイムシートは、部門マネージャーまたは人事担当者によって承認されます（通常はプロジェクトマネージャーによって承認されません）。

タイムシート承認者は、タイムシート プロファイルの作成時に定義されます。 承認者として指定するにはプラン ライセンスが必要です。

タイムシートの承認者の指定について詳しくは、[タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)の[タイムシートプロファイルの作成または編集](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create)を参照してください。

## タイムシートの承認

承認者は、自分を承認者として指定して提出されたタイムシートを承認できます。タイムシートが承認用に送信されると、タイムシートは **ホーム** ページの **承認** 領域にリストされます。 詳しくは、[作業の承認](../../review-and-approve-work/manage-approvals/approving-work.md)を参照してください。

Workfront 管理者がユーザーへのタイムシート承認イベントハンドラーとユーザーへのタイムシート拒否イベントハンドラーを有効にしている場合、タイムシートが承認または拒否された後に通知が届きます。イベント通知の有効化について詳しくは、[ イベント通知タイプ ](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md) を参照してください。

タイムシートを承認するには：

{{step1-to-timesheets}}

**タイムシート** エリアが開きます。

1. ページの右上にある「**マイタイムシート承認**」を選択し、承認するタイムシートを表示します。

   または

   タイムシートのリストの一番上で「**マイタイムシート承認**」フィルターを選択します。

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Workfront管理者またはグループ管理者が、「設定」エリアのリストコントロールまたはレイアウトテンプレートから「タイムシート承認」フィルターを削除した場合、「自分のタイムシート承認」オプションは、タイムシートリストの上部またはフィルターのリストに表示されません。 詳しくは、次の記事を参照してください。
   >
   >   
   >   
   >   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
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
