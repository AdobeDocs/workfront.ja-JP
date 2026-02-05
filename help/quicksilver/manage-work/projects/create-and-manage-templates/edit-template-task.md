---
product-area: templates
keywords: タスク,デフォルト,自動化,作成
navigation-topic: templates-navigation-topic
title: テンプレート タスクの編集
description: テンプレートを作成した後、テンプレートタスクに関する情報を編集できます。テンプレートタスクで更新した情報は、テンプレートを使用してプロジェクトを作成した後、またはテンプレートをプロジェクトに添付した後、プロジェクトタスクに関連付けられます。
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: c9fa6d97607990710e6c2a74f3b373d06201d721
workflow-type: tm+mt
source-wordcount: '7460'
ht-degree: 70%

---

# テンプレートタスクを編集

<!--Audited: 11/2025-->

<!--take out production and preview references and new/ old experiences at release-->

<div class="preview">

このページで強調表示されている情報は、まだ一般公開されていない機能を示しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 プレビューリリースから 1 週間後に、すべてのお客様の実稼動環境でも同じ機能が使用できるようになります。

詳しくは、[ インターフェイスの最新化 ](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md) を参照してください。

</div>

テンプレートの作成後、テンプレートタスクの情報を編集できます。 テンプレートタスクで更新した情報は、テンプレートを使用してプロジェクトを作成した後、またはテンプレートをプロジェクトに添付した後、プロジェクトタスクに関連付けられます。

テンプレートの作成の詳細については、[プロジェクトテンプレートを作成](../../../manage-work/projects/create-and-manage-templates/create-template.md)を参照してください。

一度に 1 つのテンプレートタスクを編集することも、テンプレートタスクを一括編集することもできます。

>[!NOTE]
>
>異なるテンプレートに属するテンプレートタスクは、一括編集できません。同じテンプレートに属するテンプレートタスクのみ編集できます。

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
   <p>プラン </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>テンプレートへの編集アクセス</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限 </td> 
   <td> <p>テンプレートの権限を管理します。 </p> <p>テンプレートタスクは共有できません。 </p> </td> 
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
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Templates</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions </td> 
   <td> <p>Manage permissions for a template. </p> <p>You cannot share a template task. </p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 前提条件

開始する前に、

* テンプレートを作成する必要があります。

  テンプレートの作成の詳細については、[プロジェクトテンプレートを作成](../../../manage-work/projects/create-and-manage-templates/create-template.md)を参照してください。

## テンプレートタスクを編集

テンプレートタスクの編集は、タスクを編集する環境によって異なります。

### 実稼動環境でのテンプレートタスクの編集

