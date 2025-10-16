---
product-area: projects
navigation-topic: create-projects
title: プロジェクトを作成
description: プロジェクトは、Adobe Workfront における作業の大きな単位です。プロジェクトは最初から作成するだけでなく、テンプレートを使用したり、イシューやタスクからプロジェクトに変換したりすることもできます。
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 91%

---

# プロジェクトを作成

<!--remove Preview and Production references-->

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

プロジェクトは、Adobe Workfront で行う必要がある大量の作業を表します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
        <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトを作成すると、そのプロジェクトに対する管理権限が自動的に付与されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project, you automatically receive Manage permissions to the project.</p> </td> 
  </tr> 
 </tbody> 
</table>-->


## プロジェクトの作成方法

Workfront でプロジェクトを作成するには、次のような方法があります。

* テンプレートを使用せずに、プロジェクトを最初から作成します。この記事では、プロジェクトを最初から作成する方法について説明します。

* 既存のプロジェクトのコピー。\
  プロジェクトのコピーについて詳しくは、 [プロジェクトをコピー](../../../manage-work/projects/manage-projects/copy-project.md)を参照してください。

* テンプレートを使用します。\
  テンプレートを使用して新しいプロジェクトを作成する方法について詳しくは、[テンプレートを使用してプロジェクトを作成](../../../manage-work/projects/create-projects/create-project-from-template.md)を参照してください。

* Microsoft Project からプロジェクトを読み込みます。\
  Microsoft Project からプロジェクトを読み込む方法について詳しくは、[Microsoft Project からプロジェクトを読み込む](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)を参照してください。

* キックスタートを使用してプロジェクトを読み込みます。

  Workfront の管理者は、キックスタートを使用してプロジェクトを読み込むことができます。

  Workfront でのキックスタートを使用したデータの読み込みについて詳しくは、[キックスタートテンプレートを使用して Adobe Workfront にデータを読み込む](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)を参照してください。

  キックスタートを使用したプロジェクトの読み込みについて詳しくは、[キックスタートシナリオ：シンプルなプロジェクトおよびタスクの読み込みの準備](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md)を参照してください。

