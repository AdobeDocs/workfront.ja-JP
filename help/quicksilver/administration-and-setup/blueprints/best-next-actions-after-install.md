---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: ブループリントのインストール後に実行するアクション
description: この記事では、 [!DNL Adobe Workfront] にブループリントをインストールした後でシステムのユーザーにブループリントを完全にデプロイするために必要なことについて、概要を説明します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: ht
source-wordcount: '1139'
ht-degree: 100%

---

# ブループリントのインストール後に実行するアクション

この記事では、[!DNL Adobe Workfront]にブループリントをインストールした後でシステムのユーザーにブループリントを完全にデプロイするために必要なことについて、概要を説明します。

* [プロジェクトテンプレートの推奨事項](#project-template-recommendations)
* [組織構造の推奨事項](#organizational-structure-recommendations)
* [ダッシュボードの推奨事項](#dashboard-recommendations)

## プロジェクトテンプレートの推奨事項 {#project-template-recommendations}

この節では、ブループリントと共にインストールされるプロジェクトテンプレートの推奨事項について説明します。

### 新しく作成された役割とチームへのユーザーの割り当て {#assign-users-to-newly-created-roles-and-teams}

ブループリントのインストールプロセス中に作成された役割やチームには、ユーザーが自動的には関連付けられていません。新しく追加された役割やチームにユーザーを割り当てないと、誰も引き受けない機能の作業を作成することになります。場合によっては、これらの役割とチームを担うために新しいユーザーを作成する必要があります。新しいユーザーの作成については、[ユーザーの追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

### テンプレートとテンプレートタスクへのカスタムフォームの適用 {#apply-a-custom-form-to-the-template-and-the-template-tasks}

インストールプロセスでは、プロジェクトテンプレートはどのカスタムフォームにも関連付けられません。プロジェクトまたはタスクで、レポートの一貫性を保つために特定のフォームまたはフィールドに値を入力する必要がある場合や、プロジェクトレベルで保持する必要があるフィールドがデジタルリクエストフォームに含まれている場合は、テンプレートまたはテンプレートタスクをそれらのフィールドに関連付けることをお勧めします。詳しくは、[オブジェクトへのカスタムフォームの追加](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。

### テンプレートタスク期間と作業量見積もりの更新 {#update-template-task-duration-and-effort-estimates}

テンプレート内のすべてのタスクには、予定期間と計画作業量見積もりが含まれています。これらの見積もりは、これらのアクティビティに費やされる期間や時間の出発点となります。ただし、組織の能力、スキルおよびペースはそれぞれ異なります。各タスクの期間と作業量の見積もりをレビューして、組織のニーズを反映するように調整してください。詳しくは、[「[!UICONTROL タスク詳細の概要]」エリアでのタスク情報の管理](../../manage-work/tasks/manage-tasks/task-information-in-overview.md)を参照してください。

### マイルストーンパスとマイルストーンの関連付け {#associate-a-milestone-path-and-milestones}

インストールプロセスでは、プロジェクトテンプレートとマイルストーンパスは関連付けられません。マイルストーンパスをテンプレートに適用し、テンプレート内の主要なタスクにマイルストーンを適用して、マイルストーンレポートのニーズをサポートします。詳しくは、[マイルストーンとタスクの関連付け](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)を参照してください。

### チームへのテンプレートのロールアウト {#roll-out-the-template-to-your-team}

このテンプレートを使用する作業管理者と、プロジェクトテンプレート内の作業を実行する個々の参加者の両方を対象にトレーニング資料を準備します。

### レポートとダッシュボードの作成または更新 {#create-or-update-reports-and-dashboards}

ソリューションが、組織がこれまでに [!DNL Workfront] で実行したことのない新しいタイプの作業を表している場合は、その作業をサポートするための新しいレポートとダッシュボードを作成する必要がある可能性があります。詳しくは、[カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)と[ダッシュボードの作成](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)を参照してください。

ソリューションが [!DNL Workfront] で既に実行している作業と類似している場合は、その作業が既存のレポートとダッシュボードに想定どおりに反映されることを確認してください。既存のレポートに反映されない場合は、フィルターを更新するか新しいレポートを作成するためのアクションを実行してください。

## 組織構造の推奨事項 {#organizational-structure-recommendations}

この節では、ブループリントと共にインストールされる組織構造要素の推奨事項について説明します。

### 会社

会社を含むブループリントをインストールした後、以下を実行します。

* カスタムフォームを追加して、会社レコードを有益な詳細情報で拡充します（フォームとその詳細はそれぞれのケースで異なります）。詳しくは、[オブジェクトへのカスタムフォームの追加](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。
* 会社がクライアントを表している場合は、その会社に関連付けられている上書き率をレビューします。詳しくは、[会社レベルでの担当業務請求料率の上書き](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)を参照してください。
* 会社がクライアントを表しており、その組織に固有のプロジェクトテンプレートが他にもある場合は、まずそのプロジェクトテンプレートを新しく追加した会社に事前に関連付けます。詳しくは、[プロジェクトテンプレートの編集](../../manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。
* 会社がクライアントまたはベンダーを表している場合は、既に環境内に存在する可能性がある外部組織の既存ユーザーを関連付けます。詳しくは、[会社の作成と編集](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)を参照してください。
* 会社がクライアントまたはベンダーを表している場合は、コミュニケーション、作業の実行および承認を効率化するために環境で必要になる可能性がある外部組織の追加の共同作業者ユーザーを作成します。新しいユーザーの作成については、[ユーザーの追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。
* 新しく追加された会社に関連付けられたユーザーの組織図における関係を更新します。詳細については、[ダイレクトレポートを作成する](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md)および[組織図を表示する](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md)を参照してください。

会社について詳しくは、[会社を作成および編集](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)を参照してください。

## ダッシュボードの推奨事項 {#dashboard-recommendations}

この節は、ブループリントとともにインストールされるダッシュボードとレポートに関する推奨事項を含みます。

### 新しく作成したダッシュボードを更新して、レポートを追加または削除します。

ブループリントから追加されたダッシュボードには、1 つ以上のレポート、外部ページ、またはカレンダーがあります。他のユーザーと共有する前に、すべてのレポートやその他のダッシュボード要素が必要にならない場合や、既存のレポート、外部ページ、カレンダーをダッシュボードを拡張する必要があります。詳しくは、[ダッシュボードへのレポートの追加](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)を参照してください。

### 新しく作成したレポートを更新して、列やフィルター条件を追加または削除します。

ダッシュボードのブループリントを通じて配信されるレポートには、[!DNL Workfront] の設定をサポートするすべての列またはフィルター条件が含まれていません。基準内に収まるようにレポートをいくつか調整することが予想されます。環境内の他のレポートとの一貫性を保つために、リストされるオブジェクトのすべてのレポートに含める列を追加したり、特定のプロジェクトタイプまたはユーザーグループに結果を制限するフィルター条件を追加したりすることができます。詳しくは、[ビューの作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)および[フィルターの作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

### ダッシュボードまたはレポートをユーザーと共有する

レイアウトテンプレートにダッシュボードを配置しない場合は、そのダッシュボードを役に立つユーザーと共有する必要があります。詳しくは、[ダッシュボードの共有](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)および[レポートの共有](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)を参照してください。

### ダッシュボードをレイアウトテンプレートに追加する

他のユーザーが情報を利用できるようにする最善の方法は、ダッシュボードをレイアウトテンプレートに追加することです。ダッシュボードを定期的に確認して、最もメリットがあるユーザーのレイアウトテンプレートを特定し、そのレイアウトテンプレートに新しく作成したダッシュボードを追加します。詳しくは、[レイアウトテンプレートを作成および管理](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

### 他のダッシュボードとレポートを更新する

新しいダッシュボードとそのレポートが導入されると、他の既存のダッシュボードとレポートを廃止して調整できる場合があります。時間をかけて既存のレポートを確認し、冗長なレポートと矛盾するレポートを特定します。

### 関連するフォームにカスタムデータを配布する

ダッシュボードのブループリントに含まれる一部のレポートには、レポートの表示、フィルター、またはグループ化のカスタムデータフィールドがあります。場合によっては、ブループリントには、これらのフィールドが関連付けられたフォームも含まれます。ただし、多くの場合、カスタムフィールドはカスタムフォームに適用されません。列、フィルター、またはグループが正しく機能するには、これらのフィールドは、ユーザー、プロジェクト、タスク、またはその他のオブジェクトレコードに接続されているフォームに関連付ける必要があります。詳しくは、[カスタムフォームにカスタムフィールドを追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)を参照してください。
