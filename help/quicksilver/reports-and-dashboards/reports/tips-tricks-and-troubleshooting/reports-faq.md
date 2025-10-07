---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: レポートに関する FAQ
description: レポートに関する FAQ
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 58567104d88e7e1363d4196aec8a36ee0566b95a
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 86%

---

# レポートに関する FAQ

<!--Audited: 05/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

レポートに関するよくある質問を次に示します。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。 

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td><p>新規：標準</p> 
   <p>現在：ワーク以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 時間差のカスタム計算で列に正しい結果が表示されないのはなぜですか？

<!--this section is linked from the Actual Hours article for Tasks in the Task Information folder; edit the links or do not delete or change this section-->

プロジェクト レポートに、予定時間数から実際の時間数を引く計算があります。

得られる結果が正しくありません。

<!--this changed with this issue in May 2025; Actual Hours changed from actualWorkRequired to actualWorkRequiredDouble: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/68108e860000120e90a79cb82e5811c2/updates : On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  -->

次が私の計算です。

`valueexpression=SUB(workRequired,actualWorkRequired)`

### 回答

Workfrontで時間を使用するほとんどのフィールドは分単位で保存されます。 これらのフィールドを計算で使用すると、ほとんどの場合、結果は数分です。 時間単位の結果を取得するには、計算の結果または参照するフィールドを 60 で割る必要があります。

予定時間数は分単位で保存されます。

計算に使用する [ 実際の時間数 ] フィールドに応じて、正しい数式は次のとおりです。

* 分単位で保存される従来の実際の時間の場合：

  `valueexpression=SUB(workRequired,actualWorkRequired)/60`

* 時間数に格納される実際の時間数の場合：

  `valueexpression=SUB(workRequired/60,actualWorkRequiredDouble)`

詳しくは、[ 実際の時間数を表示 ](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md) を参照してください。

## レポート内の各グラフ要素の値がグラフに表示されないのはなぜですか？

### 回答

レポートグラフに 50 を超えるグラフ要素がある場合、各要素の値はグラフに表示されません。

グラフにある要素が 50 個未満の場合、各要素の値がグラフに表示されます。グラフの各要素に表示する項目数を制限するには、フィルターを追加するか、レポートのグループ化を変更することを検討してください。

## レポートの返される結果が多すぎてグラフを表示できないのはなぜですか？

グラフを含むレポートを実行すると、「Whoa there...」というエラーメッセージが表示されます。このレポートが非常に多量のデータを返しているため、グラフが読み取れなくなっています。フィルターを追加したり、グラフのグループ化を変更したりして、結果を絞り込むことを検討してください。

### 回答

このエラーは、グラフに最大 618 個の個別の結果が含まれることを意味します。例えば、棒グラフに 618 個を超える棒が含まれる場合などです。表示の問題を解決するには、現在のフィルターとグループ化の選択を変更して、結果を絞り込む必要があります。

フィルターとグループ化の変更について詳しくは、[フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)および[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)の記事を参照してください。

## 同僚と同じレポート（またはカレンダー）にアクセスし、同僚には同僚のタスクが表示され、私には自分のタスク（またはイシュー）が表示されるのはなぜですか？

### 回答

レポートまたはカレンダーには、ログインしたユーザーを指すワイルドカードフィルター変数が含まれている場合があります。この場合、レポートには、ログインしたユーザーに基づく情報が表示されます。フィルターを調整して、ログインしたユーザーを指すワイルドカードを削除します。\
![ ユーザー ID フィルター変数 ](assets/qs--user.id-filter-variable-350x79.png)

ユーザーベースのワイルドカードフィルター変数の完全なリストについて詳しくは、[ワイルドカードフィルター変数の概要](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)を参照してください。

## レポート内のデータが不完全だと思われるのはなぜですか？

### 回答

ほとんどの場合これが発生するのは、アクセスが制限されてシステム内の項目を表示できない場合です。さらに、参照しようとしているアイテムが共有されていません。

レポートの作成者は、レポートを編集して、システム管理者またはデータを参照するアクセス権を持つ任意のプランユーザーのアクセス権限で実行できます。

詳しくは、[別のユーザーのアクセス権限を使用したレポートの実行と配信](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)を参照してください。

## 自分が割り当てられているタスク（またはイシュー）に関するレポートを、それらの所有者かどうかに関係なく作成するにはどうすればよいですか？

### 回答

自分に割り当てられているすべてのタスクまたはイシューを、所有者（またはプライマリ担当者）であるかどうかに関わらず参照するには、タスクレポートまたはイシューレポートで次のフィルターを使用します。

1. タスクレポートまたはイシューレポートにアクセスします。
1. 「**フィルター**」タブで、「**フィルター規則の追加**」をクリックします。

1. 「**フィールド名を入力...**」フィールドで、**割り当てられたユーザー名**&#x200B;と入力していき、リストに表示されたらそれを選択します。

   >[!NOTE]
   >
   >「**名前の割り当て**」フィールドは使用しないでください。これは、自分がプライマリ担当者または所有者であるタスクやイシューのみに絞り込む働きをするからです。

