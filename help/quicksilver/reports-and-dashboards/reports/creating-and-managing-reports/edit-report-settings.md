---
product-area: reporting
navigation-topic: create-and-manage-reports
title: レポート設定を編集する
description: レポートの設定を編集して、他のユーザーに対するレポートの表示方法や、レポートを実行する前にユーザーが求める情報の種類を定義できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 96%

---

# レポート設定を編集する

<!-- Audited: 11/2024 -->

レポートの設定を編集して、他のユーザーに対するレポートの表示方法や、レポートを実行する前にユーザーが求める情報の種類を定義できます。

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
      <p>標準</p>
      <p>プラン</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
 <td> <p>レポートに対する権限を管理します。</p></td>  
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 操作手順

1. レポートの作成を開始するには、**メインメニュー**／**レポート**&#x200B;に進み、レポートのオブジェクトを選択します。

   または

   既存のレポートを開き、**レポートのアクション**／**編集**&#x200B;をクリックします。

1. レポートビルダーの右上隅にある「**レポート設定**」をクリックします。
1. 次のレポート設定を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">報告書タイトル</td> 
      <td>レポートのタイトルを指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>レポートの目的と用途を説明するステートメントを指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">次のアクセス権限でこの報告書を作成する</td> 
      <td>このレポートを他のユーザーに表示するときに使用するアクセス権を持つユーザーを選択します。別のユーザーのアクセス権を使用したレポートの実行について詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">別のユーザーのアクセス権を使用してレポートを実行して配信</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告書を読み込んだときに表示</td> 
      <td>レポートの読み込み時にすべてのユーザーに表示されるデフォルトのタブを選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">レポートがダッシュボードに読み込まれると、... 項目が表示される</td> 
      <td>レポートがダッシュボードに読み込まれる際にすべてのユーザーに表示する項目数を指定します。デフォルトは 15 項目で、最大項目数は 200 です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">「詳細」タブに、リソースグリッドビューを表示する</td> 
      <td> <p>（ユーザーレポートのみ）このオプションを選択すると、レポートの「詳細」タブにリソースグリッドが表示されます。</p> <p>メモ：リソースグリッドビューをユーザーレポートに適用すると、レポートには「現在」ステータスのプロジェクトのみが表示されます。他のステータスでプロジェクトを表示する場合は、グローバルナビゲーションバーのユーザーエリアの「ユーザー稼働率」タブを使用し、そこにリソースグリッドビューを適用します。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">詳細タブに特別ビューを表示する</td> 
      <td>（プロジェクトレポートのみ）ユーザーが「詳細」タブでこの情報にアクセスしたときに表示される表示の種類を指定します。例えば、マイルストーン表示またはガントチャート表示を選択できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">既定ではこの報告書をガントビューで表示する</td> 
      <td>（プロジェクトレポートおよびタスクレポートのみ）このオプションを選択すると、ユーザーがこのレポートの「詳細」タブを表示するときに、ガントチャートビューが自動的に有効になります。<br>プロジェクトレポートとタスクレポートでのガントチャートの表示について詳しくは、<a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">ガントチャートに情報を表示</a>の記事の「プロジェクトリストガントチャートでタスク情報を表示」の節を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告書でビューを変更できるようにする</td> 
      <td>このオプションを選択すると、ユーザーはレポートの実行時に表示を変更できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告書でグループを変更できるようにする</td> 
      <td>このオプションを選択すると、ユーザーがレポートの実行時にグループを変更できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告書でフィルターを変更できるようにする</td> 
      <td>このオプションを選択すると、ユーザーがレポートの実行時にフィルターを変更できます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**レポートのプロンプト**」をクリックして、レポートのプロンプトを設定します。\
   レポートへのプロンプトの追加について詳しくは、[レポートにプロンプトを追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)の記事を参照ください。

1. **完了** をクリックしてから、**保存して閉じる** をクリックします。

## 追加情報

関連トピック：

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [レポートの基本を学ぶ](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Adobe Workfront のビルトインのレポートを使用](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
