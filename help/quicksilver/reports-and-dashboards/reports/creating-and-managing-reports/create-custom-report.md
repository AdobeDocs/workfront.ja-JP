---
product-area: reporting
navigation-topic: create-and-manage-reports
title: カスタムレポートの作成
description: レポートを作成することで、Adobe Workfront内で組織が必要とする情報にアクセスできるようにすることができます。 Workfrontで利用可能な組み込みレポートを使用することも、カスタムレポートを一から作成することもできます。
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1817'
ht-degree: 1%

---


# カスタムレポートの作成

<!--Audited: 12/2023-->

レポートを作成して、組織がAdobe Workfrontで必要とする情報へのアクセス権を付与できます。 Workfrontで利用可能な組み込みレポートを使用することも、カスタムレポートを一から作成することもできます。

組み込みレポートの詳細については、 [Adobe Workfrontの組み込みレポートの使用](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

レポートをコピーして作成する方法について詳しくは、 [レポートのコピーの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

クラス、ビデオ、チュートリアルなどのレポートの作成と管理の詳細については、Adobe Experience Leagueサイトの「学習」セクションを参照してください。

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
   <td> <p>新規：標準 </p>
   または
   <p>現在：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p><b>メモ</b></p>
   <p> まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>作成したレポートに対する管理権限を取得します。</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## レポートの作成 {#create-a-report}

{{step1-to-reports}}

1. クリック **新しいレポート**&#x200B;をクリックし、レポートに表示するオブジェクトの種類を選択します。

   Report Builder が読み込まれます。

   使用可能なオブジェクトレポートの詳細については、「 [オブジェクトに関するレポート](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 記事内 [Adobe Workfrontのオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >また、既存のレポートのコピーを作成して、レポートを作成することもできます。 詳しくは、 [レポートのコピーの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Report Builder で、次の内容をレポートに追加します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>機能</th> 
      <th>説明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>カラム （表示）</td> 
      <td> <p>レポートに列を追加することで、レポートに含まれる情報が決まります。</p> <p>列の追加方法については、 <a href="#add-columns-view-to-a-report" class="MCXref xref">レポートへの列の追加（表示）</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>グループ化</td> 
      <td> <p>レポートにグループを追加することで、レポートの編成方法が決まります。</p> <p>グループ化を追加する方法については、 <a href="#add-groupings-to-a-report" class="MCXref xref">レポートへのグループの追加</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>フィルター</td> 
      <td> <p>レポートにフィルタールールを追加すると、レポートに表示される情報が決まります。</p> <p>フィルターの追加方法については、 <a href="#add-filters-to-a-report" class="MCXref xref">レポートへのフィルターの追加</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>グラフ</td> 
      <td> <p>レポートにグラフを追加することで、レポートの情報を視覚的に表示する方法が決まります。</p> <p>グラフを追加する方法については、 <a href="#add-a-chart-to-a-report" class="MCXref xref">レポートにグラフを追加する</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. レポート作成プロセスの任意の時点で、「 **適用** をクリックして変更を保存します。
1. 完了したら、「 **保存して閉じる**.

### レポートへの列の追加（表示） {#add-columns-view-to-a-report}

1. レポートの作成を開始します (「 [レポートの作成](#create-a-report) 」の節を参照してください。
1. Report Builder で、 **列（表示）** タブを使用して、レポートに表示する列を指定します。
1. （オプション）「 **既存のビューの適用** をクリックし、ドロップダウンメニューでビューの名前をクリックして、既存のビューを使用します。

   ビューの作成について詳しくは、 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. （オプション）既存の列を削除するには、削除する列をクリックし、 **x** 列ヘッダーの現在の名前の横に表示されます。

1. 新しい列を追加するには、 **列を追加**.

   または

   既存の列を変更するには、列をクリックし、 **削除** アイコン ![](assets/x-icon-circled.png) を **この列フィールドに表示** 」ボックスをクリックし、新しいフィールドを入力して、リストに表示されたらクリックします。

   列に表示されるフィールドの詳細については、 [Adobe Workfrontの用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. （オプション） **列設定** 領域、選択 **この列で並べ替え** 列の値を降順のアルファベット順で昇順に並べ替えるには、リストでこの列を最初の並べ替えとして使用するかどうかを指定します。

   1 つの列の値で並べ替える場合は、1 つのレポートビューで複数のレベルの並べ替えを行い、もう 1 つの列の値で並べ替える場合は、複数のレベルの並べ替えを行うことができます。

   1 番目の並べ替え条件に従って複数の結果が同一の場合は、2 番目の並べ替え条件に従って並べ替えられます。 1 番目と 2 番目の並べ替え条件に従って複数の結果が同一の場合、3 番目の並べ替えに従って並べ替えられます。

   >[!NOTE]
   >
   >レポート対象のオブジェクトから遠すぎるオブジェクトを参照するフィールドを追加すると、このフィールドで並べ替えできない場合があります。\
   >例えば、問題レポートは「プロジェクト所有者」フィールドで並べ替えできません。このレポートは、「プロジェクト」、「所有者」、「名前」の 3 つの追加オブジェクトを参照しています。 ただし、このフィールドをイシューレポートに追加して、その情報を表示することはできます。

   <!--outdated: To learn more about cross-object references in reports, see the section "Advanced Reporting Part 1 of 3" in the [Reports and Dashboards Learning Path](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).-->

1. （オプション）グループ化を使用している場合に、列の情報を要約（集計）するには、 **この列の要約基準** ドロップダウンリスト **列設定** 「 」領域で、列の情報の集計に使用するオプションを選択します。

   集計された情報は、グループ化行の列に表示されます。

   ![グループ化の概要を集計](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   列内のデータの要約について詳しくは、 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >次の例外は、グループ化で次のフィールドの値を集計する場合に親オブジェクト（親タスクなど）に適用されます。
   >
   >* 「実績時間」以外のすべての数値および通貨フィールド（「計画または実績労務費」、「計画費」または「実績費用」、「計画原価」または「実績原価」、「計画時間」など）は、子タスクとスタンドアロンタスクの値のみを集計します。 親タスクや親の値は集計されません。
   >* [ 実績時間 ] は、メインの親タスクとスタンドアロンのタスクの値を集計します。親タスクの親や子タスクの数値は集計されません。
   >* 数値および通貨値のカスタムデータフィールドは、親、子、親の親、スタンドアロンタスクのすべてのタスクを集計します。

   レポートでのグループ化の使用について詳しくは、 [Adobe Workfrontでのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. （オプション）「 **詳細オプション** 列に次の情報を指定するには：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">カスタム列ラベル</td> 
      <td> <p>列のカスタムラベルを指定します。 このラベルは、デフォルトのラベルを置き換えます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">フィールド形式</td> 
      <td> <p>列のフィールドに値を表示する形式を選択します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ダッシュボードにこのカラムを表示</td> 
      <td> <p>このオプションを選択すると、レポートが別のレポートと並べて表示される場合に、この列がダッシュボードに表示されます。 このオプションを選択しない場合、レポートが並べて表示されるダッシュボードでレポートを表示する際に、この列は表示されません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カラムのルール</td> 
      <td> <p>クリック <strong>この列にルールを追加する</strong> をクリックして、列に条件付き書式を追加します。 ルールを追加した後、そのルールに一致するフィールドの表示方法に対して、フィールドおよびテキストスタイルを定義できます。 クリック <strong>ルールを追加</strong> ルールの定義が完了したら、次の手順に従います。 ビューの条件付き書式について詳しくは、 <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">ビューでの条件付き書式の使用</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **適用** 」をクリックして変更を適用し、以下のオプションを使用してレポートの編集を続行します。

   クリック **保存して閉じる** レポートの列の編集が終了し、レポートを保存する場合。

### レポートへのグループの追加 {#add-groupings-to-a-report}

1. レポートの作成を開始します (「 [レポートの作成](#create-a-report) 」の節を参照してください。
1. Report Builder で、 **グループ化** タブを使用して、レポート内の項目をグループ化する方法を指定します。
1. クリック **グループを追加** をクリックして新しいグループを追加します。

   または

   選択 **既存のグループの適用** をクリックして、既存のグループを選択します（リストに表示される場合）。

   ![](assets/nwe-add-grouping-350x230.png)

1. グループ化として追加するフィールドの入力を開始します。 フィールドが使用可能な場合は、関連付け可能な各オブジェクトに対してが設定されます。 フィールドの名前をクリックして、そのグループに追加します。
1. （オプション）テキストモードでグループ化を作成する場合は、「 **テキストモードに切り替え**. テキストモードの使用について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   新しいグループ化の作成について詳しくは、 [Adobe Workfrontでのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. （オプション）「 」を選択します。 **デフォルトでこのグループ化を折りたたむ** 展開されるのではなく折りたたまれた状態でこのグループの結果を表示する場合。

   この設定はデフォルトで無効になっており、グループ化の結果は常に展開されたリストに表示されます。

   >[!TIP]
   >
   >* リスト表示時にグループを手動で調整すると、Workfrontでは、ログアウトするまで手動の設定が記憶されます。 再度ログインすると、この設定に従ってリストが表示されます。
   >* グループ化の結果は、グラフ要素からアクセスした後で常に展開表示されます。

1. （オプション）「 **マトリックスグループ化に切り替え**&#x200B;をクリックし、マトリックスのグループ化を作成して、結果をグリッド形式で表示します。

   マトリックスレポートの作成について詳しくは、 [マトリックスレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. クリック **適用** 」をクリックして変更を適用し、以下のオプションを使用してレポートの編集を続行します。

   クリック **保存して閉じる** レポートのグループ化の編集が終了し、レポートを保存する場合。

### レポートへのフィルターの追加 {#add-filters-to-a-report}

1. レポートの作成を開始します (「 [レポートの作成](#create-a-report) 」の節を参照してください。
1. Report Builder で、 **フィルター** タブを使用して、レポートに含める情報の量を指定します。
1. クリック **フィルタールールを追加する** をクリックして、カスタムフィルターを追加します。\
   または\
   選択 **既存のフィルターの適用** 既存のフィルターを使用する場合。

   ![](assets/nwe-add-a-filter-350x93.png)

1. クリックした場合 **フィルタールールを追加する**&#x200B;をクリックし、フィルターとして追加するフィールドの入力を開始します。 フィールドが使用可能な場合は、関連付け可能な各オブジェクトに対してが設定されます。 フィールドの名前をクリックして、そのフィルターに追加します。\
   フィルター修飾子を使用して、フィルターを作成します。 フィルタ修飾子の詳細については、 [フィルターおよび条件修飾子](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   新しいフィルターの作成について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （オプション）テキストモードでフィルターを作成するには、 **テキストモードに切り替え**.

   テキストモードの使用について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. クリック **適用** レポートのフィルターの編集が終了したら、それまでに変更を適用し、次のオプションを使用してレポートの編集を続行します。

   クリック **保存して閉じる** を選択します。

### レポートにグラフを追加する {#add-a-chart-to-a-report}

1. レポートの作成を開始します (「 [レポートの作成](#create-a-report) 」の節を参照してください。
1. Report Builder で、 **グラフ** 「 」タブで、追加するグラフのタイプを選択します。

   ![](assets/nwe-add-a-chart-350x247.png)

   レポートでのグラフの作成について詳しくは、 [レポートにグラフを追加する](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. クリック **適用** 」をクリックして変更を適用し、以下のオプションを使用してレポートの編集を続行します。

   クリック **保存して閉じる** レポートの編集が終了し、レポートを保存する場合。
