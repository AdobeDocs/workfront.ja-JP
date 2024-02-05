---
navigation-topic: use-lists
title: ' [!DNL Adobe Workfront] のリストの概要'
description: ' [!DNL Adobe Workfront]  内のオブジェクトのリストを表示して、オブジェクトの開始日と期限、オブジェクトに割り当てられたユーザー、オブジェクトに関連付けられている他のオブジェクトなどの情報を取得できます。'
feature: Get Started with Workfront
author: Lisa
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '2397'
ht-degree: 99%

---

# [!DNL Adobe Workfront] のリストの概要

<!--
{{highlighted-preview}}
-->

[!DNL Adobe Workfront] 内のオブジェクトのリストを表示して、オブジェクトの開始日と期限、オブジェクトに割り当てられたユーザー、オブジェクトに関連付けられている他のオブジェクトなどの情報を取得できます。

[!DNL Workfront] に含まれるリストの特徴の一部を以下に示します。

* リストは 5 分ごとに自動的に更新され、システム内の他のユーザーが別の場所で更新した情報が更新されます。
* [!DNL Workfront] の一部のエリアは、オブジェクトのデフォルトリストで事前に設定されています。

  これらの事前に設定されたリストのほとんどはカスタマイズ可能です。

* [!DNL Workfront] 管理者はカスタムリストを作成して、[!DNL Workfront] の様々なエリアに適用できます。

  システムレベルのリストの作成について詳しくは、[デフォルトのフィルター、ビュー、グループの作成、編集および共有](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Request] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>フィルター、ビュー、グループに対する [!UICONTROL View] 以上のアクセス権</p> <P>[!UICONTROL Setup] エリアの項目の場合、項目の管理アクセス権、または [!UICONTROL System Administrator] のアクセスレベルが必要です。</P> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されているか [!DNL Workfront] 管理者に確認してください。<br>[!DNL Workfront] 管理者がアクセスレベルを変更する方法に関して詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>共有のアクセス権を持つ [!UICONTROL View] 以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td>
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## オブジェクトリスト

以下に、[!DNL Workfront] にあるオブジェクトリストの一部のタイプ、およびオブジェクトの表示権限を持っている場合にデフォルトで表示されるエリアの一部を示します。

>[!NOTE]
>
>* このリストは包括的なものではありません。それぞれのオブジェクトリストは、レポートまたはダッシュボードにも表示できます。例えばプロジェクトレポートや、プロジェクトレポートを含むダッシュボードには、プロジェクトのリストも表示されます。
>* このリストで「選択」とは、名前の左にあるチェックボックスではなく、項目の名前をクリックする必要があることを意味します。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] リスト</strong></th> 
   <th><strong>オブジェクトリストの場所</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ポートフォリオのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>プログラムのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Portfolios]／[!UICONTROL select a portfolio]／[!UICONTROL Programs]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL Programs]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>プロジェクトのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfolios]／[!UICONTROL select a portfolio]／[!UICONTROL Projects]</p> </li> 
     <li> <p>[!UICONTROL Portfolios]／[!UICONTROL select a portfolio]／[!UICONTROL Programs]／[!UICONTROL select a program]／[!UICONTROL Projects]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>タスクのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Tasks]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Tasks]／[!UICONTROL select a task]／[!UICONTROL Subtasks]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Tasks]／[!UICONTROL select a task]／ [!UICONTROL Predecessors*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>イシューのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Tasks]／[!UICONTROL select a task]／[!UICONTROL Issues]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Tasks]／[!UICONTROL select a task]／[!UICONTROL Subtasks]／[!UICONTROL select a task]／[!UICONTROL Issues]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>レポートのリスト</td> 
   <td> 
    <ul> 
     <li> <p>  [!UICONTROL Reports]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>ダッシュボードのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Dashboards]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>反復のリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams]／[!UICONTROL Iterations]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>ユーザーのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Users]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>ドキュメントのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portfolios]／[!UICONTROL select a portfolio]／[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Portfolios]／[!UICONTROL select a portfolio]／[!UICONTROL Programs]／[!UICONTROL select a program]／[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Tasks]／[!UICONTROL select a task]／[!UICONTROL Documents]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Issues]／[!UICONTROL select an issue]／[!UICONTROL Documents]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>タイムシートのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Timesheets]／[!UICONTROL All Timesheets]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求料金のリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Billing Rates*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>請求レコードのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Billing Records]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>リスクのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Risks]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>費用のリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project／[!UICONTROL Expenses]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Tasks]／[!UICONTROL select a task]／[!UICONTROL Expenses]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>時間エントリのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Tasks]／[!UICONTROL select a task]／[!UICONTROL Hours]</p> </li> 
     <li> <p>[!UICONTROL Projects]／[!UICONTROL select a project]／[!UICONTROL Issues]／[!UICONTROL select an issue]／[!UICONTROL Hours]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td class="preview">カスタムフォームのリスト</td> 
   <td> 
    <ul> 
     <li class="preview"> <p>[!UICONTROL Setup]／[!UICONTROL Custom Forms]</p>
     <!--Remove the following note box when this goes to Production. Or do this when the Preview highlighting becomes available.-->
     <p><b>メモ</b>：現在、プレビュー環境でのみ使用できます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>グループまたはサブグループのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup]／[!UICONTROL Groups]</p> </li>
     <li> <p>[!UICONTROL Setup]／[!UICONTROL Groups]／[!UICONTROL select the parent group]／[!UICONTROL Subgroups] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>チームのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup]／[!UICONTROL Teams]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>会社のリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup]／[!UICONTROL Companies]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>スケジュールのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup]／[!UICONTROL Schedules]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>レイアウトテンプレートのリスト</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup]／[!UICONTROL Layout Templates]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

