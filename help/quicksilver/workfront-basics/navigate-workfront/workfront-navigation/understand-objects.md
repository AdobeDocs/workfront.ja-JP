---
content-type: overview;reference
navigation-topic: workfront-navigation
title: でのオブジェクトについて [!DNL Adobe Workfront]
description: でのオブジェクトについて [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: a2650ccc3deffd841a7b497e6ff1b5eed6145211
workflow-type: tm+mt
source-wordcount: '2255'
ht-degree: 7%

---

# でのオブジェクトについて [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

表示する情報 [!DNL Adobe Workfront] は、 [!DNL Workfront] データベース。 オブジェクトは、情報を駆動する要素です。 [!DNL Workfront].

でのオブジェクトの定義方法について [!DNL Workfront] は、組織で必要なニーズに合わせて正しいオブジェクトを使用できるように重要です。

例えば、大量の作業を計画する場合、 [!UICONTROL プロジェクト] オブジェクトを使用して、その動作を定義します。 この作業をより少ない計画増分に分割するには、 [!UICONTROL タスク] オブジェクト。 予定されていない作業量や予期せぬ作業量が少ない場合は、Issue オブジェクトを使用できます。 プロジェクトのグループの進捗状況、予算やタイムラインへの準拠を追跡する場合は、次のように整理できます。 [!UICONTROL Portfolio] および [!UICONTROL プログラム]. 作業を解決する他の要素を定義するには、に保存されている他のオブジェクトを使用します。 [!UICONTROL プロジェクト], [!UICONTROL タスク], [!UICONTROL 問題]または [!UICONTROL Portfolio]，次に類似 [!UICONTROL ドキュメント], [!UICONTROL 更新], [!UICONTROL 時間], [!UICONTROL ユーザー]または [!UICONTROL ジョブの役割].

[!UICONTROL レポート] および [!UICONTROL ダッシュボード] は、でのデータ量の整理に役立つオブジェクトのもう 1 つの例です。 [!DNL Workfront] すべてのユーザーが簡単にアクセスできるように、視覚的に説明します。

のオブジェクトの完全なリスト [!DNL Workfront]を参照し、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

## オブジェクトの相互依存性と階層

オブジェクトは、 [!UICONTROL Workfront]. 例えば、タスクやイシューをプロジェクト外に個別に存在させることはできません。 [!UICONTROL タスク] および [!UICONTROL 問題] は、 [!UICONTROL プロジェクト] オブジェクト。 [!UICONTROL タスク] および [!UICONTROL 問題] は、プロジェクトに対する子オブジェクトと見なされます。

次に、で最もよく使用されるオブジェクトの一部を示します。 [!DNL Workfront] そして、それぞれの親オブジェクトと子オブジェクト

| **オブジェクト** | **親オブジェクト** | **子オブジェクト** |
|---|---|---|
| [!UICONTROL ポートフォリオ] |  | [!UICONTROL プログラム], [!UICONTROL プロジェクト], [!UICONTROL ドキュメント], [!DNL Notes], [!UICONTROL ユーザー] |
| [!UICONTROL プログラム] | [!UICONTROL ポートフォリオ] | [!UICONTROL プロジェクト], [!UICONTROL ドキュメント], [!UICONTROL メモ], [!UICONTROL ユーザー] |
| [!UICONTROL プロジェクト] | [!UICONTROL Portfolio], [!UICONTROL プログラム] | [!UICONTROL タスク], [!UICONTROL 問題], [!UICONTROL ドキュメント], [!UICONTROL メモ], [!UICONTROL 時間], [!UICONTROL ユーザー] |
| [!UICONTROL タスク] | [!UICONTROL プロジェクト] | [!UICONTROL 問題], [!UICONTROL 子タスク], [!UICONTROL ドキュメント], [!UICONTROL メモ], [!UICONTROL 時間], [!UICONTROL ユーザー] |
| [!UICONTROL 問題] | [!UICONTROL タスク], [!UICONTROL プロジェクト] | [!UICONTROL ドキュメント], [!UICONTROL メモ], [!UICONTROL 時間], [!UICONTROL ユーザー] |
| [!UICONTROL ダッシュボード] |  | [!UICONTROL レポート]、外部ページ |
| [!UICONTROL レポート] | [!UICONTROL ダッシュボード] |  |
| [!UICONTROL グループ] |  | [!UICONTROL ユーザー] |
| [!UICONTROL チーム] |  | [!UICONTROL ユーザー] |
| [!UICONTROL ユーザー] | [!UICONTROL グループ], [!UICONTROL チーム], [!UICONTROL 会社] | [!UICONTROL 担当業務] |
| [!UICONTROL 会社] |  | [!UICONTROL ユーザー] |
| [!UICONTROL ドキュメント] | [!UICONTROL タスク], [!UICONTROL 問題], [!UICONTROL プロジェクト], [!UICONTROL Portfolio], [!UICONTROL プログラム], [!UICONTROL ユーザー] |  |
| [!UICONTROL 計画]* |  | [!UICONTROL イニシアチブ] |
| [!DNL Goals]* |  | [!UICONTROL 結果], [!UICONTROL アクティビティ] |

のオブジェクトの完全なリスト [!DNL Workfront]を参照し、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

*プランは、 [!DNL Adobe Workfront Scenario Planner]. 詳しくは、 [!DNL Scenario Planner]を参照してください。 [The [!UICONTROL シナリオプランナー] 概要](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL 目標] は次の対象です： [!DNL Adobe Workfront Goals]. 詳しくは、 [!DNL Workfront Goals]を参照してください。 [[!DNL Adobe Workfront Goals] 概要](../../../workfront-goals/goal-management/wf-goals-overview.md).


## オブジェクト名のカスタマイズ

As a [!DNL Workfront] 管理者は、 [!DNL Workfront] を使用して  [!UICONTROL レイアウトテンプレート].

を使用してオブジェクト名をカスタマイズする方法の詳細  [!UICONTROL レイアウトテンプレート]を参照してください。 [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

レイアウトテンプレートをカスタマイズしてユーザに割り当てると、そのユーザには、オブジェクトのカスタマイズ名が表示されます。 レイアウトテンプレートに割り当てられたユーザーには、Web アプリケーション内の任意の場所にオブジェクトのデフォルト名が表示されなくなります。

>[!NOTE]
>
>新しいオブジェクト名をユーザーに表示するには、ログアウトしてからに再度ログインする必要があります。 [!DNL Workfront] 保存後  [!UICONTROL レイアウトテンプレート].

>[!IMPORTANT]
>
>The [!DNL Workfront] ドキュメントでは、常にオブジェクトのデフォルト名を参照します。 As a [!DNL Workfront] 管理者は、オブジェクト名の変更をユーザーに通知し、ユーザーがオブジェクト名の使用方法を理解できるようにします。 [!DNL Workfront] ドキュメント、およびオブジェクトの名前の変更を反映しないアプリケーションの領域。

* [を使用してカスタマイズ可能なオブジェクト名  [!UICONTROL レイアウトテンプレート]](#object-names-that-can-be-customized-using-a-layout-template)
* [領域： [!DNL Workfront] カスタマイズされたオブジェクト名を反映した](#areas-of-workfront-that-reflect-the-customized-object-names)
* [領域： [!DNL Workfront] カスタマイズされたオブジェクト名を反映していない](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### を使用してカスタマイズ可能なオブジェクト名 [!UICONTROL レイアウトテンプレート]

As a [!DNL Workfront] 管理者は、次のオブジェクトの名前をカスタマイズして、組織内の用語に合わせることができます。

* [!UICONTROL ポートフォリオ]
* [!UICONTROL プログラム]
* [!UICONTROL プロジェクト]
* [!UICONTROL タスク]
* [!UICONTROL イシュー]
* [!UICONTROL 目標]*
* [!UICONTROL 結果]*
* [!UICONTROL アクティビティ]*

  *[!UICONTROL 目標], [!UICONTROL 結果]、および [!UICONTROL アクティビティ] は、会社がを購入した場合にのみ使用できます [!DNL Workfront Goals]. 詳しくは、 [!DNL Workfront Goals]を参照してください。 [[!DNL Adobe Workfront Goals] 概要](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL イニシアチブ]**
* [!UICONTROL シナリオ]**
* [!UICONTROL 計画]**

  **[!UICONTROL イニシアチブ], [!UICONTROL シナリオ]、および [!UICONTROL プラン] は、会社が [!DNL Workfront Scenario Planner]. 詳しくは、 [!DNL Scenario Planner]を参照してください。 [の基本を学ぶ [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


例えば、組織の作業量が多い場合に「エンゲージメント」と呼ばれる場合は、「 」という名前に置き換えることができます[!UICONTROL プロジェクト]&#39;が&#39;エンゲージメント&#39;を持っています。 お使いの [!DNL Workfront] インターフェイスには、「 」ではなく「Engagement」と表示されます[!UICONTROL プロジェクト]&#39;名前&#39;[!UICONTROL プロジェクト]&#39;が表示されます。

を使用してオブジェクト名をカスタマイズする方法の詳細  [!UICONTROL レイアウトテンプレート]を参照してください。 [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Workfrontの他のオブジェクトの名前はカスタマイズできません。 のオブジェクトの完全なリスト [!DNL Workfront]を参照し、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

オブジェクトの名前をカスタマイズすると、そのオブジェクトの新しい名前が [!DNL Workfront] そのオブジェクト名が表示されるアプリケーション。

### 領域： [!DNL Workfront] カスタマイズされたオブジェクト名を反映した

次の領域に、更新されたオブジェクト名を示します。

* トップ ナビゲーション
* 左パネルナビゲーションのすべてのセクション
* すべてのメニュー
* アプリ内通知
* Report Builder とレポートの要素（表示、フィルターおよびグループ化）
* [!UICONTROL 保存] ボタン
* 書き出されたファイル
* メール
* モバイルアプリ

### 領域： [!DNL Workfront] カスタマイズされたオブジェクト名を反映していない

以下の領域では、更新されたオブジェクトの名前は表示されません。

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] アドイン

### オブジェクト名のカスタマイズの影響

でオブジェクト名をカスタマイズする場合は、次の点に注意してください。 [!DNL Workfront]:

* システム表示で、スタイルや文法上の誤りが発生する場合があります。 例えば、「[!UICONTROL 問題]&#39;を&#39;Request&#39;に変更した場合、システム内のどこかに「An request」というフレーズが表示されますが、これは意図したとおりに機能しており、バグと見なされません。
* オブジェクトのカスタム名は翻訳できません。 次の項目のみ [!DNL Workfront] デフォルトの名前は、サポートされている言語で翻訳できます。 でサポートされる言語の詳細 [!DNL Workfront]を参照してください。 [でサポートされている言語 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). カスタムオブジェクト名フィールドは外部文字をサポートしているので、任意の言語で用語を入力できます。
* を使用してオブジェクト名をカスタマイズする場合  [!UICONTROL レイアウトテンプレート]を割り当てる場合は、  [!UICONTROL レイアウトテンプレート] ( ビジネスユニット（チームまたはグループ）に対して )\
   混乱を避けるために、これらのビジネスユニットのユーザーが明確に理解できる名前を使用することをお勧めします。
* 電子メール通知と配信レポートには、常に、  [!UICONTROL レイアウトテンプレート] 電子メールを生成するユーザーの ユーザーが他のチームやグループのユーザーから電子メール通知を受け取った場合、ユーザーのグループやチームに関連しないオブジェクト名を電子メールで確認する準備が整います。\
   As a [!DNL Workfront] 管理者は、各オブジェクトに関連付けられたアイコンをユーザーに通知します。 アイコンは、データベースに表示される様々なオブジェクト名とデフォルトのオブジェクトとの一貫性を保ちます。 すべての [!DNL Workfront] オブジェクトに関連付けられたアイコン： [オブジェクトアイコン](#object-icons).

  >[!TIP]
  >
  >組織での一般的なタスクについては、用語を反映したカスタムドキュメントの作成を検討してください。

## オブジェクトアイコン

The [!DNL Workfront] ドキュメントでは、常にオブジェクトのデフォルト名を参照します。 オブジェクトの名前がカスタマイズされている場合は、関連付けられたアイコンを使用して、どのカスタマイズされたオブジェクトがどのオブジェクトに対応するかを把握できます [!DNL Workfront] デフォルトのオブジェクト。

でカスタマイズされた名前を持つオブジェクトの詳細については、 [!DNL Workfront]を参照してください。 [を使用してカスタマイズ可能なオブジェクト名  [!UICONTROL レイアウトテンプレート]](#object-names-that-can-be-customized-using-a-layout-template).

次に、Workfrontのオブジェクトと対応するアイコンのリストを示します。

| **オブジェクト** | **アイコン** | **カスタマイズ可能なオブジェクト名** |
|---|---|---|
| [!UICONTROL 会社] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL ダッシュボード] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 目標] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL グループ] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL イシュー] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 担当業務] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 計画] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL ポートフォリオ] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL プログラム] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL プロジェクト] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL レポート] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL タスク] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL チーム] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL テンプレート] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## オブジェクトの参照番号

