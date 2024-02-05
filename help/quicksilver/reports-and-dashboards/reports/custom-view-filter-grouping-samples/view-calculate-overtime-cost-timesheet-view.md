---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：タイムシートビューでの超過作業時間コストの計算」
description: Adobe Workfront では、超過作業時間はデフォルトでは計算されませんが、超過作業時間を計算するタイムシートレポートを作成できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 96%

---

# ビュー：タイムシートビューでの超過作業時間コストの計算

Adobe Workfront では、超過作業時間はデフォルトでは計算されませんが、超過作業時間を計算するタイムシートレポートを作成できます。

ユーザーがプロファイルの「1 時間当たりのコスト」レートに関連付けられている場合は、そのユーザーの超過作業時間のコストの量も計算できます。\
ユーザーと 1 時間当たりのコストの関連付けについては、「[個人設定の指定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)」を参照してください。

>[!NOTE]
>
>リストまたはレポートのタイムシートビューに追加できる「超過作業時間」フィールドには、タイムシートの「超過作業時間」フィールドの情報が表示されます。この情報は、タイムシートを変更するアクセス権を持つユーザーが手動で更新します。タイムシートの [ 超過作業時間 ] フィールドの詳細については、「 [タイムシートレイアウトの概要](../../../timesheets/timesheets/timesheet-layout.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>表示の変更をリクエスト </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## タイムシートビューでの超過作業時間コストの計算

タイムシートビューに計算された超過作業時間列を追加するには、次の手順に従います。

1. タイムシートの一覧に移動するか、タイムシートレポートを作成します。

   レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

1. タイムシートのリストで「**ビューをカスタマイズ**」をクリックします。

   または

   タイムシートレポートで「**列（ビュー）**」タブを選択します。

1. 「**列を追加**」をクリックします。
1. 「**テキストモードに切り替え**」をクリックします。
1. **この列に表示**&#x200B;エリアで、「**クリックしてテキストを編集**」をクリックします。
1. 次のテキストモードコードをコピーして&#x200B;**テキストモード**&#x200B;ダイアログボックスにペーストします。
   <pre>displayname=Calculated Overtime Cost<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >この計算は、ユーザーが通常 40 時間働くことを前提としています。

1. 「**保存**」をクリックして、新しいビューに名前を付け、タイムシートのリストで「**ビューを保存**」をクリックします。

   または

   タイムシートレポートで「**保存して閉じる**」をクリックします。

1. （オプションおよび条件付き）タイムシートレポートを作成している場合は、レポートの名前を指定し、「**レポートを保存**」をクリックします。

   各ユーザーの超過作業時間コストが **計算された超過作業時間コスト**&#x200B;列に表示されます。

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
