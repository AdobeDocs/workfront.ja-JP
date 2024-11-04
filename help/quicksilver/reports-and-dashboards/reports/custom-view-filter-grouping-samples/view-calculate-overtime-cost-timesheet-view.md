---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: 「表示：タイムシートで超過コストを計算」
description: Adobe Workfront では、超過作業時間はデフォルトでは計算されませんが、超過作業時間を計算するタイムシートレポートを作成できます。
author: Nolan
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 76%

---

# ビュー：タイムシートビューでの超過作業時間コストの計算

<!--Audited: 11/2024-->

Adobe Workfront では、超過作業時間はデフォルトでは計算されませんが、超過作業時間を計算するタイムシートレポートを作成できます。

ユーザーがプロファイルの「1 時間当たりのコスト」レートに関連付けられている場合は、そのユーザーの超過作業時間のコストの量も計算できます。\
ユーザーと 1 時間当たりのコストの関連付けについては、[個人設定の指定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)を参照してください。

>[!NOTE]
>
>リストまたはレポートのタイムシートビューに追加できる「超過作業時間」フィールドには、タイムシートの「超過作業時間」フィールドの情報が表示されます。この情報は、タイムシートを変更するアクセス権を持つユーザーが手動で更新します。タイムシートの「超過作業時間」フィールドについて詳しくは、[タイムシートのレイアウトの概要](../../../timesheets/timesheets/timesheet-layout.md)を参照してください。

![calculated_overtime_cost_in_timesheet_report.png](assets/calculated-overtime-cost-in-timesheet-report-350x92.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
    <p>新規：</p>
   <ul><li><p>フィルターを変更するコントリビューター </p></li>
   <li><p>レポートを変更する場合は Standard</p></li> </ul>

<p>現在：</p>
   <ul><li><p>フィルターを変更する場合は「要求」 </p></li>
   <li><p>レポートを変更するためのプラン</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## タイムシートビューでの超過作業時間コストの計算

タイムシートビューに計算された超過作業時間列を追加するには、次の手順に従います。

1. タイムシートの一覧に移動します。

1. **表示**&#x200B;ドロップダウンメニューをクリックして、「**新規ビュー**」をクリックします。

1. 「**列を追加**」をクリックします。
1. **テキストモードに切り替え** をクリックしてから、**テキストモードを編集** をクリックします。
1. **テキストモードを編集** ボックスで、ボックス内のテキストを削除し、次のテキストモードコードをコピー&amp;ペーストします。

   ```
   displayname=Calculated Overtime Cost
   linkedname=direct
   namekey=totalHours
   querysort=totalHours 
   textmode=true
   valueexpression=IF({totalHours}>40,({totalHours}-40)*{user}.{costPerHour},{totalHours}*{user}.{costPerHour})
   valueformat=currencyStringCurrencyRounded
   ```

   >[!NOTE]
   >
   >この計算は、ユーザーが通常 40 時間働くことを前提としています。

1. 「**完了**」をクリックして、新しいビューに名前を付け、タイムシートのリストで「**ビューを保存**」をクリックします。

   各ユーザーの超過作業時間コストが **計算された超過作業時間コスト**&#x200B;列に表示されます。