で作成された各オブジェクト [!DNL Workfront] は一意の参照番号を割り当てられます。 参照番号は、同じ名前のタスクなど、他の類似した 2 つのオブジェクトを区別する場合に便利です。 参照番号を使用してオブジェクトを検索し、レポートに参照番号を含めることができます。

参照番号を使用してオブジェクトを検索する方法については、 [オブジェクトの参照数を使用](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## オブジェクト固有の検索

で検索可能なすべてのオブジェクトを検索できます。 [!DNL Workfront]または、基本検索と詳細検索で、検索する特定のオブジェクトを選択することもできます。

すべてのオブジェクトがで検索可能とは限りません。 [!DNL Workfront]. で以下のオブジェクトに対して、基本検索と詳細検索を実行できます。 [!DNL Workfront]:

| **オブジェクト** | **基本検索** | **詳細検索** |
|---|---|---|
| [!UICONTROL プロジェクト] | ✓ | ✓ |
| [!UICONTROL タスク] | ✓ | ✓ |
| [!UICONTROL 問題] | ✓ | ✓ |
| [!UICONTROL レポート] | ✓ | ✓ |
| [!UICONTROL ユーザー] | ✓ | ✓ |
| [!UICONTROL テンプレート] | ✓ | ✓ |
| [!UICONTROL ドキュメント] | ✓ | ✓ |
| [!UICONTROL ポートフォリオ] | ✓ | ✓ |
| [!UICONTROL プログラム] | ✓ | ✓ |
| [!UICONTROL ダッシュボード] | ✓ | ✓ |
| [!UICONTROL 会社] | ✓ | ✓ |
| [!UICONTROL メモ] ( または [!UICONTROL 更新]) | ✓ |  |

での基本検索と詳細検索の実行に関する詳細 [!DNL Workfront]を参照してください。 [検索 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## オブジェクトに関するレポート

オブジェクトの階層と相互依存関係を理解することは、 [!DNL Workfront]. レポートはオブジェクト固有です。 必要なデータを表示する前に、レポートに適したオブジェクトを選択する必要があります。

レポートに対して選択したオブジェクトに応じて、レポートのオブジェクトに直接リンクされているオブジェクトにのみアクセスできます。

>[!IMPORTANT]
>
>選択したオブジェクトと同じレポート内の親オブジェクトについてのみレポートできます。 親オブジェクトレポートの子オブジェクトに関する情報を持つことはできません。 たとえば、プロジェクト情報はタスクレポートには表示できますが、プロジェクトレポートには表示できません。

オープン API を使用して、データベース内のすべてのオブジェクトに関するレポートを作成できます。 データベース内のすべてのオブジェクトの完全なリストについては、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>レイアウトテンプレートを使用してオブジェクトの名前をカスタマイズした場合は、Report Builder のオブジェクト名もカスタマイズされています。 カスタマイズされたオブジェクトがわかっていることと、Report Builder でカスタマイズされた名前を探すことができます。 でカスタマイズされた名前を持つオブジェクトの詳細については、 [!DNL Workfront]を参照してください。 *[を使用してカスタマイズ可能なオブジェクト名  [!UICONTROL レイアウトテンプレート]](#object-names-that-can-be-customized-using-a-layout-template).*
>レポートでテキストモードを使用する場合、テキストモードの式で使用されるオブジェクトの名前は、 [!DNL Workfront]カスタマイズされたオブジェクト名ではありません。 レポートでのテキストモードの使用について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
API について詳しくは、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

Report Builder を使用する際に、 [!DNL Workfront] web アプリケーション：

* [!UICONTROL プロジェクト]
* [!UICONTROL タスク]
* [!UICONTROL 時間]
* [!UICONTROL イシュー]
* [!UICONTROL ユーザー]
* [!UICONTROL アクセスレベル]
* [!UICONTROL 承認]
* [!UICONTROL 承認プロセス]
* [!UICONTROL 割り当て]
<!--this is no longer available: * [!UICONTROL Backlog Work Item]\
   Displays tasks or issues on the agile backlog. For more information about the agile backlog, see [Manage the agile backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).-->

* [!UICONTROL ベースライン]
* [!UICONTROL ベースライン タスク]
* [!UICONTROL 請求記録]
* [!UICONTROL 予算計上時間数]

  これが [!UICONTROL 予算時間]( 従来の非推奨（廃止予定）のリソース管理ツールで表示される )

  「バド。 Hours」フィールド ( [!UICONTROL 予算時間] レポートは、 [!UICONTROL リソースプランナー]. 詳しくは、 [理解 [!UICONTROL 予算労務費] および [!UICONTROL 予算時間] プロジェクトの場合](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL カレンダー イベント]
* [!UICONTROL 会社]
* [!UICONTROL カスタムフォーム]
* [!UICONTROL ダッシュボード]
* [!UICONTROL ドキュメント]
* [!UICONTROL ドキュメントの承認]
* [!UICONTROL ドキュメント バージョン]\
   ドキュメントのバージョン、バージョンが関連付けられているドキュメント、バージョンの作成者、およびドキュメントのバージョンに対して配達確認を作成したユーザー（存在する場合）に関する情報を表示できます。
* [!UICONTROL メールテンプレート]
* [!UICONTROL 費用]
* [!UICONTROL 費用タイプ]
* [!UICONTROL 外部ページ]
* [!UICONTROL お気に入り]
* [!UICONTROL フィルター]
* [!UICONTROL 目標]

  戦略目標のレポートを作成したり、プロジェクトが目標アクティビティとして目標に関連付けられている場合に、目標関連情報をプロジェクトレポートに表示したりできます。 組織が [!DNL Workfront Goals] ライセンス。 詳しくは、 [!DNL Workfront Goals]を参照してください。 [[!DNL Workfront Goals] 概要](../../../workfront-goals/goal-management/wf-goals-overview.md). プロジェクトを戦略目標に接続する方法については、 [Adobe Workfront目標の目標へのプロジェクトの追加](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

  >[!TIP]
  >
  >に関連付けられたプロジェクト目標についてはレポートできません。 [!UICONTROL ビジネス事例]. プロジェクト目標と戦略目標の詳細については、 [用語集 [!DNL Adobe Workfront] 用語](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL グループ]
* [!UICONTROL グループ化]
* [!UICONTROL 時間タイプ]
* [!UICONTROL イニシアチブ]

  企業が [!DNL Workfront Scenario Planner] ライセンス。 イニシアチブについて詳しくは、 [以下の取り組みの概要 [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).


* イニシアティブの担当業務

  企業が [!DNL Workfront Scenario Planner] ライセンス。 イニシアチブの作成とジョブの役割との関連付けについて詳しくは、 [のイニシアチブを作成および編集します。 [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).


* [!UICONTROL 反復]
* [!UICONTROL 担当業務]
* [!UICONTROL ジャーナル エントリ]

  追跡されたシステム更新については、 [!UICONTROL 更新] タスク、プロジェクト、問題などのオブジェクトの領域 詳しくは、 [レポート [!UICONTROL 更新] 領域](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL レイアウトテンプレート]
* [!UICONTROL マイルストーン]
* [!UICONTROL マイルストーン パス]
* [!UICONTROL 注意] または [!UICONTROL 更新]

  >[!NOTE]
  >
  >個々のユーザーが追加したコメントに関するレポートを作成できます。

* [!UICONTROL パラメーター] ( または [!UICONTROL カスタムフィールド])
* [!UICONTROL パラメータグループ] ( または [!UICONTROL 断面分割])
  <!--this is no longer in the UI: * [!UICONTROL Portal Profile] (this displays information that has been deprecated)-->
* [!UICONTROL ポートフォリオ]
* [!UICONTROL プログラム]
* [!UICONTROL プロジェクト] ([!UICONTROL 財務データ])

  >[!NOTE]
  >
  >財務情報が [!UICONTROL プロジェクト] ([!UICONTROL 財務データ]) は、そのレポートに関連付けられているデータが 5 歳未満の場合にのみ表示されます。 例えば、ジョブの役割が 2015 年 1 月にタスクに割り当てられ、今日が 2021 年 9 月の場合、 [!UICONTROL 配分日] ( ジョブの役割が [!UICONTROL プロジェクト（財務データ）] レポート。

* [!UICONTROL プルーフの承認]\
   配達確認の承認に関する様々な情報 ( 承認用に送信された配達確認、 [!UICONTROL 承認者]，請求者に関する情報 ( 請求者がライセンスを受けた場合 [!DNL Workfront] ユーザー )、バージョン情報、配達確認 ID および配達確認の作成日です。\
   [!UICONTROL 配達確認の承認] レポートには、ユーザーの自分の作業領域で、まだ決定がおこなわれていない配達確認のみが含まれます。\
   配達確認の承認は、 [!DNL Workfront] 説明に従って [配達確認にユーザーを追加](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [内で配達確認を共有 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL キュー]
* [!UICONTROL キュー トピック]
* [!UICONTROL 率] （これはジョブの役割を表示します） [!UICONTROL 請求率] 情報 )
* [!UICONTROL リマインダ通知]
* [!UICONTROL レポート]
* [!UICONTROL リソース プール]
* [!UICONTROL 危険]
* [!UICONTROL 危険タイプ]
* [!UICONTROL スケジュール]
* [!UICONTROL スコアカード]
* [!UICONTROL チーム]
* [!UICONTROL テンプレート]
* [!UICONTROL テンプレート タスク]
* [!UICONTROL 休暇]

  ユーザーのプロファイル内でユーザーが示したように、ユーザーの休日をレポートできます。

* [!UICONTROL タイムシート]
* [!UICONTROL 定期タイムシート]
* [!UICONTROL トピック グループ]
* [!UICONTROL ユーザーによる承認]
* [!UICONTROL ユーザーの委任]

  不在時に他のユーザーのタスクや問題を実行するために委任されたユーザーについてレポートできます。 このレポートには、不在のユーザーと不在の間に職務を遂行するユーザーが表示されます。

* [!UICONTROL ユーザーの決定]

  今月にユーザーが配達確認およびドキュメントに対しておこなった決定の数をレポートできます。

* [!UICONTROL ビュー]
* [!UICONTROL 作業項目] （これにより、タスクと問題に関するレポートが生成されます）
