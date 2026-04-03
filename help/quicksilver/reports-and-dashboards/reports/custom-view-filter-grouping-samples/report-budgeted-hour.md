---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: レポート：予算計上時間数
description: レポート：予算計上時間数
author: Courtney
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 72%

---

# レポート：予算計上時間数

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

リソースプランナーへのアクセス権がない他のユーザーと予算計上時間数の情報を共有したい場合は、予算計上時間数のレポートを作成することで共有できます。そのレポートを他のユーザーと共有できます。

>[!IMPORTANT]
>
>予算計上時間数は、通常、Adobe Workfront データベースで 1 時間ごとに更新されます（まれに、最大 3 時間かかる場合があります）。レポートを更新しても、そのレポート内の時間数の情報は必ずしも更新されるわけではありません。前回のアップデート以降の経過時間は、それぞれの予算計上時間数のレポートの右上隅に表示されます。レポートを更新すると、前回のアップデートから 1 時間以上経過した場合にのみ、レポート内の情報がアップデートされます。
>
>![予算計上時間レポート時間同期の警告](assets/budgeted-hour-report-time-sync-warning-350x74.png)

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

## 予算計上時間数のレポートを作成

1. 右上隅の&#x200B;**メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png)、または左上隅の&#x200B;**メインメニュー** アイコン ![ メインメニュー行](assets/lines-main-menu.png)をクリックし、使用可能な場合は&#x200B;**レポート**&#x200B;をクリックします。

1. **新規レポート** > **詳細** > **予算計上時間**&#x200B;をクリックします。

   デフォルトのビューがレポートに適用されます。

1. （オプション）レポートを読みやすくするには、**Budをクリックします。 時間**&#x200B;列を選択し、**テキストモードに切り替え**、次に「**テキストモードを編集**」をクリックします。
1. `valuefield`行を`valueexpreesion`に変更し、丸め式を入力します。

   これにより、予算時間数が指定した小数点以下の桁数に丸められます。

   Workfront で数値を四捨五入する方法について詳しくは、[計算済みデータ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)の記事を参照してください。

1. 「**完了**」をクリックします。
1. （オプション）「**列を追加**」をクリックして、列を追加します。
1. （オプション）レポートを読みやすくするために、そのレポートにグループ化を追加することをお勧めします。以下のグループ化をお勧めします。

   「**グループ化**」タブをクリックし、次の操作のいずれかを行います。

   * 「**グループ化を追加**」をクリックし、「プロジェクト名」を入力し始め、リストに表示されたら選択します。
   * 「**グループ化を追加**」をクリックし、「担当業務の名前」を入力し、リストに表示されたら選択します。
   * 「**グループ化を追加**」をクリックし、「割り当て日」と入力し始めます。リストに表示されたら選択し、「**日付でグループ化**」フィールドからグループ化する期間を選択します。

1. （オプション）「**フィルター**」をクリックして、レポートにフィルターを追加します。
1. （オプション）「**グラフ**」をクリックして、レポートにグラフを追加します。
1. 「**保存して閉じる**」をクリックします。

## 予算計上時間数のレポートを確認

デフォルトでは、以下の情報が予算計上時間数のレポートに表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">プロジェクト </td> 
   <td>予算計上時間数に関連付けられたプロジェクトの名前です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>担当業務</p> </td> 
   <td>予算計上時間数に関連付けられた担当業務の名前です。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザー</td> 
   <td>予算計上時間数に関連付けられたユーザーの名前です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">配分日</td> 
   <td> <p>配分日です。時間数を予算計上する週の最初の日（日曜日）です。</p> <p>ヒント：  <p>週が 2 か月にまたがる場合、レポートには 2 つの行が作成されます。1 行目は週の最初の日（最初の月の日曜日）に対応し、2 行目は 2 か月目の最初の日（任意の曜日）に対応します。</p> <p>例えば、あるユーザーに対して 6月30日（日曜日）～ 7月6日（土曜日）（PT）の週に 8 時間の予算を計上した場合、2 つの行には 6月30日と 7月1日の配分日が表示されます。</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">予算計上時間数</td> 
   <td>リソースプランナーのユーザーに割り当てられた予算計上時間数です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">予定予算計上時間数</td> 
   <td>これは、リソースプランナーで担当業務やプロジェクトに割り当てられている予算計上時間数です。</td> 
  </tr> 
 </tbody> 
</table>
