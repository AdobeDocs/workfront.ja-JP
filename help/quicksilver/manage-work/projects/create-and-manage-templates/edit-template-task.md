---
product-area: templates
keywords: タスク,デフォルト,自動化,作成
navigation-topic: templates-navigation-topic
title: テンプレート タスクの編集
description: テンプレートを作成した後、テンプレートタスクに関する情報を編集できます。テンプレートタスクで更新した情報は、テンプレートを使用してプロジェクトを作成した後、またはテンプレートをプロジェクトに添付した後、プロジェクトタスクに関連付けられます。
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: e186b4aa0b5c229015cf8f3dcd8993f8f0443c44
workflow-type: tm+mt
source-wordcount: '2958'
ht-degree: 68%

---

# テンプレートタスクを編集

<!--Audited: 11/2025-->

<!--take out production and preview references and new/ old experiences at release-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

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
      * **すべて折りたたむ** アイコン ![&#x200B; すべて折りたたむアイコン &#x200B;](assets/collapse-all-icon.png) をクリックすると、すべての領域が折りたたまれます。
      * **編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックして、下の任意の領域から選択するか、**すべて編集** をクリックして、すべての領域の情報を編集します。

         * 概要
         * カスタムForms
カスタムフォームの名前は、テンプレートタスクに添付されたカスタムフォームがある場合にのみ表示されます。
         * 財務

        >[!TIP]
        >
        >「詳細」領域に表示されるすべてのフィールドについて詳しくは、以下に説明するように、「テンプレートタスクを編集」ボックスを使用してすべてのフィールドを引き続き編集します。

   1. （任意）左側のパネルで「**サブタスク**」セクションをクリックして、テンプレートタスクの子を追加します。 テンプレートタスクのサブタスクの追加は、プロジェクトタスクのサブタスクの追加と似ています。 詳しくは、「サブタスクの作成」の「タスクサブタスクからサブタスクを作成する [&#x200B; 節を参照してくだ &#x200B;](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md) い。
   1. （任意）左側のパネルで **費用** をクリックし、テンプレートタスクに費用を追加します。 テンプレートタスクの費用は、テンプレートを使用してプロジェクトを作成する際に、将来のプロジェクトタスクに転送されます。
   1. （任意）左側のパネルの **承認** をクリックして承認を作成するか、テンプレートタスクにグローバルまたはグループレベルの承認を添付します。 承認は、今後のプロジェクトタスクに転送されます。
   1. （任意）左側のパネルで「**先行タスク**」セクションをクリックして、テンプレートタスクの先行タスクを追加します。 テンプレートタスク先行タスクの追加は、プロジェクトタスク先行タスクの追加と似ています。 詳しくは、[&#x200B; 先行タスクエリアを使用した先行タスク関係の作成 &#x200B;](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md) を参照してください。

1. （条件付き）テンプレートタスクまたは複数のタスクに関するすべての情報を同時に編集するには、リストから選択をクリックし、リストの上部にある **編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックします。

   「**テンプレートタスクの編集**」ボックスが表示されます。

   ![&#x200B; テンプレートの編集タスクの新しいエクスペリエンス &#x200B;](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >また、リストでテンプレートタスクを選択し、ヘッダーのテンプレートタスク名の右側にある **編集** をクリックして **テンプレートタスクを編集** ボックスを開くこともできます。

1. 次のセクションのいずれかに情報を指定することを検討してください。

* [テンプレート タスク名](#template-task-name)
* [概要](#overview)
* [割り当て](#assignments)
* [財務](#finance)
* [カスタムフォーム](#custom-forms)
* [設定](#settings)
* [コメント](#comment)

1. 以下の節で説明するように、テンプレートタスクの編集を続けます。

### テンプレート タスク名

>[!TIP]
>
>テンプレートタスクを一括編集する場合、「テンプレートタスク名」セクションは使用できません。


1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. [ テンプレート タスクの編集 ] ボックスで、[**テンプレート タスク名**] をクリックし、テンプレート タスクの名前を追加します。

   テンプレートタスクを一括編集する場合、このビューは使用できません。

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

### 概要 {#overview}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **概要** をクリックします。

   ![&#x200B; テンプレートタスク編集の概要セクション &#x200B;](assets/template-task-edit-overview.png)

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
      <p>テンプレート タスクの編集時に [ 作業量 ] フィールドが表示されるのは、テンプレート タスクの編集時に &lbrack;<b> 作業量を使用してタスクの予定時間数を自動的に計算する </b> 設定を選択した場合のみです。</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   「**保存**」をクリックします。

### 割り当て {#assignments}

1. 上記の説明に従って、テンプレートタスクの編集を開始します。
1. 左側のパネルで「**割り当て**」をクリックします。

   **割り当て** エリアが開きます。

   ![&#x200B; テンプレートタスクの割り当て &#x200B;](assets/assignments-edit-template-tasks-box.png)

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
1. 担当者の名前の上にマウスポインターを置いて、「プライマリを作成 **をクリックし** す。 これは、今後のプロジェクトタスクの **所有者** になります。

   >[!TIP]
   >
   >チームは、タスクまたはテンプレートタスクの所有者またはプライマリ割り当てとして指定することはできません。

1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

### 財務 {#finance-2}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **財務** をクリックします。

   ![&#x200B; テンプレート タスク編集財務セクション &#x200B;](assets/template-task-edit-finance.png)

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

### カスタムフォーム {#custom-forms-2}

タスクがプロジェクトに追加された際に、デフォルトでタスクに自動的に添付されるカスタムフォームを定義できます。 既定のタスクのカスタム フォームを含めるためのプロジェクトの設定については、「プロジェクトの編集 [&#x200B; の [ タスク ] セクションを参照し &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) ください。

また、カスタムフォームをテンプレートタスクに追加することで、テンプレートからプロジェクトを作成する際に、プロジェクトの今後のタスクにカスタムフォームを追加することもできます。

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **カスタムForms** をクリックします。

   ![&#x200B; テンプレート タスクのカスタム フォームの編集セクション &#x200B;](assets/template-task-edit-custom-forms.png)

1. テンプレートタスクに関連付けるカスタムフォームを選択します。

   このフィールドで選択できるカスタムフォームを作成する必要があります。
アクティブなカスタムフォームのみがリストに表示されます。

   カスタムフォームの作成について詳しくは、「[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

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

### 設定 {#settings-2}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. **テンプレート タスクを編集ボックス** で、左パネルの **設定** をクリックします。

   ![&#x200B; テンプレート タスク編集設定セクション &#x200B;](assets/template-task-edit-settings.png)

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

### コメント {#comment-2}

1. 前述の説明に従って、テンプレートタスクの編集を開始します。
1. 「**テンプレートタスクを編集**」ボックスで、左パネルの **コメント** をクリックします。

   ![&#x200B; テンプレート タスクのコメント セクションの編集 &#x200B;](assets/template-task-edit-comment.png)

1. **テンプレートタスクに更新を追加** 領域で、テンプレートタスクの更新ストリームに表示するコメントを使用可能フィールドに指定します。 このコメントは、テンプレートおよびテンプレートタスクへの表示アクセス権とメモの表示アクセス権を持つすべてのユーザーに表示されます。
1. 「**保存**」をクリックします。

   本ユーザーまたは別のユーザーがこのテンプレートからプロジェクトを作成すると、テンプレートタスクに適用したすべての設定がプロジェクトタスクの設定になります。


<!--Temporary content for Assignments redesign:

Editing template tasks differs depending on which environment you choose to edit the tasks. 

### Edit template tasks in the Production environment

>[!NOTE]
>
><span class="preview">Some customers can edit template tasks in their Production environments the same way they edit them in their Preview environment.</span>
>
><span class="preview">For information about editing tasks in the Preview environment, see the section [Edit template tasks in the Preview environment](#edit-template-tasks-in-the-preview-environment) in this article. </span>


You can edit a template task using the Edit Template Task or Template Task Details areas. 

{{step1-to-templates}}

1. Click the name of a template to open it.
1. Click **Template Tasks** in the left panel. 
1. Click the name of a template task in the list to open the template task.
1. To edit limited information about the template task, do the following: 
   1. (Optional) Click **Updates** in the left panel to add updates to the template task. Template task updates do not transfer to project tasks when the template is used to create a project.
   1. (Optional) Click **Documents** in the left panel to add documents to the template task. The documents will transfer to the project tasks when you use the template to create the project. 
   1. (Conditional) To edit limited information about a template task, click **Template Task Details** in the left panel, then go to the areas of the Details section to edit information for each area.
   1. (Optional) Do any of the following: 
      * Click the **Collapse all** icon ![Collapse all icon](assets/collapse-all-icon.png) to collapse all areas. 
      * Click the **Edit** icon ![Edit icon](assets/edit-icon.png), then select from any of the areas below, or click **Edit all** to edit information in all areas:

         * Overview
         * Custom Forms
            Names of customs forms display only if there are custom forms attached to the template task.
         * Finance

         >[!TIP]
         >
         >For information about all fields that display in the Details area, continue with editing all fields using the Edit Template Task box, as described below.

   1. (Optional) Click the **Subtasks** section in the left panel to add children for the template task. Adding subtasks for template tasks is similar to adding project task subtasks. For information, see the section  "Create subtasks from the task Subtasks section" in the article [Create subtasks](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md). 
   1. (Optional) Click **Expenses** in the left panel, and add expenses to the template tasks. Template task expenses transfer to future project tasks, when the template is used to create a project. 
   1. (Optional) Click **Approvals** in the left panel to create approvals or attach global or group-level approvals to the template tasks. The approvals transfer to future project tasks. 
   1. (Optional) Click the **Predecessors** section in the left panel to add predecessors for the template tasks. Adding template task predecessors is similar to adding project task predecessors. For information, see [Create a predecessor relationship using the Predecessors area](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md). 

1. (Optional) To edit several template tasks in bulk, select multiple template tasks, then click **Edit** at the top of the template list.
1. (Conditional) To edit all information about the template task or about several tasks at the same time, click to select them from a list, then click the **Edit** icon ![Edit icon](assets/edit-icon.png) at the top of the list.

   The **Edit Template Task** box displays in the new experience.

   ![New experience for Edit Template Task](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >You can also select a template task in a list, then click **Edit** to the right of the template task name in the header, to open the **Edit Template Task** box.

   Continue editing the template task as described in the [Edit a template task using the new experience](#edit-a-template-task-using-the-new-experience) section in this article.
   
1. (Optional) Click **Switch back to old experience** at the bottom of the **Edit Template Task** box to open the **Edit Template Task** box in the old experience. 

   ![Edit template task](assets/edit-template-tasks-box-classic-350x356.png)

1. Consider specifying information in any of the following sections:

   * [Overview](#overview)
   * [Finance](#finance)
   * [Settings](#settings)
   * [Assignments](#assignments)
   * [Custom Forms](#custom-forms)
   * [Comment](#comment)

1. Continue editing the template task as described in the [Edit a template task using the old experience](#edit-a-template-task-using-the-old-experience) section in this article.

#### Edit a template task using the old experience

##### Overview {#overview}

1. Begin editing a template task as described above.
1. Click **Overview**.

   ![edit_task_overview.png](assets/edit-task-overview-350x438.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td>Specify a name for the template task. This field does not display when editing template tasks in bulk.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Add additional information about the template task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Specify a web link that relates to the information about the template task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong> </td> 
      <td> <p>This is a visual flag for you which allows you to prioritize your template tasks. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>None</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p> <b>Normal</b></p> </li> 
        <li> <p><b>High</b> </p> </li> 
        <li> <p><b>Urgent</b> </p> </li> 
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Duration Type</strong> </td> 
      <td> <p>The future task created from this template will have this Duration Type. <br>Duration Type identifies the relationship between the following:</p> <p>- number of resources assigned to a task</p> <p>- the total effort required to complete the task</p> <p>- the total duration of the task. </p> <p>Duration Types enable you to set consistent resource assignments based on the needs of the task. For more information about the Duration Type of a task, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calculated Assignment</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calculated Work</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Effort Driven</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Simple</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Duration</strong> </td> 
      <td> <p>Specify the Duration of the future tasks, in minutes, hours, days, weeks, or months. The future task created from this template will have the Duration specified here.</p> <p>By default, Workfront measures Duration in days. This is the amount of time that you allow for the task to remain incomplete, before it must be completed. You cannot specify the Duration of a task when the <strong>Duration Type</strong> of the task is <strong>Simple</strong>, or when the <strong>Task Constraint</strong> is <strong>Fixed Dates</strong>.</p> <p><b>IMPORTANT</b></p> <p>Duration is typically the amount of time between the Planned Start and the Planned Completion Dates of a template task, and for this reason, it affects the timeline of the template. This determines the timeline of the future project created from the template. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Hours</strong> </td> 
      <td> <p>Specify the number of Planned Hours for the future task on the project created with this template. This is the amount of actual time it would take the assignees of the task to complete it. You can only specify the number of Planned Hours for a task when the <strong>Duration Type</strong> is set to <strong>Calculated Assignment</strong>. </p> </td> 
     </tr> 
     
     <tr> 
      <td role="rowheader"><strong>Task Constraint</strong> </td> 
      <td> <p>The task on the project created from this template will have this constraint. Task Constraints identify when a task must be completed. </p> <p>Select from the following options:</p> 
       <ul> 
        <li><strong>Fixed Dates</strong>. Specify a <strong>Planned Start</strong> and a <strong>Planned Completion Date.</strong></li> 
        <li><strong>Must Start On</strong>. Specify a <strong>Planned Start Date.</strong></li> 
        <li><strong>Must Finish On</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
        <li><strong>As Soon as Possible</strong> </li> 
        <li><strong>As Late as Possible</strong> </li> 
        <li style="font-weight: bold;"><strong>Earliest Available Time</strong> </li> 
        <li style="font-weight: bold;"><strong>Latest Available Time</strong> </li> 
        <li>Start No Later Than. Specify a <strong>Planned Start Date</strong>.</li> 
        <li><strong>Start No Earlier Than</strong>. Specify a <strong>Planned Start Date</strong>.</li> 
        <li><strong>Finish No Later Than</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
        <li><strong>Finish No Earlier Than</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
       </ul> <p>For more information on Task Constraint, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Start Day</span><span style="font-weight: normal;"> (Optional and conditional)</span> </td> 
      <td> <p> You can specify the Start Day of a template task only when the Task Constraint is one of the following:</p> 
       <ul> 
        <li>Must Start On</li> 
        <li>Start No Earlier Than</li> 
        <li>Start No Later Than</li> 
        <li>Fixed Dates</li> 
       </ul> <p>This will correspond to the date within the timeline of the future project when the task will start. For all other constraints, Workfront calculates the Start Day based on predecessor dependency between the tasks. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Day</strong><span style="font-weight: normal;"> (Optional and conditional)</span> </td> 
      <td> <p> You can specify the Completion Day of a template task only when the Task Constraint is one of the following:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Must Finish On</li> 
        <li>Finish No Earlier Than</li> 
        <li>Finish No Later Than</li> 
        <li>Fixed Dates</li> 
       </ul> <p>This will correspond to the date within the timeline of the future project when the task will complete. For all other constraints, Workfront calculates the Completion Day based on Duration and predecessor dependency. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

##### Finance {#finance}

1. Begin editing a template task as described above.
1. Click **Finance**.

   ![edit_task_finance.png](assets/edit-task-finance-350x216.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Cost Type</strong> </td> 
      <td> <p>Specify the Cost Type for the future task. This is going to determine how the Cost on the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>No Cost</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Fixed Hourly</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>User Hourly</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Role Hourly</span> </p> </li> 
       </ul> <p>For more information about tracking costs, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Revenue Type</strong> </td> 
      <td> <p>Specify the Revenue Type for the future task. This is going to determine how the Revenue on the task is calculated, based on the number of hours on the tasks.</p> <p style="font-weight: normal;">Select from the following options: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Not Billable</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly</p> </li> 
        <li> <p style="font-weight: normal;">Fixed Hourly</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly w/Cap</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly w/Cap</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly Plus Fixed</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly Plus Fixed</p> </li> 
        <li> <p style="font-weight: normal;">Fixed Revenue</p> </li> 
       </ul> <p>For more information about tracking revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

##### Settings {#settings}

1. Begin editing a template task as described above.
1. Click **Settings**.

   ![Edit template task settings](assets/edit-template-tasks-settings-classic-350x231.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Milestone</b></p></strong> </td> 
      <td> <p>Choose a milestone to associate with the selected template task.</p>
      
   <p><b>IMPORTANT</b></p>
   <p>You must associate a milestone path with a template for this field to display. For more information, see <a href="../create-and-manage-templates/edit-templates.md">Edit project templates</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Tracking Mode</strong> </td> 
      <td> <p>Specify how the progress status of the future task will be tracked. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>User Must Update</strong> </p> </li> 
        <li> <p><strong>Assume on Time</strong> </p> </li> 
        <li> <p><strong>Ignore Late Warnings</strong> </p> </li> 
        <li> <p><strong>Autocomplete</strong> </p> </li> 
        <li> <p><strong>Predecessor</strong> </p> </li> 
       </ul> <p>For more information about the Tracking Mode on tasks, see <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Task Tracking Mode overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template task. Your Workfront administrator must define system-level task Approval Processes before you can associate them with template tasks. <span>A user with administrative access to Approval processes can also create group-specific approval processes.</span> For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
       <ul> 
       <li>Only active approval processes display in the list. </li> 
       <li> <p>System-wide and group-specific approval processes display in the list. Approval processes associated with a group other than that of the template do not display in the list.</p> <p>Important: If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
       <li> <p>If you added a single-use approval process, it displays as "&lt;Custom&gt;" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>************************* </li> 
       <li> <p>When bulk-editing template tasks, the following scenarios exist:</p> 
       <ul> 
       <li> <p>When you select template tasks from the same template group, both system-level and group-level approval processes display in this field.</p> </li> 
       <li> <p>When you select template tasks from different template groups, only system-level approval processes display in this field.</p> </li> 
       <li> <p>When any of the template tasks has a single-use approval process attached, it is replaced by the system-level <span>or group-level approval process</span> you select. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notifications</strong> </td> 
      <td> <p>Select which Reminder Notifications you would like to attach to the template task. They will be attached to the future tasks on the project created from this template. Your system administrator must configure Reminder Notifications before you can select them on a task. For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

##### Assignments {#assignments}

1. Begin editing a template task as described above.
1. Click **Assignments**.

   ![assignments_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. Click **Add Assignee** to add a new assignee to the template task. You can assign users, roles, or teams to a task. You can have multiple assignees on a task. The future tasks will have the same resources assigned to it when created from this template task. 
1. (Optional) If you have multiple assignees, select the **Owner** radio button to indicate which user or role is considered the Task Owner or the Primary Assignee. Workfront marks the first user or job role that you assign to a template task as the Owner or Primary Assignee. 
1. (Conditional and optional) If your **Duration Type** is **Calculated Work** or **Effort Driven**, specify the **Allocation %** (allocation percentage) for each assignee. This is the amount of time from the schedule of the assignee that they can spend on this task. Changing the allocation percentage for an assignee will change the Planned Hours of a task. 
1. (Conditional and optional) If your **Duration Type** is **Simple**, specify the **Hours** of each assignee

   Or

   Specify the total number of **Planned Hours** for the template task. This distributes the total hours equally between all the assignees. 

1. (Conditional and optional) If your **Duration Type** is Simple, specify the **Duration** of the template task in days. This will become the duration of the task created from this template. 
1. (Optional) Select a role from the **Assignee's Role** drop-down menu. This is the role that the assignee can fulfill on this future task. Only the job roles associated with each assignee in their profile appear in the drop-down menu.
1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

##### Custom Forms {#custom-forms}

You can define custom forms to be automatically attached by default to tasks when the tasks are added to a project. For information about setting up the project to include default task custom forms, see the "Tasks" section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

You can also add custom forms to the future tasks of a project when the project is created from a template, by adding the custom forms to the template tasks. 

1. Begin editing a template task as described above.
1. Click **Custom Forms**.

   ![custom_forms_edit_task.png](assets/custom-forms-edit-task-350x136.png)

1. Select the custom form or forms that you want to associate with the template task. 

   You must build the custom forms before they are available to select in this field. 
   Only active custom forms display in the list. 
   For more information about building custom forms, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). 
   You can add up to ten custom forms to a template task. 
   The forms are automatically added to the tasks created from the template. 
1. (Conditional and optional) If you attached a custom form to the template task, edit any fields on the form. You must specify all required fields before you can save the template task.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the template task or the future task.   
   >For information about setting permissions on sections of a custom form, see [Share a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).   
   >For information about setting task permissions, see [Share a task](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).   
   >For information about setting template permissions, see [Share a template](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

##### Comment {#comment}

1. Begin editing a template task as described above.
1. Click **Comment**.

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. Specify a comment that you want to display in the updates stream of the template task in the available field. This comment is visible for everyone with View access to the template and the template task and with access to view Notes.
1. Click **Save Changes**.

   When you or another user creates a project from this template, all settings you applied to template tasks become the settings for the project tasks.

#### Edit a template task using the new experience

After opening the **Edit Template Task** box in the new experience, consider specifying information in any of the following sections:

* [Template task name](#template-task-name)
* [Overview](#overview-1)
* [Assignments](#assignments-1)
* [Finance](#finance-1)
* [Custom Forms](#custom-forms-1)
* [Settings](#settings-1)
* [Comment](#comment-1)

##### Template Task Name

>[!TIP]
>
>The Template Task Name section is not available when editing template tasks in bulk.


1. Begin editing a template task as described above.
1. In the Edit Template Task box, click **Template Task Name** and add a name for the template task. 

   This view is not available when editing template tasks in bulk. 

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**. 

##### Overview {#overview-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Overview** in the left panel. 

   ![Template task edit overview section](assets/template-task-edit-overview.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Add additional information about the template task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong> </td> 
      <td> <p>This is a visual flag for you which allows you to prioritize your template tasks. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>None</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p> <b>Normal</b></p> </li> 
        <li> <p><b>High</b> </p> </li> 
        <li> <p><b>Urgent</b> </p> </li> 
       </ul> <p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Constraint</strong> </td> 
      <td> <p>The task on the project created from this template will have this constraint. Task Constraints identify when a task must be completed. </p> <p>Select from the following options:</p> 
       <ul> 
        <li><strong>Fixed Dates</strong>. Specify a <strong>Planned Start</strong> and a <strong>Planned Completion Date.</strong></li> 
        <li><strong>Must Start On</strong>. Specify a <strong>Planned Start Date.</strong></li> 
        <li><strong>Must Finish On</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
        <li><strong>As Soon as Possible</strong> </li> 
        <li><strong>As Late as Possible</strong> </li> 
        <li style="font-weight: bold;"><strong>Earliest Available Time</strong> </li> 
        <li style="font-weight: bold;"><strong>Latest Available Time</strong> </li> 
        <li>Start No Later Than. Specify a <strong>Planned Start Date</strong>.</li> 
        <li><strong>Start No Earlier Than</strong>. Specify a <strong>Planned Start Date</strong>.</li> 
        <li><strong>Finish No Later Than</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
        <li><strong>Finish No Earlier Than</strong>. Specify a <strong>Planned Completion Date</strong>.</li> 
       </ul> <p>For more information on Task Constraint, see <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">Start Day</span><span style="font-weight: normal;"> (Optional and conditional)</span> </td> 
      <td> <p> You can specify the Start Day of a template task only when the Task Constraint is one of the following:</p> 
       <ul> 
        <li>Must Start On</li> 
        <li>Start No Earlier Than</li> 
        <li>Start No Later Than</li> 
        <li>Fixed Dates</li> 
       </ul> <p>This will correspond to the date within the timeline of the future project when the task will start. For all other constraints, Workfront calculates the Start Day based on predecessor dependency between the tasks. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Day</strong><span style="font-weight: normal;"> (Optional and conditional)</span> </td> 
      <td> <p> You can specify the Completion Day of a template task only when the Task Constraint is one of the following:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Must Finish On</li> 
        <li>Finish No Earlier Than</li> 
        <li>Finish No Later Than</li> 
        <li>Fixed Dates</li> 
       </ul> <p>This will correspond to the date within the timeline of the future project when the task will complete. For all other constraints, Workfront calculates the Completion Day based on Duration and predecessor dependency. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>Specify a web link that relates to the information about the template task.</td> 
     </tr> 

     <tr> 
      <td role="rowheader"><strong>Work Effort</strong> </td> 
      <td>Choose from the following options:
      <ul><li>Small</li>
      <li>Medium</li>
      <li>Large</li></ul>

      <p><b>IMPORTANT</b></p>
      <p>The Work Effort field displays when editing a template task only when you select the <b>Use Work Effort to automatically calculate task Planned Hours</b> setting when editing the template.</p>

      </td> 
     </tr> 
     </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

##### Assignments {#assignments-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Assignments** in the left panel.

   ![Template task edit assignments](assets/template-task-edit-assignments.png)

1. In the **Search people, role, or teams** field, start typing the name of an assignee, then select it when it displays in the list

   Or

   Click **Assign to me** to assign the template task to yourself.
1. Consider updating the following information: 

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 

   <tr> 
         <td role="rowheader"><strong>Duration Type</strong> </td> 
         <td> <p>The future task created from this template will have this Duration Type. <br>The Duration Type identifies the relationship between the following:</p> 
         <ul>
         <li><p>Number of resources assigned to a task</p> </li>
         <li><p>The total effort required to complete the task</p></li> 
         <li><p>The total duration of the task </p></li></ul> <p>Using Duration Types, you can set consistent resource assignments based on the needs of the task. For more information about the Duration Type of a task, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> <p>Select from the following options:</p> 
         <ul> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calculated Assignment</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Calculated Work</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Effort Driven</span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;">Simple</span> <br> </p> </li> 
         </ul> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Duration</strong> </td> 
         <td> <p>Specify the Duration of the future tasks, in minutes, hours, days, weeks, or months. The future task created from this template will have the Duration specified here.</p> <p>By default, Workfront measures Duration in days. This is the amount of time that you allow for the task to remain incomplete, before it must be completed. You cannot specify the Duration of a task when the <strong>Duration Type</strong> of the task is <strong>Simple</strong>, or when the <strong>Task Constraint</strong> is <strong>Fixed Dates</strong>.</p> <p><b>IMPORTANT</b></p> <p>Duration is typically the amount of time between the Planned Start and the Planned Completion Dates of a template task, and for this reason, it affects the timeline of the template. This determines the timeline of the future project created from the template. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>Planned Hours</strong> </td> 
         <td> <p>Specify the number of Planned Hours for the future task on the project created with this template. This is the amount of actual time it would take the assignees of the task to complete it. You can only specify the number of Planned Hours for a task when the <strong>Duration Type</strong> is set to <strong>Calculated Assignment</strong>. </p> </td> 
      </tr> 
   </tbody> 
      </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

##### Finance {#finance-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Finance** in the left panel.

   ![Template task edit finance section](assets/template-task-edit-finance.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Cost Type</strong> </td> 
      <td> <p>Specify the Cost Type for the future task. This is going to determine how the Cost on the task is calculated, based on the number of hours on the tasks. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>No Cost</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Fixed Hourly</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>User Hourly</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>Role Hourly</span> </p> </li> 
       </ul> <p>For more information about tracking costs, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Revenue Type</strong> </td> 
      <td> <p>Specify the Revenue Type for the future task. This is going to determine how the Revenue on the task is calculated, based on the number of hours on the tasks.</p> <p style="font-weight: normal;">Select from the following options: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Not Billable</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly</p> </li> 
        <li> <p style="font-weight: normal;">Fixed Hourly</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly w/Cap</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly w/Cap</p> </li> 
        <li> <p style="font-weight: normal;">User Hourly Plus Fixed</p> </li> 
        <li> <p style="font-weight: normal;">Role Hourly Plus Fixed</p> </li> 
        <li> <p style="font-weight: normal;">Fixed Revenue</p> </li> 
       </ul> <p>For more information about tracking revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

##### Custom Forms {#custom-forms-1}

You can define custom forms to be automatically attached by default to tasks when the tasks are added to a project. For information about setting up the project to include default task custom forms, see the "Tasks" section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

You can also add custom forms to the future tasks of a project when the project is created from a template, by adding the custom forms to the template tasks. 

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Custom Forms** in the left panel.

   ![Template task edit custom forms section](assets/template-task-edit-custom-forms.png)

1. Select the custom form or forms that you want to associate with the template task. 

   You must build the custom forms before they are available to select in this field. 
   Only active custom forms display in the list. 

   For more information about building custom forms, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). 

   You can add up to ten custom forms to a template task. 
   The forms are automatically added to the tasks created from the template. 
1. (Conditional and optional) If you attached a custom form to the template task, edit any fields on the form. You must specify all required fields before you can save the template task.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the template task or the future task.   
   >For information about setting permissions on sections of a custom form, see [Share a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).   
   >For information about setting task permissions, see [Share a task](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).   
   >For information about setting template permissions, see [Share a template](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save**.

##### Settings {#settings-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task Box**, click **Settings** in the left panel.

   ![Template task edit settings section](assets/template-task-edit-settings.png)

1. Update any of the following:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Milestone</b></p></strong> </td> 
      <td> <p>Choose a milestone to associate with the selected template task.</p>
      
   <p><b>IMPORTANT</b></p>
   <p>You must associate a milestone path with a template for this field to display. For more information, see <a href="../create-and-manage-templates/edit-templates.md">Edit project templates</a>.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>Tracking Mode</strong> </td> 
      <td> <p>Specify how the progress status of the future task will be tracked. </p> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>User Must Update</strong> </p> </li> 
        <li> <p><strong>Assume on Time</strong> </p> </li> 
        <li> <p><strong>Ignore Late Warnings</strong> </p> </li> 
        <li> <p><strong>Autocomplete</strong> </p> </li> 
        <li> <p><strong>Predecessor</strong> </p> </li> 
       </ul> <p>For more information about the Tracking Mode on tasks, see <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Task Tracking Mode overview</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notifications</strong> </td> 
      <td> <p>Select which Reminder Notifications you would like to attach to the template task. They will be attached to the future tasks on the project created from this template. Your system administrator must configure Reminder Notifications before you can select them on a task. For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template task. Your Workfront administrator must define system-level task Approval Processes before you can associate them with template tasks. <span>A user with administrative access to Approval processes can also create group-specific approval processes.</span> For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
       <ul> 
       <li>Only active approval processes display in the list. </li> 
       <li> <p>System-wide and group-specific approval processes display in the list. Approval processes associated with a group other than that of the template do not display in the list.</p> <p>Important: If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
       <li> <p>If you added a single-use approval process, it displays as "&lt;Custom&gt;" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p>  </li> 
       <li> <p>When bulk-editing template tasks, the following scenarios exist:</p> 
       <ul> 
       <li> <p>When you select template tasks from the same template group, both system-level and group-level approval processes display in this field.</p> </li> 
       <li> <p>When you select template tasks from different template groups, only system-level approval processes display in this field.</p> </li> 
       <li> <p>When any of the template tasks has a single-use approval process attached, it is replaced by the system-level <span>or group-level approval process</span> you select. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save**.

##### Comment {#comment-1}

1. Begin editing a template task as described above.
1. In the **Edit Template Task** box, click **Comment** in the left panel.

   ![Template task edit Comment section](assets/template-task-edit-comment.png)

1. In the **Add an update to the template task** area, specify a comment that you want to display in the updates stream of the template task in the available field. This comment is visible for everyone with View access to the template and the template task and with access to view Notes.
1. Click **Save**.

   When you or another user creates a project from this template, all settings you applied to template tasks become the settings for the project tasks.


<div class="preview">

### Edit template tasks in the Preview environment-->