1. **が次に等しい**&#x200B;修飾子を選択します。
1. テキストボックスに *$$USER.ID* と入力していき、表示されるドロップダウンリストから選択します。\
   これにより、ログインしたユーザーに割り当てられているすべてのタスクとイシューを確認できます。ワイルドカードを特定のユーザー名に置き換えることができます。\
   ![ 自分に割り当てられたタスク ](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. 「**保存して閉じる**」をクリックします。

## プロジェクトのイシューリストやタスクリストの下部に「イシューを追加」または「タスクの追加」リンクが表示されないのはなぜですか？

### 回答

まず、プロジェクトにイシューやタスクを追加するための正しいアクセス権と権限があることを確認してください。その場合、**イシュー**&#x200B;リストや&#x200B;**タスク**&#x200B;リストの下部に、「**イシューを追加**」リンクや「**タスクの追加**」リンクが表示されるはずです。

ただし、これらのリンクが表示されない可能性がある状況が次のようにいくつかあります。

* これらのリストにクイックフィルターを適用している場合、リンクは表示されません。クイックフィルターを削除すると、リンクが表示され、プロジェクトにイシューやタスクを追加できるようになります。\
  クイックフィルターについては、[Adobe Workfront のリストの基本を学ぶ](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)を参照してください。

* これらのリストに&#x200B;**グループ化**&#x200B;が適用されていると、リンクは表示されません。**グループ化**&#x200B;を削除すると、リンクが表示されて、プロジェクトにイシューやタスクを追加できるようになります。\
  グループ化の作成については、[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

* プロジェクトのデフォルト通貨以外の通貨が選択されている&#x200B;**ビュー**&#x200B;がこれらのリストに適用されている場合、リンクは表示されません。**ビュー**&#x200B;を&#x200B;**プロジェクトの元の通貨**&#x200B;に変更すると、リンクが表示されて、プロジェクトにイシューやタスクを追加できるようになります。\
  ビューでの通貨の変更について詳しくは、[一意の為替レートを使用した財務データレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)を参照してください。

![ プロジェクト通貨 ](assets/nwe-project-original-currency-350x229.png)

## レポートやダッシュボードの情報は自動的に更新されますか？

### 回答

レポートやダッシュボードの情報は、自動的には更新されません。

情報は、キャッシュされたレポートで手動で更新できます。\
キャッシュされたレポートの更新について詳しくは、[レポートの実行](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md)を参照してください。

情報は、キャッシュされたダッシュボードで手動で更新できます。\
キャッシュされたダッシュボードの更新について詳しくは、[ダッシュボードの基本を学ぶ](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)の記事で[ダッシュボードの表示](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards)の節を参照してください。

## レポートの所有者を変更できますか？

### 回答

レポートの所有者は変更できません。ただし、レポートを作成したユーザーは、他のユーザーにレポートの編集を許可できます。ユーザーにレポートの編集を許可する方法は、ご自身のユーザータイプによって異なります。

* システム管理者は、プランライセンスを持つユーザーにレポートの編集を許可できます。それには、「レポート」行の「編集」オプションを設定して、レポートを作成するためのアクセス権を含めます。\
  詳しくは、[レポート、ダッシュボード、カレンダーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)を参照してください。

* レポートを作成および共有するためのアクセス権を持つエンドユーザーは、他のユーザーに個々のレポートの編集を許可できます。それには、レポートを共有し、他のユーザーにそのレポートの管理権限を与えます。\
  詳しくは、[Adobe Workfront でのレポートの共有](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)を参照してください。

レポートの表示または管理の権限を持っている場合は、レポートのコピーを作成することもできます。その場合は、ご自身がデフォルトでコピーの所有者になります。レポートのコピーについて詳しくは、[レポートのコピーの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)を参照してください。

## 非アクティブ化されたユーザーが所有するレポートにアクセスできないのはなぜですか？

### 回答

時には、レポートの所有者が、レポートの「**次のアクセス権限でこの報告書を作成する**」フィールドで指定されたユーザーにもなっている場合があります。**アクセス権限でこの報告書を実行：** ユーザーが非アクティブになっている場合、報告書を共有しているユーザーに対しては、報告書が表示されなくなります。 その場合は、「**アクセス権限でこのレポートを実行：** を空白にするか、フィールドにアクティブなユーザーを入力することで、レポートに再度アクセスできるようにします。

「**次のアクセス権限でこのレポートを作成：**」フィールドの詳細情報については、[別のユーザーのアクセス権を使用したレポートの実行と配信](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)を参照してください。ディアクティベートされているユーザーが所有するすべてのレポートの識別については、[レポートアクティビティに関するレポートの作成](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md)を参照してください。

## 削除されたユーザーが所有するレポートを含むダッシュボードにアクセスするには、どうすればよいですか？

### 回答

ユーザーを削除しても、そのユーザーが作成した任意のレポートにアクセスできますが、そのレポートに含まれているダッシュボードは削除されます。つまり、次の項目にアクセスできなくなります。

* オブジェクトの左側のパネルにあるダッシュボードを含む、レポートを含んだダッシュボード

ユーザーの削除による影響の詳細情報については、[ユーザーの削除](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)を参照してください。

レポートに対する表示アクセス権を持っている場合は、次の操作を実行できます。

1. レポートのコピーを作成します。\
   レポートのコピー作成の詳細情報については、[レポートのコピーの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)を参照してください。

1. コピーしたレポートを含めるようにダッシュボードを更新します。\
   ダッシュボードの編集方法については、[ダッシュボードの編集](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md)を参照してください。
