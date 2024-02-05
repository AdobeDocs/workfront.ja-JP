---
content-type: overview;reference
navigation-topic: workfront-navigation
title: '"[!DNL Adobe Workfront] オブジェクトの概要'
description: 「表示する情報 [!DNL Adobe Workfront] は、 [!DNL Workfront] データベース。 オブジェクトは、情報を駆動する要素です。 [!DNL Workfront]. これらのオブジェクトの詳細については、この記事を参照してください。」
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '2306'
ht-degree: 86%

---

# [!DNL Adobe Workfront] オブジェクトの概要

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

[!DNL Adobe Workfront] で表示する情報は、[!DNL Workfront] データベース内で保存されるオブジェクトで表されます。オブジェクトは、[!DNL Workfront] の情報を駆動する要素です。

[!DNL Workfront] でのオブジェクトの定義方法に関する理解は、組織で必要なニーズに合わせて正しいオブジェクトを使用できるようにするために重要です。

例えば、大量の作業を計画する場合、[!UICONTROL プロジェクト]オブジェクトを使用して、その作業を定義する必要があります。この作業をより少ない計画増分に分割するには、[!UICONTROL タスク]オブジェクトを使用できます。予定されていない作業量や予期せぬ作業量が少ない場合は、イシューオブジェクトを使用できます。プロジェクトのグループの進捗状況、予算やタイムラインへの準拠を追跡する場合は、[!UICONTROL ポートフォリオ]および[!UICONTROL プログラム]で整理できます。作業を解決する他の要素を定義するには、に保存されている他のオブジェクトを使用します。 [!UICONTROL プロジェクト], [!UICONTROL タスク], [!UICONTROL 問題]または [!UICONTROL Portfolio]，次に類似 [!UICONTROL ドキュメント], [!UICONTROL 更新], [!UICONTROL 時間], [!UICONTROL ユーザー]または [!UICONTROL ジョブの役割].

すべてのユーザーが簡単にアクセスできるようにするために、[!UICONTROL レポート]および[!UICONTROL ダッシュボード]は、[!DNL Workfront] のデータ量を視覚的に整理するのに役立つオブジェクトのもう 1 つの例です。

[!DNL Workfront] のオブジェクトの完全なリストについては、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を参照してください。

## オブジェクトの相互依存性と階層

オブジェクトは、[!UICONTROL Workfront] で相互にリンクされています。例えば、タスクやイシューをプロジェクト外に個別に存在させることはできません。[!UICONTROL タスク]および[!UICONTROL イシュー]は、[!UICONTROL プロジェクト]オブジェクトに保存されるオブジェクトの例です。[!UICONTROL タスク]および[!UICONTROL イシュー]は、プロジェクトに対する子オブジェクトと見なされます。

次に、[!DNL Workfront] およびそれぞれの親オブジェクトと子オブジェクト内で最もよく使用されるオブジェクトの一部を示します。

| **オブジェクト** | **親オブジェクト** | **子オブジェクト** |
|---|---|---|
| [!UICONTROL ポートフォリオ] |  | [!UICONTROL プログラム]、[!UICONTROL プロジェクト]、[!UICONTROL ドキュメント]、[!DNL Notes]、[!UICONTROL ユーザー] |
| [!UICONTROL プログラム] | [!UICONTROL ポートフォリオ] | [!UICONTROL プロジェクト]、[!UICONTROL ドキュメント]、[!UICONTROL メモ]、[!UICONTROL ユーザー] |
| [!UICONTROL プロジェクト] | [!UICONTROL ポートフォリオ]、[!UICONTROL プログラム] | [!UICONTROL タスク]、[!UICONTROL イシュー]、[!UICONTROL ドキュメント]、[!UICONTROL メモ]、[!UICONTROL 時間]、[!UICONTROL ユーザー] |
| [!UICONTROL タスク] | [!UICONTROL プロジェクト] | [!UICONTROL イシュー]、[!UICONTROL 子タスク]、[!UICONTROL ドキュメント]、[!UICONTROL メモ]、[!UICONTROL 時間]、[!UICONTROL ユーザー] |
| [!UICONTROL イシュー] | [!UICONTROL タスク]、[!UICONTROL プロジェクト] | [!UICONTROL ドキュメント]、[!UICONTROL メモ]、[!UICONTROL 時間]、[!UICONTROL ユーザー] |
| [!UICONTROL ダッシュボード] |  | [!UICONTROL レポート]、外部ページ |
| [!UICONTROL レポート] | [!UICONTROL ダッシュボード] |  |
| [!UICONTROL グループ] |  | [!UICONTROL ユーザー] |
| [!UICONTROL チーム] |  | [!UICONTROL ユーザー] |
| [!UICONTROL ユーザー] | [!UICONTROL グループ]、[!UICONTROL チーム]、[!UICONTROL 会社] | [!UICONTROL 担当業務] |
| [!UICONTROL 会社] |  | [!UICONTROL ユーザー] |
| [!UICONTROL ドキュメント] | [!UICONTROL タスク]、[!UICONTROL イシュー]、[!UICONTROL プロジェクト]、[!UICONTROL ポートフォリオ]、[!UICONTROL プログラム]、[!UICONTROL ユーザー] |  |
| [!UICONTROL 計画]* |  | [!UICONTROL 取り組み] |
| [!DNL Goals]* |  | [!UICONTROL 結果]、[!UICONTROL アクティビティ] |

