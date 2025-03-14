---
product-area: reporting
navigation-topic: reporting-elements
title: 日付ベースのワイルドカードを使用したレポートの一般化
description: 特定のレポート要素を作成するときに、特定の情報の代わりにワイルドカードを使用することで、レポートを一般化できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 92%

---

# 日付ベースのワイルドカードを使用したレポートの一般化

<!-- Audited: 11/2024 -->

特定のレポート要素を作成するときに、特定の情報の代わりにワイルドカードを使用することで、レポートを一般化できます。

例えば、特定の予定開始日を持つタスクを表示するレポートを作成する場合は、フィルターでカレンダーの日付選択ツールを使用して特定の日付を選択できます。ただし、レポートにアクセスした日から特定の期間内に予定開始日があるタスクを表示するレポートを作成する場合は、誰かがレポートを表示すると、レポートを表示した時点に関係のある期間の情報がレポートに表示されることを示すワイルドカードを使用できます。

例えば、過去 1 週間、過去 1 年、今後 2 週間などです。このように、レポートは一度作成しますが、フィルターでワイルドカードを使用しているので、レポートを読むたびに異なる結果が生成されます。レポートの実行日に合わせてレポートの内容が変わるからです。

次のレポート要素を作成する際に、日付ベースのワイルドカードを使用できます。

* フィルター
* カスタムプロンプト
* 列のルールを追加するときのビュー

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
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
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>ポート、ダッシュボード、カレンダーへの編集アクセスでレポートのレポート要素の編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>レポートの管理権限（レポート内のレポート要素を編集するため）</p> <p>ビューまたはフィルターの管理権限（これらを編集するため）</p></td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 前提条件

レポートにワイルドカード変数を追加するには、まずレポートを作成する必要があります。

レポートの作成については、[レポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)を参照してください。

## 操作手順

日付ベースのワイルドカードをレポートに挿入するには、次の手順に従います。

1. 日付ベースのワイルドカードを挿入するレポートに移動します。
1. 「**報告書アクション**」をクリックし、次に「**編集**」を選択します。
1. 「**フィルター**」タブをクリックします。
1. 「**フィルター規則の追加**」をクリックします。
1. フィルタリングの条件に使用するフィールドの名前を入力していきます。\
   日付を参照するフィールドを入力する必要があります。
1. フィルター変数のドロップダウンメニューで「**が次に等しい**」を選択します。

   >[!TIP]
   >
   >Adobe Workfront でワイルドカードを使用する場合は、常に&#x200B;**が次に等しい**&#x200B;フィルター変数を選択する必要があります。

1. **相対的な日付を設定** トグルをクリックし、表示されるテキストボックスで「`$$TODAY`」と入力します（レポートが実行されるのと同じ日に発生した事象に関する情報を表示する場合）。

   または

   レポートの実行日時と同じ日時に発生した事象に関する情報を表示する場合は、`$$NOW` と入力します。

   この日付は、ユーザーがレポートを実際に表示した日付によって変わるので、常に異なります。したがって、レポートの情報は日によって異なります。

1. （オプション）レポートの実行日以降の期間内に発生する情報を表示する場合、次の週の情報を表示するには `$$TODAY+1w` と入力し、次の 2 か月の情報を表示には `$$TODAY+2m` と入力します。四半期、時間、日または年の期間を指定することもできます。
1. （オプション）レポートの実行日より前の期間内に発生した事象に関する情報を表示する場合、前の週の情報を表示するには `$$TODAY-1w` と入力し、前の 2 か月の情報を表示するには `$$TODAY-2m` と入力します。四半期、時間、日または年の期間を指定することもできます。

   日付ベースのワイルドカードで使用できる属性、修飾子および演算子の完全なリストについては、[ワイルドカードフィルター変数の概要](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)の記事を参照してください。

1. 「**保存して閉じる**」をクリックします。

## 追加情報

関連トピック：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [ワイルドカードフィルター変数の概要](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Adobe Workfront でフィルターを作成または編集](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [ビューでの条件付き形式の使用](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