指定したエリアではリストをカスタマイズできません。[!DNL Workfront] 管理者は、システムレベルでカスタマイズされたリストを作成できます。また、レポートの編集が可能なアクセスレベルを持っている場合は、このオブジェクトのレポートを作成できます。

## リスト要素

リストには、形式と表示される情報を定義する特定の要素が含まれます。デフォルトで使用可能な複数のシステムリスト要素を検索できます。また、必要に応じて、カスタム要素を作成することもできます。

>[!NOTE]
>
>新しいフィルター、ビューまたはグループ化をリストから選択した場合、[!DNL Workfront] からログアウトしても、選択内容は保持されます。

リストの要素を次に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>要素</strong></th> 
   <th><strong>説明</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Filter]</strong></td> 
   <td> <p>フィルターは、指定した条件に基づいて、不要な情報をリストから除外します。 </p> <p>詳しくは、 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">フィルターの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL View]</strong></td> 
   <td> <p>ビューは、画面に表示するフィールド（列）を定義するものです。</p> <p>詳しくは、<a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">[!DNL Adobe Workfront]</a> のビューの概要を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Grouping]</strong></td> 
   <td> <p>グループ化では、指定した条件に基づいて、リスト上のオブジェクトがエリアで分割されます。</p> <p>例えば、リスト内のイシューは、ステータス別または優先度別のセクションに表示されます。</p> <p>標準のグループ化では、最大 3 つのレイヤーのグループ化を設定できます。また、テキストモードでグループ化を設定する場合は、4 つ目のレイヤーを追加できます。</p> <p>グループ化について詳しくは、<a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">[!DNL Adobe Workfront]</a> でのグループ化の概要を参照してください。</p> <p>テキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">テキストモードの概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

これらの要素は、デフォルトで各リストの上部に表示されます。固定されており、リストをスクロールしても移動しません。各要素を識別するアイコンにポインタを合わせます。

![](assets/nwe-list-elements.png)

次のエリアでリスト要素をカスタマイズし、他のユーザーと共有できます。

