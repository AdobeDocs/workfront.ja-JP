---
product-area: projects
navigation-topic: create-projects
title: プロジェクトの作成
description: プロジェクトは、Adobe Workfrontでの作業の大きな単位です。 プロジェクトは、ゼロから作成したり、テンプレートを使用したり、イシューやタスクをプロジェクトに変換したりできます。
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: 45c82f659d02dca69d2a2c390b084330773d4252
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 1%

---

# プロジェクトの作成

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

プロジェクトとは、Adobe Workfrontで行う必要のある大量の作業を表します。

## アクセス要件

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>新規プラン：標準</p>
        <p>または</p>
        <p>現在のプラン：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 プロジェクトへのアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">プロジェクトへのアクセス権の付与</a>. Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>プロジェクトを作成すると、そのプロジェクトに対する管理権限が自動的に付与されます。</p> <p> プロジェクト権限について詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfrontでプロジェクトを共有する</a>.</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトを作成する方法

次のいずれかの方法で、Workfrontでプロジェクトを作成できます。

* テンプレートを使用せずに、ゼロからプロジェクトを作成する。 この記事では、プロジェクトを最初から作成する方法について説明します。

* 既存のプロジェクトをコピーします。\
  プロジェクトのコピーの詳細については、「 [プロジェクトのコピー](../../../manage-work/projects/manage-projects/copy-project.md).

