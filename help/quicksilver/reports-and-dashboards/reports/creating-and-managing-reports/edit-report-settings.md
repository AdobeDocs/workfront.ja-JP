---
product-area: reporting
navigation-topic: create-and-manage-reports
title: レポート設定の編集
description: レポートの設定を編集して、他のユーザーに対するレポートの表示方法や、レポートを実行する前にユーザーが求める情報の種類を定義できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 9%

---

# レポート設定の編集

レポートの設定を編集して、他のユーザーに対するレポートの表示方法や、レポートを実行する前にユーザーが求める情報の種類を定義できます。

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

## ハウツー手順

1. レポートの作成を開始するには、 **メインメニュー** > **レポート**&#x200B;をクリックし、レポートのオブジェクトを選択します。

   または

   既存のレポートを開き、「 **レポートのアクション** > **編集**.

1. クリック **レポート設定** をクリックします。
1. 次のレポート設定を指定します。

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
      <td>レポートの目的と用途を説明する文を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">次のアクセス権限でこの報告書を作成する</td> 
      <td>他のユーザーに対してこのレポートを表示する際に使用するアクセス権を持つユーザーを選択します。 別のユーザーのアクセス権を使用してレポートを実行する方法について詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">別のユーザーのアクセス権を持つレポートの実行と配信</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告書を読み込んだときに表示</td> 
      <td>レポートの読み込み時にすべてのユーザーに表示されるデフォルトのタブを選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">レポートがダッシュボードに読み込まれるときに、「。..項目を表示」を選択します。</td> 
      <td>レポートがダッシュボードに読み込まれる際にすべてのユーザーに対して表示する項目数を指定します。 デフォルトは 15 項目、最大は 200 項目です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[ 詳細 ] タブに [ リソースグリッド ] ビューを表示する</td> 
      <td> <p>（ユーザーレポートのみ）このオプションを選択すると、レポートの「詳細」タブにリソースグリッドが表示されます。</p> <p>注意：リソースグリッドビューをユーザーレポートに適用すると、レポートには現在のステータスのプロジェクトのみが表示されます。 他の状態でプロジェクトを表示する場合は、グローバルナビゲーションバーの「人」領域の「ユーザー使用率」タブを使用し、そこにリソースグリッドビューを適用します。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">詳細タブに特別ビューを表示する</td> 
      <td>（プロジェクトレポートのみ）ユーザーが「詳細」タブでこの情報にアクセスしたときに表示される表示のタイプを指定します。 たとえば、マイルストーン表示またはガント表示を選択できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">既定ではこの報告書をガント ビューで表示する</td> 
      <td>（プロジェクトレポートおよびタスクレポートのみ）ユーザーがこのレポートの [ 詳細 ] タブを表示するときに、ガントチャートビューを自動的に有効にするには、このオプションを選択します。<br>プロジェクトレポートとタスクレポートでガントチャートを表示する方法の詳細については、この記事の「プロジェクトリストでタスク情報を表示するガントチャート」の節を参照してください <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">ガントチャートで情報を表示 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告書でビューを変更できるようにする</td> 
      <td>このオプションを選択すると、ユーザーはレポートの実行時に表示を変更できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告書でグループを変更できるようにする</td> 
      <td>ユーザーがレポートの実行時にグループを変更できるようにするには、このオプションを選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告書でフィルターを変更できるようにする</td> 
      <td>ユーザーがレポートの実行時にフィルターを変更できるようにするには、このオプションを選択します。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **レポートのプロンプト** をクリックして、レポートのプロンプトを設定します。\
   レポートへのプロンプトの追加の詳細については、「 [レポートにプロンプトを追加する](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. クリック&#x200B;**完了** 次に、 **保存して閉じる**.

## 追加情報

関連項目：

* [新しいWorkfrontエクスペリエンスのための基本レポート作成プログラム](https://one.workfront.com/s/basic-report-creation-program)
* [Adobe Workfrontでのレポートの概要](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Adobe Workfrontの組み込みレポートの使用](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