* Adobe Workfront シナリオプランナーのシナリオからイニシアチブを公開します。

  Workfront のシナリオプランナーについて詳しくは、[シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。

  公開したイニシアチブからプロジェクトを作成する方法について詳しくは、[シナリオプランナでイニシアチブを公開してプロジェクトを更新または作成する](../../../scenario-planner/publish-scenarios-update-projects.md)を参照してください。

* Workfront Planning のレコードタイプからプロジェクトを接続するときに追加します。

  Workfront Planning へのアクセスについて詳しくは、[ アクセスの概要 ](/help/quicksilver/planning/access/access-overview.md) を参照してください。

  レコードにプロジェクトを追加して作成する方法の詳細については、「レコードに接続する際にWorkfront Planning からWorkfront オブジェクトを作成する [ の「Workfront Planning からレコードにプロジェクトを接続する場合のプロジェクトの作成」を参照してください ](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)

## 前提条件

開始する前に、次の点を確認する必要があります。

* システム管理者またはグループ管理者が、設定エリアで「テンプレートを使用しないプロジェクトの作成をユーザーに許可」環境設定を有効にしました。

  詳しくは、[システム全体のプロジェクト環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

## 新しいプロジェクトのデフォルト設定

プロジェクトを作成すると、Workfront では一連のデフォルト設定がプロジェクトに適用されます。例えば、プロジェクトを作成すると、ステータス、グループ、スケジュールモードがプリセットされています。

次の点に注意してください。

* Workfront 管理者またはグループ管理者は、Workfront 全体のインスタンスやあるグループのプロジェクト環境設定を行う際に、新しいプロジェクトのデフォルト設定を指定できます。
* Workfront では、グループの設定があれば、Workfront 管理者が指定した設定よりも優先して適用します。
* 新しいプロジェクトのデフォルトステータスは、メインのプロジェクト環境設定エリアで Workfront 管理者が定義したステータス、またはグループのプロジェクト環境設定エリアでグループ管理者（または Workfront 管理者）が定義したステータスに対応します。

  >[!NOTE]
  >
  >新規プロジェクトのデフォルトステータスは、計画中に設定することをお勧めします。これで、新しいプロジェクトに変更を加えても、そのプロジェクトに割り当てられているユーザーに通知が送信されなくなります。
  >
  >新しいプロジェクトのデフォルトステータスおよびその他のデフォルト設定の指定の詳細については、[システム全体のプロジェクト環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)または[グループのプロジェクト環境設定を指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)を参照してください。

* Workfront で新しいプロジェクトのグループとステータスを定義する方法については、次のシナリオが存在します。

   * プロジェクトを最初から作成する場合は、プロジェクトのグループがホームグループになります。

     プロジェクトのステータスは、ホームグループ（存在する場合）または Workfront インスタンスのプロジェクト環境設定のデフォルトステータスになります。プロジェクトの作成時のデフォルトステータスは、プロジェクトのグループで使用可能な任意のステータスに変更できます。

   * テンプレートを使用してプロジェクトを作成する場合は、テンプレートの設定が、Workfront 管理者またはグループ管理者が指定した設定よりも優先されます。

     新しいプロジェクトのグループは、テンプレートのグループです。テンプレートがグループに関連付けられていない場合、プロジェクトのグループは、プロジェクトを作成したユーザーのホームグループになります。

     テンプレートから作成された新しいプロジェクトのデフォルトステータスは、メインのプロジェクト環境設定エリアで Workfront 管理者が定義したステータス、またはグループのプロジェクト環境設定エリアでグループ管理者（または Workfront 管理者）が定義したステータスに対応します。テンプレートからプロジェクトを作成する際のデフォルトのステータスは、テンプレートのグループまたはプロジェクトを作成するユーザーのホームグループであるプロジェクトのグループのステータスのいずれかに変更できます。

   * イシューを変換してプロジェクトを作成する場合、新しいプロジェクトのグループは、イシューの既存のプロジェクトのグループになります。イシューを変換するユーザーがイシューのプロジェクトにアクセスできない場合、またはイシューのプロジェクトにグループがない場合は、イシューを変換するユーザーのホームグループが新しいプロジェクトのグループになります。

     新しいプロジェクトのステータスは、元のプロジェクトのグループ、またはイシューを変換するユーザーのホームグループである、プロジェクトに関連付けられたグループのグループステータスと一致します。

     イシューを変換してプロジェクトを作成する際にテンプレートを使用している場合は、上記の 2 つ目のシナリオを参照して、新しいプロジェクトに適用されるグループと Workfront のステータスを把握してください。

## ゼロからのプロジェクトの作成

>[!NOTE]
>
>テンプレートを使用してプロジェクトを作成する場合は、[テンプレートを使用したプロジェクトの作成](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)の記事もご覧になることをお勧めします。

1. 次のいずれかの操作を行います。

   * Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png)（利用可能な場合）、または左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックします。「**プロジェクト**」をクリックして、**新規プロジェクト**&#x200B;を展開します。
   * ポートフォリオに移動し、**新規プロジェクト**&#x200B;を展開します。
   * プログラムに移動し、「**新規プロジェクト**」を展開します。
   * グループ管理者の場合は、管理するグループの「プロジェクト」セクションでプロジェクトを作成することもできます。詳しくは、[グループのプロジェクトの作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)を参照してください。

   ![新規プロジェクトメニュー](assets/new-project-dropdown-nwe-350x358.png)

1. プロジェクトを最初から作成する場合、「**新規プロジェクト**」をクリックします。
1. プロジェクトの名前を入力します。Enter キーを押して名前を保存します。

   ![プロジェクトの名前を入力](assets/rename-untitled-project.png)

   プロジェクトページのヘッダーには、プロジェクトの現在の正常性と進行状況の概要がすばやく表示されます。プロジェクトの情報が更新されると、プロジェクトのヘッダーの情報が変更されます。

1. 「**タスクを追加**」をクリックします。

   または

   「**新規タスク**」をクリックして、プロジェクトにタスクを追加し、リソースを割り当てます。

   プロジェクトへのタスクの追加について詳しくは、[プロジェクトにタスクを作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)を参照してください。

1. プロジェクト名の横にある **詳細** メニューをクリックし、**編集** ![ 編集アイコン ](assets/qs-edit-icon.png) をクリックして、プロジェクト詳細を編集します。

   **プロジェクトを編集**&#x200B;ダイアログボックスが開きます。

   プロジェクトの編集について詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

1. （オプション）プロジェクトの設定を行い、タスクを追加すると、プロジェクトのステータスを「**現在**」に変更できます。

   これは、プロジェクトを開始する準備が整い、タスクに割り当てられたユーザーが、プロジェクトで作業を開始できる状態になったことを示します。

   プロジェクトのステータスについて詳しくは、[システムプロジェクトステータスのリストにアクセス](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)を参照してください。