* システムのデフォルトリスト（この記事の[ [!DNL Adobe Workfront]](#default-workfront-lists) のリストの基本を学ぶの節を参照）
* 自分と共有されているレポート

リストの構成要素は、レポートの構成要素と同じです。

リストとレポートの構成要素の作成とカスタマイズについて詳しくは、[レポート要素：フィルター、ビューおよびグループ化](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)を参照してください。

## リストのアクション

リストでは、次のアクションを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>アクション</strong></th> 
   <th><strong>情報</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>インライン編集</strong> </td> 
   <td> <p>リスト内のオブジェクトとその情報を直接編集します。</p> <p>詳しくは、<a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">[!DNL Adobe Workfront]</a> のリスト内の項目のインライン編集を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>[!UICONTROL Summary] を使用した更新</strong> </td> 
   <td> <p>[!UICONTROL Summary] パネルを使用して、プロジェクトレベルのタスクとイシューを更新します。</p> <p>ヒント：概要は一部のオブジェクトには使用できません。また、タスクやイシューのレポートでは使用できません。</p> <p>詳しくは、<a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">概要について</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>リスト表示をカスタマイズ</strong> </td> 
   <td> <p>リストの外観、列の配置、項目の並べ替え順、表示する項目の数をカスタマイズします。</p> <p>メモ：ページに表示する項目数についての変更は、[!DNL Workfront] からログアウトしたときや、ブラウザーを閉じたときに元に戻ります。また、8 時間の期間が経過すると、変更が元に戻る場合もあります。</p> <p>詳しくは、<a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">リストの表示方法の変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>クイックフィルター</strong> </td> 
   <td> <p>クイックフィルターを適用すると、重要な項目だけを検索して、簡単にレビューや更新、他のユーザーとの共有を行うことができます。</p> <p>重要：クイックフィルターを使用して検索語を含む項目を検索するとき、画面に表示されている項目か、ページの下までスクロールした後に表示される項目かを指定できます。ブラウザーの検索機能を使用すると、既に画面に表示されている項目のみを検索できます。リストに複数のページがある場合、クイックフィルターは現在のページの項目のみを検索します。</p> <p>詳しくは、<a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">クイックフィルターのリストへの適用</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>書き出し</strong> </td> 
   <td> <p>[!DNL Workfront] からオブジェクトのリストを書き出します。リストに 2,000 個を超える項目が含まれている場合、1 ページですべての項目をレビューする唯一の方法が、リストの書き出しです。</p> <p>リストの書き出しについて詳しくは、<a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">リストの書き出し</a>を参照してください。書き出し形式と制限について詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">データの書き出し</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### リストツールバー

次の表に、ツールバーで使用できるアイコンの多くを示し、クリックしたときの動作を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>アイコン</strong></td> 
   <td><strong>説明</strong></td> 
   <td><strong>クリック時</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL Add item or user]</td> 
   <td>新しい項目やユーザーの追加など、その他のオプションを開きます。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insert task above]</td> 
   <td> <p>選択したタスクの上にタスクを挿入します。</p> <p>これは、タスクに対してのみ使用できます。 </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Insert task below]</td> 
   <td> <p>選択したタスクの下にタスクを挿入します。</p> <p>これは、タスクに対してのみ使用できます。 </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL Edit]</td> 
   <td>選択した項目を編集します。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copy]</td> 
   <td>選択した項目をコピーします。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Delete]</td> 
   <td>選択した項目を削除します。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL Add to]</td> 
   <td> <p>選択したイシューをイテレーションに追加するためのダイアログボックスを開きます。</p> <p>これは、イシューに対してのみ使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL Share]</td> 
   <td>選択した項目を共有します。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Indent and outdent tasks] </td> 
   <td> <p>選択したタスクのレベルを上下させます。 </p> <p>これは、タスクに対してのみ使用できます。 </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL More]</td> 
   <td>選択した項目の追加のオプションを開きます。</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL Quick filter] </p> </td> 
   <td> <p>表示されたリスト内の項目を検索するクイックフィルター検索ボックスを開きます。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL Export]</td> 
   <td>リストを PDF、Excel、またはタブ区切り形式のファイルに書き出します。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>リストをアジャイルビューで表示します。<br>これは、タスクに対してのみ使用できます。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>リストを [!UICONTROL Gantt Chart] ビューで表示します。</p> <p>これは、プロジェクトとタスクに対してのみ使用できます。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>[!UICONTROL Filter] ドロップダウンメニュー</td> 
   <td> <p>フィルターのリストと、フィルターを管理するための追加のオプション（フィルターの作成など）を表示します。 </p> <p>小さい画面では、フィルター名がフィルターアイコンに置き換えられます。「[!UICONTROL All]」以外のフィルターを適用すると、フィルターアイコンに青い点が表示されます。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[!UICONTROL View] ドロップダウンメニュー</td> 
   <td> <p>ビューのリストと、ビューを管理するための追加のオプション（ビューの作成など）を表示します。 </p> <p>小画面では、ビュー名が [!UICONTROL view] アイコンに置き換えられます。「[!UICONTROL Standard]」以外のビューを適用すると、[!UICONTROL View] アイコンに青い点が表示されます。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[!UICONTROL Grouping] ドロップダウンメニュー</td> 
   <td> <p>グループ化のリストと、グループ化を管理するための追加のオプション（グループ化の作成など）を表示します。 </p> <p>小画面では、グループ名が [!UICONTROL grouping] アイコンに置き換えられます。「[!UICONTROL Nothing]」以外のグループ化を適用すると、[!UICONTROL Grouping] アイコンに青い点が表示されます。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL Plan mode]</p> </td> 
   <td> <p>加えた変更をタスクリストに自動で保存するか、手動で保存するかを選択します。 </p> <p>リスト内のタスクの編集について詳しくは、<a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">リスト内のタスクを編集</a>を参照してください。 </p> <p>これは、タスクに対してのみ使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL Summary]</td> 
   <td> <p>選択した項目の [!UICONTROL Summary] ボックスの表示と非表示を切り替えます。</p> <p>これは、タスクとイシューに対してのみ使用できます。</p> <p>新しい [!DNL Adobe Workfront] エクスペリエンスの [!UICONTROL Summary] パネルについて詳しくは、<a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">概要の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Remove]</td> 
   <td>リストから何かを削除します。例えば、グループまたはサブグループのメンバーシップを管理するグループ管理者は、<a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">グループのメンバーシップを表示および管理</a>で説明されているように、グループメンバーを削除します。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comment] /[!UICONTROL Update]</td> 
   <td> <p>コメントを入力するか、更新します。</p> </td> 
  </tr> 
 </tbody> 