[!DNL Workfront] のオブジェクトの完全なリストについては、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を参照してください。

*プランは、[!DNL Adobe Workfront Scenario Planner] のオブジェクトです。[!DNL Scenario Planner] について詳しくは、[[!UICONTROL シナリオプランナー]の概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。

*[!UICONTROL 目標] は [!DNL Adobe Workfront Goals] のオブジェクトです。[!DNL Workfront Goals] について詳しくは、[[!DNL Adobe Workfront Goals]  の概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。


## オブジェクト名のカスタマイズ

As a [!DNL Workfront] 管理者は、 [!DNL Workfront] を使用して [!UICONTROL レイアウトテンプレート].

[!UICONTROL レイアウトテンプレート]を使用してオブジェクト名をカスタマイズする方法について詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

レイアウトテンプレートをカスタマイズしてユーザーに割り当てると、そのユーザーには、オブジェクトのカスタマイズ名が表示されます。レイアウトテンプレートに割り当てられたユーザーには、web アプリケーション内のどの場所にも、オブジェクトのデフォルト名が表示されなくなります。

例えば、組織内で大規模な作業を「エンゲージメント」と呼ぶ場合は、「[!UICONTROL プロジェクト]」という名前を「エンゲージメント」のという名前に置き換えることができます。置き換えると、 [!DNL Workfront] インターフェイスで「[!UICONTROL プロジェクト]」が表示される場所にはすべて、「[!UICONTROL プロジェクト]」ではなく「エンゲージメント」と表示されます。

>[!NOTE]
>
>新しいオブジェクト名がユーザーに表示されるには、管理者が[!UICONTROL レイアウトテンプレート]を保存した後に、ユーザーが [!DNL Workfront] からログアウトし、再度ログインする必要があります。

>[!IMPORTANT]
>
>[!DNL Workfront] ドキュメントでは、常にオブジェクトのデフォルト名を参照します。[!DNL Workfront] 管理者は、オブジェクト名の変更をユーザーに通知し、[!DNL Workfront] ドキュメントの使用方法およびオブジェクト名の変更が反映されないアプリケーション範囲についてユーザーが理解できるようにします。

* [[!UICONTROL レイアウトテンプレート]を使用してカスタマイズ可能なオブジェクト名](#object-names-that-can-be-customized-using-a-layout-template)
* [カスタマイズされたオブジェクト名が反映される  [!DNL Workfront]  の範囲](#areas-of-workfront-that-reflect-the-customized-object-names)
* [カスタマイズされたオブジェクト名が反映されない  [!DNL Workfront]  の範囲](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### [!UICONTROL レイアウトテンプレート]を使用してカスタマイズ可能なオブジェクト名

[!DNL Workfront] 管理者は、次のオブジェクトの名前をカスタマイズして、組織の用語に合わせることができます。

* [!UICONTROL ポートフォリオ]
* [!UICONTROL プログラム]
* [!UICONTROL プロジェクト]
* [!UICONTROL タスク]
* [!UICONTROL イシュー]
* [!UICONTROL 目標]*
* [!UICONTROL 結果]*
* [!UICONTROL アクティビティ]*

  *[!UICONTROL 目標]、[!UICONTROL 結果]および[!UICONTROL アクティビティ]は、[!DNL Workfront Goals] を購入した場合にのみ使用できます。[!DNL Workfront Goals] について詳しくは、[[!DNL Adobe Workfront Goals] 概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。

* [!UICONTROL イニシアチブ]**
* [!UICONTROL シナリオ]**
* [!UICONTROL 計画]**

  **[!UICONTROL イニシアチブ]、[!UICONTROL シナリオ]および[!UICONTROL プラン]は、[!DNL Workfront Scenario Planner] を購入した場合にのみ使用できます。[!DNL Scenario Planner] について詳しくは、[ [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md) の基本を学ぶを参照してください。



[!UICONTROL レイアウトテンプレート]を使用してオブジェクト名をカスタマイズする方法について詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

Workfront の他のオブジェクトの名前はカスタマイズできません。[!DNL Workfront] のオブジェクトの完全なリストについては、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を参照してください。

オブジェクトの名前をカスタマイズすると、[!DNL Workfront] アプリケーションでそのオブジェクト名が表示されるほとんどの場所において、オブジェクトの新しい名前が表示されます。

### カスタマイズされたオブジェクト名が反映される [!DNL Workfront] のエリア

次のエリアに、更新されたオブジェクト名が表示されます。

* トップ ナビゲーション
* 左側のパネルナビゲーションのすべてのセクション
* すべてのメニュー
* アプリ内通知
* Report Builder とレポートの要素（ビュー、フィルターおよびグループ化）
* [!UICONTROL 保存]ボタン
* 書き出されたファイル
* メール
* モバイルアプリ

### カスタマイズされたオブジェクト名を反映していない [!DNL Workfront] のエリア

次のエリアでは、更新されたオブジェクトの名前は表示されません。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] アドイン

### オブジェクト名のカスタマイズの影響

[!DNL Workfront] でオブジェクト名をカスタマイズする場合は、次の点に注意してください。

* システム表示で、スタイルや文法上の誤りが発生する場合があります。例えば、「[!UICONTROL イシュー]」から「リクエスト」に名前を変更した場合、システム内で「リクエスト」というフレーズが表示されますが、これは意図したとおりに機能しており、バグと見なされません。
* オブジェクトのカスタム名は翻訳できません。[!DNL Workfront] デフォルトの名前のみは、サポートされている言語で翻訳できます。[!DNL Workfront] でサポートされる言語について詳しくは、[ [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md) でサポートされている言語を参照してください。カスタムオブジェクト名フィールドは外部文字をサポートしているので、任意の言語で用語を入力できます。
* を使用してオブジェクト名をカスタマイズする場合  [!UICONTROL レイアウトテンプレート]を割り当てる場合は、  [!UICONTROL レイアウトテンプレート] ビジネスユニット（チームまたはグループ）に基づいて\
   混乱を避けるために、これらのビジネスユニットのユーザーが明確に理解できる名前を使用することをお勧めします。
* メール通知と配信されたレポートには、メールを生成したユーザーの[!UICONTROL レイアウトテンプレート]で定義されたオブジェクト名が常に含まれます。ユーザーは、他のチームやグループのユーザーからメール通知を受信した場合、自分のグループやチームに関係のないオブジェクト名がメールに表示されることを覚悟しておく必要があります。\
   [!DNL Workfront] 管理者として、各オブジェクトに関連付けられているアイコンに注意するようにユーザーにアドバイスしてください。アイコンは、さまざまなオブジェクト名間で一貫性を保ち、データベースに表示されるデフォルトオブジェクトと一貫性を保ちます。オブジェクトに関連付けられたすべての [!DNL Workfront] アイコンのリストについては、[オブジェクトアイコン](#object-icons)を参照してください。

  >[!TIP]
  >
  >組織内の一般的なタスクについては、用語を反映するカスタムドキュメントを作成することを検討してください。

## オブジェクトアイコン

[!DNL Workfront] ドキュメントでは、常にオブジェクトのデフォルト名を参照します。オブジェクトの名前がカスタマイズされている場合は、オブジェクトに関連付けられたアイコンを頼りに、どのカスタマイズされたオブジェクトがどの [!DNL Workfront] デフォルトオブジェクトに対応するかを理解できます。

[!DNL Workfront] でカスタマイズした名前を付けることができるオブジェクトについて詳しくは、[[!UICONTROL レイアウトテンプレートを使用してカスタマイズできるオブジェクト名]](#object-names-that-can-be-customized-using-a-layout-template)を参照してください。

次に、Workfront のオブジェクトとそれに対応するアイコンのリストです。

| **オブジェクト** | **アイコン** | **カスタマイズ可能なオブジェクト名** |
|---|---|---|
| [!UICONTROL 会社] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL ダッシュボード] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 目標] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL グループ] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL イシュー] | ![](assets/issue-icon-nwe.png)、![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 担当業務] | ![job_role_icon.png](assets/job-role-icon-52x50.png)、![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png)、![](assets/job-role-nwe-no-color.png)、![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL プラン] | ![](assets/plan-icon.png)、![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL ポートフォリオ] | ![](assets/portfolio-icon-nwe.png)、![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL プログラム] | ![](assets/program-icon-nwe.png) 、![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL プロジェクト] | ![](assets/project-icon-nwe.png) 、![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL レポート] | ![](assets/report-icon-nwe.png)、![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL タスク] | ![](assets/task-icon-new.png)、![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL チーム] | ![](assets/team-icon-nwe.png)、![](assets/team-icon-nwe-color.png)、![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL テンプレート] | ![](assets/template-icon-nwe.png)、![](assets/nwe-templates-icon.png) |  |

## オブジェクトの参照番号

[!DNL Workfront] で作成された各オブジェクトには、一意の参照番号が割り当てられます。参照番号は、2 つの類似したオブジェクト（同じ名前のタスクなど）を区別するのに役立ちます。参照番号を使用してオブジェクトを検索したり、レポートに参照番号を含めたりできます。

参照番号でオブジェクトを検索する方法について詳しくは、[オブジェクトの参照番号の使用](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)を参照してください。

## オブジェクト固有の検索

[!DNL Workfront] で検索可能なすべてのオブジェクトを検索することも、基本検索および詳細検索で特定のオブジェクトを選択して検索することもできます。

[!DNL Workfront] のすべてのオブジェクトが検索できるわけではありません。[!DNL Workfront] では、次のオブジェクトに対して基本検索と詳細検索を実行できます。

| **オブジェクト** | **基本検索** | **詳細検索** |
|---|---|---|
| [!UICONTROL プロジェクト] | ✓ | ✓ |
| [!UICONTROL タスク] | ✓ | ✓ |
| [!UICONTROL イシュー] | ✓ | ✓ |
| [!UICONTROL レポート] | ✓ | ✓ |
| [!UICONTROL ユーザー] | ✓ | ✓ |
| [!UICONTROL テンプレート] | ✓ | ✓ |
| [!UICONTROL ドキュメント] | ✓ | ✓ |
| [!UICONTROL ポートフォリオ] | ✓ | ✓ |
| [!UICONTROL プログラム] | ✓ | ✓ |
| [!UICONTROL ダッシュボード] | ✓ | ✓ |
| [!UICONTROL 会社] | ✓ | ✓ |
| [!UICONTROL メモ] ( または [!UICONTROL 更新]) | ✓ |  |

[!DNL Workfront] での基本検索と高度な検索の実行の詳細については、[検索 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md)を参照してください。

## オブジェクトに関するレポート

[!DNL Workfront] でレポートの作成を開始する前に、オブジェクトの階層と相互依存性について理解することが非常に重要です。レポートはオブジェクトに固有のものです。 必要なデータを表示するには、レポートに適切なオブジェクトを選択する必要があります。

>[!IMPORTANT]
>
>同じレポートでは、選択したオブジェクトとその親オブジェクトについてのみレポートできます。子オブジェクトに関する情報を親オブジェクトのレポートに含めることはできません。例えば、プロジェクト情報はタスクレポートに表示できますが、タスク情報をプロジェクトレポートに表示することはできません。

アドビのオープン API を使用すれば、データベース内のすべてのオブジェクトについてレポートできます。データベース内のすべてのオブジェクトの完全なリストについては、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を参照してください。

>[!NOTE]
>
> * レイアウトテンプレートを使用してオブジェクトの名前をカスタマイズした場合は、レポートビルダー内のオブジェクトの名前もカスタマイズされます。どのオブジェクトがカスタマイズされているかを確認し、レポートビルダーでカスタマイズされた名前を探してください。でカスタマイズされた名前を持つオブジェクトの詳細については、 [!DNL Workfront]を参照してください。 [を使用してカスタマイズ可能なオブジェクト名  [!UICONTROL レイアウトテンプレート]](#object-names-that-can-be-customized-using-a-layout-template) 」を参照してください。
> * レポートでテキストモードを使用する場合、テキストモード式内のオブジェクト名は、カスタマイズされたオブジェクト名ではなく、[!DNL Workfront] の標準名です。レポートでのテキストモードの使用について詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)を参照してください。

レポートの作成に関して詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。\
API の詳細については、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を参照してください。

### レポートで使用できるオブジェクト

Report Builder を使用する際に、 [!DNL Workfront] web アプリケーション。 インデントされた箇条書きは、オブジェクトに関する詳細情報を提供し、追加のオブジェクトを表すものではありません。

* [!UICONTROL プロジェクト]
* [!UICONTROL タスク]
* [!UICONTROL 時間]
* [!UICONTROL イシュー]
* [!UICONTROL ユーザー]
* [!UICONTROL アクセスレベル]
* [!UICONTROL 承認]
* [!UICONTROL 承認プロセス]
* [!UICONTROL 割り当て]
* [!UICONTROL ベースライン]
* [!UICONTROL ベースラインタスク]
* [!UICONTROL 請求記録]
* [!UICONTROL 予算計上時間数]
   * これは、古い非推奨のリソース管理ツールに表示される [!UICONTROL 予算時間] です。
   * The &quot;Bud. [!UICONTROL 予算時間] レポートの「予算時間」フィールドは、[!UICONTROL リソースプランナー] でジョブの役割に対して予算が設定されている時間を示します。詳しくは、[[!UICONTROL 予算人件費]および[!UICONTROL プロジェクトの予算計上時間]を理解](../../../manage-work/projects/project-finances/budgeted-labor-cost.md)を参照してください。

* [!UICONTROL カレンダーイベント]
* [!UICONTROL 会社]
* [!UICONTROL カスタムフォーム]
* [!UICONTROL ダッシュボード]
* [!UICONTROL ドキュメント]
* [!UICONTROL ドキュメントの承認]
* [!UICONTROL ドキュメントバージョン]
   * ドキュメントのバージョン、バージョンが関連付けられているドキュメント、バージョンの作成者、およびドキュメントのバージョンに対して配達確認を作成したユーザー（存在する場合）に関する情報を表示できます。
* [!UICONTROL メールテンプレート]
* [!UICONTROL 費用]
* [!UICONTROL 費用タイプ]
* [!UICONTROL 外部ページ]
* [!UICONTROL お気に入り]
* [!UICONTROL フィルター]
* [!UICONTROL 目標]
   * 戦略的目標のレポートを作成したり、プロジェクトが目標アクティビティとして目標に関連付けられている場合は、プロジェクトレポートに目標関連情報を表示したりできます。組織が [!DNL Workfront Goals] ライセンスを購入している場合にのみ、戦略的目標を作成し、プロジェクトに結び付けることができます。[!DNL Workfront Goals] について詳しくは、[[!DNL Workfront Goals]  の概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。プロジェクトを戦略目標に接続する方法については、 [Adobe Workfront目標の目標へのプロジェクトの追加](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
* [!UICONTROL ビジネス事例]. プロジェクトの目標と戦略的目標の詳細については、[ [!DNL Adobe Workfront]  用語の用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

* [!UICONTROL グループ]
* [!UICONTROL グループ化]
* [!UICONTROL 時間タイプ]
* [!UICONTROL イニシアチブ]
   * 会社が [!DNL Workfront Scenario Planner] ライセンスを購入している場合にのみ、計画の子オブジェクトであるイニシアティブのレポートを作成できます。イニシアチブの詳細については、[ [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md)のイニシアチブの概要を参照してください。

* イニシアティブの担当業務
   * 会社が [!DNL Workfront Scenario Planner] ライセンスを購入している場合にのみ、プラン内のイニシアチブに関連付けられた担当業務のレポートを作成できます。イニシアティブの作成と担当業務への関連付けの詳細については、[イニシアチブの作成と編集 [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md)を参照してください。

* [!UICONTROL イテレーション]
* [!UICONTROL 担当業務]
* [!UICONTROL ジャーナルエントリ]
   * タスク、プロジェクト、イシューなどのオブジェクトの「[!UICONTROL アップデート]」エリアで、追跡されたシステムアップデートについてレポートできます。詳しくは、 [レポート [!UICONTROL 更新] 領域](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL レイアウトテンプレート]
* [!UICONTROL マイルストーン]
* [!UICONTROL マイルストーンパス]
* [!UICONTROL 注意] または [!UICONTROL 更新]
   * 個々のユーザーが追加したコメントについてレポートできます。

* [!UICONTROL パラメーター]（または [!UICONTROL カスタムフィールド]）
* [!UICONTROL パラメーターグループ]（または[!UICONTROL セクション区切り]）
* [!UICONTROL ポートフォリオ]
* [!UICONTROL プログラム]
* [!UICONTROL プロジェクト]（[!UICONTROL 財務データ]）

  >[!NOTE]
  >
  >[!UICONTROL プロジェクト]（[!UICONTROL 財務データ]）レポートに財務情報が入力されるのは、関連付けられたデータが 5 年未満である場合のみです。例えば、担当業務が 2015年1月（PT）にタスクに割り当てられ、今日が 2021年9月（PT）である場合、その担当業務の [!UICONTROL 配分日] のような財務ファイルは [!UICONTROL  プロジェクト（財務データ）]レポートに入力されません。

* [!UICONTROL プルーフの承認]
   * 承認のために送信されたプルーフ、[!UICONTROL 承認者] に関する情報、リクエスターに関する情報（リクエスターがライセンスを取得した [!DNL Workfront] ユーザーの場合）バージョン情報、プルーフ ID、プルーフの作成日など、プルーフの承認に関するさまざまな情報を表示できます。\
      [!UICONTROL 配達確認の承認] レポートには、ユーザーの自分の作業領域で、まだ決定が下されていない配達確認のみが含まれます。\
   * [ [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) でのプルーフを共有の[プルーフへのユーザーを追加](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add)で説明されているように、プルーフの承認は [!DNL Workfront] で割り当てられます。

* [!UICONTROL キュー]
* [!UICONTROL キューのトピック]
* [!UICONTROL 評価]（担当業務の[!UICONTROL 請求評価]情報が表示されます）
* [!UICONTROL リマインダ通知]
* [!UICONTROL レポート]
* [!UICONTROL リソースプール]
* [!UICONTROL リスク]
* [!UICONTROL リスクタイプ]
* [!UICONTROL スケジュール]
* [!UICONTROL スコアカード]
* [!UICONTROL チーム]
* [!UICONTROL テンプレート]
* [!UICONTROL テンプレートのタスク]
* [!UICONTROL 休暇]
   * ユーザーのプロファイルに記載されている休暇についてレポートできます。

* [!UICONTROL タイムシート]
* [!UICONTROL タイムシートプロファイル]
* [!UICONTROL トピックグループ]
* [!UICONTROL ユーザーの承認]
* [!UICONTROL ユーザーの委任]

   * 不在の際に他の人のタスクやイシューの実行を委任されたユーザーについてレポートできます。このレポートには、不在ユーザーと不在の間に職務を遂行するユーザーが表示されます。

* [!UICONTROL ユーザーの決定]

   * 今月にユーザーが配達確認およびドキュメントに対しておこなった決定の数をレポートできます。

* [!UICONTROL 表示]
* [!UICONTROL 作業項目] （これにより、タスクと問題に関するレポートが生成されます）