>[!NOTE]
>
><span class="preview"> 一部のお客様は、プレビュー環境で編集するのと同じ方法で、実稼動環境でテンプレートタスクを編集できます。</span>
>
><span class="preview"> プレビュー環境でのタスクの編集について詳しくは、この記事の [ プレビュー環境でのテンプレートタスクの編集 ](#edit-template-tasks-in-the-preview-environment) を参照してください。</span>


テンプレートタスクを編集は、テンプレートタスクを編集またはテンプレートタスクの詳細領域を使用して編集できます。

{{step1-to-templates}}

1. テンプレートの名前をクリックして開きます。
1. 左パネルの「**テンプレートタスク**」をクリックします。
1. リスト内のテンプレートタスクの名前をクリックして、テンプレートタスクを開きます。
1. テンプレートタスクに関する制限付きの情報を編集するには、次の手順を実行します。
   1. （任意）左側のパネルで「**更新**」をクリックして、テンプレートタスクに更新を追加します。 テンプレートを使用してプロジェクトを作成する場合、テンプレートタスクの更新がプロジェクトタスクに転送されない。
   1. （任意）左側のパネルで **ドキュメント** をクリックして、ドキュメントをテンプレートタスクに追加します。 テンプレートを使用してプロジェクトを作成すると、ドキュメントはプロジェクトタスクに転送されます。
   1. （条件付き）テンプレートタスクに関する限られた情報を編集するには、左パネルで「**テンプレートタスクの詳細**」をクリックし、詳細セクションのエリアに移動して、それぞれのエリアの情報を編集します。
   1. （オプション）次のいずれかの操作を行います。
      * **すべて折りたたむ** アイコン ![ すべて折りたたむアイコン ](assets/collapse-all-icon.png) をクリックすると、すべての領域が折りたたまれます。
      * **編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックして、下の任意の領域から選択するか、**すべて編集** をクリックして、すべての領域の情報を編集します。

         * 概要
         * カスタムForms
カスタムフォームの名前は、テンプレートタスクに添付されたカスタムフォームがある場合にのみ表示されます。
         * 財務

        >[!TIP]
        >
        >「詳細」領域に表示されるすべてのフィールドについて詳しくは、以下に説明するように、「テンプレートタスクを編集」ボックスを使用してすべてのフィールドを引き続き編集します。

   1. （任意）左側のパネルで「**サブタスク**」セクションをクリックして、テンプレートタスクの子を追加します。 テンプレートタスクのサブタスクの追加は、プロジェクトタスクのサブタスクの追加と似ています。 詳しくは、「サブタスクの作成」の「タスクサブタスクからサブタスクを作成する [ 節を参照してくだ ](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md) い。
   1. （任意）左側のパネルで **費用** をクリックし、テンプレートタスクに費用を追加します。 テンプレートタスクの費用は、テンプレートを使用してプロジェクトを作成する際に、将来のプロジェクトタスクに転送されます。
   1. （任意）左側のパネルの **承認** をクリックして承認を作成するか、テンプレートタスクにグローバルまたはグループレベルの承認を添付します。 承認は、今後のプロジェクトタスクに転送されます。
   1. （任意）左側のパネルで「**先行タスク**」セクションをクリックして、テンプレートタスクの先行タスクを追加します。 テンプレートタスク先行タスクの追加は、プロジェクトタスク先行タスクの追加と似ています。 詳しくは、[ 先行タスクエリアを使用した先行タスク関係の作成 ](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md) を参照してください。

1. （オプション）複数のテンプレートタスクを一括編集するには、複数のテンプレートタスクを選択して、テンプレートリストの上部にある「**編集**」をクリックします。
1. （条件付き）テンプレートタスクに関するすべての情報、または複数のタスクに関するすべての情報を同時に編集するには、リストからタスクをクリックして選択し、リストの上部にある **編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。

   新しいエクスペリエンスに **テンプレートタスクを編集** ボックスが表示されます。

   ![ テンプレートの編集タスクの新しいエクスペリエンス ](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >また、リストでテンプレートタスクを選択し、ヘッダーのテンプレートタスク名の右側にある **編集** をクリックして **テンプレートタスクを編集** ボックスを開くこともできます。

   この記事の [ 新しいエクスペリエンスを使用したテンプレートタスクの編集 ](#edit-a-template-task-using-the-new-experience) の節で説明しているように、テンプレートタスクの編集を続行します。

1. （オプション） **テンプレートタスクを編集** ボックスの下部にある **古いエクスペリエンスに切り替える** をクリックして、古いエクスペリエンスの **テンプレートタスクを編集** ボックスを開きます。

   ![ テンプレートタスクを編集 ](assets/edit-template-tasks-box-classic-350x356.png)

1. 次のセクションのいずれかに情報を指定することを検討してください。

   * [概要](#overview)
   * [財務](#finance)
   * [設定](#settings)
   * [割り当て](#assignments)
   * [カスタムフォーム](#custom-forms)
   * [コメント](#comment)

1. この記事の [ 古いエクスペリエンスを使用したテンプレートタスクの編集 ](#edit-a-template-task-using-the-old-experience) の節で説明しているように、テンプレートタスクの編集を続行します。

#### 古いエクスペリエンスを使用したテンプレートタスクの編集

##### 概要 {#overview}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**概要**」をクリックします。

   ![edit_task_overview.png](assets/edit-task-overview-350x438.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名前</strong> </td> 
      <td>テンプレートタスクの名前を指定します。テンプレートタスクを一括編集する場合、このフィールドは表示されません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td>テンプレートタスクに関する追加情報を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>テンプレートタスクに関する情報に関連する web リンクを指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先度</strong> </td> 
      <td> <p>これは、テンプレートタスクに優先順位を付けるための視覚的なフラグです。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>なし</strong> </p> </li> 
        <li> <p><strong>低</strong> </p> </li> 
        <li> <p> <b>標準</b></p> </li> 
        <li> <p><b>高</b> </p> </li> 
        <li> <p><b>緊急</b> </p> </li> 
       </ul> <p>Workfront 管理者が選択したプロジェクト設定に応じて、優先順位の名前が異なる場合があります。優先順位の編集について詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">優先順位の作成とカスタマイズ</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>期間タイプ</strong> </td> 
      <td> <p>このテンプレートから作成される今後のタスクには、この期間タイプが設定されます。<br>期間タイプは、次の関係を識別します。</p> <p>- タスクに割り当てられたリソースの数</p> <p>- タスクを完了するために必要な総労力</p> <p>- タスクの総期間。 </p> <p>期間タイプを使用すると、タスクのニーズに基づいて一貫したリソース割り当てを設定できます。タスクの期間タイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク継続期間と期間タイプの概要</a>を参照してください。</p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">予定割り当て時間</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">予定作業</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">残存作業時間の優先</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">シンプル</span><br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>期間</strong> </td> 
      <td> <p>今後のタスクの期間を分、時間、日、週または月単位で指定します。このテンプレートから作成される将来のタスクは、ここで指定した期間になります。</p> <p>デフォルトで、Workfront は期間を日数単位で測定します。タスクが完了するまで、タスクを未完了のままにしておく時間です。タスクの期間は、タスクの<strong>期間タイプ</strong>が<strong>シンプル</strong>、または<strong>タスクの制約</strong>が<strong>固定日付</strong>である場合は指定できません。</p> <p><b>重要</b></p> <p>期間は、通常、テンプレートのタスクの予定開始日から予定完了日までの期間です。そのため、テンプレートのタイムラインに影響を与えます。これにより、テンプレートから作成される今後のプロジェクトのタイムラインが決まります。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>予定時間数</strong> </td> 
      <td> <p>このテンプレートで作成されたプロジェクトの将来のタスクの予定時間数を指定します。タスクの担当者がタスクを完了するのにかかる実際の時間です。タスクの予定時間数は、<strong>期間タイプ</strong>が<strong>予定割り当て時間</strong>である場合にのみ指定できます。 </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>タスクの制約</strong> </td> 
      <td> <p>このテンプレートから作成されたプロジェクトのタスクには、この制約が適用されます。タスク制約は、タスクを完了する必要があるタイミングを識別します。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li><strong>固定日付</strong>：<strong>予定開始日</strong>および<strong>予定完了日</strong>を指定します。</li> 
        <li><strong>指定日に開始</strong>：<strong>予定開始日</strong>を指定します。</li> 
        <li><strong>指定日に終了</strong>：<strong>予定完了日</strong>を指定します。</li> 
        <li><strong>できるだけ早く</strong> </li> 
        <li><strong>できるだけ遅く</strong> </li> 
        <li style="font-weight: bold;"><strong>最も早い空き時間</strong> </li> 
        <li style="font-weight: bold;"><strong>最も遅い空き時間</strong> </li> 
        <li>指定日までに開始：<strong>予定開始日</strong>を指定します。</li> 
        <li><strong>指定日以後に開始</strong>：<strong>予定開始日</strong>を指定します。</li> 
        <li><strong>これよりも遅く終了しない</strong>：<strong>予定完了日</strong>を指定します。</li> 
        <li><strong>これよりも早く終了しない</strong>：<strong>予定完了日</strong>を指定します。</li> 
       </ul> <p>タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスクの制約の概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">開始日</span><span style="font-weight: normal;">（オプションおよび条件付き）</span> </td> 
      <td> <p> テンプレート タスクの開始日は、タスク制約が次のいずれかである場合にのみ指定できます。</p> 
       <ul> 
        <li>指定日に開始</li> 
        <li>指定日以降に開始</li> 
        <li>指定日までに開始</li> 
        <li>固定日付</li> 
       </ul> <p>タスクが開始される将来のプロジェクトのタイムライン内の日付に対応します。その他のすべての制約については、Workfront がタスク間の先行タスクの依存関係に基づいて開始日を計算します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完了日</strong><span style="font-weight: normal;">（オプションおよび条件付き）</span> </td> 
      <td> <p> テンプレートのタスクの完了日は、タスク制約が次のいずれかの場合にのみ指定できます。</p> 
       <ul style="list-style-type: circle;"> 
        <li>指定日に終了</li> 
        <li>これよりも早く終了しない</li> 
        <li>これよりも遅く終了しない</li> 
        <li>固定日付</li> 
       </ul> <p>これは、タスクが終了される将来のプロジェクトのタイムライン内の日付に対応します。その他のすべての制約については、Workfront が期間と先行タスクの依存関係に基づいて完了日を計算します。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**変更を保存**」をクリックします。

##### 財務 {#finance}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**財務**」をクリックします。

   ![edit_task_finance.png](assets/edit-task-finance-350x216.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>コストの種類</strong> </td> 
      <td> <p>将来のタスクのコストタイプを指定します。これにより、タスクの時間数に基づいて、タスクのコストの計算方法が決まります。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>コストなし</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>固定（毎時）</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>ユーザー（毎時）</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>役割（毎時）</span> </p> </li> 
       </ul> <p>コストの追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>収益タイプ</strong> </td> 
      <td> <p>将来のタスクの収益タイプを指定します。これにより、タスクの時間数に基づいて、タスクの収益の計算方法が決まります。</p> <p style="font-weight: normal;">次のオプションから選択します。 </p> 
       <ul> 
        <li> <p style="font-weight: normal;">請求不可</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー (毎時)</p> </li> 
        <li> <p style="font-weight: normal;">役割（毎時）</p> </li> 
        <li> <p style="font-weight: normal;">固定 (毎時)</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー (毎時) (キャップ付き)</p> </li> 
        <li> <p style="font-weight: normal;">役割（毎時）（キャップ付き）</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー（毎時）+ 固定</p> </li> 
        <li> <p style="font-weight: normal;">役割（毎時）+ 固定</p> </li> 
        <li> <p style="font-weight: normal;">固定収益</p> </li> 
       </ul> <p>収益の追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**変更を保存**」をクリックします。

##### 設定 {#settings}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**設定**」をクリックします。

   ![ テンプレート タスク設定の編集 ](assets/edit-template-tasks-settings-classic-350x231.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>マイルストーン</b></p></strong> </td> 
      <td> <p>選択したテンプレートのタスクに関連付けるマイルストーンを選択します。</p>

   <p><b>重要</b></p>
   <p>このフィールドを表示するには、マイルストーンパスをテンプレートに関連付ける必要があります。詳しくは、<a href="../create-and-manage-templates/edit-templates.md">プロジェクトテンプレートの編集</a>を参照してください。</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>追跡モード</strong> </td> 
      <td> <p>今後のタスクの進捗ステータスの追跡方法を指定します。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>ユーザーが更新する必要あり</strong> </p> </li> 
        <li> <p><strong>時間通りを想定</strong> </p> </li> 
        <li> <p><strong>遅延警告を無視</strong> </p> </li> 
        <li> <p><strong>オートコンプリート</strong> </p> </li> 
        <li> <p><strong>先行タスク</strong> </p> </li> 
       </ul> <p>タスクのトラッキングモードについて詳しくは、<a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">タスクトラッキングモードの概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>承認プロセス</strong> </td> 
      <td> <p>テンプレートタスクに関連付ける承認プロセスを選択します。ユーザーが承認プロセスをテンプレートタスクに関連付けるには、Workfront 管理者がシステムレベルのタスク承認プロセスを定義しておく必要があります。<span>承認プロセスへの管理者アクセス権を持つユーザーは、グループ固有の承認プロセスを作成することもできます。</span> 承認プロセスの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業アイテムの承認プロセスを作成</a>を参照してください。</p> <p>承認プロセスを追加する際は、次の点を考慮してください。 </p> 
       <ul> 
       <li>アクティブな承認プロセスのみがリストに表示されます。 </li> 
       <li> <p>システム全体およびグループ固有の承認プロセスがリストに表示されます。テンプレートのグループ以外のグループに関連付けられている承認プロセスは、リストに表示されません。</p> <p>重要：テンプレートに関連付けられているグループが変更されると、グループ固有の承認プロセスが 1 回限りの承認プロセスになります。プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループと承認プロセスの変更が割り当てられた承認プロセスに及ぼす影響</a>を参照してください。 </p> </li> 
       <li> <p>1 回限りの承認プロセスを追加した場合は、このフィールドに「&lt;Custom&gt;」として表示されます。詳しくは、<a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">新規または既存の承認プロセスを作業に関連付ける</a>を参照してください。 </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>--> </li> 
       <li> <p>テンプレートタスクを一括編集する場合は、次のシナリオが存在します。</p> 
       <ul> 
       <li> <p>同じテンプレートグループからテンプレートタスクを選択した場合、システムレベルとグループレベルの両方の承認プロセスがこのフィールドに表示されます。</p> </li> 
       <li> <p>別のテンプレートグループからテンプレートタスクを選択すると、システムレベルの承認プロセスのみがこのフィールドに表示されます。</p> </li> 
       <li> <p>テンプレートタスクに 1 回限りの承認プロセスが添付されている場合、その承認プロセスは選択したシステムレベル<span>またはグループレベルの承認プロセス</span>で置き換えられます。 </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>リマインダー通知</strong> </td> 
      <td> <p>テンプレートタスクに添付するリマインダー通知を選択します。このテンプレートから作成されたプロジェクトの今後のタスクに添付されます。タスクでリマインダー通知を選択するには、システム管理者がリマインダー通知を設定しておく必要があります。リマインダー通知の設定のについて詳しくは、<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">リマインダー通知の設定</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**変更を保存**」をクリックします。

##### 割り当て {#assignments}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**割り当て**」をクリックします。

   ![assignments_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. 「**割り当て先の追加**」をクリックして、新しい担当者をテンプレートタスクに追加します。ユーザー、役割、チームをタスクに割り当てることができます。1 つのタスクに複数の担当者を割り当てることができます。このテンプレートタスクから作成された場合、今後のタスクには同じリソースが割り当てられます。
1. （オプション）複数の担当者がいる場合は、「**所有者**」ラジオボタンを選択して、タスク責任者またはプライマリ担当者と見なされるユーザーまたは役割を示します。Workfront は、テンプレートタスクに最初に割り当てたユーザーまたは担当業務を、所有者またはプライマリ担当者としてマークします。
1. （条件付きおよびオプション） **期間タイプ** が **計算済み作業** または **作業優先** の場合、担当者ごとに **割り当て %** （割り当て率）を指定します。 これは、担当者がスケジュールからこのタスクに費やすことができる時間です。担当者の配分率を変更すると、タスクの予定時間数が変更されます。
1. （条件付きおよびオプション） **期間タイプ** が **シンプル** の場合、各担当者の **時間** を指定します

   または

   テンプレートタスクの「**予定時間数**」の合計の数を指定します。これにより、合計時間がすべての担当者間で均等に配分されます。

1. （条件付きおよびオプション） **期間タイプ** が「シンプル」の場合は、テンプレートタスクの **期間** を日数で指定します。 これが、このテンプレートから作成されるタスクの期間になります。
1. （オプション）**割り当て先の役割**&#x200B;ドロップダウンメニューから役割を選択します。これが、今後のタスクで担当者が果たせる役割になります。プロファイル内で各担当者に関連付けられている担当業務のみがドロップダウンメニューに表示されます。
1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**変更を保存**」をクリックします。

##### カスタムフォーム {#custom-forms}

タスクがプロジェクトに追加された際に、デフォルトでタスクに自動的に添付されるカスタムフォームを定義できます。 既定のタスクのカスタム フォームを含めるためのプロジェクトの設定については、「プロジェクトの編集 [ の [ タスク ] セクションを参照し ](../../../manage-work/projects/manage-projects/edit-projects.md) ください。

また、カスタムフォームをテンプレートタスクに追加することで、テンプレートからプロジェクトを作成する際に、プロジェクトの今後のタスクにカスタムフォームを追加することもできます。

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**カスタムフォーム**」をクリックします。

   ![custom_forms_edit_task.png](assets/custom-forms-edit-task-350x136.png)

1. テンプレートタスクに関連付けるカスタムフォームを選択します。

   このフィールドで選択できるカスタムフォームを作成する必要があります。
アクティブなカスタムフォームのみがリストに表示されます。
カスタムフォームの作成について詳しくは、「[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。
テンプレートタスクには最大 10 個のカスタムフォームを追加できます。
フォームは、テンプレートから作成されたタスクに自動的に追加されます。
1. （条件付きおよびオプション）テンプレートタスクにカスタム フォームを添付した場合は、フォーム上のフィールドを編集します。テンプレートタスクを保存する前に、すべての必須フィールドを指定する必要があります。

   >[!NOTE]
   >
   >Workfront 管理者がカスタムフォーム内のセクションに権限を設定する方法によっては、特定のカスタムフォーム上の同じフィールドを誰もが表示または編集できるわけではありません。カスタムフォームのセクション内のフィールドを編集する権限は、テンプレートタスクまたは将来のタスクに対して持っている権限によって異なります。\
   >カスタムフォームのセクションに対する権限の設定については、[カスタムフォームを共有する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)を参照してください。\
   >タスク権限の設定については、[タスクを共有する](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)を参照してください。\
   >テンプレートの権限の設定については、[テンプレートの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)を参照してください。

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**変更を保存**」をクリックします。

##### コメント {#comment}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**コメント**」をクリックします。

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. 使用可能なフィールドにあるテンプレートタスクの、更新ストリームに表示するコメントを指定します。このコメントは、テンプレートおよびテンプレートタスクへの表示アクセス権とメモの表示アクセス権を持つすべてのユーザーに表示されます。
1. 「**変更を保存**」をクリックします。

   本ユーザーまたは別のユーザーがこのテンプレートからプロジェクトを作成すると、テンプレートタスクに適用したすべての設定がプロジェクトタスクの設定になります。

#### 新しいエクスペリエンスを使用したテンプレートタスクの編集

新しいエクスペリエンスで **テンプレートタスクを編集** ボックスを開いた後、次の節のいずれかで情報を指定することを検討してください。

* [テンプレート タスク名](#template-task-name)
* [概要](#overview-1)
* [割り当て](#assignments-1)
* [財務](#finance-1)
* [カスタムフォーム](#custom-forms-1)
* [設定](#settings-1)
* [コメント](#comment-1)

##### テンプレート タスク名

>[!TIP]
>
>テンプレートタスクを一括編集する場合、「テンプレートタスク名」セクションは使用できません。


1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. [ テンプレート タスクの編集 ] ボックスで、[**テンプレート タスク名**] をクリックし、テンプレート タスクの名前を追加します。

   テンプレートタスクを一括編集する場合、このビューは使用できません。

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

##### 概要 {#overview-1}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **概要** をクリックします。

   ![ テンプレートタスク編集の概要セクション ](assets/template-task-edit-overview.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td>テンプレートタスクに関する追加情報を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先度</strong> </td> 
      <td> <p>これは、テンプレートタスクに優先順位を付けるための視覚的なフラグです。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>なし</strong> </p> </li> 
        <li> <p><strong>低</strong> </p> </li> 
        <li> <p> <b>標準</b></p> </li> 
        <li> <p><b>高</b> </p> </li> 
        <li> <p><b>緊急</b> </p> </li> 
       </ul> <p>Workfront 管理者が選択したプロジェクト設定に応じて、優先順位の名前が異なる場合があります。優先度の編集について詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">優先度の作成およびカスタマイズ</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>タスクの制約</strong> </td> 
      <td> <p>このテンプレートから作成されたプロジェクトのタスクには、この制約が適用されます。タスク制約は、タスクを完了する必要があるタイミングを識別します。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li><strong>固定日付</strong>：<strong>予定開始日</strong>および<strong>予定完了日</strong>を指定します。</li> 
        <li><strong>指定日に開始</strong>：<strong>予定開始日</strong>を指定します。</li> 
        <li><strong>指定日に終了</strong>：<strong>予定完了日</strong>を指定します。</li> 
        <li><strong>できるだけ早く</strong> </li> 
        <li><strong>できるだけ遅く</strong> </li> 
        <li style="font-weight: bold;"><strong>最も早い空き時間</strong> </li> 
        <li style="font-weight: bold;"><strong>最も遅い空き時間</strong> </li> 
        <li>指定日までに開始：<strong>予定開始日</strong>を指定します。</li> 
        <li><strong>指定日以後に開始</strong>：<strong>予定開始日</strong>を指定します。</li> 
        <li><strong>これよりも遅く終了しない</strong>：<strong>予定完了日</strong>を指定します。</li> 
        <li><strong>これよりも早く終了しない</strong>：<strong>予定完了日</strong>を指定します。</li> 
       </ul> <p>タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスクの制約の概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">開始日</span><span style="font-weight: normal;">（オプションおよび条件付き）</span> </td> 
      <td> <p> テンプレート タスクの開始日は、タスク制約が次のいずれかである場合にのみ指定できます。</p> 
       <ul> 
        <li>指定日に開始</li> 
        <li>指定日以降に開始</li> 
        <li>指定日までに開始</li> 
        <li>固定日付</li> 
       </ul> <p>タスクが開始される将来のプロジェクトのタイムライン内の日付に対応します。その他のすべての制約については、Workfront がタスク間の先行タスクの依存関係に基づいて開始日を計算します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完了日</strong><span style="font-weight: normal;">（オプションおよび条件付き）</span> </td> 
      <td> <p> テンプレートのタスクの完了日は、タスク制約が次のいずれかの場合にのみ指定できます。</p> 
       <ul style="list-style-type: circle;"> 
        <li>指定日に終了</li> 
        <li>これよりも早く終了しない</li> 
        <li>これよりも遅く終了しない</li> 
        <li>固定日付</li> 
       </ul> <p>これは、タスクが終了される将来のプロジェクトのタイムライン内の日付に対応します。その他のすべての制約については、Workfront が期間と先行タスクの依存関係に基づいて完了日を計算します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>テンプレートタスクに関する情報に関連する web リンクを指定します。</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong> 作業量 </strong> </td> 
      <td>次のオプションから選択します。
      <ul><li>小</li>
      <li>中</li>
      <li>大</li></ul>

   <p><b>重要</b></p>
      <p>テンプレート タスクの編集時に [ 作業量 ] フィールドが表示されるのは、テンプレート タスクの編集時に [<b> 作業量を使用してタスクの予定時間数を自動的に計算する </b> 設定を選択した場合のみです。</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

##### 割り当て {#assignments-1}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **割り当て** をクリックします。

   ![ テンプレート タスク編集割り当て ](assets/template-task-edit-assignments.png)

1. 「**ユーザー、役割、チームを検索**」フィールドに担当者の名前の入力を開始し、リストに表示されたら選択します

   または

   「**自分に割り当て**」をクリックして、テンプレートタスクを自分に割り当てます。
1. 次の情報の更新を検討してください。

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody>

   <tr> 
         <td role="rowheader"><strong>期間タイプ</strong> </td> 
         <td> <p>このテンプレートから作成される今後のタスクには、この期間タイプが設定されます。<br> 期間タイプは、次の項目間の関係を示します。</p> 
         <ul>
         <li><p>タスクに割り当てられたリソースの数</p> </li>
         <li><p>タスクの完了に必要な合計作業量</p></li> 
         <li><p>タスクの合計期間 </p></li></ul> <p>期間タイプを使用すると、タスクのニーズに基づいて一貫したリソース割り当てを設定できます。 タスクの期間タイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク継続期間と期間タイプの概要</a>を参照してください。</p> <p>次のオプションから選択します。</p> 
         <ul> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">予定割り当て時間</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">予定作業</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">残存作業時間の優先</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">シンプル</span><br> </p> </li> 
         </ul> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>期間</strong> </td> 
         <td> <p>今後のタスクの期間を分、時間、日、週または月単位で指定します。このテンプレートから作成される将来のタスクは、ここで指定した期間になります。</p> <p>デフォルトで、Workfront は期間を日数単位で測定します。タスクが完了するまで、タスクを未完了のままにしておく時間です。タスクの期間は、タスクの<strong>期間タイプ</strong>が<strong>シンプル</strong>、または<strong>タスクの制約</strong>が<strong>固定日付</strong>である場合は指定できません。</p> <p><b>重要</b></p> <p>期間は、通常、テンプレートのタスクの予定開始日から予定完了日までの期間です。そのため、テンプレートのタイムラインに影響を与えます。これにより、テンプレートから作成される今後のプロジェクトのタイムラインが決まります。 </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>予定時間数</strong> </td> 
         <td> <p>このテンプレートで作成されたプロジェクトの将来のタスクの予定時間数を指定します。タスクの担当者がタスクを完了するのにかかる実際の時間です。タスクの予定時間数は、<strong>期間タイプ</strong>が<strong>予定割り当て時間</strong>である場合にのみ指定できます。 </p> </td> 
      </tr> 
   </tbody> 
      </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

##### 財務 {#finance-1}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **財務** をクリックします。

   ![ テンプレート タスク編集財務セクション ](assets/template-task-edit-finance.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>コストの種類</strong> </td> 
      <td> <p>将来のタスクのコストタイプを指定します。これにより、タスクの時間数に基づいて、タスクのコストの計算方法が決まります。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>コストなし</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>固定（毎時）</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>ユーザー（毎時）</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>役割（毎時）</span> </p> </li> 
       </ul> <p>コストの追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>収益タイプ</strong> </td> 
      <td> <p>将来のタスクの収益タイプを指定します。これにより、タスクの時間数に基づいて、タスクの収益の計算方法が決まります。</p> <p style="font-weight: normal;">次のオプションから選択します。 </p> 
       <ul> 
        <li> <p style="font-weight: normal;">請求不可</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー (毎時)</p> </li> 
        <li> <p style="font-weight: normal;">役割（毎時）</p> </li> 
        <li> <p style="font-weight: normal;">固定 (毎時)</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー (毎時) (キャップ付き)</p> </li> 
        <li> <p style="font-weight: normal;">役割（毎時）（キャップ付き）</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー（毎時）+ 固定</p> </li> 
        <li> <p style="font-weight: normal;">役割（毎時）+ 固定</p> </li> 
        <li> <p style="font-weight: normal;">固定収益</p> </li> 
       </ul> <p>収益の追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

##### カスタムフォーム {#custom-forms-1}

タスクがプロジェクトに追加された際に、デフォルトでタスクに自動的に添付されるカスタムフォームを定義できます。 既定のタスクのカスタム フォームを含めるためのプロジェクトの設定については、「プロジェクトの編集 [ の [ タスク ] セクションを参照し ](../../../manage-work/projects/manage-projects/edit-projects.md) ください。

また、カスタムフォームをテンプレートタスクに追加することで、テンプレートからプロジェクトを作成する際に、プロジェクトの今後のタスクにカスタムフォームを追加することもできます。

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **カスタムForms** をクリックします。

   ![ テンプレート タスクのカスタム フォームの編集セクション ](assets/template-task-edit-custom-forms.png)

1. テンプレートタスクに関連付けるカスタムフォームを選択します。

   このフィールドで選択できるカスタムフォームを作成する必要があります。
アクティブなカスタムフォームのみがリストに表示されます。

   カスタムフォームの作成について詳しくは、「[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

   テンプレートタスクには最大 10 個のカスタムフォームを追加できます。
フォームは、テンプレートから作成されたタスクに自動的に追加されます。
1. （条件付きおよびオプション）テンプレートタスクにカスタム フォームを添付した場合は、フォーム上のフィールドを編集します。テンプレートタスクを保存する前に、すべての必須フィールドを指定する必要があります。

   >[!NOTE]
   >
   >Workfront 管理者がカスタムフォーム内のセクションに権限を設定する方法によっては、特定のカスタムフォーム上の同じフィールドを誰もが表示または編集できるわけではありません。カスタムフォームのセクション内のフィールドを編集する権限は、テンプレートタスクまたは将来のタスクに対して持っている権限によって異なります。\
   >カスタムフォームのセクションに対する権限の設定については、[カスタムフォームを共有する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)を参照してください。\
   >タスク権限の設定については、[タスクを共有する](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)を参照してください。\
   >テンプレートの権限の設定については、[テンプレートの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)を参照してください。

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

##### 設定 {#settings-1}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. **テンプレート タスクを編集ボックス** で、左パネルの **設定** をクリックします。

   ![ テンプレート タスク編集設定セクション ](assets/template-task-edit-settings.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>マイルストーン</b></p></strong> </td> 
      <td> <p>選択したテンプレートのタスクに関連付けるマイルストーンを選択します。</p>

   <p><b>重要</b></p>
   <p>このフィールドを表示するには、マイルストーンパスをテンプレートに関連付ける必要があります。詳しくは、<a href="../create-and-manage-templates/edit-templates.md">プロジェクトテンプレートの編集</a>を参照してください。</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>追跡モード</strong> </td> 
      <td> <p>今後のタスクの進捗ステータスの追跡方法を指定します。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>ユーザーが更新する必要あり</strong> </p> </li> 
        <li> <p><strong>時間通りを想定</strong> </p> </li> 
        <li> <p><strong>遅延警告を無視</strong> </p> </li> 
        <li> <p><strong>オートコンプリート</strong> </p> </li> 
        <li> <p><strong>先行タスク</strong> </p> </li> 
       </ul> <p>タスクのトラッキングモードについて詳しくは、<a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">タスクトラッキングモードの概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>リマインダー通知</strong> </td> 
      <td> <p>テンプレートタスクに添付するリマインダー通知を選択します。このテンプレートから作成されたプロジェクトの今後のタスクに添付されます。タスクでリマインダー通知を選択するには、システム管理者がリマインダー通知を設定しておく必要があります。リマインダー通知の設定のについて詳しくは、<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">リマインダー通知の設定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>承認プロセス</strong> </td> 
      <td> <p>テンプレートタスクに関連付ける承認プロセスを選択します。ユーザーが承認プロセスをテンプレートタスクに関連付けるには、Workfront 管理者がシステムレベルのタスク承認プロセスを定義しておく必要があります。<span>承認プロセスへの管理者アクセス権を持つユーザーは、グループ固有の承認プロセスを作成することもできます。</span> 承認プロセスの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業アイテムの承認プロセスを作成</a>を参照してください。</p> <p>承認プロセスを追加する際は、次の点を考慮してください。 </p> 
       <ul> 
       <li>アクティブな承認プロセスのみがリストに表示されます。 </li> 
       <li> <p>システム全体およびグループ固有の承認プロセスがリストに表示されます。テンプレートのグループ以外のグループに関連付けられている承認プロセスは、リストに表示されません。</p> <p>重要：テンプレートに関連付けられているグループが変更されると、グループ固有の承認プロセスが 1 回限りの承認プロセスになります。プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループと承認プロセスの変更が割り当てられた承認プロセスに及ぼす影響</a>を参照してください。 </p> </li> 
       <li> <p>1 回限りの承認プロセスを追加した場合は、このフィールドに「&lt;Custom&gt;」として表示されます。詳しくは、<a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">新規または既存の承認プロセスを作業に関連付ける</a>を参照してください。 </p>  </li> 
       <li> <p>テンプレートタスクを一括編集する場合は、次のシナリオが存在します。</p> 
       <ul> 
       <li> <p>同じテンプレートグループからテンプレートタスクを選択した場合、システムレベルとグループレベルの両方の承認プロセスがこのフィールドに表示されます。</p> </li> 
       <li> <p>別のテンプレートグループからテンプレートタスクを選択すると、システムレベルの承認プロセスのみがこのフィールドに表示されます。</p> </li> 
       <li> <p>テンプレートタスクに 1 回限りの承認プロセスが添付されている場合、その承認プロセスは選択したシステムレベル<span>またはグループレベルの承認プロセス</span>で置き換えられます。 </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr>

   </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

##### コメント {#comment-1}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **コメント** をクリックします。

   ![ テンプレート タスクのコメント セクションの編集 ](assets/template-task-edit-comment.png)

1. **テンプレートタスクに更新を追加** 領域で、テンプレートタスクの更新ストリームに表示するコメントを使用可能フィールドに指定します。 このコメントは、テンプレートおよびテンプレートタスクへの表示アクセス権とメモの表示アクセス権を持つすべてのユーザーに表示されます。
1. 「**保存**」をクリックします。

   本ユーザーまたは別のユーザーがこのテンプレートからプロジェクトを作成すると、テンプレートタスクに適用したすべての設定がプロジェクトタスクの設定になります。


<div class="preview">

### プレビュー環境でのテンプレートタスクの編集

テンプレートタスクを編集は、テンプレートタスクを編集またはテンプレートタスクの詳細領域を使用して編集できます。

{{step1-to-templates}}

1. テンプレートの名前をクリックして開きます。
1. 左パネルの「**テンプレートタスク**」をクリックします。
1. リスト内のテンプレートタスクの名前をクリックして、テンプレートタスクを開きます。
1. テンプレートタスクに関する制限付きの情報を編集するには、次の手順を実行します。
   1. （任意）左側のパネルで「**更新**」をクリックして、テンプレートタスクに更新を追加します。 テンプレートを使用してプロジェクトを作成する場合、テンプレートタスクの更新がプロジェクトタスクに転送されない。
   1. （任意）左側のパネルで **ドキュメント** をクリックして、ドキュメントをテンプレートタスクに追加します。 テンプレートを使用してプロジェクトを作成すると、ドキュメントはプロジェクトタスクに転送されます。
   1. （条件付き）テンプレートタスクに関する限られた情報を編集するには、左パネルで「**テンプレートタスクの詳細**」をクリックし、詳細セクションのエリアに移動して、それぞれのエリアの情報を編集します。
   1. （オプション）次のいずれかの操作を行います。
      * **すべて折りたたむ** アイコン ![ すべて折りたたむアイコン ](assets/collapse-all-icon.png) をクリックすると、すべての領域が折りたたまれます。
      * **編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックして、下の任意の領域から選択するか、**すべて編集** をクリックして、すべての領域の情報を編集します。

         * 概要
         * カスタムForms
カスタムフォームの名前は、テンプレートタスクに添付されたカスタムフォームがある場合にのみ表示されます。
         * 財務

        >[!TIP]
        >
        >「詳細」領域に表示されるすべてのフィールドについて詳しくは、以下に説明するように、「テンプレートタスクを編集」ボックスを使用してすべてのフィールドを引き続き編集します。

   1. （任意）左側のパネルで「**サブタスク**」セクションをクリックして、テンプレートタスクの子を追加します。 テンプレートタスクのサブタスクの追加は、プロジェクトタスクのサブタスクの追加と似ています。 詳しくは、「サブタスクの作成」の「タスクサブタスクからサブタスクを作成する [ 節を参照してくだ ](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md) い。
   1. （任意）左側のパネルで **費用** をクリックし、テンプレートタスクに費用を追加します。 テンプレートタスクの費用は、テンプレートを使用してプロジェクトを作成する際に、将来のプロジェクトタスクに転送されます。
   1. （任意）左側のパネルの **承認** をクリックして承認を作成するか、テンプレートタスクにグローバルまたはグループレベルの承認を添付します。 承認は、今後のプロジェクトタスクに転送されます。
   1. （任意）左側のパネルで「**先行タスク**」セクションをクリックして、テンプレートタスクの先行タスクを追加します。 テンプレートタスク先行タスクの追加は、プロジェクトタスク先行タスクの追加と似ています。 詳しくは、[ 先行タスクエリアを使用した先行タスク関係の作成 ](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md) を参照してください。

1. （条件付き）テンプレートタスクまたは複数のタスクに関するすべての情報を同時に編集するには、リストから選択をクリックし、リストの上部にある **編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。

   「**テンプレートタスクの編集**」ボックスが表示されます。

   ![ テンプレートの編集タスクの新しいエクスペリエンス ](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >また、リストでテンプレートタスクを選択し、ヘッダーのテンプレートタスク名の右側にある **編集** をクリックして **テンプレートタスクを編集** ボックスを開くこともできます。

1. 次のセクションのいずれかに情報を指定することを検討してください。

* [テンプレート タスク名](#template-task-name)
* [概要](#overview-2)
* [割り当て](#assignments-2)
* [財務](#finance-2)
* [カスタムフォーム](#custom-forms-2)
* [設定](#settings-2)
* [コメント](#comment-2)

1. 以下の節で説明するように、テンプレートタスクの編集を続けます。

#### テンプレート タスク名

>[!TIP]
>
>テンプレートタスクを一括編集する場合、「テンプレートタスク名」セクションは使用できません。


1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. [ テンプレート タスクの編集 ] ボックスで、[**テンプレート タスク名**] をクリックし、テンプレート タスクの名前を追加します。

   テンプレートタスクを一括編集する場合、このビューは使用できません。

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

#### 概要 {#overview-2}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **概要** をクリックします。

   ![ テンプレートタスク編集の概要セクション ](assets/template-task-edit-overview.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td>テンプレートタスクに関する追加情報を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先度</strong> </td> 
      <td> <p>これは、テンプレートタスクに優先順位を付けるための視覚的なフラグです。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>なし</strong> </p> </li> 
        <li> <p><strong>低</strong> </p> </li> 
        <li> <p> <b>標準</b></p> </li> 
        <li> <p><b>高</b> </p> </li> 
        <li> <p><b>緊急</b> </p> </li> 
       </ul> <p>Workfront 管理者が選択したプロジェクト設定に応じて、優先順位の名前が異なる場合があります。優先度の編集について詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">優先度の作成およびカスタマイズ</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>タスクの制約</strong> </td> 
      <td> <p>このテンプレートから作成されたプロジェクトのタスクには、この制約が適用されます。タスク制約は、タスクを完了する必要があるタイミングを識別します。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li><strong>固定日付</strong>：<strong>予定開始日</strong>および<strong>予定完了日</strong>を指定します。</li> 
        <li><strong>指定日に開始</strong>：<strong>予定開始日</strong>を指定します。</li> 
        <li><strong>指定日に終了</strong>：<strong>予定完了日</strong>を指定します。</li> 
        <li><strong>できるだけ早く</strong> </li> 
        <li><strong>できるだけ遅く</strong> </li> 
        <li style="font-weight: bold;"><strong>最も早い空き時間</strong> </li> 
        <li style="font-weight: bold;"><strong>最も遅い空き時間</strong> </li> 
        <li>指定日までに開始：<strong>予定開始日</strong>を指定します。</li> 
        <li><strong>指定日以後に開始</strong>：<strong>予定開始日</strong>を指定します。</li> 
        <li><strong>これよりも遅く終了しない</strong>：<strong>予定完了日</strong>を指定します。</li> 
        <li><strong>これよりも早く終了しない</strong>：<strong>予定完了日</strong>を指定します。</li> 
       </ul> <p>タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスクの制約の概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">開始日</span><span style="font-weight: normal;">（オプションおよび条件付き）</span> </td> 
      <td> <p> テンプレート タスクの開始日は、タスク制約が次のいずれかである場合にのみ指定できます。</p> 
       <ul> 
        <li>指定日に開始</li> 
        <li>指定日以降に開始</li> 
        <li>指定日までに開始</li> 
        <li>固定日付</li> 
       </ul> <p>タスクが開始される将来のプロジェクトのタイムライン内の日付に対応します。その他のすべての制約については、Workfront がタスク間の先行タスクの依存関係に基づいて開始日を計算します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完了日</strong><span style="font-weight: normal;">（オプションおよび条件付き）</span> </td> 
      <td> <p> テンプレートのタスクの完了日は、タスク制約が次のいずれかの場合にのみ指定できます。</p> 
       <ul style="list-style-type: circle;"> 
        <li>指定日に終了</li> 
        <li>これよりも早く終了しない</li> 
        <li>これよりも遅く終了しない</li> 
        <li>固定日付</li> 
       </ul> <p>これは、タスクが終了される将来のプロジェクトのタイムライン内の日付に対応します。その他のすべての制約については、Workfront が期間と先行タスクの依存関係に基づいて完了日を計算します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>テンプレートタスクに関する情報に関連する web リンクを指定します。</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong> 作業量 </strong> </td> 
      <td>次のオプションから選択します。
      <ul><li>小</li>
      <li>中</li>
      <li>大</li></ul>

   <p><b>重要</b></p>
      <p>テンプレート タスクの編集時に [ 作業量 ] フィールドが表示されるのは、テンプレート タスクの編集時に [<b> 作業量を使用してタスクの予定時間数を自動的に計算する </b> 設定を選択した場合のみです。</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

#### 割り当て {#assignments-2}

1. 上記の説明に従って、テンプレートタスクの編集を開始します。
1. 左側のパネルで「**割り当て**」をクリックします。

   **割り当て** エリアが開きます。

   ![ テンプレートタスクの割り当て ](assets/assignments-edit-template-tasks-box.png)

1. **ユーザー、担当業務、またはチームを検索** フィールドにユーザー、担当業務、またはチームの名前を入力し始め、リストに表示されたら選択します。

1. 次の情報を更新します。

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">期間タイプ</td> 
   <td> <p>これにより、以下の項目間の関係が明らかになります。 </p> 
   <ul> 
   <li> <p>タスクに割り当てられたリソースの数 </p> </li> 
   <li> <p>タスクの完了に必要な合計作業量 </p> </li> 
   <li> <p> タスクの合計期間。 </p> </li> 
   </ul> <p>Workfront管理者またはグループ管理者が、システムまたはグループのタスクに対してデフォルトの「期間タイプ」設定を選択します。 プロジェクトのデフォルトの設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref"> システム全体のタスクおよびイシューの環境設定の設定 </a> を参照してください。 </p> <p>期間タイプを使用すると、タスクのニーズに基づいて一貫したリソース割り当てを設定できます。タスクの期間タイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク継続期間と期間タイプの概要</a>を参照してください。 </p> <p>次のオプションから選択します。 </p> 
   <ul> 
   <li> <p>予定割り当て時間 </p> </li> 
   <li> <p> 予定作業 </p> </li> 
   <li> <p>残存作業時間の優先 </p> </li> 
   <li> <p>シンプル</p> </li> 
   </ul> </td> 
   </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">発生ごとの所要時間</td> 
   <td> <p>これは、定期タスクの親にのみ表示されます。タスクが作成された時点で定義された、各定期タスクの期間が表示されます。定期タスクの作成について詳しくは、<a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">定期タスクの作成</a>を参照してください。 </p> <p> <b>メモ</b>

   個々の定期タスクで変更された期間には、このフィールドに示された値は表示されません。 </p> </td>
   </tr> 
   <tr> 
   <td role="rowheader">期間</td> 
   <td> 
   <div> 
   <div> 
   <p>タスクが完了するまでタスクを開いたままにしておくことができる時間です。 </p> 
   <p><b>重要</b></p>
   <p>タスク期間は通常、予定開始日から予定完了日までの時間で、プロジェクトのタイムラインに影響します。</p> 
   <p>タスクの期間と時間の単位を指定するには、以下を行います。</p> 
   <ul> 
   <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">時間の長さを入力し、ドロップダウンメニューに表示される時間の単位から選択します。</p> <p><b>ヒント</b></p>
   タスクリストのタスクの期間を更新する際は、時間の単位の省略形を使用できます。 </p> </li> 
   </ul> 
   <p> 次の表にある通常時間または経過時間のオプションから選択できます。 </p> 
   <table style="table-layout:auto"> 
   <col> 
   <col data-mc-conditions=""> 
   <tbody> 
   <tr> 
   <td>時間の単位</td> 
   <td>省略形</td> 
   </tr> 
   <tr> 
   <td>分</td> 
   <td>M</td> 
   </tr> 
   <tr> 
   <td>時間</td> 
   <td>H</td> 
   </tr> 
   <tr> 
   <td>日 これがデフォルトです。 </td> 
   <td>D</td> 
   </tr> 
   <tr> 
   <td>週</td> 
   <td>W</td> 
   </tr> 
   <tr> 
   <td>か月</td> 
   <td>T</td> 
   </tr> 
   <tr> 
   <td>経過時間数 (分)</td> 
   <td>EM</td> 
   </tr> 
   <tr> 
   <td>経過時間数</td> 
   <td>EH</td> 
   </tr> 
   <tr> 
   <td>経過日数</td> 
   <td>ED</td> 
   </tr> 
   <tr> 
   <td>経過週数</td> 
   <td>EW</td> 
   </tr> 
   <tr> 
   <td>経過月数</td> 
   <td>ET</td> 
   </tr> 
   </tbody> 
   </table>

   <p><b>メモ</b>

   <p>経過時間は、タスクの期間の時間単位です。タスクの予定開始日から予定完了日までの時間で、休日、週末および休暇を含みます。つまり、経過時間はカレンダーの日数の経過です。

   通常の時間は、休日、週末および休暇を考慮し、これらをタスクの期間から除外します。タスクの期間について詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>を参照してください。 </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">予定時間数</td> 
   <td> <p>タスクの予定時間数を時間単位で指定します。 これは、タスクの担当者が完了するまでにかかる実際の時間です。 タスクの予定時間数を指定できるのは、[ 期間タイプ ] が [ 割り当て計算 ] に設定されている場合のみです。 期間のタイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>を参照してください。</p> 
   <b>メモ</b>
   <p>
   繰り返しタスクを作成する場合、予定時間数はそれぞれの繰り返しタスクの時間です。親タスクの予定時間数は、すべてのタスクからのすべての予定時間数の合計です。繰り返しタスクの作成について詳しくは、<a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">繰り返しタスクを作成</a>を参照してください。
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">配分</td> 
   <td> <p>タスクの制約事項が「予定作業」または「残存作業時間の優先」である場合は、それぞれの担当者の<strong>配分 ％</strong>（配分率）を指定します。これは、担当者がスケジュールからこのタスクに費やすことができる時間です。担当者の配分率を変更すると、タスクの予定時間数が変更されます。 </p> <p>タスクの制約事項が「シンプル」の場合は、以下の項目を指定することができます。</p> 
   <ul> 
   <li> <p>それぞれの担当者の時間配分数。</p> </li> 
   <li> <p>タスクの予定時間数</p> </li> 
   <li> <p>タスクの期間</p> </li> 
   </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">割り当て先の役割</td> 
   <td> <p>個人を担当者として選択した場合は、「<strong>担当者の役割</strong>」ドロップダウンメニューから役割を選択します。これは、担当者がこのタスクで果たすことができる役割です。 </p> <p><b>ヒント</b>

   プロファイル内で各担当者に関連付けられている担当業務のみがドロップダウンメニューに表示されます。</p> </td>
   </tr> 
   </tbody> 
   </table>

1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

#### 財務 {#finance-2}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **財務** をクリックします。

   ![ テンプレート タスク編集財務セクション ](assets/template-task-edit-finance.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>コストの種類</strong> </td> 
      <td> <p>将来のタスクのコストタイプを指定します。これにより、タスクの時間数に基づいて、タスクのコストの計算方法が決まります。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>コストなし</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>固定（毎時）</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>ユーザー（毎時）</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>役割（毎時）</span> </p> </li> 
       </ul> <p>コストの追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>収益タイプ</strong> </td> 
      <td> <p>将来のタスクの収益タイプを指定します。これにより、タスクの時間数に基づいて、タスクの収益の計算方法が決まります。</p> <p style="font-weight: normal;">次のオプションから選択します。 </p> 
       <ul> 
        <li> <p style="font-weight: normal;">請求不可</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー (毎時)</p> </li> 
        <li> <p style="font-weight: normal;">役割（毎時）</p> </li> 
        <li> <p style="font-weight: normal;">固定 (毎時)</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー (毎時) (キャップ付き)</p> </li> 
        <li> <p style="font-weight: normal;">役割（毎時）（キャップ付き）</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー（毎時）+ 固定</p> </li> 
        <li> <p style="font-weight: normal;">役割（毎時）+ 固定</p> </li> 
        <li> <p style="font-weight: normal;">固定収益</p> </li> 
       </ul> <p>収益の追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

#### カスタムフォーム {#custom-forms-2}

タスクがプロジェクトに追加された際に、デフォルトでタスクに自動的に添付されるカスタムフォームを定義できます。 既定のタスクのカスタム フォームを含めるためのプロジェクトの設定については、「プロジェクトの編集 [ の [ タスク ] セクションを参照し ](../../../manage-work/projects/manage-projects/edit-projects.md) ください。

また、カスタムフォームをテンプレートタスクに追加することで、テンプレートからプロジェクトを作成する際に、プロジェクトの今後のタスクにカスタムフォームを追加することもできます。

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **カスタムForms** をクリックします。

   ![ テンプレート タスクのカスタム フォームの編集セクション ](assets/template-task-edit-custom-forms.png)

1. テンプレートタスクに関連付けるカスタムフォームを選択します。

   このフィールドで選択できるカスタムフォームを作成する必要があります。
アクティブなカスタムフォームのみがリストに表示されます。

   カスタムフォームの作成について詳しくは、「[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

   テンプレートタスクには最大 10 個のカスタムフォームを追加できます。
フォームは、テンプレートから作成されたタスクに自動的に追加されます。
1. （条件付きおよびオプション）テンプレートタスクにカスタム フォームを添付した場合は、フォーム上のフィールドを編集します。テンプレートタスクを保存する前に、すべての必須フィールドを指定する必要があります。

   >[!NOTE]
   >
   >Workfront 管理者がカスタムフォーム内のセクションに権限を設定する方法によっては、特定のカスタムフォーム上の同じフィールドを誰もが表示または編集できるわけではありません。カスタムフォームのセクション内のフィールドを編集する権限は、テンプレートタスクまたは将来のタスクに対して持っている権限によって異なります。\
   >カスタムフォームのセクションに対する権限の設定については、[カスタムフォームを共有する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)を参照してください。\
   >タスク権限の設定については、[タスクを共有する](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)を参照してください。\
   >テンプレートの権限の設定については、[テンプレートの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)を参照してください。

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

#### 設定 {#settings-2}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. **テンプレート タスクを編集ボックス** で、左パネルの **設定** をクリックします。

   ![ テンプレート タスク編集設定セクション ](assets/template-task-edit-settings.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>マイルストーン</b></p></strong> </td> 
      <td> <p>選択したテンプレートのタスクに関連付けるマイルストーンを選択します。</p>

   <p><b>重要</b></p>
   <p>このフィールドを表示するには、マイルストーンパスをテンプレートに関連付ける必要があります。詳しくは、<a href="../create-and-manage-templates/edit-templates.md">プロジェクトテンプレートの編集</a>を参照してください。</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>追跡モード</strong> </td> 
      <td> <p>今後のタスクの進捗ステータスの追跡方法を指定します。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>ユーザーが更新する必要あり</strong> </p> </li> 
        <li> <p><strong>時間通りを想定</strong> </p> </li> 
        <li> <p><strong>遅延警告を無視</strong> </p> </li> 
        <li> <p><strong>オートコンプリート</strong> </p> </li> 
        <li> <p><strong>先行タスク</strong> </p> </li> 
       </ul> <p>タスクのトラッキングモードについて詳しくは、<a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">タスクトラッキングモードの概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>リマインダー通知</strong> </td> 
      <td> <p>テンプレートタスクに添付するリマインダー通知を選択します。このテンプレートから作成されたプロジェクトの今後のタスクに添付されます。タスクでリマインダー通知を選択するには、システム管理者がリマインダー通知を設定しておく必要があります。リマインダー通知の設定のについて詳しくは、<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">リマインダー通知の設定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>承認プロセス</strong> </td> 
      <td> <p>テンプレートタスクに関連付ける承認プロセスを選択します。ユーザーが承認プロセスをテンプレートタスクに関連付けるには、Workfront 管理者がシステムレベルのタスク承認プロセスを定義しておく必要があります。<span>承認プロセスへの管理者アクセス権を持つユーザーは、グループ固有の承認プロセスを作成することもできます。</span> 承認プロセスの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業アイテムの承認プロセスを作成</a>を参照してください。</p> <p>承認プロセスを追加する際は、次の点を考慮してください。 </p> 
       <ul> 
       <li>アクティブな承認プロセスのみがリストに表示されます。 </li> 
       <li> <p>システム全体およびグループ固有の承認プロセスがリストに表示されます。テンプレートのグループ以外のグループに関連付けられている承認プロセスは、リストに表示されません。</p> <p>重要：テンプレートに関連付けられているグループが変更されると、グループ固有の承認プロセスが 1 回限りの承認プロセスになります。プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループと承認プロセスの変更が割り当てられた承認プロセスに及ぼす影響</a>を参照してください。 </p> </li> 
       <li> <p>1 回限りの承認プロセスを追加した場合は、このフィールドに「&lt;Custom&gt;」として表示されます。詳しくは、<a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">新規または既存の承認プロセスを作業に関連付ける</a>を参照してください。 </p>  </li> 
       <li> <p>テンプレートタスクを一括編集する場合は、次のシナリオが存在します。</p> 
       <ul> 
       <li> <p>同じテンプレートグループからテンプレートタスクを選択した場合、システムレベルとグループレベルの両方の承認プロセスがこのフィールドに表示されます。</p> </li> 
       <li> <p>別のテンプレートグループからテンプレートタスクを選択すると、システムレベルの承認プロセスのみがこのフィールドに表示されます。</p> </li> 
       <li> <p>テンプレートタスクに 1 回限りの承認プロセスが添付されている場合、その承認プロセスは選択したシステムレベル<span>またはグループレベルの承認プロセス</span>で置き換えられます。 </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr>

   </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

#### コメント {#comment-2}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **コメント** をクリックします。

   ![ テンプレート タスクのコメント セクションの編集 ](assets/template-task-edit-comment.png)

1. **テンプレートタスクに更新を追加** 領域で、テンプレートタスクの更新ストリームに表示するコメントを使用可能フィールドに指定します。 このコメントは、テンプレートおよびテンプレートタスクへの表示アクセス権とメモの表示アクセス権を持つすべてのユーザーに表示されます。
1. 「**保存**」をクリックします。

   本ユーザーまたは別のユーザーがこのテンプレートからプロジェクトを作成すると、テンプレートタスクに適用したすべての設定がプロジェクトタスクの設定になります。

</div>