</table>

## リストとレポートの違い

リストとレポートは、両方とも、オブジェクトのタイプに関する情報を含むグリッドです。

次の表に、リストとレポートの類似点と相違点の概要を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>機能</strong> </th> 
   <th><strong>リスト</strong> </th> 
   <th><strong>レポート</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>誰でも作成できる</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Workfront] 管理者と [!UICONTROL Plan] ライセンスを持つユーザーのみが作成できる</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>デフォルトのセットは、次の場所から利用できます。 [!DNL Workfront]</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>標準モードでカスタマイズ可能</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>テキストモードでカスタマイズ可能</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>他のユーザーと共有できる</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>システム全体で共有できる</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>システム外で共有できる</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>.pdf、[!DNL Excel]、およびタブ区切り形式に書き出すことができる</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>メールで配信をスケジュールできる</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>レイアウトテンプレートに追加できる</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>カスタムセクションに追加できる </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>ダッシュボードに追加できます</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>プロンプトを使用して、表示内容をカスタマイズできます</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>グラフに表示できます</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>オブジェクトをインラインで編集できます</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

フィルター、ビュー、グループ化を作成するには、それらに対するアクセス権が必要です。詳しくは、[フィルター、ビュー、グループ化にアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)を参照してください。

レポート、ダッシュボード、カレンダーを作成するには、フィルター、ビュー、グループ化へのアクセス権に加えて、レポート、ダッシュボード、カレンダーに対するアクセス権が必要です。詳しくは、[レポート、ダッシュボード、カレンダーにアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)を参照してください。

ダッシュボードに配置されるレポートのリストは、レポートの作成者がリスト要素をダッシュボードに表示されるように設定している場合にのみ、カスタマイズできます。

>[!NOTE]
>
>レポートを作成して先にダッシュボードに追加しないと、リストをダッシュボードに追加できません。

レポートの作成について詳しくは、[カスタムレポートを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。カスタムセクションの作成については、[カスタムタブまたはセクションの作成](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)を参照してください。

## 更新されたリストと従来のリストの違い

[!DNL Workfront] には、次の 2 種類のリストがあります。

* 従来のリスト

  ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* 更新されたリスト

  ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

[!DNL Adobe Workfront] では両方のタイプのリストが使用されます。

[!DNL Adobe Workfront] のリストとレポートは、次のもの以外はすべて、更新されたリストです。

* [!UICONTROL 設定]エリアのリスト
* [!UICONTROL レポート]エリアのリスト

次の表に、[!DNL Workfront] の従来のリストと更新されたリストの相違点をいくつか示します。

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>従来のリスト</b></td> 
   <td><b>更新されたリスト</b></td> 
  </tr> 
  <tr> 
   <td> <p>従来のフォント、列ヘッダー、青系統のカラースキーム</p> </td> 
   <td> <p>更新されたフォント、列ヘッダー、グレー系統のカラースキーム</p> </td> 
  </tr> 
  <tr> 
   <td> <p>インライン編集に時間がかかる</p> </td> 
   <td> <p>インライン編集が高速化</p> </td> 
  </tr> 
  <tr> 
   <td> <p>デフォルトで <strong>100 個</strong>の項目を表示</p> </td> 
   <td> <p>デフォルトで<strong>すべて</strong>の項目または最大で <strong>2000 個</strong>の項目を表示</p> </td> 
  </tr> 
  <tr> 
   <td> <p>リスト内の項目の検索には、Ctrl + F キーを使用</p> </td> 
   <td> <p>クイックフィルターを使用して、大きなリスト内の情報をすばやく検索</p> <p>リストでのクイックフィルターの使用について詳しくは、<a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">リストへのクイックフィルターの適用</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>リッチテキスト形式のカスタムフィールドをインライン編集することはできません。</td> 
   <td> <p>書式設定機能付きのカスタムフィールドのテキストは、太字、斜体、下線、箇条書き、段落番号、ハイパーリンク、ブロック引用符を使用できるように設定できます。</p> <p>詳しくは、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>条件付き書式により、リスト内のリンクのテキストカラーを変更可能</td> 
   <td>リスト内のリンクにテキストカラーの変更を適用することは不可能</td> 
  </tr> 
 </tbody> 
</table>
