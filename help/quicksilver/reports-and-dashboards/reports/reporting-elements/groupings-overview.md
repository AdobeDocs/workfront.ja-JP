---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfrontでのグループ化の概要
description: グループを追加して、レポートやリストの情報のレイアウトを管理できます。
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Adobe Workfrontでのグループ化の概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

グループを追加して、レポートやリストの情報のレイアウトを管理できます。

次の方法で、レポートにグループを追加できます。

* 既存のグループを編集することで、グループを作成できます。

   既存のグループ化のカスタマイズについて詳しくは、 [既存のグループを編集](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* グループ化はゼロから作成できます。

   最初からグループ化を作成する方法について詳しくは、 [Adobe Workfrontでのグループ化の作成](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

デフォルトでは、グループ化は、レポートまたはリストでグレーまたはブルーのハイライトで表示されます。 レポートまたはリストの結果は、個々のグループの下に、ハイライトなしで表示されます。

1 つのレポートには、最大 3 つのグループを追加できます。 マトリックスレポートを作成することで、最大 4 つのグループに分けて情報を整理できます。 マトリックスレポートの詳細については、 [マトリックスレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

標準のグループ化レポートでは、最初のグループは濃い色で、2 番目と 3 番目のグループは明るい色です。 グループ化のハイライトの色や、グループ名のフォントはカスタマイズできません。 グループ名の後の括弧内の数は、そのグループ化の下の結果数を表します。 レポートが複数のページにわたる場合、 *すべて* 結果はレポートまたはリストに表示され、各グループの結果の正確なカウントを取得します。

![サンプルのグループ化](assets/grouping-example-blue.png)

グループ化を使用する際は、次の点に注意してください。

* 既存のグループ内の情報をカスタマイズできます。 グループを表示できるすべてのユーザーに、変更内容を表示することもできます。
* Workfrontの管理者が、グループ化を作成するために、フィルター、ビューおよびグループを編集するためのアクセス権をユーザーに付与する必要があります。

   フィルタ、ビュー、およびグループへのアクセス権の付与について詳しくは、 [フィルター、ビューおよびグループに対するアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* グループに対する権限のレベルは、グループの保存方法を示します。 最初にグループを作成した場合は、変更を保存できます。作成しない場合は、グループ化のバージョンを保存するよう求めるプロンプトが表示されます。 他のユーザーと共有したグループに変更を加えると、他のユーザーとも同様に影響を受けます。
* 自分と共有されていたグループは、そのグループを共有したユーザーが管理アクセス権を付与した場合にのみカスタマイズできます。 グループ化の共有について詳しくは、 [フィルター、表示またはグループ化の共有](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* グループ化をインラインで編集することはできません。
* 複数選択のカスタムフィールド（チェックボックスなど）や、複数の値を持つことのできるフィールド（リソースマネージャなど）でグループ化することはできません。

## グループ化に関する追加情報

グループ化を使用する場合は、グループ化行の各列の値を集計し、グループ化のフィールドで情報を並べ替えることで、レポート情報をさらに管理できます。 不要になったグループを削除することもできます。

* [グループ化での値の集計](#aggregate-values-in-groupings)
* [グループ別に並べ替え](#sort-by-a-grouping)
* [グループの削除](#remove-a-grouping)

### グループ化での値の集計 {#aggregate-values-in-groupings}

レポートの各列の値を要約することで、レポートに表示されているデータをグループ化行で集計できます。 グループ化の列データの要約について詳しくは、 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>次の例外は、グループ化で次のフィールドの値を集計する場合に親オブジェクト（親タスクなど）に適用されます。
>
>* 「実績時間」（「計画/実績労務費」、「計画/実費原価」、「計画/実費」、「計画/実費」、「計画時間」など）を除くすべての数値および通貨フィールドは、子タスクとスタンドアロンタスクの値のみを集計します。 親タスクや親の値は集計されません。
>* 実際の時間は、メインの親タスクとスタンドアロンタスクの値を集計します。親タスクの親や子タスクの数を集計しません。
>* 数値および通貨値のカスタムデータフィールドは、すべてのタスクを集計します。親、子、親の親、スタンドアロンタスク。


### グループ別に並べ替え {#sort-by-a-grouping}

グループ化は並べ替えできません。 ビューは並べ替え可能です。 グループ化で取り込んだ値でリストを並べ替えるには、ビューの列の 1 つに同じ値を含め、ビューで並べ替えを適用する必要があります。 このようにして、リストはグループ化の値で間接的に並べ替えられます（グループ化に含まれているビューの値でも並べ替えられます）。 ビューの作成と、ビュー内の値による並べ替えについて詳しくは、 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### グループの削除 {#remove-a-grouping}

グループを削除する方法は、最初にグループを作成したか、共有したかによって異なります。 デフォルトのグループ化を削除することはできません。

* **グループを作成し、削除した場合**&#x200B;の場合、グループ化はWorkfrontシステムから削除されます。 以前に共有したユーザーは、このグループ化を使用できなくなりました。
* **グループが自分と共有され、自分が削除した場合**&#x200B;の場合、グループは自分だけに対して削除されます。 最初に作成したユーザーと、そのユーザーを共有した他のユーザーは、引き続きグループ化にアクセスできます。

グループ化の削除について詳しくは、「 [フィルター、ビュー、およびグループを削除する](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
