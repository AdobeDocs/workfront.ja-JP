---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 時間枠でレポートをフィルタリングする
description: オブジェクトに存在する日付の時間枠でレポートをフィルタリングできます。 例えば、時間レポートでは、時間が入力された特定の時間枠をフィルタリングできます。
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 4%

---

# 時間枠でレポートをフィルタリングする

オブジェクトに存在する日付の時間枠でレポートをフィルタリングできます。 例えば、時間レポートでは、時間が入力された特定の時間枠をフィルタリングできます。

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

## 前提条件

結果をフィルタリングする前に、レポートを作成する必要があります。

レポートの作成について詳しくは、 [レポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 日付の時間枠でレポートをフィルタリングする {#filter-a-report-by-the-time-frame-of-a-date}

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png)を選択し、「 **レポート**.

1. クリック **新しいレポート**」をクリックして、目的のレポートのタイプを選択します。\
   例えば、「 **時間レポート**.

1. を選択します。 **フィルター** タブをクリックします。
1. クリック **フィルタールールを追加**&#x200B;を選択し、「 **時間入力日**.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. 次のドロップダウンメニューで、次のいずれかのオプションを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">が</td> 
      <td>この修飾子を選択した後、時間が入力された日付を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">等しくない</td> 
      <td>この修飾子を選択した後、時間が入力された日付を指定して、この日付をレポートから除外します。 レポートには、指定した日付に対して、すべての日付にログインした時間が表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">NULL</td> 
      <td>このモディファイアを選択すると、「入口日」がない時間のみが表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">NULL でない</td> 
      <td>「入口日」に値が設定されている時間のみを表示する場合は、このモディファイアを選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">間</td> 
      <td>この修飾子を選択した後、時間が入力された日付範囲を指定します。 レポートには、指定した日付の間に入力された時間が表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">より小さい</td> 
      <td>この修飾子を選択した後、時間を入力する前の日付を指定します。 レポートには、指定した日付の前に入力された時間と、指定した日付を含まない時間が表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">以下</td> 
      <td>この修飾子を選択した後、時間を入力する前の日付を指定します。 レポートには、指定した日付（指定した日付を含む）より前に入力された時間が表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">より大きい</td> 
      <td>この修飾子を選択した後、時間を入力した後の日付を指定します。 レポートには、指定した日付の後に入力された時間（指定した日付を含まない）が表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">以上</td> 
      <td> <p>この修飾子を選択した後、時間を入力した後の日付を指定します。 レポートには、指定した日付（指定した日付を含む）以降に入力された時間が表示されます。</p> <p>組み込みのタイムフレームモディファイヤを選択します。詳しくは、 <a href="#built-in-time-frame-modifiers" class="MCXref xref">組み込みのタイムフレームモディファイヤ</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. これらの修飾子は、フィルタ内の任意の日付フィールドまたは任意のレポート内のプロンプトに対して使用できます。
1. クリック **保存して閉じる**.

## 組み込みのタイムフレームモディファイヤ {#built-in-time-frame-modifiers}

Adobe Workfrontには、特定の日付を定義せずに使用できる、組み込みの時間枠修飾子があります。 

これらの修飾子は、フィルタ内の任意の日付フィールドまたは任意のレポート内のプロンプトに対して使用できます。 

日付に関連付けられた期間でレポートをフィルタする方法について詳しくは、  [日付の時間枠でレポートをフィルタリングする](#filter-a-report-by-the-time-frame-of-a-date).

例えば、時間レポートを作成していて、特定の時間枠に入力された時間を表示する場合、次の組み込み時間枠フィルターオプションから選択できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">今日</td> 
   <td>入口日が今日の時間を表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">今週</td> 
   <td>[ 入口日 ] が現在の週の日付である時間を表示します。週は日曜日に始まり、土曜日に終わります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">翌週</td> 
   <td>[ 入口日 ] が現在の週の次の週の日付である時間を表示します。週は日曜日に始まり、土曜日に終わります。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">先週</td> 
   <td>[ 入口日 ] が現在の週の前の週の日付である時間を表示します。週は日曜日に始まり、土曜日に終わります。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">今月</td> 
   <td>入口日が今月の日付である時間を表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">翌月</td> 
   <td>入口日が今月の翌月の日付である時間を表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">先月</td> 
   <td>入口日が当月より前の月の日付である時間を表示します</td> 
  </tr> 
  <tr> 
   <td role="rowheader">現在の四半期</td> 
   <td> <p>「入口日」が現在の四半期の日付である時間を表示します。四半期は次のように定義されます。</p> 
    <ul> 
     <li>第 1 四半期：1 月 1 日～3 月 30 日</li> 
     <li>第 2 四半期：4 月 1 日～6 月 30 日</li> 
     <li>第 3 四半期：7 月 1 日～9 月 30 日</li> 
     <li>第 4 四半期：10 月 1 日～12 月 31 日</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">次の四半期</td> 
   <td>入口日が現在の四半期の後の四半期の日付で、前述の四半期が定義されている時間を表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">前の四半期</td> 
   <td> <p>入口日が現在の四半期より前の四半期の日付で、前述の四半期が定義されている時間を表示します。</p> <p>注意：Workfront管理者がシステムのカスタム四半期を有効にして定義した場合、四半期のビルトインフィルターは、カスタム四半期情報に置き換えられます。 カスタム四半期の有効化について詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">プロジェクトのカスタム四半期を有効にする</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">今年</td> 
   <td>入口日が現在の年の日付である時間を表示します。現在の年は 1 月 1 日に始まり、12 月 31 日に終わります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">過去 1 年</td> 
   <td>入口日が過去の年の日付で、過去の年が現在の日付の 12 か月前から始まる時間を表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">昨年</td> 
   <td> <p>入口日が昨年の日付である時間を表示します。最終年は 1 月 1 日に始まり、現在の年の前の年の 12 月 31 日に終わります。</p> <p>注意：会計年度には、組み込みの期間はありません。 組織で定義されているように、会計年度の日付範囲のカスタム修飾子を使用して、レポートを作成し、日付別に情報をフィルタリングできます。 会計年度の期間をその場で選択する場合は、フィルターの代わりにプロンプトを使用する必要があります。 </p> </td> 
  </tr> 
 </tbody> 
</table>
