---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: ブループリントのインストール後に実行するアクション
description: この記事では、 [!DNL Adobe Workfront] ブループリントをシステムユーザーに完全にデプロイする場合。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# ブループリントのインストール後に実行するアクション

この記事では、 [!DNL Adobe Workfront] ブループリントをシステムユーザーに完全にデプロイする場合。

* [プロジェクトテンプレートの推奨事項](#project-template-recommendations)
* [組織構造の推奨事項](#organizational-structure-recommendations)
* [ダッシュボードの推奨事項](#dashboard-recommendations)

## プロジェクトテンプレートの推奨事項 {#project-template-recommendations}

この節では、ブループリントと共にインストールされるプロジェクトテンプレートに関する推奨事項を示します。

### 新しく作成した役割およびチームにユーザーを割り当て {#assign-users-to-newly-created-roles-and-teams}

ブループリントのインストールプロセス中に作成されたロールやチームには、ユーザーが自動的に関連付けられていません。 新しく追加した役割やチームにユーザーを割り当てずに、誰も受け取らない機能の作業を作成します。 場合によっては、これらの役割やチームに入力するために新しいユーザーを作成する必要があります。 新しいユーザーの作成について詳しくは、 [ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### テンプレートとテンプレートタスクにカスタムフォームを適用する {#apply-a-custom-form-to-the-template-and-the-template-tasks}

インストールプロセスでは、プロジェクトテンプレートをカスタムフォームに関連付けることはできません。 レポートの一貫性を確保するために、プロジェクトやタスクで特定のフォームやフィールドを設定する必要がある場合、またはデジタルリクエストフォームに、プロジェクトレベルで保持する必要があるフィールドが含まれる場合は、テンプレートやテンプレートタスクを関連付けます。 詳しくは、 [オブジェクトへのカスタムフォームの追加](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### テンプレートタスクの期間と労力の見積もりを更新 {#update-template-task-duration-and-effort-estimates}

テンプレート内の各タスクには、計画期間と計画作業量の見積もりが含まれます。 これらの見積もりは、これらのアクティビティの期間と滞在時間の出発点となります。 ただし、組織の能力、スキル、ペースは独自のものです。 各タスクの推定期間と労力を確認し、組織のニーズに合わせて調整する必要があります。 詳しくは、 [でタスク情報を管理 [!UICONTROL タスクの詳細の概要] 領域](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### マイルストーンパスとマイルストーンの関連付け {#associate-a-milestone-path-and-milestones}

インストールプロセスでは、プロジェクトテンプレートとマイルストーンパスが関連付けられません。 マイルストーンレポートのニーズに応じて、テンプレートにマイルストーンパスを適用し、テンプレート内の主要タスクにマイルストーンを適用します。 詳しくは、 [タスクへのマイルストーンの関連付け](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### テンプレートをチームに展開 {#roll-out-the-template-to-your-team}

このテンプレートを使用する作業管理者と、プロジェクトテンプレート内で作業を実行する個々のコントリビューターの両方に対して、トレーニング資料を準備します。

### レポートとダッシュボードを作成または更新 {#create-or-update-reports-and-dashboards}

ソリューションが、組織が以前に実行したことのない新しいタイプの作業を表す場合 [!DNL Workfront]を使用する場合、作業をサポートするために、新しいレポートやダッシュボードを作成する必要が生じる場合があります。 詳しくは、 [カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) および [ダッシュボードの作成](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

ソリューションがで既に実行している動作と似ている場合 [!DNL Workfront]作業が既存のレポートやダッシュボードに期待どおりに送信されていることを確認する必要があります。 既存のレポートにフィードしない場合は、フィルターを更新するか新しいレポートを作成するためのアクションを実行します。

## 組織構造の推奨事項 {#organizational-structure-recommendations}

この節では、ブループリントと共にインストールされる組織構造要素に関する推奨事項を示します。

### 会社

会社を含むブループリントをインストールした後：

* カスタムフォームを追加して、会社のレコードに有用な詳細情報を追加します（フォームとその詳細はユーザー独自です）。 詳しくは、 [オブジェクトへのカスタムフォームの追加](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* 会社がクライアントを表す場合は、会社に関連する上書き率を確認します。 詳しくは、 [会社レベルでのジョブロール請求率の上書き](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* 会社がクライアントを表し、その組織に固有のプロジェクトテンプレートが他にある場合は、最初にプロジェクトテンプレートを新しく追加した会社に事前に関連付けます。 詳しくは、 [プロジェクトテンプレートの編集](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* 会社がクライアントまたはベンダーを代表する場合は、既にお客様の環境にある可能性のある外部組織の既存のユーザーを関連付けます。 詳しくは、 [会社の作成と編集](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* 会社がクライアントまたはベンダーを代表する場合は、環境内で必要になる外部組織のコラボレータユーザーを追加作成して、通信、作業実行、承認を合理化します。 新しいユーザーの作成について詳しくは、 [ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* 新しく追加された会社に関連付けられたユーザーの組織図の関係を更新します。 詳しくは、 [ダイレクトレポートの作成](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) および [組織図を表示](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

会社について詳しくは、 [会社の作成と編集](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## ダッシュボードの推奨事項 {#dashboard-recommendations}

この節では、ブループリントと共にインストールされるダッシュボードとレポートに関する推奨事項を示します。

### 新しく作成したダッシュボードを更新して、レポートを追加または削除します。

ブループリントから追加されたダッシュボードには、1 つ以上のレポート、外部ページ、またはカレンダーがあります。 他のユーザーと共有する前に、すべてのレポートやその他のダッシュボード要素が必要にならない場合や、既存のレポート、外部ページ、カレンダーをダッシュボードに追加する必要がある場合があります。 詳しくは、 [ダッシュボードへのレポートの追加](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### 新しく作成したレポートを更新して、列やフィルター条件を追加または削除します。

ダッシュボードのブループリントを通じて配信されるレポートには、の設定に対応するすべての列やフィルター条件がない [!DNL Workfront]. 標準に合わせてレポートを調整することが期待されます。 環境内の他のレポートとの一貫性を保つために、リストされるオブジェクトのすべてのレポートに含める列を追加したり、特定のプロジェクトタイプまたはユーザーグループに結果を制限するフィルタ条件を追加したりできます。 詳しくは、 [ビューの作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) および [フィルターを作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### ダッシュボードまたはレポートをユーザーと共有する

レイアウトテンプレートにダッシュボードを配置しない場合は、そのダッシュボードを役に立つユーザーと共有する必要があります。 詳しくは、 [ダッシュボードの共有](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) および [レポートの共有](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### ダッシュボードをレイアウトテンプレートに追加する

他のユーザーが情報を利用できるようにする最善の方法は、ダッシュボードをレイアウトテンプレートに追加することです。 ダッシュボードを定期的に確認して、最もメリットがあるユーザーのレイアウトテンプレートを特定し、そのレイアウトテンプレートに新しく作成したダッシュボードを追加します。 詳しくは、 [レイアウトテンプレートの作成と管理](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### 他のダッシュボードとレポートを更新する

新しいダッシュボードとそのレポートが導入されると、他の既存のダッシュボードとレポートを廃止して調整できる場合があります。 時間をかけて既存のレポートを確認し、冗長なレポートと矛盾するレポートを特定します。

### 関連するフォームにカスタムデータを配布する

ダッシュボードのブループリントに含まれる一部のレポートには、レポートの表示、フィルターまたはグループ化のカスタムデータフィールドがあります。 場合によっては、ブループリントに、これらのフィールドが関連付けられたフォームが含まれることがあります。 ただし、多くの場合、カスタムフィールドはカスタムフォームに適用されません。 列、フィルターまたはグループが正しく機能するには、これらのフィールドを、ユーザー、プロジェクト、タスクまたは他のオブジェクトレコードに接続されているフォームに関連付ける必要があります。 詳しくは、 [カスタムフォームにカスタムフィールドを追加する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
