---
product-area: reporting
navigation-topic: create-and-manage-reports
title: データの書き出し
description: 様々なリスト、レポート、ダッシュボード、検索からAdobe Workfrontのデータを書き出すことができます。
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '2153'
ht-degree: 81%

---

# データの書き出し

<!-- Audited: 12/2023 -->

様々なリスト、レポート、ダッシュボード、検索からAdobe Workfrontのデータを書き出すことができます。

データを書き出す理由には次のようなものがあります。

* データのハードコピーを Workfront の外部の誰かに提供する場合。
* レポートの結果を添付ファイルとして外部ユーザーに送信する場合。
* Workfront データの外部バックアップを作成する場合。
* Workfront web アプリケーション内の 1 ページに表示できる結果は 2,000 件のみという制限があります。レポートの生成量が 2,000 を超える場合は、使用可能な任意の形式にレポートをエクスポートし、レポートのすべての結果を 1 つのリストに表示できます。

Workfront インターフェイスからレポートを手動で書き出すことも、レポートの配信をスケジュールして、そのレポートを後で送信するようにもできます。配信レポートのスケジュール設定の詳細については、[レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)を参照してください。

この記事の情報は、次の書き出しには適用されません。

* チャートレポートからの情報の書き出し。

  チャートレポートの書き出しの詳細については、[レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

* ガントチャートからの情報の書き出し。

  ガントチャートの書き出しの詳細については、[ガントチャートの PDF への書き出し](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)を参照してください。

* リソースプランナーからの情報の書き出し。

  リソースプランナーからの情報の書き出しの詳細については、[リソースプランナーナビゲーションの概要](../../../resource-mgmt/resource-planning/resource-planner-navigation.md)の書き出しオプションを参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>
    <p>新規：明るいかそれ以上</p>
    <p>または</p>
    <p>現在：レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、およびレポートを書き出すためのカレンダーへのアクセス権を表示または高くします</p> <p>リストを書き出すためにリスト内で表示するオブジェクトへの表示以上のアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートまたはダッシュボードを書き出しすための、レポートまたはダッシュボードに対する表示以上の権限</p> <p>リストを書き出すために、リストで表示するオブジェクトに対する表示以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

データを書き出す前に、レポートを作成する必要があります。

レポートの作成について詳しくは、 [カスタムレポートの作成](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) または [レポートのコピーの作成](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## 書き出し形式と制限

### 書き出し形式 {#export-formats}

情報は、次の形式で書き出すことができます。

* PDF（レター横置きまたは縦置き、リーガル、帳簿および A4）
* Excel（.xls）
* Excel（xlsx）
* タブ区切り

>[!NOTE]
>
>ダッシュボードは印刷することも、.pdf ファイルにのみ書き出すこともできます。

### 書き出し制限 {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

Workfront でのレポートの表示方法、および手動で書き出し、配信されたレポート、または API を介してレポートを書き出す方法には、いくつかの制限があります。

* **50,000 セル：** Excel ファイルのレポートエクスポートで許可されるセルの最大数。
* **50,000 行：**.pdf およびタブ区切りファイルのレポートの書き出しで許可されるデータの行数。

   * Excel .xls ファイルの場合、この制限は **65,000 行**&#x200B;です。
   * Excel .xlsx ファイルの場合、この制限は **100,000 行**&#x200B;です。
   * これらの制限には、レポート内のグループ化の行だけでなく、列見出しも除外されます。例えば、1 つのレポートに 6 つのグループが含まれ、50,000 行のデータが含まれる場合、エクスポートされるファイルの行数は 50,000 行になります。

  >[!IMPORTANT]
  >
  >列内にコレクション参照を含むレポートを書き出すと、レポートがリストされた書き出し制限内にある場合でも、エラーが発生することがあります。参照されるコレクションが大きすぎる場合、書き出しプロセスがタイムアウトになり、エラーが発生します。
  >
  >このエラーを回避するには、書き出す前に、大規模なコレクションを参照する列を除外するか、参照されるコレクションのサイズを削減します。
  >

  レポートにこれらの制限を超える項目がある場合、書き出しが成功しなかったというエラーが表示されます。結果を書き出しできるようにするには、画面に表示される項目の数をこれらの制限以下に減らしてください。

  レポートに 50,000／65,000／100,000 行を超える行があり、すべてのデータを書き出す場合は、フィルターまたはプロンプトを使用して少量のデータを取得し、複数の書き出しを実行することをお勧めします。

  フィルターの使用について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  プロンプトの使用について詳しくは、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)を参照してください。

* 以下の制限が適用されます。

   * レポートの手動書き出し。
   * スケジュール済みレポート。
   * API 統合を経由した書き出し。
   * キックスタートを経由して書き出されたデータ。

     キックスタートを使用したデータのエクスポートについて詳しくは、 [「キックスタート」を使用してAdobe Workfrontからデータを書き出す](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >50,000 行をキックスタートファイルに書き出すことができますが、データは Excel 形式のファイルにのみ書き出すことができます。

   * プロジェクトの稼働率情報を書き出します。

     プロジェクトの稼働率情報を書き出す方法に関して詳しくは、[リソース稼働率レポートの概要](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project)を参照してください。

* **10 MB のファイルサイズ：**&#x200B;配信が予定されているすべての書き出しレポートのファイルサイズ制限。メールに添付された書き出し済みファイルが 5 MB を超える場合、添付の書き出し済みレポートの代わりに、ファイルをダウンロードできるリンクがメールで送信されます。
* **65,530 個のハイパーリンク：**&#x200B;これは、65,530 個を超えるハイパーリンクを含むドキュメントに対して Excel が課す制限です。これらのドキュメントは、手動で書き出した場合や、配信されたレポートに添付された場合には開けません。Excel ドキュメントのデータは 200 行に過ぎなくても、ドキュメント内に 65,530 個を超えるリンクがある場合、ドキュメントは開きません。この制限は、Excel ファイルにのみ存在し、他のサポートされている形式には該当しません。
* **256 列**：Excel が 256 列を超えるドキュメントに対して課される制限です。これらのドキュメントは、手動で書き出したり、配信されたレポートに添付して送信したりすることはできません。この制限は、Excel ファイルにのみ存在し、他のサポートされている形式には該当しません。

制限を超えてデータを書き出そうとすると、書き出しで予想されたデータの一部を受信できない場合があります。代わりに、制限内に変更されたレポートが作成されます。

加えて、実行に 60 分以上かかるレポートは停止します。

制限に関するご不明な点や問題がある場合は、Workfront 技術サポートにお問い合わせください。

## データの書き出し

### レポートまたはリストからのデータの書き出し {#export-data-from-a-report-or-list}

1. 書き出すレポートまたはリストに移動します。
1. 書き出す項目を選択します。（個々の項目を選択すると、選択した項目のみが書き出されます。）

   例えばプロジェクトで、書き出すタスクを選択します。

   または

   リスト全体を書き出すには、すべての項目を選択解除します。

1. 「**書き出し**」をクリックし、形式を選択します。

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![](assets/nwe-dashboard-export-note-350x271.png)
   -->

   または

   次をクリック： **書き出し** アイコン ![書き出しアイコン](assets/export-icon-nwe.png)をクリックし、形式を選択します。

   PDF の書き出しに使用できるオプションは、Workfront ユーザー設定のロケール設定によって異なります。

   * 北米 - レター（デフォルト）、リーガル、帳簿、A4

     <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * 北米以外のすべての場所 - A3、A4（デフォルト）、レター、リーガル、帳簿

     <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. （条件付き）使用しているオペレーティングシステムによっては、ファイルを開くか保存するかの選択肢がある場合があります。関連するアプリケーションでファイルを開くか、ハードドライブに保存します。
1. [書き出したドキュメントを使用](#use-the-exported-document)を続行します。

### ダッシュボードからのデータの書き出し {#export-data-from-a-dashboard}

情報は、ダッシュボードから印刷したり、.pdf ファイルとして書き出したりすることができます。

ダッシュボードからのデータの書き出しに関して詳しくは、[ダッシュボードの書き出し](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md)を参照してください。

## 書き出したドキュメントの使用 {#use-the-exported-document}

* [ファイル名](#file-names)
* [タイトル](#titles)
* [タイムスタンプ](#timestamps)
* [書式](#formatting)
* [リンク](#links)
* [ブランディング](#branding)

### ファイル名 {#file-names}

オブジェクトのリストやレポートを書き出す場合、書き出すファイルにはファイル名とタイトルが付きます。ファイル名を参照すると、書き出したファイルをコンピュータ上で見つけることができます。レポートのタイトルは、ユーザーが書き出したファイルを共有したときに、そのファイルが何を表しているかを示します。

#### 書き出したリストのファイル名 {#file-names-for-exported-lists}

オブジェクトのリストを書き出すと、書き出したファイルのファイル名とリストのタイトルに、オブジェクトのタイプが表示されます。

イシューまたはタスクのリストを書き出す場合、**ファイル名**&#x200B;は次のいずれかになります。

* プロジェクト内のタスクリストとタスクリストをエクスポートする場合：

   * *The_project_name_Exported_Tasks*（*PDF、Excel、Excel（.xlsx）またはタブ区切り形式）*
   * *The_project_name_Exported_Issues*（*PDF、Excel、Excel（.xlsx）またはタブ区切り形式）*

* タスク（サブタスク）内のタスクとタスクリストをエクスポートする場合：

   * **The_project_name_the_task_name_Exported_Tasks**（*PDF、Excel、Excel（.xlsx）またはタブ区切り形式）*
   * **The_project_name_the_task_name_Exported_Issues**（*PDF、Excel、Excel（.xlsx）またはタブ区切り形式）*

他のオブジェクトのリストをプロジェクトから PDF ファイルに書き出すと、書き出したドキュメントのファイル名に、書き出したオブジェクトの種類が示されます。\
例えば、次のようなファイル名を指定できます。

* *Exported_Users*（プロジェクトの「ユーザー」タブを書き出す場合。*PDF、Excel、Excel（.xlsx）またはタブ区切り形式）*
* *Exported_Risks*（プロジェクトのリスクのリストを書き出す場合。*PDF、Excel、Excel（.xlsx）またはタブ区切り形式）*

#### 書き出したレポートのファイル名 {#file-names-for-exported-reports}

レポートを書き出す場合、書き出したレポートのファイル名は次のようになります。

*The_report_name*（*PDF、Excel、Excel（.xlsx）またはタブ区切り形式）*

### タイトル {#titles}

オブジェクトのリストを書き出す場合、タイトルを持つのは PDF 形式のファイルだけです。リストまたはレポートを Excel、Excel(.xlsx) またはタブ区切り形式で書き出す場合、ファイルにはタイトルが含まれません。

#### 書き出したリストのタイトル {#titles-for-exported-lists}

プロジェクト内のタスクとタスクリストをPDFファイルに書き出す場合、書き出されるドキュメントのタイトルは次のいずれかになります。

* *プロジェクト名 - 書き出したタスク*
* *プロジェクト名 - 書き出したイシュー*

タスク内のタスクとタスクリストをPDFファイルにエクスポートする場合、エクスポートされるドキュメントのタイルは次のいずれかになります。

* *プロジェクト名 - タスク名 - 書き出したタスク*
* *プロジェクト名 - タスク名 - 書き出したイシュー*

他のオブジェクトのリストをプロジェクトから PDF ファイルに書き出すと、書き出したドキュメントのタイトルに、書き出したオブジェクトの種類が示されます。\
例えば、タイトルは次のようになります。

* *書き出したユーザー*（プロジェクトの「ユーザー」タブを書き出す場合）。
* *書き出したリスク*（プロジェクトのリスクのリストを書き出す場合）。

#### 書き出したレポートのタイトル {#titles-for-exported-reports}

PDFファイルにエクスポートされるレポートには、タイトルが付きます。

レポートを Excel、Excel(.xlsx)、タブ区切り形式のいずれかにエクスポートした場合、エクスポートしたレポートにはタイトルが付きません。 書き出したファイルのタイトルは、Workfront web アプリケーションに表示されるレポートの名前です。

レポートに説明が含まれる場合は、エクスポートされたファイルに含まれます。

### タイムスタンプ {#timestamps}

タイムスタンプは、項目を書き出したユーザーのコンテキストから書き出したドキュメントに表示されます。

タイムスタンプには以下が含まれます。

* 日付
* 時間
* 項目が書き出されたタイムゾーン

書き出すドキュメントの種類に応じて、タイムスタンプは様々な場所に表示されます。

* **PDF：**&#x200B;タイムスタンプは、各ページのフッターとファイル名に表示されます。
* **Excel：**&#x200B;タイムスタンプはファイル名に表示されます。

### 書式 {#formatting}

プロジェクトを .pdf に書き出すと、サブタスクは親タスクに対してインデントされて表示されます。書き出したリストは、親タスクを折りたたみません。

レポートに特別な表示がない限り、レポートの送信または配信スケジュールを行うときには、常にレポートのデフォルトタブが表示されます。

Web アプリケーションでレポートに特別な書式が設定されている場合、.pdf および Excel ファイルの場合のみ、「詳細」タブと「マトリックス」タブが配信されるときに、レポートが特別な書式で配信される必要があります。

>[!NOTE]
>
>書き出すデータに共有列が含まれ、Excel またはタブ区切り形式で書き出す場合、これらの列は書き出したファイル内で分割されます。

レポートの書式設定をカスタマイズする方法について詳しくは、[ビューでの条件付き書式の使用](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)を参照してください。

### リンク {#links}

リンクは、Workfront 内のリンクをサポートする任意のオブジェクトを指すことができます。Workfront でリストを .pdf に書き出すと、元のドキュメントに存在する、サポート対象のリンクは、書き出したドキュメント内に残ります。

>[!TIP]
>
>カスタムフィールド列の行 `valueformat=HTML` がテキストモードで表示され、書き出した .pdf ファイルにリンクの値が表示されない場合は、追加のコード行をテキストモードで列に入力する必要があります。
>
>例えば、「Open Q1 Projects」という名前のカスタムフィールドにリンクが含まれている場合、次のコードを追加します。
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

Excel 形式に書き出す場合、書き出されるファイルには Workfront 内のオブジェクトへのリンクのみが含まれ、レポート配信など、書き出した Excel ドキュメント内のリンクを許可するように選択できる場所でのみサポートされます。

## ブランディング {#branding}

>[!IMPORTANT]
>
>ブランディングは、まだAdobe Experience Cloudにオンボーディングされていない組織にのみ適用されます。
>
>組織がAdobe Experience Cloudにオンボーディングされている場合、ブランディングは使用できません。

Workfront 管理者がグローバルナビゲーションバー用に Workfront インスタンスにカスタマイズしたブランディングを追加した場合は、書き出した .pdf ファイルにパーソナライズされたロゴも含まれます。

その他の形式で書き出されたデータは、ロゴでパーソナライズできません。

Workfront インスタンスとグローバルナビゲーションバーのブランディングについて詳しくは、[Adobe Workfront インスタンスのブランディング](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)を参照してください。
