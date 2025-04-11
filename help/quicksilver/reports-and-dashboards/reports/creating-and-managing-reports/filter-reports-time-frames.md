---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 時間枠でレポートをフィルタリング
description: オブジェクトに存在する日付の時間枠でレポートをフィルタリングできます。 例えば、時間が入力された特定の時間枠について、時間レポートをフィルタリングできます。
author: Courtney
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: f78a86dcdf7b63e98bec5216fb5ab7622775a053
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 70%

---

# 時間枠でレポートをフィルタリング

<!-- Audited: 4/2025 -->

オブジェクトに存在する日付の時間枠でレポートをフィルタリングできます。 例えば、時間が入力された特定の時間枠について、時間レポートをフィルタリングできます。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
      <td> 
      <p>新規：標準</p>
       <p> または</p>
      <p>現在：プラン</p>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p> <p>フィルター、ビュー、グループ化へのアクセスの編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

結果をフィルターする前に、レポートを作成する必要があります。

レポートの作成について詳しくは、[レポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)を参照してください。

## 日付の時間枠でレポートをフィルタリングします {#filter-a-report-by-the-timeframe-of-a-date}

{{step1-to-reports}}

1. 左上隅にある **新規レポート** をクリックし、作成するレポートのタイプを選択します。

1. **新しいレポート** ページで、「**フィルター**」タブを選択します。

1. **フィルタールールを追加** をクリックしてから、**フィールドを選択** をクリックします。

1. **フィールドの選択** ダイアログボックスで、「**時間**」、「**エントリ日** の順に選択します。
   ![ 時間枠ごとの時間レポートのフィルタリング ](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. 表示されるドロップダウンで、次のいずれかのオプションを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">が次に等しい</td> 
      <td>この修飾子を選択した後、時間が入力された日付を指定します。</td> 
     </tr>

   <tr> 
      <td role="rowheader">等しくない</td> 
      <td>この修飾子を選択した後、時間が入力された日付を指定して、この日付をレポートから除外します。 レポートには、指定した日付を除くすべての日付にログインした時間が表示されます。</td> 
     </tr>

   <tr> 
      <td role="rowheader">より小さい</td> 
      <td>この修飾子を選択した後、時間が入力された前日の日付を指定します。レポートには、指定した日付を含まない、指定した日付より前に入力された時間が表示されます。</td> 
     </tr>

   <tr> 
      <td role="rowheader">が次よりも小さいか等しい</td> 
      <td>この修飾子を選択した後、時間が入力された前日の日付を指定します。レポートには、指定した日付（指定した日付を含む）以前に入力された時間が表示されます。</td> 
     </tr>

   <tr> 
      <td role="rowheader">より大きい</td> 
      <td>この修飾子を選択した後、時間を入力した後の日付を指定します。レポートには、指定した日付を含まず、指定した日付より後に入力された時間が表示されます。</td> 
     </tr>

   <tr> 
      <td role="rowheader">が次よりも大きいか等しい</td> 
      <td> この修飾子を選択した後、時間を入力した後の日付を指定します。レポートには、指定した日付（指定した日付を含む）以降に入力された時間が表示されます。 </td> 
     </tr>

   <tr> 
      <td role="rowheader">間</td> 
      <td>この修飾子を選択した後、時間が入力された日付範囲を指定します。レポートには、指定した日付の間に入力された時間が表示されます。</td> 
     </tr>

   <tr> 
      <td role="rowheader">NULL</td> 
      <td>この修飾子を選択すると、「エントリ日」がない時間のみが表示されます。</td> 
     </tr>

   <tr> 
      <td role="rowheader">NULL でない</td> 
      <td>この修飾子を選択すると、エントリ日に値が設定されている時間のみが表示されます。</td> 
     </tr>

   </tbody> 
   </table>

1. 「**保存して閉じる**」をクリックします。

## 組み込みの時間修飾子 {#built-in-timeframe-modifiers}

Adobe Workfrontには、具体的な日付を定義せずに使用できる組み込みの時間修飾子があります。 これらの修飾子は、フィルター内の任意の日付フィールドまたは任意のレポート内のプロンプトに対して使用できます。

例えば、時間レポートを作成し、特定の期間に入力された時間を表示する場合、次の組み込み期間フィルターオプションから選択できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">今日</td> 
   <td>エントリ日が今日の時間を表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">今週</td> 
   <td>エントリ日が現在の週の日付である時間を表示します（週の始まりは日曜日、終わりは土曜日）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">翌週</td> 
   <td>エントリ日が現在の週の次の週の日付である時間を表示します（週の始まりは日曜日、終わりは土曜日）。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">先週</td> 
   <td>エントリ日が現在の週の前の週の日付である時間を表示します（週の始まりは日曜日、終わりは土曜日）。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">今月</td> 
   <td>エントリ日が現在の月の日付である時間を表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">翌月</td> 
   <td>エントリ日が現在の月の翌月の日付である時間を表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">先月</td> 
   <td>エントリ日が現在の月の前月の日付である時間を表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">現在の四半期</td> 
   <td> <p>エントリ日が現在の四半期の日付である時間を表示します。四半期は次のように定義されます。</p> 
    <ul> 
     <li>第 1 四半期：1月1日～ 3月30日</li> 
     <li>第 2 四半期：4月1日～ 6月30日</li> 
     <li>第 3 四半期：7月1日～ 9月30日</li> 
     <li>第 4 四半期：10月1日～ 12月31日</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">次の四半期</td> 
   <td>入力日が現在の四半期の次の四半期の日付である時間を表示します。四半期は前述のように定義されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">前の四半期</td> 
   <td> <p>入力日が現在の四半期の前の四半期の日付である時間を表示します。四半期は前述のように定義されます。</p> <p>注意：Workfront 管理者がシステムのカスタム四半期を有効にして定義している場合、組み込みの四半期のフィルターはカスタム四半期情報に置き換えられます。カスタム四半期の有効化について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">プロジェクトのカスタム四半期の有効化</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">今年</td> 
   <td>入力日が現在の年の日付である時間を表示します。今年は1月1日に始まり12月31日に終わります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">過去 1 年</td> 
   <td>入力日が過去 1 年間の日付である時間を表示します。過去 1 年間は現在の日付の12カ月前から始まります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">昨年</td> 
   <td> <p>入力日が昨年の日付である時間を表示します。昨年は今年の前年の1月1日に始まり、12月31日に終わります。</p> <p>メモ：会計年度には組み込みの期間はありません。レポートを作成し、組織で定義されている会計年度の日付範囲のカスタム修飾子を使用して、日付で情報をフィルタリングすることができます。会計年度の期間をその場で選択する場合は、フィルターの代わりにプロンプトを使用する必要があります。 </p> </td> 
  </tr> 
 </tbody> 
</table>
