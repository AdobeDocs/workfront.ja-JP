---
content-type: reference
product-area: reporting;timesheets
navigation-topic: custom-view-filter-and-grouping-samples
title: ビュー：タイムシート ビューでの超過時間コストの計算
description: Adobe Workfront では、超過作業時間はデフォルトでは計算されませんが、超過作業時間を計算するタイムシートレポートを作成できます。
author: Courtney
feature: Reports and Dashboards
exl-id: ad6205cd-7534-49e5-b142-09f90bf672ce
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 78%

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>コントリビューターまたはフィルターを変更するリクエスト </p>
   <p>レポートを修正する標準または計画</p>
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

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## タイムシートビューでの超過作業時間コストの計算

タイムシートビューに計算された超過作業時間列を追加するには、次の手順に従います。

1. タイムシートのリストに移動します。

1. **表示**&#x200B;ドロップダウンメニューをクリックして、「**新規ビュー**」をクリックします。

1. 「**列を追加**」をクリックします。
1. 「**テキストモードに切り替え**」をクリックし、「**テキストモードを編集**」をクリックします。
1. **テキストモードを編集** ボックスで、ボックス内のテキストを削除し、次のテキストモードコードをコピーして貼り付けます。

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

1. 「**完了**」をクリックし、新しいビューに名前を付けて、タイムシートのリストで「**ビューを保存**」をクリックします。

   各ユーザーの超過作業時間コストが **計算された超過作業時間コスト**&#x200B;列に表示されます。


