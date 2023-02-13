---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトを編集
description: 必要に応じて、Adobe Workfrontでプロジェクトを編集できます。 プロジェクトが Planning ステータスの場合は、プロジェクトを編集するのが理想的です。
author: Alina
feature: Work Management
exl-id: a6a1f178-189a-4c41-835b-7726081a2b49
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '6382'
ht-degree: 2%

---

# プロジェクトを編集

<!--drafted for bulk editing projects: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

<!--
<p>***Linked to many articles,</p>
<p>The Resource Pools part also duplicates in the "Working with Resource Pools" article -</p>
<p>The Update Type section is also documented in Selecting the Project Update Type article</p>
<p>Keep the reference link to the other article that also documents the Update Type) </p>
<p>(NOTE 2: information described here also exists in these articles:</p>
<p>** Project Overview area</p>
<p>**Manage project Finance area</p>
<p>If you need to update just one field, check to see if that field is also listed there and update in both places.)</p>
</div>
-->

必要に応じて、Adobe Workfrontでプロジェクトを編集できます。 ステータスが「現在」に変わった後は、プロジェクトを最小限に抑えて編集することをお勧めします。これにより、変更に関する通知をプロジェクトチーム全体に送信して混乱を避けることができます。 プロジェクトが Planning ステータスの場合は、プロジェクトを編集するのが理想的です。 プロジェクトチームの詳細については、 [プロジェクトチームの概要](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## アクセス要件

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a project to edit it in the Project Details area </p> </li> 
     <li> <p>Manage permissions to a project to edit it in the Edit Project box</p> </li> 
    </ul> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 プロジェクトへのアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">プロジェクトへのアクセス権の付与</a>. Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <ul> 
     <li> <p>プロジェクトに権限を付与して、「プロジェクトの詳細」領域で編集する </p> </li> 
     <li> <p>プロジェクトに対する権限を管理して、「プロジェクトを編集」ボックスで編集します</p> </li> 
    </ul> <p> プロジェクト権限について詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfrontでプロジェクトを共有する</a>.</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## プロジェクト編集の制限

プロジェクトを編集できない場合がある制限事項があります。

プロジェクトを編集する際は、次の点を考慮してください。

* 承認プロセス中のプロジェクトは、ログ時間以外は編集できません。
* 「完了」、「無効」、または「承認待ち」のステータスを持つプロジェクトにドキュメントやテンプレートを添付できるのは、Workfront管理者またはグループ管理者が「プロジェクト環境設定」領域でこの機能を有効にした場合のみです。 プロジェクトの環境設定の詳細については、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 無効または完了のステータスのプロジェクトに関する次の情報のみを編集できます。

   * 既存の費用を変更します。
   * カスタムフォームを追加、削除、または編集します。

## プロジェクトの編集

プロジェクトを編集すると、プロジェクトの情報や設定、およびプロジェクトのタスクや問題を変更できます。

この記事で説明する一部の設定は、プロジェクトの作成元のテンプレート内の状態によって、デフォルトの状態から変更される場合があります。 テンプレートの編集について詳しくは、 [プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **プロジェクト**.
1. （オプション）「 **自分がいるプロジェクト** または **自分が所有するプロジェクト** 右上隅には、自分が所有者であるプロジェクト、または自分がプロジェクトチームに属しているプロジェクトが表示されます。

   ![](assets/projects-on-my-own-buttons-350x302.png)

1. 編集するプロジェクトの名前をクリックして、プロジェクトページを開きます。

   >[!NOTE]
   >
   >グループ管理者は、グループ領域と「プロジェクト」領域で、グループのプロジェクトを表示および編集できます。 詳しくは、 [グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. （オプション）プロジェクトに関する限定的な情報を編集するには、 **プロジェクトの詳細** をクリックします。

   ![](assets/nwe-project-details-expanded-350x298.png)

   >[!NOTE]
   >
   >Workfront管理者またはグループ管理者がレイアウトテンプレートを変更した方法に応じて、「プロジェクトの詳細」領域のフィールドが再配置されたり表示されなかったりする場合があります。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   「詳細」セクションの情報を編集するには、次の手順を実行します。

   1. （オプション） **すべて折りたたむ** アイコンを使用して、すべての領域を折りたたみます。
   1. （オプションおよび条件付き）領域が折りたたまれている場合、 **右向き矢印** ![](assets/right-pointing-arrow.png) 各領域の横に、編集する領域を展開します。
   1. [ プロジェクトの詳細 ] タブでの情報の編集の詳細については、次の記事を参照してください。

      * [プロジェクトの概要領域で情報を管理します。](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)
      * [プロジェクトの財務エリアで情報を管理します](../../../manage-work/projects/project-finances/manage-project-finance-area.md)
   1. （オプション）カスタムフォームを添付するには、 **カスタムフォームを追加** フィールドに値を入力し、リストに表示されるタイミングで選択して、 **変更を保存**.
   1. （オプション） **書き出し** アイコン ![](assets/export.png) 概要およびカスタムフォームの情報を書き出すには、PDF・ファイルに **書き出し**. 次の中から選択します。

      * すべてを選択（少なくとも 1 つのカスタムフォームが添付されている場合にのみ表示）
      * 概要
      * 1 つまたは複数のカスタムフォームの名前

      PDFファイルがコンピューターにダウンロードされます。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      詳しくは、 [カスタムフォームとオブジェクトの詳細のエクスポート](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).
   「プロジェクトの詳細」セクションに表示されるフィールドの詳細については、次に説明するように、「プロジェクトを編集」ボックスでプロジェクトを編集します。
1. プロジェクトに関するすべての情報を編集するには、 **詳細** メニュー ![](assets/qs-more-menu.png) プロジェクト名の横にあるをクリックし、 **編集**.

   または

   プロジェクトのリストから、プロジェクトを選択し、 **編集** アイコン ![](assets/edit-icon.png) をクリックします。

   この **プロジェクトを編集** ボックスが開きます。

   >[!IMPORTANT]
   >
   >「編集」オプションを表示するには、プロジェクトに対する管理権限が必要です。

   すべてのプロジェクトフィールドは、「プロジェクトを編集」ボックスで使用でき、左パネルに表示される領域でグループ化されます。

   >[!NOTE]
   >
   >Workfront管理者またはグループ管理者がレイアウトテンプレートを変更した方法に応じて、「プロジェクトを編集」ボックスの左側のパネルにある領域またはこれらの領域に表示されるフィールドの順序が変わったり表示されなかったりします。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. （条件付き） **詳細** メニューとメニュー **編集**&#x200B;では、左側のパネルに次のいずれかの領域で情報の更新を検討してください。

   * [プロジェクト名](#project-name)
   * [概要](#overview)
   * [カスタムフォーム](#custom-forms)
   * [財務](#finance)
   * [プロジェクト設定](#project-settings)
   * [タスク設定](#task-settings)
   * [問題設定](#issue-settings)
   * [アクセス](#access)

   >[!NOTE]
   >
   >Workfront管理者がプロジェクトの「詳細」領域にレイアウトテンプレートを設定する方法に応じて、「プロジェクトを編集」ボックスのセクションとフィールドが環境によって異なる場合があります。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### プロジェクト名 {#project-name}

1. 前述の説明に従って、プロジェクトの編集を開始します。
1. クリック **プロジェクト名** をクリックします。

   ![](assets/nwe-project-name-in-edit-project-box-350x125.png)

1. プロジェクトの名前を更新します。

   プロジェクトを一括編集する際には、プロジェクト名を編集できません。

### 概要 {#overview}

1. 前述の説明に従って、プロジェクトの編集を開始します。
1. クリック **概要** をクリックします。

   ![](assets/nwe-overview-in-edit-project-box-350x172.png)

1. プロジェクトに関する次の情報を更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td> <p>プロジェクトに関する追加情報を追加します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ステータス</strong> </td> 
      <td> <p>プロジェクトのステータスを選択します。 すべてのタスクとタスクが完了する前に、プロジェクトを完了とマークすることはできません。 プロジェクトのステータスについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref">システムプロジェクトステータスのリストへのアクセス</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先度</strong> </td> 
      <td> <p> <p>これは、プロジェクトに優先順位を付けるための視覚的なフラグです。</p> <p>Workfront管理者が選択したプロジェクトの環境設定によっては、優先度の名前が異なる場合があります。 優先度の編集の詳細については、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">優先度の作成とカスタマイズ</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>このプロジェクトに関する情報に関する Web リンクを指定します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>状況タイプ</strong> </td> 
      <td> <p>次の条件タイプの中から選択します。 
        <ul> 
         <li><strong>手動：</strong> プロジェクト所有者が、手動でプロジェクトに条件を設定します。</li> 
         <li><strong>進捗状況ステータス：</strong> Workfrontは、クリティカルパス上のタスクの進捗状況ステータスに基づいて、条件を自動的に設定します。 進捗状況ステータスについて詳しくは、 <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">タスクの進捗状況ステータスの概要</a>.</li> 
        </ul><p>Workfront管理者<span> またはグループ管理者</span> システムに対するプロジェクトの条件の計算方法のデフォルトを選択します <span>またはグループ</span>. プロジェクトの既定値の設定については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>. </p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>状況</strong> </td> 
      <td> <p> <p>(「 <strong>手動</strong> の <strong>条件タイプ</strong>):「条件」を選択して、プロジェクトの進行方法を示します。 </p> <p>プロジェクト条件を自動または手動で設定する方法については、 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">プロジェクト条件と条件タイプの概要</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>スケジュール モード</strong> </td> 
      <td> <p>プロジェクトを「開始日」からスケジュールするか、「完了日」からスケジュールするかを指定します。 この選択により、プロジェクト上のタスクの予定日が決まります。 
        <ul> 
         <li><strong>開始日</strong>:プロジェクトの最初のタスクには、デフォルトで、プロジェクトと同じ計画開始日が設定されます。 計画開始日タスクの詳細は、 <a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">タスクの計画開始日の概要</a>. プロジェクトタイムラインは開始日から計算され、プロジェクトの完了日は、すべてのタスクの期間に基づいてシステムによって計算されます。 </li> 
         <li><strong>完了日</strong>:プロジェクトの最後のタスクには、プロジェクトと同じ計画完了日が設定されます。 プロジェクトタイムラインは、プロジェクトの完了日から計算され、プロジェクトの開始日は、プロジェクトの完了日からすべてのタスクの期間を引くことで、システムによって計算されます。 </li> 
        </ul><p>Workfront管理者<span> またはグループ管理者</span> システムまたはグループのデフォルトのスケジュールモード設定を選択します。 プロジェクトの既定値の設定については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>.</p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計画開始日時</strong> </td> 
      <td> <p> <p>選択時の日付を指定 <strong>スケジュール：開始日</strong>. <br></p> <p>これは、 <strong>完了日からのスケジュール</strong>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計画完了日時</strong> </td> 
      <td> <p>選択時の日付を指定 <strong>完了日からのスケジュール</strong>. </p> <p>これは、 <strong>開始日からのスケジュール</strong>.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ポートフォリオ</strong></td> 
      <td>プロジェクトが属するPortfolioを示します。 Portfolioは、ドロップダウンリストに表示される前に、最初に作成する必要があります。 プロジェクトに関連付けることができるのは、アクティブなポートフォリオのみです。 ポートフォリオの作成について詳しくは、 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">ポートフォリオの作成 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プログラム</strong></td> 
      <td> <p>プロジェクトのPortfolioを選択した場合は、プロジェクトのプログラムを指定します。 一部のPortfolioにはプログラムがない可能性があります。 このドロップダウンリストに表示される前に、最初にプログラムを作成する必要があります。 プロジェクトに関連付けることができるのは、アクティブなプログラムのみです。 </p> <p>プログラムの作成の詳細については、 <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">プログラムの作成</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>グループ</strong></td> 
      <td> <p> <p>プロジェクトに関連付けられているグループの名前を指定します。 </p>これは必須フィールドです. グループに関連付けられていないプロジェクトを持つことはできません。 </p> <p>適切なグループを選択していることを確認するには、グループにカーソルを移動して、情報アイコンをクリックします <img src="assets/info-icon.png"> その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> 別のグループを指定しない限り、デフォルトでは、次のグループの 1 つがプロジェクトの作成時に自動的にプロジェクトに関連付けられます。</p> 
        <ul> 
         <li> <p><span>プロジェクトを「プロジェクト」領域から作成すると、プロジェクト作成者の「ホームグループ」がプロジェクトに関連付けられます。</span> </p> <p>これは、ポートフォリオまたはプログラムの「プロジェクト」セクションからプロジェクトを作成した場合にも当てはまります。</p> </li> 
         <li> <p>設定領域のグループのメインページからプロジェクトを作成すると、そのグループがプロジェクトに関連付けられます。</p> </li> 
        </ul> </p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> <p>グループレベルのカスタムステータスを使用して、プロジェクト、またはそのタスクまたは問題が既にグループレベルの承認プロセスに関連付けられている場合、グループを変更すると、前のグループの承認ステータスとシステムレベルの承認ステータスが競合する可能性があります。 グループを更新する前に、プロジェクト上のグループレベルの承認プロセス、またはそのタスクや問題を削除することを検討してください。 グループレベルの承認プロセスの作成について詳しくは、 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">グループレベルの承認プロセス</a>. グループレベルのカスタムステータスの作成について詳しくは、 <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md" class="MCXref xref">グループのステータスの作成または編集</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>会社</strong> </td> 
      <td> <p>プロジェクトに関連付けられている会社を指定します。 会社をプロジェクトに関連付ける前に、会社を作成する必要があります。 プロジェクトに関連付けることができるのは、アクティブな会社のみです。 会社の作成について詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">会社の作成と編集</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プロジェクト所有者</strong> </td> 
      <td> <p>プロジェクトに追加するユーザーの名前を入力し始め、リストに表示されたら選択します。 ユーザーはプロジェクトチームに追加され、自動的にプロジェクトに対する管理権限が付与されます。 プロジェクト所有者として指定されるユーザーは、Workfrontのアクティブなユーザーである必要があります。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プロジェクト スポンサー</strong> </td> 
      <td> <p>プロジェクトに追加するユーザーの名前を入力し始め、リストに表示されたら選択します。 ユーザーはプロジェクトチームに追加され、プロジェクトに対する表示権限が自動的に付与されます。 プロジェクトスポンサーに指定されたユーザーは、Workfrontのアクティブユーザーである必要があります。<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>リソース管理者</strong> </td> 
      <td> <p> ユーザーの名前を入力してプロジェクトに追加し、リストに表示されたら選択します。 ユーザーはプロジェクトチームに追加され、自動的にプロジェクトに対する管理権限が付与され、プロジェクトのタスクやタスクにリソースを割り当てることができます。 ユーザーが「リソースマネージャー」フィールドから削除された場合でも、プロジェクトに対する「管理」権限が維持されます。 複数のリソースマネージャを指定できます。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >   「プロジェクト所有者」、「プロジェクトスポンサー」、「リソースマネージャー」の各フィールドを更新する際には、アバター、ユーザーのプライマリの役割、または電子メールアドレスに注意して、同じ名前のユーザーを区別します。 ユーザーを追加したときに表示するには、少なくとも 1 つのジョブの役割に関連付ける必要があります。

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

### カスタムフォーム {#custom-forms}

1. 前述の説明に従って、プロジェクトの編集を開始します。
1. クリック **カスタムForms** をクリックします。

   ![](assets/nwe-custom-forms-in-edit-project-box-350x170.png)

1. 次をクリック： **カスタムフォームを追加** ボックスを選択し、リストからフォームを選択して、プロジェクトに添付します。

   カスタムフォームをこのフィールドで選択できるようにするには、事前にカスタムフォームを作成する必要があります。 アクティブなカスタムフォームのみがリストに表示されます。 カスタムフォームの作成について詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 1 つのプロジェクトに最大 10 個のカスタムフォームを追加できます。

1. （条件付き）カスタムフォームをプロジェクトに添付した場合、フォーム上の任意のフィールドを編集します。 プロジェクトを保存する前に、すべての必須フィールドを指定する必要があります。

   >[!NOTE]
   >
   >Workfront管理者がカスタムフォームのセクションに対して権限を設定した方法に応じて、すべてのユーザーが特定のカスタムフォームの同じフィールドを表示または編集できるわけではありません。 カスタムフォームのセクション内のフィールドを編集する権限は、プロジェクト自体に対する権限によって異なります。 カスタムフォームのセクションに対する権限の設定について詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). プロジェクトに対する権限の設定については、 [Adobe Workfrontでプロジェクトを共有する](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

1. （オプション） **X アイコン** 削除するカスタムフォームの名前の右側にあるをクリックし、 **削除**.
1. （オプション）変更する情報に応じて、以降のセクションの編集を続けます

   または

   「**保存**」をクリックします。

### 財務 {#finance}

1. 前述の説明に従って、プロジェクトの編集を開始します。
1. クリック **金融** をクリックします。

   ![](assets/nwe-finance-in-edit-project-box-350x183.png)

1. プロジェクトの次の財務情報を更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>通貨</strong> </td> 
      <td> <p> <p>システムのデフォルトの通貨と異なる場合は、プロジェクトの通貨を指定します。 プロジェクトに既に財務情報がある場合は、プロジェクトの通貨を変更できません。 システムにデフォルトの通貨のみが存在する場合、このフィールドは表示されません。 </p> <p>通貨について詳しくは、 <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">為替レートの設定</a>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>予算</strong> </td> 
      <td> <p>プロジェクトの予算を指定します。<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>パフォーマンス インデックス メソッド</strong> </td> 
      <td> <p>選択 <b>時間ベース</b>または <b>コストベース</b> プロジェクトの [ 達成額 ] 指標（[ コスト効果指数 ] や [ 推定実績コスト ] など）が、時間またはコストを使用して計算されるかどうかを指定します。 </p> <p>Performance Index メソッドの詳細については、 <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">パフォーマンスインデックスメソッド (PIM) の設定</a>. </p> <p>Workfront管理者<span> またはグループ管理者</span> システムまたはグループの既定の [ パフォーマンスインデックス方法 ] 設定を選択します。 プロジェクトの既定値の設定については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完成時総コスト見積り</strong> </td> 
      <td> <p> <p>Workfrontが完了時の推定 (EAC) を計算する方法を指定します。 </p>
      次のオプションから選択します。 
      <ul><li><b>プロジェクト レベルで計算する</b></li>
      <li><b>タスク/サブタスクからロールアップする</b></li> </ul>
      <p>完了時の見積もりの計算方法の詳細については、 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">完了時の推定 (EAC) を計算</a>.</p> <p>Workfrontまたはグループ管理者が、ご使用のシステムまたはグループのデフォルトの「完了時の推定」設定を選択します。 プロジェクトの既定値の設定については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>予定便益</strong> </td> 
      <td> <p>プロジェクトの計画的利益とは何かを見積もります。 これは、プロジェクトのビジネスケースとPortfolioの最適化で使用されます。 プロジェクトの計画的利益の詳細は、 <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">プロジェクト計画福利厚生の概要</a>. プロジェクトの正味価値が計算される際には、プロジェクトの計画特典が考慮されます。 </p> <p>詳しくは、 <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Management Optimizer でのプロジェクトのPortfolio</a> .<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>実際の便益</strong> </td> 
      <td> <p>プロジェクトの実際の利益を見積もります。 これは、このプロジェクトが完了した後に企業または部門が得る利益を表す通貨金額です。 </p> </td> 
     </tr> 
      <tr> 
      <td role="rowheader"><strong>固定コスト</strong> </td> 
      <td> <p>プロジェクトの固定コストを指定します。 これは、プロジェクトの時間に基づく人件費と、プロジェクトの費用の額に基づく費用コストとは異なります。 プロジェクトの固定コストは、プロジェクトの正味値を計算する際に考慮され、予算コストに含まれます。<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>固定収益</strong> </td> 
      <td> <p>プロジェクトの固定売上高を指定します。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

### プロジェクト設定 {#project-settings}

1. 前述の説明に従って、プロジェクトの編集を開始します。
1. クリック **プロジェクト設定** をクリックします。

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. 次の情報を更新します。

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>マイルストーン パス</strong> </td> 
       <td> <p>プロジェクトのマイルストーンパスを選択します。 アクティブなマイルストーンパスのみがリストに表示されます。</p> <p>マイルストーンパスの詳細については、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">マイルストーンパスを作成</a>.</p> </td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>完了モード</strong> </td> 
      <td> <p>プロジェクトを完了としてマークする方法を制御します。 次のオプションから選択します。 
       <ul> 
       <li><p><strong>自動</strong>:すべてのタスクと問題が完了すると、プロジェクトは「完了」とマークされます。</p><p>タスクが完了したときに、プロジェクトのステータスが [ 現在 ] になった場合にのみ、プロジェクトのステータスが [ 完了 ] に自動的に変更されます。 </p></li> 
       <li><strong>手動</strong>:すべてのタスクと問題が完了したら、プロジェクトの完了ステータスを手動で選択する必要があります。</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>概要完了モード</strong></td> 
       <td> <p>親タスクを [ 完了 ] としてマークする方法を制御します。 次のオプションから選択します。 
       <ul> 
       <li><strong>自動</strong>:親タスクは「完了」とマークされ、子タスクが完了し、子タスクの完了率が更新されると、完了率が自動的に更新されます。 </li> 
       <li><strong>手動</strong>:子タスクに加えられた変更に関係なく、完了率と親タスクのステータスを手動で更新する必要があります。</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>更新の種類</strong></td> 
       <td> <p>プロジェクトタイムラインに対して行った変更を、プロジェクトまたは親タスクに保存するタイミングを制御します。 例えば、プロジェクトトリガーに対する次の変更や、プロジェクトのタイムラインへの更新があります。 
       <ul> 
       <li>タスクの日付を更新</li> 
       <li>タスクの先行関係の変更</li> 
       <li><p>タスクの制約や期間の種類の変更に加えて、親子関係を変更し、割り当てを追加または削除します。</p><p>タスクが更新されると、親オブジェクト（親タスクまたはプロジェクト）は、[ 更新の種類 ] で示された時点で更新されます。 </p><p>「自動および変更時」または「変更のみ」更新タイプを選択した場合に、変更直後に親オブジェクトが更新されない場合は、ページを更新します</p><p>次のオプションから選択します。 </p><p>- <strong>自動および変更時</strong> （デフォルト設定）:プロジェクトの変更がプロジェクト内で発生するたび、またはプロジェクトが依存する別のプロジェクト内で変更が発生するたびに、プロジェクトタイムラインが更新されます（変更時）。 また、プロジェクトのタイムラインは毎晩更新されます（自動）。</p><p>プロジェクトが常に最新であることを確認するので、このフィールドでは推奨される設定です。</p><p>タイムラインの再計算をトリガーにするタスクまたはプロジェクトに対してアクションを実行すると、使用可能なすべての日付が直ちに表示され、作業を続行できます。 タスクが 100 を超えるプロジェクトでは、再計算に時間がかかる日付が疑問符（1～5 秒、大きなプロジェクトの場合は 1 分まで）として表示されます。 これは、再計算がまだ完了しておらず、日付が変更される可能性があることを示しています。</p><p>- <strong>変更のみ</strong>:プロジェクトタイムラインは、プロジェクト内またはプロジェクトが依存する別のプロジェクト内で変更が発生するたびに更新されます。 プロジェクトや、タイムラインが依存する他のプロジェクトで変更がほとんど発生しない場合は、このオプションを選択できます。</p><p>- <strong>自動のみ</strong>:プロジェクトのタイムラインは毎晩更新され、変更を加えても、タイムラインは直ちには更新されません。</p><p>プロジェクトまたはタイムラインが依存する他のプロジェクトで毎日多くの変更が発生する場合に、このオプションを選択できます。 ただし、変更を加えてもプロジェクトは更新されないので、この設定を選択したことに注意してください。</p><p>- <strong>手動のみ</strong>:プロジェクトタイムラインは、「タイムラインを再計算」オプションを選択した場合にのみ更新されます。 プロジェクトタイムラインを手動で再計算する方法について詳しくは、 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">プロジェクトタイムラインを再計算</a>. </p><p>一度に多くの変更を加え、個々の変更の後ではなく、すべての変更が行われた後にタイムラインの再計算を行う場合は、このオプションを選択します。</p></li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>スケジュール</strong> </td> 
       <td> <p>プロジェクトのスケジュールを選択します。 これは、プロジェクトで作業しているほとんどの人に割り当てられたのと同じスケジュールである必要があります。 スケジュールをプロジェクトまたはユーザーに割り当てるには、事前にスケジュールを作成する必要があります。 システムでカスタムスケジュールを作成していない場合は、「デフォルトスケジュール」(Default Schedule) が選択されます。</p> <p>スケジュールの作成について詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールの作成</a>. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>ユーザーの休暇</strong> </td> 
       <td> <p>タスクのプライマリ担当者の時間が、プロジェクト上のタスクの予定日を調整するかどうかを指定します。 </p><p>Workfront管理者<span> またはグループ管理者</span> システムのこの設定の既定を選択します <span>またはグループ</span>. プロジェクトの既定値の設定については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>. </p><p>次のオプションから選択します。<br>- <strong>タスク期間でのユーザーのオフ時間を考慮する</strong>:このオプションを選択すると、タスクの期間中にプライマリの時間が発生した場合、タスクの担当者の時間に応じてタスクの予定日が調整されます。 </p><p>たとえば、タスクに [ 可能な限り早く ] という制約が付いている場合、プライマリが 6 月 1 日に開始し、6 月 3 日に完了するようにスケジュールされ、タスク担当者が 6 月 2 日に [ タイムオフ ] とマークされていると、タスクの予定日は 6 月 1 日から 6 月 4 日です。 タスク制約に応じて、次のシナリオが存在します。 </p> 
       <ul> 
       <li>計画に関連するタスク制約（可能な限り早く、利用可能な時間が最も早く、開始日が次の日よりも早く、開始日が次の日より後でなければ、開始日は変更されません）の場合は、計画開始日は変更されます。</li> 
       <li>完了日からの計画に関連するタスク制約（可能な限り遅延、最新の使用可能な時間、完了日が次の日まで、完了日が次の日まで、完了日が次の日までに完了する必要がある）では、計画完了日は変更されませんが、計画開始日は変更されます。</li> 
       <li>「固定日付」の制約を持つタスクの場合、「計画開始日」も「完了日」も変更されません。 </li> 
       </ul><p>この設定を選択した場合、タスクの期間は変更されません。 タスク制約に応じて、計画日のみが変更されます。 タスク制約の詳細については、 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>. </p><p>- <strong>タスク期間のユーザーのオフ時間を無視する</strong>:このオプションを選択すると、タスクのプライマリ担当者がタスクの期間中に休暇を取った場合でも、プロジェクトのタスクの予定日は当初の予定どおりに保たれます。 </p><p>この設定のオプションを選択する際は、次の点に注意してください。</p> 
       <ul> 
       <li><p>新しいプロジェクトに対するこの設定の既定のオプションは、システムレベルのプロジェクト環境設定と同じです。 </p><p>システムレベルでのプロジェクトのプリファレンスの詳細については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>. </p></li> 
       <li>テンプレートを既存のプロジェクトにアタッチすると、プロジェクトの設定が、テンプレートの設定に合わせて更新されます。 </li> 
       <li><p>Workfrontは、タスクの [ タスク制約 ] の値に従って、調整する予定タスクの日付を決定します。 計画開始日と計画完了日、またはその両方が影響を受ける場合や、同じままになる場合があります。 たとえば、タスクに [ 固定日付 ] の制約がある場合、プライマリ担当者がタイムオフになった時点では、タスクの日付が調整されません。 <strong>タスク期間でのユーザーのオフ時間を考慮する</strong> が選択されている。 </p></li> 
       </ul></td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>リソースの標準化モード</strong> </td> 
       <td> <p> <p>次のオプションから選択します。</p> <p>- <strong>手動</strong>:手動でリソースをレベル設定する必要があります（これはデフォルト設定です）</p> <p>- <strong>自動</strong>:Workfrontは、リソースをレベル分けします。</p> <p>リソースの平準化の詳細については、「 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">ガントチャートのリソースレベル設定 </a>.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>危険</strong> </td> 
       <td> <p> <p>プロジェクトのリスクレベルを定義します。 リスクは、プロジェクトがどの程度リスクが高いかを示す指標に過ぎません。 リスクのレベルに基づいて、プロジェクトの実行を優先順位付けできます。</p> <p> <p>次のリスクレベルから選択することを検討します。</p> <p>- 極低</p> <p>- 低</p> <p>- 中</p> <p>- 高</p> <p>- 極高</p> <p>ここで示すリスクのレベルはカスタマイズできません。</p> <p>これらは、プロジェクトの存続中に発生する可能性のある潜在的なリスク（プロジェクトの「リスク」タブまたはビジネス事例に記録する必要がある）とは関係ありません。 潜在的なプロジェクトのリスクについては、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md" class="MCXref xref">リスクタイプの編集と作成</a>. </p> </p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>リソース プール</strong> </td> 
       <td> <p> <p>プロジェクトに関連付けられた資源プールを指定します。 資源プールとは、プロジェクトの完了に同時に必要なユーザーの集まりで、資源プランナーでプロジェクトの予算を作成できます。 リソースプールの詳細については、 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> リソースプールの概要 </a>. </p> <p>プロジェクトを一括で編集すると、選択したすべてのプロジェクトに共通のリソースプールのみがこのフィールドに表示されます。 選択したプロジェクトに共有リソースプールがない場合、このフィールドは空になります。 ここで指定したリソースプールは、プロジェクトの個々のリソースプールを上書きします。</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <strong>会社レベルでの請求率によるプロジェクトレベルの請求率の上書きを許可</strong></td> 
       <td>このオプションを選択すると、会社レベルの請求率で、請求済みとしてマークされていない限り、ジョブの役割率の履歴を上書きできます。 このオプションを有効にすると、請求済みとしてマークされていない限り、過去のジョブロール率が上書きされます。 <br>詳しくは、 <a href="../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md" class="MCXref xref">プロジェクト・レベルの請求率を会社レベルの請求率で上書き</a>.</td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>プロジェクト時間の承認</strong></td> 
       <td> <p> このオプションを選択すると、プロジェクト所有者がプロジェクトにログオンした時間を承認する必要があります。 請求レコードを使用している場合、このオプションを選択すると、プロジェクトで承認された時間のみが請求レコードの請求可能時間として表示されます。 プロジェクトの承認時間は、タイムシートの承認とは無関係です。 </p> <p>プロジェクトで時間を承認する必要がある場合の詳細については、 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">プロジェクトの承認に時間が必要</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>時間タイプをフィルター</strong> および</span> <strong>時間タイプ</strong></td> 
       <td> <p> <p>次のオプションから選択します。</p> 
       <ul> 
       <li> <p>選択 <strong>いいえ</strong> プロジェクトでプロジェクト固有の時間タイプをすべて使用できるようにする。 （これはデフォルトの選択です）</p> <p>または</p> </li> 
       <li>選択 <strong>はい</strong> プロジェクト固有の時間タイプのサブセットのみをプロジェクトで使用可能にするには、使用可能にする時間タイプを選択します。 （複数の時間タイプを選択するには、Shift キーを押したままにします）。</li> 
       <p>このオプションを選択した場合、選択した時間タイプのみが、プロジェクトでの時間（またはプロジェクト内のタスクと問題）のログ記録時に選択できます。 1 時間以上のタイプを選択する必要があります。このオプションを選択し、どの時間タイプも選択しない場合、すべての時間タイプがプロジェクトで使用可能になります。</p> </ul>

   <p>ユーザーがプロジェクト上でこれらの時間タイプのオプションを表示するには、同じ時間タイプを個々のユーザーレベルで選択する必要があります。 ユーザーレベルで時間タイプを定義する方法について詳しくは、 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">ログ時間</a>. </p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>リマインダ通知</strong> </td> 
       <td> <p> <p>プロジェクトに関連付ける「リマインダー通知」を選択します。 プロジェクトの編集中にこのフィールドを表示するには、プロジェクトのリマインダー通知を設定する必要があります。 リマインダー通知の設定の詳細については、 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md"><a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">リマインダー通知の設定</a> .</a></p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>承認プロセス</strong></td> 
       <td> <p>プロジェクトに関連付ける承認プロセスを選択します。 Workfront管理者は、プロジェクトに関連付ける前に、システムレベルの承認プロセスを定義する必要があります。 <span>承認プロセスへの管理者アクセス権を持つユーザーは、グループ固有の承認プロセスを作成することもできます。</span> 承認プロセスの作成について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業項目の承認プロセスの作成</a>.</p> <p>承認プロセスを追加する際は、次の点を考慮してください。 </p> 
       <ul> 
       <li>アクティブな承認プロセスのみがリストに表示されます。 </li> 
       <li> <p>システム全体およびグループ固有の承認プロセスがリストに表示されます。 プロジェクトの承認プロセス以外のグループに関連付けられている承認プロセスは、リストに表示されません。</p> <p>プロジェクトに関連付けられたグループが変更されると、グループ固有の承認プロセスが単一使用の承認プロセスになります。 プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループと承認プロセスの変更が、割り当てられた承認プロセスに及ぼす影響</a>. </p> </li>

   <!--(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)-->

   <p>プロジェクトの一括編集では、次のシナリオが存在します。</p>

   <ul> 
   <li> <p>同じグループからプロジェクトを選択すると、システムレベルとグループレベルの両方の承認プロセスがこのフィールドに表示されます。</p> </li> 
   <li> <p>異なるグループからプロジェクトを選択すると、このフィールドにはシステムレベルの承認プロセスのみが表示されます。</p> </li> 
   <li> <p>プロジェクトに 1 回限りの承認プロセスが添付されている場合、選択したシステムレベルまたはグループレベルの承認プロセスに置き換えられます。 </p> </li> 
   </ul> 
      </ul> </td> 
      </tr> 
      <tr> 
      </tr> 
      </tbody> 
      </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

### タスク設定 {#task-settings}

プロジェクトに追加する際に、すべての新しいタスクに関連付けるデフォルトを定義できます。

これらの設定が新しいタスクの作成に与える影響については、「 [タスクをプロジェクトに追加する際のタスクのデフォルト](../../../manage-work/tasks/create-tasks/create-tasks-overview.md#understa) 記事内 [タスクの作成の概要](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. 前述の説明に従って、プロジェクトの編集を開始します。
1. クリック **タスク設定** をクリックします。

   ![](assets/nwe-task-settings-in-edit-project-box-350x211.png)

1. 内 **タスクのデフォルトの承認プロセス** ボックスで、プロジェクトに追加する際に、すべての新しいタスクに関連付けるタスク承認プロセスを選択します。

   Workfront管理者（または承認プロセスへの管理者アクセス権を持つユーザー）は、タスクをプロジェクトに関連付ける前に、タスクのシステムレベルの承認プロセスを作成する必要があります。 アクティブな承認プロセスのみがリストに表示されます。 承認プロセスの作成について詳しくは、 [作業項目の承認プロセスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md). プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、 [グループと承認プロセスの変更が、割り当てられた承認プロセスに及ぼす影響](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

   プロジェクトの一括編集では、次のシナリオが存在します。

   * 同じグループから複数のプロジェクトを選択すると、システムレベルとグループ固有のタスク承認プロセスの両方がこのフィールドに表示されます。
   * 異なるグループから複数のプロジェクトを選択する場合、このフィールドにはシステムレベルのタスク承認プロセスのみが表示されます。

1. 内 **タスクのデフォルトのカスタムForms** ボックスで、プロジェクトに追加する際に、すべての新しいタスクに関連付けるカスタムフォームまたはフォームを選択します。 カスタムフォームをこのフィールドで選択できるようにするには、事前にカスタムフォームを作成する必要があります。 リストには、アクティブなカスタムフォームのみが表示されます。 カスタムフォームの作成について詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 1 つのタスクに最大 10 個のカスタムフォームを関連付けることができます。
1. （オプション）「 」を選択します。 **作業工数を使用してタスク計画時間を自動的に計算** 「計画時間」ではなく「作業工数」を使用して、タスクの作業量の管理を有効にする場合。

   ![](assets/nwe-work-effort-on-projects-350x182.png)

1. （条件付きおよびオプション）「作業量を使用してタスクの計画時間を自動的に計算」を選択した場合、各作業量レベルのドロップダウン・メニューをクリックし、各レベルの割合を選択します。 次のパーセンテージ値がデフォルトです。

   | サイズ | 百分率 |
   |---|---|
   | 小 | 25% |
   | 中 | 50% |
   | 大 | 75% |

   >[!TIP]
   >
   >プロジェクトの [ 更新の種類 ] が [ 自動 ] に設定され、この設定を選択した場合、タスクの [ 期間 ] と [ 作業時間 ] の割合（0 に設定されている場合）に応じて、タスクの [ 予定時間 ] が更新されます。 作業量を使用してタスクの取り組みを計画する方法の詳細については、「 [作業量の概要](../../../manage-work/tasks/task-information/work-effort.md).

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

### 問題設定 {#issue-settings}

1. 前述の説明に従って、プロジェクトの編集を開始します。
1. クリック **問題の設定** をクリックします。

   ![](assets/nwe-issue-settings-in-edit-project-box-350x306.png)

1. （オプション） **ユーザーがイシューをインラインで追加することを許可** オプション。 デフォルトで選択されています。

   このオプションの選択を解除すると、ユーザーは、プロジェクトまたは「問題」セクションのタスクに問題をインラインで追加できません。

   >[!TIP]
   >
   >ユーザーが新しい問題に関連する新しい問題フィールドやカスタムフォームを強制的に入力する場合は、このオプションの選択を解除します。 ユーザーがイシューをインラインで入力できるようにすると、イシューを作成する際に、新しいイシューフィールドとカスタムフォームをスキップすることができます。 新しい問題に対するフィールドおよびカスタムフォームの設定について詳しくは、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   このオプションの選択を解除する場合、プロジェクトまたはタスクにイシューを追加する権限を持つユーザーは、次の方法でイシューを追加できます。

   * プロジェクトまたはタスクの「問題」セクションの問題の一覧の上部にある「新しい問題」をクリックします。
   * プロジェクトをリクエストキューとして設定すると、新しいリクエストを「リクエスト」領域に入力できます。

   >[!NOTE]
   >
   >一括でプロジェクトを編集する場合、この設定は、少なくとも 1 つのプロジェクトで有効になっている場合に有効になり、選択したすべてのプロジェクトで無効になっている場合に無効になります。

   <!--drafted for bulk edit projects: the statement above needs to be corrected when the new UI for bulk edit projects is updated; not sure if we'll need to describe this at all or we can cover this in  a "Considerations" mini section inside the Editing in bulk section below- ??? -->

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

### アクセス {#access}

1. 前述の説明に従って、プロジェクトの編集を開始します。
1. クリック **アクセス** をクリックします。

   ![](assets/nwe-access-in-edit-project-box-350x262.png)

1. 以下を指定します。 **アクセス** プロジェクトの情報：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>誰かがタスクに割り当てられたとき</strong></td> 
      <td><p>次から選択： <strong>表示</strong>, <strong>投稿、</strong> または <strong>管理</strong> タスクへのアクセス タスクに割り当てられたユーザーには、このタスクへのアクセス権が自動的に付与されます。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>プロジェクトへのアクセス権も付与</strong></td> 
      <td><p>次から選択： <strong>表示</strong>, <strong>投稿</strong>または <strong>管理</strong> プロジェクトへのアクセス タスクに割り当てられたユーザーにも、プロジェクトへのこのアクセス権が自動的に付与されます。<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>誰かが問題に割り当てられたとき</strong></td> 
      <td><p>次から選択： <strong>表示</strong>, <strong>投稿、</strong> または <strong>管理</strong> イシューにアクセスする。 イシューに割り当てられたユーザーには、そのイシューに対するこのアクセス権が自動的に付与されます。 詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有 </a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>プロジェクトへのアクセス権も付与</strong></td> 
      <td><p>次から選択： <strong>表示</strong>, <strong>投稿</strong>または <strong>管理</strong> プロジェクトへのアクセス イシューに割り当てられたユーザーにも、プロジェクトへのアクセス権が自動的に付与されます。<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>誰かがリクエストを送信したとき：アクセス権を付与</strong></td> 
      <td><p>次から選択： <strong>表示</strong>, <strong>投稿</strong>または <strong>管理</strong> リクエストへのアクセス プロジェクトが要求キューでもあり、ユーザーが要求をプロジェクトに送信すると、ユーザーは、送信した要求に対してこのアクセス権を付与されます。 プロジェクトをリクエストキューとして設定する方法については、 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>同じ会社の担当者は、すべてのリクエストに対して同じ権限を継承します</strong></td> 
      <td><p>同じ会社の担当者が、送信したかどうかに関わらず、プロジェクトのすべての要求に同じアクセス権を持つようにする場合は、このフィールドを選択します。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>誰かがこのプロジェクトへのアクセス権を付与されたとき：ユーザーに次へのアクセス権を付与します。</strong></td> 
      <td><p>プロジェクトがプロジェクトと共有されている場合に、ユーザーがプロジェクトに対して持つアクセスオプションを選択します。 ユーザーが <strong>ビューア</strong>, <strong>寄稿者</strong>または <strong>管理者</strong> プロジェクトを共有する際に使用します。 </p><p>この <strong>削除</strong> の <strong>管理</strong> 権限レベルは、ユーザーがプロジェクト自体を削除できるかどうかを決定します。 次を持つユーザー： <strong>管理</strong> プロジェクトにアクセスすると、このオプションが選択されているかどうかに関係なく、プロジェクト内のタスクやタスクを削除できます（タスクがある場合） <strong>管理</strong> タスクおよび問題に対する権限。 </p></td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

## プロジェクトヘッダーでプロジェクトを編集する（制限あり）

プロジェクトのヘッダーで編集できる情報の量は限られています。

システム管理者またはグループ管理者は、プロジェクトヘッダーに表示されるフィールドをカスタマイズできます。

![](assets/project-header-350x18.png)

デフォルトでは、次のフィールドがプロジェクトヘッダーに含まれています。

* プロジェクト名
* プロジェクト所有者
* 計画完了日時

   >[!NOTE]
   >
   >このフィールドは、プロジェクトが「完了日」からスケジュールされている場合にのみ編集できます。 プロジェクトが開始日からスケジュールされる場合、Workfrontは、タスクの期間に基づいて計画完了日時を計算します。

* 状況

   >[!NOTE]
   >
   >このフィールドは、プロジェクトの「条件タイプ」が「手動」の場合にのみ編集できます。 「条件の種類」が「進捗状況ステータス」に設定されている場合、Workfrontはタスクの進捗状況に基づいて条件を計算します。 詳しくは、 [プロジェクト条件と条件タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

* ステータス
* 現在の承認プロセスで承認者として設定されている場合、承認の決定をおこないます

## プロジェクトの一括編集

プロジェクトは一括で編集し、すべての情報を同時に更新できます。

プロジェクトを一括編集するには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **プロジェクト**.
1. リストから複数のプロジェクトを選択します。
1. クリック **編集**.

   この **プロジェクトを編集** ダイアログボックスが開きます。

   ![](assets/edit-projects-in-bulk-nwe-350x303.png)

1. 次のセクションで、選択したすべてのプロジェクトの情報を指定します。

   * **概要**

      詳しくは、 [概要](#overview) 」の節を参照してください。

   * **財務**

      詳しくは、 [金融](#finance) 」の節を参照してください。

   * **ポートフォリオ**

      詳しくは、 [概要](#overview) 」の節を参照してください。

   * **設定**

      詳しくは、 [プロジェクト設定](#project-settings) 」の節を参照してください。

   * **アクセス**

      詳しくは、 [アクセス](#access) 」の節を参照してください。

   * **カスタムフォーム**

      詳しくは、次の手順 7 に進んでください。

      <!--   
     <p>(NOTE:&nbsp;make sure this stays accurate)</p>   
     -->

   * **タスク**

      詳しくは、 [タスク設定](#task-settings) 」の節を参照してください。

   * **問題**

      詳しくは、   [問題の設定](#issue-settings) 」の節を参照してください。

   * **コメント**

      詳しくは、次の手順 9 に進んでください。

      <!--   
     <p>(NOTE: ensure this step stays accurate)</p>   
     -->
   >[!NOTE]
   >
   >選択したすべてのプロジェクトで変更する情報は、個々のプロジェクトに関する既存の情報 ( **リソースマネージャ** フィールドに入力します。 一括編集で新しいリソースマネージャーを追加すると、選択したすべてのプロジェクトにそのマネージャーが追加されます。 他のリソースマネージャが選択したプロジェクトに関連付けられている場合、一括編集で追加されたプロジェクトに加えて、プロジェクトに残ります。

1. （オプション）「Settings」領域で、次のいずれかのオプションを選択します。

   * **コストと売上高の再計算**:選択したすべてのプロジェクトのコストと売上高を再計算するには、このオプションを選択します。
   * **タイムラインを再計算**:選択したすべてのプロジェクトのタイムラインを再計算するには、このオプションを選択します。
   * **スコアカードを再計算**:選択したすべてのプロジェクトのスコアカード値を再計算するには、このオプションを選択します。

   ![recalculate_costs__scorecards__etc_in_bulk_edit_for_projects.PNG](assets/recalculate-costs--scorecards--etc-in-bulk-edit-for-projects-350x225.png)

1. クリック **カスタムForms** 選択したすべてのプロジェクトに添付されたカスタムフォームを編集する場合。

   選択したプロジェクトに共通のカスタムフォームがない場合、このセクションにはフォームが表示されません。

   選択したすべてのプロジェクトに添付され、編集権限を持つフォーム上のフィールドのみを編集できます。

1. （オプション）「カスタムForms」セクションで、 **カスタム式の再計算** オプションを使用して、選択したプロジェクトに関連付けられているカスタムForms上の計算カスタムフィールドがすべて最新であることを確認します。

   >[!IMPORTANT]
   >
   >カスタム式を再計算する場合は、一度に 500 個を超えるプロジェクトを選択しないことをお勧めします。

1. （オプション）「 **コメント**&#x200B;次に、「各プロジェクトに更新を投稿」ボックスを選択し、「使用可能」フィールドでプロジェクトの更新ストリームに表示するコメントを指定し、次のいずれかの操作をおこないます。

   * 次をクリック： **人** アイコン ![](assets/people-icon-updates-classic.png) コメントに関する通知を受け取るユーザーにタグを付けます。
   * 次をクリック： **ロック** アイコン ![](assets/lock-icon-open-updates-classic.png) を使用して、社内のユーザーのみにコメントを制限します。

   このコメントは、プロジェクトへの表示アクセス権を持ち、メモの表示アクセス権を持つすべてのユーザーに対して表示されます。

1. クリック **変更を保存**.

   これで、行った変更が、選択したすべてのプロジェクトに表示されます。