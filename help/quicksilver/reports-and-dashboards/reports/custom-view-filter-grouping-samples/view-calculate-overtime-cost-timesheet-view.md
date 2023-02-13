---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: '表示：タイムシートビューの超過コストを計算する'
description: Adobe Workfrontでは、超過作業時間は既定では計算されませんが、超過作業時間を計算するタイムシートレポートを作成できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 表示：タイムシートビューでの超過コストの計算

Adobe Workfrontでは、超過作業時間は既定では計算されませんが、超過作業時間を計算するタイムシートレポートを作成できます。

ユーザーがプロファイルの「時間あたりのコスト」レートに関連付けられている場合は、そのユーザーの時間外のコストの量も計算できます。\
ユーザーと時間単価の関連付けについては、「 [設定を行う](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

>[!NOTE]
>
>リストまたはレポートの [ タイムシート ] ビューに追加できる [ 超過作業時間 ] フィールドには、タイムシートの [ 超過作業時間 ] フィールドの情報が表示されます。 この情報は、タイムシートを変更するアクセス権を持つユーザーが手動で更新します。 タイムシートの [ 超過作業時間 ] フィールドの詳細については、「 [タイムシートレイアウトを理解する](../../../timesheets/timesheets/timesheet-layout.md).

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
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タイムシートビューでの超過コストの計算

タイムシートビューに計算された [ 超過 ] 列を追加するには、次の手順に従います。

1. タイムシートの一覧に移動するか、タイムシートレポートを作成します。

   レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. クリック **表示をカスタマイズ** （タイムシートのリスト）

   または

   を選択します。 **列（表示）** タブをクリックします。

1. クリック **列を追加**.
1. クリック **テキストモードに切り替え**.
1. 内 **この列に表示** 領域、クリック **クリックしてテキストを編集**.
1. 次のテキストモードコードを **テキストモード** ダイアログボックス
   <pre>displayname=計算された時間外コスト<br>linkedname=direct<br>namekey=totalHours<br>querysort=totalHours <br>textmode=true<br>valueexpression=IF({totalHours}&gt;40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}。{costPerHour})<br>valueformat=currencyStringCurrencyRounded</pre>

   >[!NOTE]
   >
   >この計算は、ユーザーが通常 40 時間働くことを前提としています。

1. クリック **保存**&#x200B;次に、新しいビューに名前を付け、 **ビューを保存** （タイムシートのリスト）

   または

   クリック **保存して閉じる** をタイムシートレポートに追加します。

1. （オプションおよび条件付き）タイムシートレポートを作成する場合は、レポートの名前を指定し、 **レポートを保存**.

   各ユーザーの時間外のコストが **計算された超過コスト** 列。

   ![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)
