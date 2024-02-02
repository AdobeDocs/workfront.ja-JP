---
product-area: projects
navigation-topic: manage-tasks
title: タスクの詳細の概要エリアでタスク情報を管理
description: タスクの詳細の概要エリアでタスク情報を管理
author: Alina
feature: Work Management
exl-id: 4980b28f-914d-4cf9-813f-14983aac660b
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: ht
source-wordcount: '2089'
ht-degree: 100%

---

# タスクの詳細の概要エリアでタスク情報を管理

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, do it in both articles)</p>
-->

「タスクの詳細」セクションの概要エリアにアクセスすることで、タスクの情報を表示または編集することができます。このエリアで表示または編集できるフィールドは限られています。タスクのすべての情報の編集については、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

この記事では、「タスクの詳細」の概要エリアで情報を表示または編集する方法について説明しています。「タスクの詳細」の他のエリアの更新については、次の記事を参照してください。

* [「タスクの詳細」セクションでのタスクの財政の管理](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
* [オブジェクトへのカスタムフォームの追加](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)
* [オブジェクトに添付されたカスタムフォームを管理](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
   *保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。 
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> プラン*</b> </p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> ライセンス*</b> </p> </td> 
   <td> <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>プロジェクトとタスクへのアクセス権またはそれ以上の権限</p> <p>適切なアクセスレベルを持っていても「タスクの詳細」セクションを編集できない場合は、アクセスレベルに追加の制限が設定されていないかどうかを Adobe Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクト権限</strong> </p> </td> 
   <td> <p>プロジェクトへの参加権限またはそれ以上の権限</p> <p>「タスクの詳細」セクションの情報を閲覧するための、タスクの表示権限。 </p> 
   <p>「タスクの詳細」セクションの以下の情報を更新するための、タスクへの参加権限</p>

<ul>
   <li>説明</li>
   <li>ステータス</li>
   </ul>

<p>「タスクの詳細」セクションのすべての情報を更新するための、タスクの管理権限。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 「タスクの詳細」セクションの概要エリアでのタスク情報の編集

1. 表示または編集するタスクに移動します。
1. 左パネルの「**タスクの詳細**」をクリックします。
1. **概要**&#x200B;エリアに移動して、タスクに関する詳細情報を表示します。

   デフォルトでは、概要は「タスクの詳細」セクションの最初のエリアで、既に展開されています。

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者がレイアウトテンプレートを設定する方法によっては、「タスクの詳細」セクションのフィールドが再配置されるか、表示されない場合があります。詳しくは、[レイアウトテンプレートを使用した詳細表示のカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

1. 「タスクの詳細」セクションの右上隅にある&#x200B;**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックしたあと、「**概要**」をクリックします。

   >[!TIP]
   >
   >Workfront で自動的に生成されたフィールドや、編集権限がないフィールドは編集できません。

1. 編集可能なフィールドをシングルクリックして編集するか、「**+ 追加**」をクリックして空のフィールドに情報を追加します。
1. 下記のフィールドのいずれかを表示または編集します。

   すべてのフィールドが編集可能であるわけではありません。 

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
      <td>これはタスクの一意の値で、システム内のあらゆるオブジェクトに対して Workfront で生成されるものです。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>タスクに対する管理権限を持つユーザーは、このフィールドに内部ページまたは外部ページへのリンクを指定できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステータス</td> 
      <td> <p>タスクが開発のどのような段階にあるかを示す、タスクのステータスを選択します。</p> <p>ヒント：タスクヘッダーでタスクのステータスを更新できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">優先度</td> 
      <td> <p>これは、タスクを優先付けするための視覚的なフラグです。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p> なし</p> </li> 
        <li> <p> 低 </p> </li> 
        <li> <p>標準 </p> </li> 
        <li> <p>高 </p> </li> 
        <li> <p> 緊急 </p> </li> 
       </ul> <p>Workfront 管理者が選択したプロジェクト設定に応じて、優先順位の名前が異なる場合があります。タスクの優先度については、<a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">タスクの優先度の更新</a>.を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間タイプ</td> 
      <td> <p>これにより、以下の項目間の関係が明らかになります。 </p> 
       <ul> 
        <li> <p>タスクに割り当てられたリソースの数 </p> </li> 
        <li> <p>タスクの完了に必要な合計作業量 </p> </li> 
        <li> <p> タスクの合計期間。 </p> </li> 
       </ul> <p>システムまたはグループのタスクについては、Workfront 管理者<span>またはグループ管理者</span>がデフォルトの「期間タイプ」設定を選択します。プロジェクトデフォルトの設定については、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>を参照してください。 </p> <p>期間タイプを使用すると、タスクのニーズに基づいて一貫したリソース割り当てを設定できます。タスクの期間タイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク継続期間と期間タイプの概要</a>を参照してください。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p>予定割り当て時間 </p> </li> 
        <li> <p> 予定作業 </p> </li> 
        <li> <p>残存作業時間の優先 </p> </li> 
        <li> <p>シンプル</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td> 
       <div> 
        <div> 
         <p>タスクが完了するまでタスクを開いたままにしておくことができる時間です。 </p> 
         <p>重要：タスク継続期間は通常、予定開始日から予定完了日までの時間なので、プロジェクトのタイムラインに影響を及ぼします。</p> 
         <p>タスクの期間と時間の単位を指定するには、以下を行います。</p> 
         <ul> 
          <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">時間の長さを入力し、ドロップダウンメニューに表示される時間の単位から選択します。</p> </li> </ul>

   <p><strong>ヒント</strong></p> <p> タスクリストのタスクの期間を更新する際は、時間の単位の省略形を使用できます。 </p>      <p> 次の表にある通常時間または経過時間のオプションから選択できます。 </p> 
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
            <td>日。これがデフォルトです。 </td> 
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
         <p><strong>メモ</strong> </p>
         <p> 経過時間は、タスクの期間の時間単位です。タスクの予定開始日から予定完了日までの時間で、休日、週末および休暇を含みます。つまり、経過時間はカレンダーの日数の経過です。通常の時間は、休日、週末および休暇を考慮し、これらをタスクの期間から除外します。タスクの期間について詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間タイプの概要</a>を参照してください。 </p> 
         <p> 
         <!--You cannot specify the Duration of a task when the Duration Type of the task is Simple, or when the Task Constraint is Fixed Dates. (NOTE: Anna said this is now possible for all duration types in the Assignments area. It's not here, but to clear confusion, I am drafting this out of here.)--></p> 
        </div> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">見込み期間</td> 
      <td> <p>見込み開始日から見込み完了日までの日数。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の期間</td> 
      <td> <p>実際の開始日から実際の完了日までの日数。その作業を完了するのに実際にかかった時間です。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定時間数</td> 
      <td> <p>タスクの予定時間数を時間単位で指定します。タスクの担当者がタスクを完了するのにかかる実際の時間です。タスクの予定時間数を指定できるのは、期間タイプが予定割り当て時間に設定されている場合のみです。期間タイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間タイプの概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の時間数</td> 
      <td>ユーザーがタスクに関して記録した時間数。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">作業量 </td> 
      <td> 
       <div> 
        <p>タスクの完了に必要な工数。プロジェクトマネージャーは、タスクの完了に必要な作業量を見積もる際に、予定時間数の代わりにこのフィールドを使用することにします。このフィールドは、次の条件を満たした場合にのみ表示されます。</p> 
        <ul> 
         <li> <p>タスクの期間タイプが「シンプル」である。 </p> <p>ヒント：タスクの期間タイプを変更すると、このフィールドはグレー表示になります。 </p> </li> 
         <li>プロジェクトマネージャーが、プロジェクトの「作業量を使うとタスクの予定時間数を自動的に計算できます」フィールドを有効にしてある。 </li> 
        </ul> 
        <p>次のオプションから選択します。</p> 
        <ul> 
         <li>小</li> 
         <li>中<span style="font-weight: normal;">（新しいタスクのデフォルト値）</span></li> 
         <li>大</li> 
        </ul> 
        <p><strong>メモ</strong></p> 
        <p> 工数を更新すると、タスクの予定時間数が更新される可能性があります。プロジェクトの更新タイプが「自動」の場合、更新は即時に行われます。プロジェクトの更新タイプが「手動」の場合、更新された予定時間数を確認するにはタイムラインを再計算する必要があります。 </p> 
        <p>予定時間数ではなく作業量を使用したタスク工数の見積もりについては、<a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>を参照してください。 </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タスクの制約</td> 
      <td> <p>タスクをいつ完了する必要があるかを、タスクの制約を指定して決定します。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p><span>固定日付</span> </p> <p><strong>予定開始日</strong>と<strong>予定完了日</strong>を指定します。 </p> </li> 
        <li> <p><span>指定日に開始</span> </p> <p><strong>予定開始日</strong>を指定します。 </p> </li> 
        <li> <p><span>指定日に終了</span> </p> <p><strong>予定完了日</strong>を指定します。 </p> </li> 
       </ul> 
       <ul> 
        <li> <p><span>できるだけ早く</span></p> </li> 
        <li> <p><span>できるだけ遅く</span></p> </li> 
        <li> <p><span>最も早い空き時間</span></p> </li> 
        <li> <p> <span>最も遅い空き時間</span></p> </li> 
        <li> <p><span>指定日までに開始</span> </p> </li> 
        <li> <p>予定開始日を指定します。</p> </li> 
        <li> <p><span>指定日以後に開始</span> </p> <p><strong>予定開始日</strong>を指定します。 </p> </li> 
        <li> <p> <span>これよりも遅く終了しない</span></p> <p><strong>予定完了日</strong>を指定します。 </p> </li> 
        <li> <p> <span>これよりも早く終了しない</span></p> <p><strong>予定完了日</strong>を指定します。</p> </li> 
       </ul> <p>タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定開始日</td> 
      <td> <p>タスクの開始がいつに予定されているか。タスクの予定開始日が設定され、次のような様々な要因の影響を受けます。</p> 
       <ul> 
        <li>タスクの開始予定日に関するシステム全体の環境設定に応じて、プロジェクトの新規タスクの開始日は、デフォルトで本日またはプロジェクトの開始日になります。<span>プロジェクトに関連付けられたグループのグループ管理者も、グループに対してこの環境設定を行うことができます。</span>システムレベルまたはグループレベルのタスク環境設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">システム全体のタスクとイシューの環境設定の指定</a>を参照してください。</li> 
        <li>タスクの先行タスクに応じて、予定開始日は、先行タスクの終了後（または先行タスク関係によっては開始後）の次の設定可能な日付として Workfront によって選択されます。先行タスク関係について詳しくは、<a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">タスク先行タスクの概要</a>を参照してください。</li> 
        <li>タスクの制約が「固定日付」または「指定日に開始」のいずれかである場合、プロジェクトマネージャーまたはタスク責任者は、予定開始日を手動で設定できます。タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>を参照してください。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">見込み開始日</td> 
      <td> <p>前のタスクの進行状況と完了に基づいてタスクが開始される「実際の」日付。これは計算フィールドであり、手動で編集することはできません。</p> <p> プロジェクトが最初に計画された時点では、見込み開始日と予定開始日は最初は同じです。プロジェクトが進行し、タスクがまだ開始されていない場合は、見込み開始日が予定開始日からずれる可能性があります。見込み開始日について詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">プロジェクトの見込み開始日の概要</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の開始日</td> 
      <td> <p>タスクの実際の開始日を指定します。タスクのステータスを「進行中」に変更すると、デフォルトは通常、自動的に設定されます。実際の開始日は、プロジェクトマネージャーまたはタスク責任者が手動で変更することもできます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定完了日</td> 
      <td> <p>タスクの計画時に予想される完了日。予定完了日は、次のようなさまざまな要因によって設定できます。</p> 
       <ul> 
        <li>予定完了日は、予定開始日にタスクの期間を加算することによって、予定開始日から計算されます。プロジェクトマネージャーまたは Workfront 管理者がタスクの期間を指定すると、予定完了日の更新がトリガーされます。予定日が変更される原因の多くは、タスクの期間の更新です。</li> 
        <li>タスクの制約が「固定日付」か「指定日に終了」のいずれかである場合、プロジェクトマネージャーまたはタスク責任者は、予定完了日を手動で設定できます。タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>を参照してください。</li> 
        <li>タスクの期間タイプが変更され、同時にタスクのリソース数が変更されると、予定完了日も変更されます。期間タイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間タイプの概要</a>を参照してください。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">見込み完了日</td> 
      <td> <p>前のタスクの進行状況と担当者によるタスクの進行状況の更新に基づいてタスクが完了する「実際の」日付。これは計算フィールドであり、手動で編集することはできません。</p> <p> プロジェクトが最初に計画された時点では、見込み完了日と予定完了日は最初は同じです。プロジェクトが進行し、タスクがまだ開始されていない場合は、見込み完了日が予定完了日からずれる可能性があります。見込み完了日について詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">プロジェクト、タスクおよびイシューの見込み完了日の概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の完了日</td> 
      <td> <p>タスクが完了する実際の日時を指定します。タスクが完了するデフォルトの日付と時刻は、ステータスが「完了」になる実際の日時と常に一致します。実際の完了日は、プロジェクトマネージャーまたはタスク責任者が手動で変更することもできます。 </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">コミット日</td> 
      <td> <p>これは、タスクに割り当てられたユーザーがそのタスクの完了期限として約束する日付です。これは、予定完了日とは異なる場合があります。担当者のみがこのフィールドを編集できます。Workfront でのコミット日については、<a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">コミット日の概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">エントリ日</td> 
      <td>タスクが作成された日付。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">入力者</td> 
      <td>タスクを作成したユーザー。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">最終更新日</td> 
      <td> <p>タスクが最後に更新された日付。 </p> <p>ヒント：Workfront では、タスクが編集され保存されるたびに更新日を記録します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">最終更新者</td> 
      <td> <p>タスクを最後に更新したユーザー。</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">繰り返し頻度</td> 
      <td> <p>これは、定期タスクの親にのみ表示されます。これは、繰り返しの中のタスクが発生する頻度です。定期タスクの作成については、<a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">定期タスクの作成</a>を参照してください。 </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">発生ごとの所要時間</td> 
      <td> <p>これは、定期タスクの親にのみ表示されます。各定期タスクの期間を表示します。定期タスクの作成については、<a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">定期タスクの作成</a>を参照してください。 </p> <p><strong>メモ</strong></p> <p> 個々の定期タスクで変更された期間には、このフィールドに示された値は表示されません。 </p> </td> 
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
