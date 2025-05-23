---
product-area: reporting
navigation-topic: create-and-manage-reports
title: マトリックスレポートの作成
description: マトリックスレポートは、概要情報を集計表形式で表示するので、従来のレポートでのリスト表示よりも見やすくなります。
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 96%

---

# マトリックスレポートの作成

マトリックスレポートは、概要情報を集計表形式で表示するので、従来のレポートでのリスト表示よりも見やすくなります。

## マトリックスレポートを使用する場合

マトリックスレポートは、2 つ以上のグループ化を含む任意のレポートに対して作成できます。従来のレポートには最大 3 つのグループ化を含めることができますが、マトリックスレポートには最大 4 つのグループ化を含めることができます。

例えば、3 か月の期間に記録された時間を表示する時間レポートを作成し、その時間を入力したユーザーに基づいて、および月ごとおよび週ごとにレポートを整理することができます。

![ レポートマトリックスの概要 ](assets/report-matrix-overview-350x123.png)

## マトリックスレポートでのデータの表示方法

マトリックスレポートの情報は、常に数値として表示されます。ほとんどの場合、数値を含む列は、マトリックスレポートの表示に最適です（記録された時間数や実際のコストなど）。

ただし、次の図に示すように、その他の列（「ステータス」など）もマトリックスレポートに表示できます。\
![ マトリックスステータス ](assets/report-matrix-status-350x73.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
      <td> 
      <p>新規：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>プラン</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td><p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループ化へのアクセスの編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p></td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## マトリックスレポートの設定

1. レポート出力に数値データを含む従来のレポートを作成します。\
   レポートの作成方法について詳しくは、[カスタムレポートを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

1. 手順 1 で作成したレポートに移動し、「**レポートのアクション**」、「**編集**」の順にクリックします。

1. （条件付き）既にビューを作成していて、このレポートに適用する場合は、「**既存のビューを適用**」をクリックし、ドロップダウンリストからビューを選択します。
1. （条件付き）レポートの新しいビューを作成する場合は、次の手順を実行します。

   1. 「**カラム（表示）**」タブをクリックし、マトリックスレポートに要約する列を選択します。
   1. **カラム設定**&#x200B;エリアで、**このカラムの集計方法**&#x200B;ドロップダウンリストをクリックし、情報の要約に使用可能なオプションを 1 つ選択します。

      >[!IMPORTANT]
      >
      >このオプションが選択されていない場合、列の情報はマトリックスレポートに正しく表示されません。

      ![ マトリックスの要約 ](assets/qs-report-matrix-summarized-350x392.png)

   1. 「カラム（表示）」タブの各列に対してこの手順を繰り返し、「**完了**」をクリックします。

1. 「**グループ化**」タブをクリックします。
1. （条件付き）既にグループ化を作成していて、このレポートに適用する場合は、「**既存のグループ化を適用する**」を選択し、ドロップダウンリストからグループ化を選択します。
1. （条件付き）レポートの新しいマトリックスのグループ化を作成する場合は、次の手順を実行します。

   1. ビルダーインターフェイスの右上隅にある「**マトリックスグループ化に切り替え**」をクリックします。
   1. 「**行のグループ化**」セクションで、行のグループ化を指定します。このグループ化によって、テーブルの水平グループが設定されます。
   1. （オプション）行のグループ化を追加するには、「**セカンダリ行のグループ化を追加**」をクリックします。
   1. 「**列のグループ化**」セクションで、列のグループ化を指定します。これにより、テーブルの垂直のグループ化が確立されます。
   1. （オプション）列のグループ化を追加するには、「**セカンダリ列のグループ化を追加**」をクリックします。
   1. （条件付き）日付別のグループ化を追加する場合、日別、週別、月別、四半期別、年別のどの方法で結果をグループ化するか指定します。\
      ![ 日付別グループ化オプション ](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. （条件付き）日付別にグループ化し、結果を四半期別に表示する場合、例えば、データのない四半期を表示するかどうかを、「**結果のない四半期を表示**」チェックボックスで選択します。\
      ![ 結果のない四半期を表示 ](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >「**結果のない四半期を表示**」フィールドは、マトリックスグループ化に対してのみ使用でき、標準のグループ化には使用できません。\
      >有効なデータを持つ 2 つの四半期の間にデータを持たない四半期のみが、「マトリックス」タブのデータ値にゼロを表示します。フィルターによって選択された期間の最初と最後にデータがない四半期は、マトリックスグループ化には表示されません。結果のない四半期は、レポートの「詳細」タブのグループに表示されません。

1. （オプションおよび条件付き）「**マトリックス設定**」をクリックし、以下のオプションから選択します。\
   **レコード件数を表示：**&#x200B;指定したフィールドのエントリの合計数を含む行を表示するには、このオプションを選択します。\
   **[値] カラムを表示：**&#x200B;以下の情報をマトリックスに表示するには、このオプションを選択します。

   * レコード件数
   * 「値」列

     >[!NOTE]
     >
     >この列には、各行のデータが表す内容を説明する情報が含まれます。\
     >グループ化における次のフィールドの値を集計する場合、親オブジェクト（親タスクなど）には次の例外が適用されます。
     >
     >   
     >   
     >   * 実際の時間数（「予定／実際の労力コスト」、「予定／実際の費用コスト」、「予定／実際のコスト」、「予定時間数」など）を除くすべての数値フィールドと通貨フィールドでは、子タスクとスタンドアロンタスクの値のみを集計します。親タスクまたは親の親の値は集計されません。
     >   * 実際の時間数は、メインの親タスクとスタンドアロンタスクの値を集計します。親タスクの親や子タスクの数値は集計されません。
     >   * 数値および通貨の値のカスタムデータフィールドは、すべてのタスク（親、子、親の親、スタンドアロンタスク）を集計します。「予定時間数」または「実際の時間数」を「**値**」列に表示するためにマトリックスレポートを作成する場合は、親オブジェクト（親タスクなど）の時間またはコストの情報はマトリックスレポートに表示されないことに注意してください。親オブジェクトの時間を確認するには、「**詳細**」タブを表示する必要があります。
     >   
     >   
     >**条件付きルール：**&#x200B;集計される値の書式設定ルールを設定します。\

   ルールを追加した後、そのルールに一致するフィールドの表示方法について、フィールドとテキストのスタイルを定義できます。ルールの定義が完了したら「**ルールを追加**」をクリックし、「**完了**」を選択してルールを保存します。

1. 「**フィルター**」タブをクリックすることで、レポートに表示する情報を定義できます。
1. （条件付き）既にフィルターを作成していて、このレポートに適用する場合は、「**既存のフィルターを適用する**」をクリックし、ドロップダウンリストからビューを選択します。
1. （条件付き）このレポートに新しいフィルターを作成する場合は、[フィルターおよび条件修飾子](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)を参照して、

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   フィルターの作成時に使用できる様々な修飾子について詳しく確認してください。

1. 「**保存して閉じる**」をクリックして、マトリックスレポートを保存して表示します。