* テンプレートを使用します。\
  テンプレートを使用して新しいプロジェクトを作成する方法について詳しくは、 [テンプレートを使用したプロジェクトの作成](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Microsoft Project からプロジェクトを読み込みます。\
  MS Project からプロジェクトを読み込む方法について詳しくは、 [Microsoft Project からプロジェクトを読み込む](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* キックスタートを使用してプロジェクトを読み込みます。

  Workfrontの管理者は、キックスタートを使用してプロジェクトを読み込むことができます。

  Workfrontでのキックスタートを使用したデータのインポートについて詳しくは、 [キックスタートテンプレートを使用してAdobe Workfrontにデータを読み込む](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  キックスタートを使用したプロジェクトの読み込みについては、 [キック開始シナリオ：シンプルなプロジェクトおよびタスクのインポートの準備](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Adobe Workfrontシナリオプランナーのシナリオからイニシアチブを公開します。 シナリオ・プランナには、追加のライセンスが必要です。 Workfront Scenario Planner の詳細は、 [シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md). 公開イニシアチブからプロジェクトを作成する方法については、  [シナリオプランナーでイニシアチブを公開して、プロジェクトを更新または作成します](../../../scenario-planner/publish-scenarios-update-projects.md).

## 前提条件

開始する前に、次の点を確認する必要があります。

* システムまたはグループ管理者が、「セットアップ」領域で「テンプレートを使用せずにユーザーがプロジェクトを作成できるようにする」設定を有効にしました。

  詳しくは、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## 新しいプロジェクトの既定の設定

プロジェクトを作成する際、Workfrontはデフォルト設定のセットを適用します。 例えば、プロジェクトの作成時に、ステータス、グループ、スケジュールモードがあらかじめ設定されているとします。

次の点に注意してください。

* Workfront管理者またはグループ管理者は、Workfrontインスタンス全体またはグループのプロジェクト環境設定を行う際に、新しいプロジェクトのデフォルト設定を構成できます。
* Workfrontは、Workfront管理者が設定した設定を適用する前に、グループに設定がある場合は、そのグループの設定を適用します。
* 新しいプロジェクトのデフォルトのステータスは、主なプロジェクト環境設定領域のWorkfront管理者、またはグループの「プロジェクト環境設定」領域のグループ管理者 ( またはWorkfront管理者 ) が定義したステータスに対応します。

  >[!NOTE]
  >
  >新規プロジェクトのデフォルトのステータスは「計画」にすることをお勧めします。 新しいプロジェクトを変更する際に、プロジェクトに割り当てられたユーザーに通知が送信されないようにします。
  >
  >新規プロジェクトの既定の状態とその他の既定の設定の詳細については、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) または [グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* Workfrontが新しいプロジェクトのグループとステータスを定義する方法について、次のシナリオがあります。

   * プロジェクトをゼロから作成する場合、プロジェクトのグループはホームグループになります。

     プロジェクトのステータスは、ホームグループ（存在する場合）のプロジェクト環境設定のデフォルトのステータスです。または、Workfrontインスタンスのステータスです。 プロジェクトを作成する際のデフォルトのステータスは、プロジェクトのグループで使用できるステータスに変更できます。

   * テンプレートを使用してプロジェクトを作成する場合、テンプレートの設定が、Workfrontまたはグループ管理者が設定した設定よりも優先されます。

     新しいプロジェクトのグループは、テンプレートのグループです。 テンプレートがグループに関連付けられていない場合、プロジェクトのグループは、プロジェクトを作成するユーザーのホームグループになります。

     テンプレートから作成される新しいプロジェクトのデフォルトのステータスは、主な「プロジェクトの環境設定」領域のWorkfront管理者、またはグループの「プロジェクトの環境設定」領域のグループ管理者 ( またはWorkfront管理者 ) が定義したステータスに対応します。 テンプレートからプロジェクトを作成する際のデフォルトのステータスは、プロジェクトのグループ（テンプレートのグループ）またはプロジェクトを作成するユーザーのホームグループのいずれかのステータスに変更できます。

   * イシューを変換してプロジェクトを作成する場合、新しいプロジェクトのグループは、イシューの既存のプロジェクトのグループになります。 イシューを変換するユーザーがイシューのプロジェクトにアクセスできない場合、またはイシューのプロジェクトにグループがない場合、イシューを変換するユーザーのホームグループが新しいプロジェクトのグループになります。

     新しいプロジェクトのステータスは、プロジェクトに関連付けられたグループのグループステータスに一致します。グループステータスは、元のプロジェクトのグループ、またはイシューを変換するユーザーのホームグループです。

     問題を変換してプロジェクトを作成する際にテンプレートを使用している場合は、上記の 2 つ目のシナリオを参照して、新しいプロジェクトに適用されるグループとステータスWorkfrontを把握してください。

## ゼロからのプロジェクトの作成

1. 次のいずれかの操作を行います。

   * 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックします。 クリック **プロジェクト**&#x200B;を展開し、を展開します。 **新規プロジェクト**.
   * ポートフォリオに移動し、を展開します。 **新規プロジェクト**.
   * プログラムに移動し、を展開します。 **新規プロジェクト**.
   * グループ管理者は、管理するグループの「プロジェクト」セクションでプロジェクトを作成することもできます。 詳しくは、 [グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![新規プロジェクトメニュー](assets/new-project-dropdown-nwe-350x358.png)

1. クリック **新規プロジェクト** をクリックし、プロジェクトを最初から作成します。
1. プロジェクトの名前を入力します。 Enter キーを押して名前を保存します。

   ![プロジェクトの名前を入力](assets/rename-untitled-project.png)

   プロジェクトページのヘッダーには、プロジェクトの現在の正常性と進行状況の概要がすばやく表示されます。 プロジェクトの情報が更新されると、プロジェクトのヘッダーの情報が変更されます。

1. クリック **タスクの追加を開始**.

   または

   クリック **新規タスク** をクリックして、プロジェクトにタスクを追加し、リソースを割り当てます。

   プロジェクトへのタスクの追加の詳細については、「 [プロジェクトでのタスクの作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. プロジェクトの詳細を編集するには、 **その他** メニューとメニュー **編集** ![](assets/qs-edit-icon.png) プロジェクト名の横に表示されます。

   The **プロジェクトを編集** ダイアログボックスが開きます。

   プロジェクトの編集の詳細については、「 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

1. （オプション）プロジェクトの設定を行い、タスクを追加した後、プロジェクトのステータスを **現在**.

   これは、プロジェクトを開始する準備が整い、タスクに割り当てられたユーザーが、プロジェクトで作業を開始できる状態になったことを示します。

   プロジェクトのステータスの詳細については、「 [システムプロジェクトステータスのリストへのアクセス](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
