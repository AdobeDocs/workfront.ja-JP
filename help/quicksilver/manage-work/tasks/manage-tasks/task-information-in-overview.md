---
product-area: projects
navigation-topic: manage-tasks
title: 「タスクの詳細の概要」領域でタスク情報を管理します
description: 「タスクの詳細の概要」領域でタスク情報を管理します
author: Alina
feature: Work Management
exl-id: 4980b28f-914d-4cf9-813f-14983aac660b
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 5%

---

# 「タスクの詳細の概要」領域でタスク情報を管理します

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, do it in both articles)</p>
-->

タスクの情報を表示または編集するには、「タスクの詳細」セクションの「概要」領域にアクセスします。 この領域で表示または編集できるフィールドは限られています。 タスクのすべての情報の編集について詳しくは、 [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

この記事では、タスクの詳細の概要領域で情報を表示または編集する方法について説明します。 タスクの詳細のその他の領域の更新について詳しくは、次の記事を参照してください。

* [[ タスクの詳細 ] セクションでタスクの財政状況を管理します](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
* [オブジェクトにカスタムフォームを追加する](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)
* [オブジェクトに添付されたカスタムフォームの管理](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
   *保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> plan*</b> </p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> ライセンス*</b> </p> </td> 
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>プロジェクトとタスクへのアクセス権を表示または高くする</p> <p>正しいアクセスレベルを持っていても、タスクの「詳細」セクションを編集できない場合は、Adobe Workfrontにアクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクトの権限</strong> </p> </td> 
   <td> <p>プロジェクトに対する Contribute 以上の権限</p> <p>タスクの権限を表示して、「詳細」セクションの情報を表示します。 </p> 
   <p>タスクに対する Contribute の権限で、「詳細」セクションの次の情報を更新します。</p>

<ul>
   <li>説明</li>
   <li>ステータス</li>
   </ul>

<p>タスクの権限を管理して、「詳細」セクションのすべての情報を更新します。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 「タスクの詳細の概要」セクションでタスク情報を編集

1. 表示または編集するタスクに移動します。
1. クリック **タスクの詳細** をクリックします。
1. 次に移動： **概要** 領域をクリックして、タスクの詳細を表示します。

   デフォルトでは、「概要」は「タスクの詳細」セクションの最初の領域で、展開されています。

   >[!NOTE]
   >
   >Workfront管理者またはグループ管理者がレイアウトテンプレートを設定する方法に応じて、「タスクの詳細」セクションのフィールドが再配置されたり表示されなかったりする場合があります。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 次をクリック： **編集** アイコン ![](assets/edit-icon.png) 「詳細」セクションの右上隅で、 **概要**.

   >[!TIP]
   >
   >Workfrontによって自動的に生成されるフィールドや、編集する権限を持たないフィールドは編集できません。

1. フィールドをシングルクリックまたはクリックして、編集可能なフィールドを編集します。 **+追加** をクリックして、空のフィールドに情報を追加します。
1. 次のフィールドの一覧を表示または編集します。

   一部のフィールドが編集可能とは限りません。  

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td> <p>タスクに関する追加情報</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">参照番号</td> 
      <td>これは、システム内のすべてのオブジェクトに対してWorkfrontで生成されるタスクの一意の値です。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>タスクに対する管理権限を持つユーザーは、このフィールドに内部ページまたは外部ページへのリンクを指定できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステータス</td> 
      <td> <p>タスクのステータスを選択します。このステータスは、タスクが開発のどの段階にあるかを示します。</p> <p>ヒント：タスクのステータスは、タスクのヘッダーで更新できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">優先度</td> 
      <td> <p>これは、タスクを優先順位付けできる視覚的なフラグです。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p> なし</p> </li> 
        <li> <p> 低 </p> </li> 
        <li> <p>標準 </p> </li> 
        <li> <p>高 </p> </li> 
        <li> <p> 緊急 </p> </li> 
       </ul> <p>Workfront管理者が選択したプロジェクトの環境設定によっては、優先度の名前が異なる場合があります。 タスクの優先度について詳しくは、 <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">タスクの優先度を更新</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間タイプ</td> 
      <td> <p>これは、次の間の関係を識別します。 </p> 
       <ul> 
        <li> <p>タスクに割り当てられたリソースの数 </p> </li> 
        <li> <p>タスクの完了に必要な総作業量 </p> </li> 
        <li> <p> タスクの総期間。 </p> </li> 
       </ul> <p>Workfront管理者 <span> またはグループ管理者</span> システムまたはグループ内のタスクのデフォルトの「期間の種類」設定を選択します。 プロジェクトの既定値の設定については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>. </p> <p>期間タイプを使用すると、タスクのニーズに基づいて一貫したリソースの割り当てを設定できます。 タスクの期間の種類について詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>. </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p>算出した割り当て </p> </li> 
        <li> <p> 算出した作業 </p> </li> 
        <li> <p>作業優先 </p> </li> 
        <li> <p>シンプル</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td> 
       <div> 
        <div> 
         <p>タスクが完了するまで、タスクを開いたままにしておく時間です。 </p> 
         <p>重要：タスク期間は通常、計画開始日から計画完了日までの時間なので、プロジェクトのタイムラインに影響します。</p> 
         <p>タスクの期間と時間の単位を指定するには、次の手順を実行します。</p> 
         <ul> 
          <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">時間の長さを入力し、ドロップダウンメニューで使用できる時間の単位から選択します。</p> </li> </ul>

   <p><strong>ヒント</strong></p> <p> タスクリストのタスクの期間を更新する場合、時間の単位の省略形を使用できます。 </p>      <p> 次の表の通常の時間または経過時間オプションから選択できます。 </p> 
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
            <td>月</td> 
           </tr> 
           <tr> 
            <td>時間</td> 
            <td>H</td> 
           </tr> 
           <tr> 
            <td>日. これがデフォルトです。 </td> 
            <td>削</td> 
           </tr> 
           <tr> 
            <td>週</td> 
            <td>W</td> 
           </tr> 
           <tr> 
            <td>月</td> 
            <td>火</td> 
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
            <td>新規</td> 
           </tr> 
           <tr> 
            <td>経過月数</td> 
            <td>ET</td> 
           </tr> 
          </tbody> 
         </table> 
         <p><strong>メモ</strong> </p>
         <p> 経過時間は、タスクの期間の時間の単位です。 休日、週末、休日を含むタスクの計画開始日から計画完了日までの時間です。 つまり、経過時間は暦日の経過です。 通常の時間は、休日、週末、休日を考慮し、タスクの期間から除外します。 タスクの期間について詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>. </p> 
         <p> 
         <!--You cannot specify the Duration of a task when the Duration Type of the task is Simple, or when the Task Constraint is Fixed Dates. (NOTE: Anna said this is now possible for all duration types in the Assignments area. It's not here, but to clear confusion, I am drafting this out of here.)--></p> 
        </div> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">見込み期間</td> 
      <td> <p>予定開始日と予測完了日の日数の差。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の期間</td> 
      <td> <p>実際の開始日と実際の完了日の日数の差。 これが、実際にその作業を完了するのにかかった時間です。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定時間</td> 
      <td> <p>タスクの予定時間数を時間単位で指定します。 タスクの担当者がタスクを完了するのにかかる実際の時間です。 [ 期間の種類 ] が [ 割り当ての計算 ] に設定されている場合は、タスクの予定時間数のみ指定できます。 期間のタイプについて詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の時間数</td> 
      <td>タスクにユーザーがログに記録した時間。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">作業量 </td> 
      <td> 
       <div> 
        <p>タスクの完了に必要な労力の量。 プロジェクトマネージャは、タスクの完了に必要な作業量を見積もる際に、予定時間の代わりにこのフィールドを使用することにします。 このフィールドは、次の条件を満たした場合にのみ表示されます。</p> 
        <ul> 
         <li> <p>タスクには「シンプルな期間」タイプがあります。 </p> <p>ヒント： 「期間の種類」タスクを変更すると、このフィールドは淡色表示になります。 </p> </li> 
         <li>プロジェクトマネージャーが、プロジェクトの [ 作業時間を使用 ] フィールドでタスクの [ 計画時間 ] を自動的に計算できるようにしました。 </li> 
        </ul> 
        <p>次のオプションから選択します。</p> 
        <ul> 
         <li>小</li> 
         <li>中 <span style="font-weight: normal;">（これは新しいタスクのデフォルト値です）</span></li> 
         <li>大</li> 
        </ul> 
        <p><strong>メモ</strong></p> 
        <p> 作業量を更新すると、タスク「計画時間」が更新される場合があります。 プロジェクトの [ 更新タイプ ] が [ 自動 ] の場合は、更新が直ちに行われます。 プロジェクトの「更新タイプ」が「手動」の場合は、更新された計画時間を確認するために、タイムラインを再計算する必要があります。 </p> 
        <p>計画時間ではなく作業量を使用して作業量を見積もる方法については、 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タスクの制約</td> 
      <td> <p>タスク制約を指定して、タスクを完了するタイミングを決定します。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p><span>固定日付</span> </p> <p>を指定します。 <strong>計画開始</strong> および <strong>計画完了日</strong>. </p> </li> 
        <li> <p><span>指定日に開始</span> </p> <p>を指定します。 <strong>計画開始日</strong>. </p> </li> 
        <li> <p><span>指定日に終了</span> </p> <p>を指定します。 <strong>計画完了日</strong>. </p> </li> 
       </ul> 
       <ul> 
        <li> <p><span>できるだけ早く</span></p> </li> 
        <li> <p><span>できるだけ遅く</span></p> </li> 
        <li> <p><span>最も早い空き時間</span></p> </li> 
        <li> <p> <span>最も遅い空き時間</span></p> </li> 
        <li> <p><span>指定日までに開始</span> </p> </li> 
        <li> <p>計画開始日の指定</p> </li> 
        <li> <p><span>指定日以後に開始</span> </p> <p>を指定します。 <strong>計画開始日</strong>. </p> </li> 
        <li> <p> 完了 <span>指定の日まで</span></p> <p>を指定します。 <strong>計画完了日</strong>. </p> </li> 
        <li> <p> 完了 <span>次の値より前：</span></p> <p>を指定します。 <strong>計画完了日</strong></p> </li> 
       </ul> <p>タスク制約の詳細については、 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定開始日</td> 
      <td> <p>タスクを開始する予定の日時。 タスクの計画開始日は、次のような要因によって設定され、影響を受けます。</p> 
       <ul> 
        <li>タスクの計画開始日に対するシステム全体の優先度に応じて、既定では、プロジェクトの新しいタスクの開始日は今日にすることも、プロジェクトの開始日にすることもできます。 <span>プロジェクトに関連付けられたグループのグループ管理者も、グループに対してこの環境設定を設定できます。</span> システムレベルまたはグループレベルのタスク環境設定の詳細については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">システム全体のタスクと問題の環境設定を構成する</a>.</li> 
        <li>タスクの先行タスクに応じて、予定開始日がWorkfrontによって選択され、先行タスクの終了後の次の使用可能な日付、または先行タスクの関係に応じて開始日になります。 先行関係の詳細については、「 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">タスクの先行タスクの概要</a>.</li> 
        <li>プロジェクトマネージャまたはタスク所有者は、タスク制約が [ 固定日付 ] または [ 開始日 ] の場合に、計画開始日を手動で設定できます。 タスクの制約の詳細については、 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">見込み開始日</td> 
      <td> <p>前のタスクの進行状況と完了に基づいてタスクが開始される「実際の期間」の日付。 これは計算フィールドで、手動で編集することはできません。</p> <p> プロジェクトが最初に計画されたときに、予定開始日と計画開始日が同じになって開始します。 プロジェクトが進展し、タスクがまだ開始されていない場合は、予定開始日から移動できます。 予定開始日について詳しくは、 <a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">プロジェクトの概要予定開始日</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の開始日</td> 
      <td> <p>タスクの実績開始日を指定します。 通常、デフォルト値は、タスクのステータスを「処理中」に変更すると自動的に設定されます。 実際の開始日は、プロジェクトマネージャまたはタスク所有者が手動で変更することもできます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計画完了日</td> 
      <td> <p>タスクが計画された際に示される、完了予定日。 計画完了日は、次の要因で設定できます。</p> 
       <ul> 
        <li>計画完了日は、タスクの期間を計画開始日に追加することで、計画開始日から計算されます。 プロジェクトマネージャーまたはWorkfrontがタスクの期間を指定すると、計画完了日がトリガーに更新されます。 予定日が変更された場合、多くの場合、の期間が更新されたことが原因です。</li> 
        <li>プロジェクトマネージャまたはタスク所有者は、タスク制約が [ 固定日付 ] または [ 終了日 ] の場合に、計画完了日を手動で設定できます。 タスクの制約の詳細については、 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>.</li> 
        <li>タスクの期間タイプが変更され、タスクのリソース数が同時に変更される場合は、計画完了日も変更されます。 期間のタイプについて詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">見込み完了日</td> 
      <td> <p>前のタスクの進捗状況と、担当者がタスクに対しておこなった進捗状況の更新に基づいてタスクを完了する「実際の期間」の日付です。 これは計算フィールドで、手動で編集することはできません。</p> <p> プロジェクトが最初に計画されたときに、予定完了日と計画完了日が同じ日付で開始します。 プロジェクトが進展し、タスクがまだ開始されていない場合は、予定完了日から移動できます。 予定完了日について詳しくは、 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">プロジェクト、タスクおよび問題に関する予定完了日の概要</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の完了日</td> 
      <td> <p>タスクが完了する実際の日時を指定します。 タスクが完了した既定の日時は、常に、ステータスが [ 完了 ] になった実際の日時と一致します。 実際の完了日は、プロジェクトマネージャまたはタスク所有者が手動で変更することもできます。 </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">コミット日</td> 
      <td> <p>タスクに割り当てられたユーザーが、タスクを完了させるためにコミットする日付です。 これは、「計画完了日」とは異なる場合があります。 委託人のみがこのフィールドを編集できます。Workfrontでのコミット日について詳しくは、 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">コミット日の概要</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">エントリ日</td> 
      <td>タスクが作成された日付。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">入力者</td> 
      <td>タスクを作成した人物。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">最終更新日</td> 
      <td> <p>タスクが最後に更新された日付。 </p> <p>ヒント： Workfrontは、タスクを編集および保存するたびに更新日を記録します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">最終更新者</td> 
      <td> <p>タスクを最後に更新した担当者。</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">繰り返し頻度</td> 
      <td> <p>これは、繰り返しタスクの親にのみ表示されます。 繰り返しのタスクが発生する頻度です。 繰り返しタスクの作成について詳しくは、 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">繰り返しタスクの作成</a>. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">発生ごとの所要時間</td> 
      <td> <p>これは、繰り返しタスクの親にのみ表示されます。 各繰り返しタスクの期間が表示されます。 繰り返しタスクの作成について詳しくは、 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">繰り返しタスクの作成</a>. </p> <p><strong>メモ</strong></p> <p> 個々の定期タスクで変更された期間は、このフィールドに示される値を表示しません。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted, to keep it focused JUST on the Overview section and not others.) </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Custom Forms</strong> to add or forms or edit information on the existing custom forms.&nbsp;</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand any of the existing custom forms to edit them, or start typing in the <strong>Add custom form</strong> box in the upper-right corner to add a new form. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding or editing custom forms, see the following articles:</p>
   -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md" class="MCXref xref">Add a custom form to an object</a> </li>   
     -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md" class="MCXref xref">Manage custom forms attached to objects</a> </li>   
     -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click&nbsp;<strong>Finance</strong>, then <strong>Edit Finance</strong> to view or edit financial information for the task. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand the <strong>Finance</strong> area in the Details section, then double-click any editable field to update it. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about editing financial information for a task, see <a href="../../../manage-work/tasks/manage-tasks/task-finances-in-details.md" class="MCXref xref">Manage task finances in the Task Details section</a>. </p>
   -->

1. 「**変更を保存**」をクリックします。
