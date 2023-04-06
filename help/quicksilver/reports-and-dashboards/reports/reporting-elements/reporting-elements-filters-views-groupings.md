---
product-area: reporting
navigation-topic: reporting-elements
title: '''レポート要素：フィルター、ビュー、グループ化`'
description: Workfrontでは、すべてのリストとレポートに含める必要がある主な要素は、フィルター、ビューおよびグループです。 各要素は、どのレポート内でも異なる情報を提供します。
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# レポート要素：フィルター、ビュー、グループ化

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

Adobe Workfrontでリストやレポートを使用できるようにする要素は、いくつかあります。 すべてのリストとレポートに必要な主な要素は、フィルター、ビュー、グループ化です。 各要素は、どのレポート内でも異なる情報を提供します。

## レポート要素に関する考慮事項

フィルター、ビューおよびグループを使用する際は、次の点に注意してください。

* レポート要素は、レポートの構成要素として機能します。 レポートやリストの外観、およびレポートやリストに含まれる情報を定義します。
* Workfrontのレポートは、1 つのオブジェクトに固有です。 レポートを作成する前に、レポートのメインオブジェクトを定義する必要があります。 したがって、すべてのレポート要素はオブジェクトに固有です。
* Workfrontの管理者がリストやレポートで表示または編集できるようにするには、ユーザーに対し、アクセスレベルでのフィルター、ビューおよびグループへのアクセス権を付与する必要があります。

   フィルタ、ビュー、およびグループへのアクセス権の付与について詳しくは、 [フィルター、ビューおよびグループに対するアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* レポートを表示または編集するには、Workfront管理者がアクセスレベルでレポート、ダッシュボード、カレンダーへのアクセス権を付与する必要があります。

   レポート、ダッシュボード、およびカレンダーへのアクセス権の付与について詳しくは、 [レポート、ダッシュボード、カレンダーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* レポートまたはリストでフィルタ、表示、またはグループ化を選択した場合、Workfrontでは、ブラウザをログアウトまたは閉じても、そのオブジェクトのリストに対する選択が保持されます。 たとえば、タスクレポートの特定のビューを選択すると、その選択は他のタスクリスト（プロジェクト上のタスクのリストなど）に対して表示されます。

## フィルター

フィルターは、レポートに表示される結果を制御します。通常、結果を一般から特定に絞り込みます。 これは、必要な情報を取得し、その情報をレポートに戻すだけの篩のように機能します。

例えば、ログインしたユーザーに割り当てられたタスクのみを表示する場合は、「マイタスク」という名前のフィルタを作成し、そのフィルタに満たす必要のある条件を定義してレポートを実行し、ログインしたユーザーに割り当てられたタスクのみを表示します。

フィルターの属性には、次のものがあります。

* Workfrontには、様々なオブジェクトに対する多数のフィルターがデフォルトで用意されています。
* 所有または管理するフィルターをカスタマイズできます。

   フィルターについて詳しくは、 [Adobe Workfrontのフィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![フィルターアイコン](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## ビュー

レポートのビューを定義することで、レポートに含める情報を定義できます。 すべてのレポート要素と同様に、ビューも 1 つのオブジェクトタイプに基づきます。\
たとえば、タスクレポートのビューには、期限、コストなどの主要な財務詳細が表示されたり、割り当てや配信日の詳細を表示するために使用されたりします。 表示を使用して、レポート内のデータに関する様々な詳細を配信できます。

ビューの属性には、次のものがあります。

* デフォルトのWorkfrontビューを使用することも、独自のビューを作成することもできます。
* レポートを実行した後に、「表示」ドロップダウンフィールドから追加のビューを適用できます。
* 追加のビューは、レポートの作成時に定義されたビューに一時的に置き換わります。ただし、次回レポートに戻ると、デフォルトのビューが表示されます。

   ビューの詳細については、「 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## グループ化

グループ化は、データの整理方法を制御し、読みやすく理解しやすくします。 グループ化では、レポート全体で横棒グラフが作成され、共通の属性別に結果が一覧表示されます。 グループ化を作成する際に、レポートの結果をグループ化する方法の条件を定義します。

例えば、複数のプロジェクトにまたがるタスクのリストを、プロジェクト名別にグループ化すると、1 つのプロジェクトに属するすべてのタスクが、その名前でグループ化されます。

グループ化の属性には、次のものがあります。

* グループ化は、後でレポートにグラフを追加する場合に必須のレポート要素です。
* グループ化の結果に集計値が表示されま&#x200B;す。
* グループ化によって、グラフの軸が決まります。
* グループ化によって、マトリックスレポートでのヘッダーの識別が決まります。\
   マトリックスレポートの詳細については、「 [マトリックスレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* グループ化は、レポートの「概要」タブを作成し、レポートの集計値を提供するのに役立ちます。
* Workfrontは、デフォルトで、様々なオブジェクトに対して多数のグループ化を提供します。
* 所有または管理するグループをカスタマイズできます。

   グループ化について詳しくは、 [Adobe Workfrontでのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## その他のレポート要素

フィルター、ビューおよびグループ化に加えて、次の要素をレポートに追加することもできます。

* **プロンプト**:レポートを実行するたびに異なる方法でカスタマイズおよび適用できる開いたフィルター。\
   プロンプトの詳細については、「 」を参照してください。 [レポートにプロンプトを追加する](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **グラフ**:グラフを追加し、情報を視覚的に表示することで、レポートの内容をより充実させることができます。\
   レポートのグラフの詳細については、「 [レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
