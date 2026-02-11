---
product-area: projects
navigation-topic: manage-tasks
title: タスクの編集
description: 自分で作成したタスクに関する情報を編集したり、自分が投稿権限または管理権限を持っているタスクに関する情報を編集できます。 この記事では、権限がある場合にタスクの検索、検索、編集方法を説明します。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '3928'
ht-degree: 79%

---

# タスクの編集

<!--Audited: 10/2025-->

<!--take out prod and preview references at release, or new and old experience-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a field, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).

</div> -->

自分で作成したタスクに関する情報、または Contribute または Manage 権限を持っているタスクに関する情報を編集できます。

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
   <p>Work またはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <ul> 
     <li> <p>タスクの詳細エリアで次の情報を編集するためのタスクへの参加権限： </p>
     <ul>
     <li>説明</li>
     <li>ステータス</li>
     </ul>  
      </li> 
     <li> <p>詳細エリアと「タスクを編集」ボックスのすべての情報を編集するためのタスクへの管理権限：</p> </li> 
    </ul> 
    <ul> 
     <li> <p>プロジェクトに対する参加以上の権限</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a task to edit the following information in the Task Details area: </p>
     <ul>
     <li>Description</li>
     <li>Status</li>
     </ul>  
      </li> 
     <li> <p>Manage permissions to a task to edit all the information in the Details area and the Edit Task box</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Contribute or higher permissions to the project</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>-->

## タスクの編集に関する制限

タスクを編集できない場合がある制限がいくつかあります。

タスクを編集する際は、次の点に注意してください。

* 「現在」ステータスのプロジェクトのタスクトリガーの通知の更新：タスクに割り当てられたユーザーが混乱するのを避けるには、プロジェクトのステータスが「現在」の場合に編集タスクをできる限り制限します。
* 承認プロセス内のタスクは編集できません。承認プロセスでのタスクのログ時間またはステータスの更新のみが可能です。

  ![&#x200B; 承認プロセスでタスクを編集 &#x200B;](assets/edit-task-in-approval-process-nwe-350x148.png)

* 完了、無効または承認保留中のステータスを持つプロジェクトのタスクに対するドキュメントの編集や追加は、Workfront 管理者またはグループ管理者がプロジェクト環境設定エリアでこの機能を有効にした場合にのみ行うことができます。プロジェクトの環境設定について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

* プロジェクトが「完了」、「無効」とマークされている、または「承認プロセス中」の場合、タスクに関する次の情報をいつでも編集できます。

   * 時間のログ記録
   * 既存の費用の編集
   * カスタムフォームの添付

* 他のユーザーは、タスクに対して行った更新を表示する前に、ページを更新する必要があります。

## リスト内のタスクの編集

リストのビューに表示されるインライン編集フィールドを使用して、タスクのリスト内のタスク情報を編集できます。

リスト内のタスクの編集について詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)を参照してください。

## 概要を使用してリスト内のタスクを編集

概要パネルを使用して、リスト内のタスクを編集できます。概要パネルでのタスクの編集について詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)の「概要パネルでのタスクの編集」を参照してください。

## 「タスクを編集」ボックスでのタスクの編集

タスクの編集エリアまたはタスクの詳細エリアを使用してタスクを編集できます。次の手順では、「タスクを編集」ボックスでタスクを編集する方法を説明します。

{{step1-click-main-menu}}

1. **プロジェクト**&#x200B;をクリックし、プロジェクトの名前をクリックして開きます。
1. 左側のパネルの&#x200B;**タスク**&#x200B;をクリックします。
1. 編集するタスクをクリックします。
1. （オプション）タスクに関する限定的な情報を編集するには、左側のパネルで「**タスクの詳細**」をクリックします。

   ![&#x200B; タスクの詳細が展開されました &#x200B;](assets/nwe-task-details-expanded-350x273.png)

   タスクの詳細セクションの次のエリアにある情報を編集することを検討してください。

   * **概要**

     この領域は、デフォルトで展開されます。

   * **カスタムフォーム**

     カスタムフォームの名前は、オブジェクトにカスタムフォームがアタッチされている場合にのみ表示されます。

   * **財務**

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者がレイアウトテンプレートを変更した方法に応じて、タスクの詳細エリアのフィールドが並べ替えられたり、表示されなかったりする場合があります。詳しくは、[レイアウトテンプレートを使用して詳細ビューをカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

   タスクの詳細セクションに表示されるフィールドの詳細については、次に説明するように、「タスクの編集」ボックスでタスクを編集します。

   「詳細」セクションの情報を編集するには、次の手順を実行します。

   1. （オプション）右上隅の **すべて折りたたむ** アイコン ![&#x200B; すべて折りたたむアイコン &#x200B;](assets/collapse-all-icon.png) をクリックすると、すべての領域が折りたたまれます。
   1. （オプションおよび条件付き）領域が折りたたまれたら、各領域の横にある **右向き矢印**![&#x200B; 右向き矢印 &#x200B;](assets/right-pointing-arrow.png) をクリックして、編集する領域を展開します。
   1. 「タスクの詳細」タブでの情報の編集について詳しくは、次の記事を参照してください。

      * [「タスク詳細概要」領域でのタスク情報の管理](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [タスクの詳細セクションでのタスクの財政の管理](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. （オプション）タスクにカスタムフォームが添付されていない場合は、「**カスタムフォームの追加**」フィールドに値を入力を開始し、リストに表示されたらフォームを選択して、「**変更を保存**」をクリックします。
   1. （オプション） **書き出し** アイコン ![&#x200B; 書き出しアイコン &#x200B;](assets/export.png) をクリックして、概要とカスタムフォーム情報をPDF ファイルに書き出し、「**書き出し**」をクリックします。 次の中から選択します。

      * すべてを選択（1 つ以上のカスタムフォームが添付されている場合にのみ表示）
      * 概要
      * 1 つまたは複数のカスタムフォームの名前

      PDF ファイルがお使いのコンピューターにダウンロードされます。

      ![&#x200B; 「書き出し」ボタンを含むイシューの詳細選択ボックス &#x200B;](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      詳しくは、[カスタムフォームとオブジェクトの詳細の書き出し](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)を参照してください。

1. （条件付き）タスクに関するすべての情報を編集するには、タスクの管理権限を持つユーザーとして、タスク名の横にある **詳細** メニュー ![&#x200B; 詳細アイコン &#x200B;](assets/more-icon.png) をクリックし、「**編集** をクリックします。

   または

   タスクのリストからタスクを選択し、リスト上部の **編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックします。

   タスクを編集ボックスが開きます。

   >[!IMPORTANT]
   >
   >「編集」オプションを表示するには、タスクに対する管理権限が必要です。

   すべてのタスクフィールドが、タスクを編集ボックスで使用でき、左側のパネルに表示されるエリアでグループ化されます。

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者がレイアウトテンプレートを変更した方法に応じて、タスクの詳細エリアのフィールドが並べ替えられたり、表示されなかったりする場合があります。詳しくは、[レイアウトテンプレートを使用して詳細ビューをカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

   次のセクションのいずれかに情報を指定することを検討してください。

   * [タスク名](#task-name)
   * [概要](#overview)
   * [割り当て](#assignments)
   * [カスタムフォーム](#Custom%C2%A0F)
   * [財務](#finance)
   * [設定](#settings)
   * [コメント](#comment)

   >[!NOTE]
   >
   >Workfront管理者またはグループ管理者によるレイアウト テンプレートの設定に応じて、[ タスクの編集 ] ボックスのフィールドの配置が変更されたり、表示されなかったりする場合があります。 詳しくは、[レイアウトテンプレートを使用して詳細ビューをカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

### タスク名 {#task-name}

1. 上記の説明に従って、タスクの編集を開始します。
1. 左側のパネルで&#x200B;**タスク名**&#x200B;をクリックします。

   ![&#x200B; タスクを編集ボックスの「タスク名」セクション &#x200B;](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. タスクの名前をアップデートします。

1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

### 概要 {#overview}

1. 上記の説明に従って、タスクの編集を開始します。
1. 左側のパネルで「**承認**」をクリックします。

   ![&#x200B; 概要セクションの編集タスクボックス &#x200B;](assets/nwe-overview-section-edit-task-box-350x257.png)

1. タスクに関する以下の情報をアップデートします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>タスクに関する追加情報を追加します。 </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">「基本情報」セクション</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステータス</td> 
      <td> <p>タスクの開発ステージを示すタスクのステータスを選択します。</p> <p><b>ヒント</b>

   タスクのステータスを、タスクのヘッダーでアップデートできます。 </p>

   <p>Workfrontまたはグループ管理者が、タスクステータスの名前をカスタマイズできます。 詳しくは、<a href="/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md"> ステータスの作成または編集 </a> を参照してください。 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">優先度</td> 
      <td> <p>これは、タスクに優先順位を付けることができる視覚的なフラグです。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
      <li> <p> なし</p> </li> 
      <li> <p> 低 </p> </li> 
      <li> <p>標準 </p> </li> 
      <li> <p>高 </p> </li> 
      <li> <p> 緊急 </p> </li> 
       </ul> <p>Workfront 管理者が選択したプロジェクト設定に応じて、優先順位の名前が異なる場合があります。タスクの優先度については、<a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">タスクの優先度の更新</a>.を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;"> タスクの日付と制約セクション </span> </td> 
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
       </ul> <p>タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスクの制約の概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">コミット日時</td> 
      <td> <p>これは、タスクに割り当てられたユーザーがそのタスクの完了期限として約束する日付です。この日付は、予定完了日と異なる場合があります。 担当者のみがこのフィールドを編集できます。Workfront でのコミット日について詳しくは、<a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">コミット日の概要</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定開始日時</td> 
      <td> <p>タスクの開始がいつに予定されているか。タスクの予定開始日が設定され、次のような様々な要因の影響を受けます。</p> 
       <ul> 
      <li>タスクの開始予定日に関するシステム全体の環境設定に応じて、プロジェクトの新規タスクの開始日は、デフォルトで本日またはプロジェクトの開始日になります。<span>プロジェクトに関連付けられたグループのグループ管理者も、グループに対してこの環境設定を行うことができます。</span>システムレベルまたはグループレベルのタスク環境設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">システム全体のタスクとイシューの環境設定の指定</a>を参照してください。</li> 
      <li>タスクの先行タスクに応じて、予定開始日は、先行タスクの終了後（または先行タスク関係によっては開始後）の次の設定可能な日付として Workfront によって選択されます。先行タスク関係について詳しくは、<a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">タスク先行タスクの概要</a>を参照してください。</li> 
      <li>タスクの制約が「固定日付」または「指定日に開始」のいずれかである場合、プロジェクトマネージャーまたはタスク責任者は、予定開始日を手動で設定できます。タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスクの制約の概要</a>を参照してください。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定完了日時</td> 
      <td> <p>タスクの計画時に予想される完了日。Workfrontは、次のいくつかの要因を使用して「予定完了日」を設定します。</p> 
       <ul> 
      <li>予定完了日は、予定開始日にタスクの期間を加算することによって、予定開始日から計算されます。プロジェクトマネージャーまたは Workfront 管理者がタスクの期間を指定すると、予定完了日の更新がトリガーされます。予定日が変更される場合、多くの場合、タスクの期間が更新されていることが原因です。</li> 
      <li>タスクの制約が「固定日付」か「指定日に終了」のいずれかである場合、プロジェクトマネージャーまたはタスク責任者は、予定完了日を手動で設定できます。タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>を参照してください。</li> 
      <li>タスクの期間タイプが変更され、同時にタスクのリソース数が変更されると、予定完了日も変更されます。期間のタイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>を参照してください。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の開始日時</td> 
      <td> <p>タスクの実際の開始日を指定します。デフォルトは、通常、タスクのステータスを「処理中」に変更すると自動的に入力されます。 実際の開始日は、プロジェクトマネージャーまたはタスク責任者が手動で変更することもできます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の完了日時</td> 
      <td> <p>タスクが完了する実際の日時を指定します。タスクが完了するデフォルトの日付と時刻は、ステータスが「完了」になる実際の日時と常に一致します。実際の完了日は、プロジェクトマネージャーまたはタスク責任者が手動で変更することもできます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>「作業時間」セクション</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業量 </td> 
      <td>

   <p>タスクの完了に必要な工数。プロジェクトマネージャーは、タスクの完了に必要な作業量を見積もる際に、予定時間数の代わりにこのフィールドを使用することにします。このフィールドは、次の条件を満たした場合にのみ表示されます。</p> 
      <ul> 
      <li> <p>タスクの期間タイプはシンプルです。 </p> <p><b>ヒント</b>

   タスク期間の種類を変更すると、このフィールドは淡色表示になります。 </p> </li>
   <li>プロジェクトマネージャーが、プロジェクトの「作業量を使うとタスクの予定時間数を自動的に計算できます」フィールドを有効にしてある。 </li> 
      </ul> 
      <p>次のオプションから選択します。</p> 
      <ul> 
      <li>小</li> 
      <li>中<span style="font-weight: normal;">（新しいタスクのデフォルト値）</span></li> 
      <li>大</li> 
      </ul> 
      <p><b>メモ</b>

   工数を更新すると、タスクの予定時間数が更新される可能性があります。プロジェクトの更新タイプが「自動」の場合、更新は即時に行われます。プロジェクトの更新タイプが「手動」の場合は、更新された予定時間数を表示するためにタイムラインを再計算する必要があります。 </p>

   <p>予定時間数ではなく作業量を使用してタスク量を見積もる方法について詳しくは、<a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>を参照してください。 </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックするか、次の節に進みます。

### 割り当て {#assignments}

>[!TIP]
>
>タスクの割り当てを一括で編集する場合、選択したタスク間で値が異なるフィールドに複数値インジケーターが表示されます。
>
>選択した各タスクの個々の割り当てを表示することはできません。

1. 上記の説明に従って、タスクの編集を開始します。
1. 左側のパネルで「**割り当て**」をクリックします。

   ![&#x200B; 「タスクを編集」ボックスの「割り当て」セクション &#x200B;](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. **ユーザー、役割、またはチームを検索** をクリックして、タスクに割り当てるユーザー、役割、またはチームの名前の入力を開始し、リストに表示されたらクリックするか Enter キーを押します。

   >[!TIP]
   >
   >* ユーザーの名前に特殊文字が含まれている場合は、その特殊文字を検索フィールドに含める必要があります。
   >* 複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
   >
   >* 非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
   >
   >* 作業アイテムをアクティブなリソースに再割り当てする。
   >* 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。

1. （オプション）担当者の名前にポインタを合わせて、「**プライマリする**」をクリックして、担当者をプライマリ担当者にするかタスクのオーナーにするかを指定します。 チームをタスクのプライマリ担当者にすることはできません。
1. （オプション）次のフィールドを更新します。

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
      <p><b>重要</b>

   タスク期間は通常、予定開始日から予定完了日までの時間で、プロジェクトのタイムラインに影響します。</p>

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

### カスタムフォーム

タスクがプロジェクトに追加されるときに、タスクに自動的に添付されるデフォルトのカスタムフォームを定義できます。すべての新規タスクにデフォルトのタスクカスタムフォームを含めるようにプロジェクトを設定する方法について詳しくは、[プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md)の記事にある「タスク」の節を参照してください。

1. 上記の説明に従ってタスクの編集を開始します。
1. 左側のパネルで&#x200B;**カスタムフォーム**&#x200B;をクリックするか、カスタムフォームが既に添付されている場合には、その名前をクリックします。

   ![&#x200B; カスタムフォームセクションの編集タスクボックス &#x200B;](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. 「**カスタムフォームを追加**」をクリックし、タスクに関連付けるカスタムフォームまたはフォームを選択します。このフィールドでカスタムフォームを選択できるようにするには、まずカスタムフォームを作成する必要があります。アクティブなカスタムフォームのみがリストに表示されます。

   カスタムフォームの作成について詳しくは、[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。タスクには最大 10 個のカスタムフォームを追加できます

1. （条件付き）カスタムフォームをタスクに添付した場合は、フォーム上の任意のフィールドを編集します。タスクを保存する前に、必須フィールドをすべて指定する必要があります。

   >[!NOTE]
   >
   >Workfront 管理者がカスタムフォーム内のセクションに権限を設定する方法によっては、特定のカスタムフォーム上の同じフィールドを誰もが表示または編集できるわけではありません。カスタムフォームのセクション内のフィールドを編集する権限は、タスク自体に対する権限によって異なります。タスク権限の設定については、[タスクの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)を参照してください。

1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

### 財務 {#finance}

1. [タスクを編集](#Edit2)の節の説明に従って、タスクの編集を開始します。
1. 左側のパネルで「**財務**」をクリックします。

   ![&#x200B; 財務セクションの編集タスク ボックス &#x200B;](assets/nwe-finance-section-edit-task-box-350x298.png)

1. 次のフィールドを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">コストタイプ</td> 
      <td> <p>タスクのコストタイプを指定します。これにより、タスクの時間数に基づいて、タスクのコストの計算方法が決まります。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p>コストなし</p> </li> 
        <li> <p>固定 (毎時) </p> </li> 
        <li> <p> ユーザー (毎時) </p> </li> 
        <li> <p> 役割（毎時）</p> </li> 
       </ul> <p>コストの追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。システムまたはグループのタスクに対するデフォルトのコストタイプ設定は、Workfront 管理者またはグループ管理者が選択します。プロジェクトのデフォルトの設定については、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクトの環境設定の指定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">収益タイプ</td> 
      <td> <p>タスクの収益タイプを指定します。これにより、タスクの時間数に基づいて、タスクの収益の計算方法が決まります。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
      <li> <p> 請求不可 </p> </li> 
      <li> <p>ユーザー (毎時) </p> </li> 
      <li> <p>役割（毎時） </p> </li> 
      <li> <p>固定 (毎時) </p> </li> 
      <li> <p>ユーザー (毎時) (キャップ付き) </p> </li> 
      <li> <p>役割（毎時）（キャップ付き） </p> </li> 
      <li> <p>ユーザー（毎時）+ 固定 </p> </li> 
      <li> <p>役割（毎時）+ 固定 </p> </li> 
      <li> <p>固定収益 </p> </li> 
       </ul> <p>収益の追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。 </p> <p>システムまたはグループのタスクに対する収益タイプのデフォルト設定は、Workfront 管理者またはグループ管理者が選択します。プロジェクトのデフォルトの設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクトの環境設定を指定</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

### 設定 {#settings}

1. [タスクを編集](#Edit2)の節の説明に従って、タスクの編集を開始します。
1. 左側のパネルで「**設定**」をクリックします。

   ![[ タスクの編集 ] ボックスの [ 設定 ] セクション &#x200B;](assets/nwe-settings-section-edit-task-box-350x304.png)

1. 次のフィールドを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">トラッキングモード</td> 
      <td> <p>タスクの進捗ステータスの追跡方法を指定します。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
      <li> <p> ユーザーが更新する必要あり </p> </li> 
      <li> <p>予定通りを想定 </p> </li> 
      <li> <p>遅延警告を無視</p> </li> 
      <li> <p> オートコンプリート </p> </li> 
      <li> <p>先行タスク </p> </li> 
       </ul> <p>タスクのトラッキングモードについて詳しくは、<a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">タスクトラッキングモードの概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リソースの標準化</td> 
      <td> <p>タスクに割り当てられたリソースを標準化から除外する場合は、「<strong>リソースの標準化から除外</strong>」フィールドを選択します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">標準化の遅延</td> 
      <td> <p>標準化の遅延を時間単位で指定します。 </p> <p> 平準化の遅延について詳しくは、<a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">タスクの平準化の遅延をアップデート</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認プロセス</td> 
      <td> <p>タスクに関連付ける承認プロセスを選択します。システムレベルの承認プロセスをタスクに関連付けるには、Workfront 管理者がこのプロセスを事前に定義しておく必要があります。承認プロセスへの管理者アクセス権を持つユーザーは、グループ固有の承認プロセスを作成することもできます。 </p> <p>承認プロセスの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">作業アイテムの承認プロセスの作成</a>を参照してください。承認プロセスを追加する際は、次の点を考慮してください。 </p> 
       <ul>

   <li> <p>アクティブな承認プロセスのみがリストに表示されます。 </p> </li>

   <li> <p>システム全体およびグループ固有の承認プロセスがリストに表示されます。プロジェクトの承認プロセス以外のグループに関連付けられている承認プロセスは、リストに表示されません。 </p>

   <p><b>重要</b>

   プロジェクトのグループが変更されると、以前付随していたグループ固有の承認プロセスが、単一使用承認プロセスになります。プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">グループと承認プロセスの変更が割り当てられた承認プロセスに及ぼす影響</a>を参照してください。 </p>

   </li>

   <li> <p>タスクがプロジェクトに追加されるときに、タスクに自動的に添付されるデフォルトの承認プロセスを定義できます。デフォルトのタスク承認プロセスを含めるようにプロジェクトを設定する方法については、<a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">プロジェクトの編集</a>の記事で「タスク」の節を参照してください。 </p> </li>

   <li> <p>タスクを一括編集する場合は、次のシナリオが存在します。 </p> 
      <ul> 
      <li> <p>同じグループから複数のタスクを選択すると、システムレベルとグループレベルの承認プロセスの両方がこのフィールドに表示されます。 </p> </li> 
      <li> <p>異なるグループから複数のタスクを選択すると、このフィールドにはシステムレベルの承認プロセスのみが表示されます。 </p> </li> 
      <li> <p>タスクに 1 回限りの承認プロセスが添付されている場合、選択したシステムレベルまたはグループレベルの承認プロセスに置き換えられます。 </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

### コメント

1. [タスクを編集](#Edit2)の節の説明に従って、タスクの編集を開始します。
1. 左側のパネルで **コメント** をクリックします。

   ![&#x200B; タスクを編集ボックスの「コメント」セクション &#x200B;](assets/comment-section-on-edit-task-box.png)

1. 指定されたスペースに更新を追加します。
1. （オプション）次のいずれかを更新に追加します。

   * **ユーザーをタグ付け** エリアで更新にユーザーまたはチームを追加するか、@を使用して更新に含めます。
   * 「**会社に非公開**」チェックボックスを選択して、会社内のユーザーに対して更新を非公開にします。

   >[!TIP]
   >
   >**会社に非公開** 設定は、Workfront プロファイルが会社に関連付けられている場合にのみ使用できます。

1. 「**保存**」をクリックします。

## タスクヘッダーでのタスクの編集（制限あり）

タスクヘッダーでは、わずかですが情報を編集できます。

システム管理者またはグループ管理者は、タスクヘッダーに表示されるフィールドをカスタマイズできます。詳しくは、[レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。


![&#x200B; 承認なしの依存関係を持つタスクヘッダー &#x200B;](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

次のフィールドは、デフォルトでタスクヘッダーに含まれています。

* タスク名
* 完了率

  詳しくは、[&#x200B; タスクの完了率の表示と更新 &#x200B;](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md) を参照してください。
* 割り当て
* 予定完了日

  >[!CAUTION]
  >
  >一部のタスクの制約やその他の依存関係により、タスクの予定完了日を編集できない場合があります。 タスクの制約については、[タスクの制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)を参照してください。

* ステータス
* 現在の承認プロセスで承認者として設定されている場合、承認の決定を行う

## タスクを一括編集

リスト内のタスクに加えた変更を自動的に保存する場合は、リスト内のタスクを一括で編集し、そのすべての情報を同時に更新できます。

タスクの一括保存について詳しくは、「リストでのタスクの編集 [&#x200B; の「タスクの一括編集」の節を参照してくだ &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) い。

<!--Temporary content while changing Assignments area: 

Editing assignments is different in the Edit Task box depending on which environment you choose.

#### Edit the Assignments area in the Production environment

>[!NOTE]
>
><span class="preview">Some customers can edit Assignments in the Edit Task box in their Production environments the same way they edit them in their Preview environment.</span>
>
><span class="preview">For information about editing tasks in the Preview environment, see the section [Edit the Assignments area in the Preview environment](#edit-the-assignments-area-in-the-preview-environment) in this article. </span>

1. Begin editing your task as described above.
1. Click **Assignments** in the left panel.

      The Assignments area opens in the new experience. 

1. (Conditional) Using the new experience, do the following:
 
   1. Start typing the name of a user, job role, or team in the **Search people, role or team** field, then select them when they display in the list

      Or

      Click **Assign to me** to assign the task to yourself. 

   1. Update the following information:

         <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
         <tr> 
         <td role="rowheader">Duration Type</td> 
         <td> <p>This identifies the relationship between the following: </p> 
         <ul> 
         <li> <p>The number of resources assigned to a task </p> </li> 
         <li> <p>The total effort required to complete the task </p> </li> 
         <li> <p> The total duration of the task. </p> </li> 
         </ul> <p>Your Workfront administrator or a group administrator selects the default Duration Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>. </p> <p>Duration Types enable you to set consistent resource assignments based on the needs of the task. For more information about the Duration Type of a task, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p> <p>Select from the following options: </p> 
         <ul> 
         <li> <p>Calculated Assignment </p> </li> 
         <li> <p> Calculated Work </p> </li> 
         <li> <p>Effort Driven </p> </li> 
         <li> <p>Simple</p> </li> 
         </ul> </td> 
         </tr> 
         <td role="rowheader">Duration per Occurrence</td> 
         <td> <p>This displays only on the parent of recurring tasks. It displays the duration of each recurring task, as defined when the task was created. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>. </p> <p> <b>NOTE</b>          
         Durations modified in individual recurring tasks do not display the value indicated in this field. </p> </td> 
         </tr>
         <tr> 
         <td role="rowheader">Duration</td> 
         <td> 
         <div> 
         <div> 
         <p>This is the amount of time that you allow a task to remain open before it is completed. </p> 
         <p><b>IMPORTANT</b>
      
         Because the task duration is typically the amount of time between the Planned Start and the Planned Completion Dates, it affects the timeline of the project.</p> 
      
         <p>To indicate the Duration of the task and the unit of time do the following:</p> 
         <ul> 
         <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Type the length of time and select from the units of time available in the drop-down menu.</p> <p><b>TIP</b></p>
         When you update the Duration of tasks in a task list, you can use the abbreviation for the unit of time. </p> </li> 
         </ul> 
         <p> You can choose from the regular time or elapsed time options in the following table: </p> 
         <table style="table-layout:auto"> 
         <col> 
         <col data-mc-conditions=""> 
         <tbody> 
         <tr> 
         <td>Unit of Time</td> 
         <td>Abbreviation</td> 
         </tr> 
         <tr> 
         <td>Minutes</td> 
         <td>M</td> 
         </tr> 
         <tr> 
         <td>Hours</td> 
         <td>H</td> 
         </tr> 
         <tr> 
         <td>Days. This is the default. </td> 
         <td>D</td> 
         </tr> 
         <tr> 
         <td>Weeks</td> 
         <td>W</td> 
         </tr> 
         <tr> 
         <td>Months</td> 
         <td>T</td> 
         </tr> 
         <tr> 
         <td>Elapsed Minutes</td> 
         <td>EM</td> 
         </tr> 
         <tr> 
         <td>Elapsed Hours</td> 
         <td>EH</td> 
         </tr> 
         <tr> 
         <td>Elapsed Days</td> 
         <td>ED</td> 
         </tr> 
         <tr> 
         <td>Elapsed Weeks</td> 
         <td>EW</td> 
         </tr> 
         <tr> 
         <td>Elapsed Months</td> 
         <td>ET</td> 
         </tr> 
         </tbody> 
         </table> 

         <p><b>NOTE</b>
         
         <p>Elapsed time is a unit of time for a task's Duration. It is the time between the Planned Start Date and the Planned Completion Date of a task that includes holidays, weekends, and time off. In other words, elapsed time is the passage of calendar days. 

         Regular time takes into account holidays, weekends, and time off and excludes them from the Duration of the task. For more information about task duration, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p>
         </td> 
         </tr> 
         <tr> 
         <td role="rowheader">Planned Hours</td> 
         <td> <p>Specify the number of Planned Hours for the task, in hours. This is the amount of actual time that it would take the assignees of the task to complete it. You can only specify the number of Planned Hours for a task when the Duration Type is set to Calculated Assignment. For more information about duration types, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> 
         <b>NOTE</b>
         <p>
         When creating recurring tasks, the Planned Hours are those of each occurrence. The Planned Hours of the parent tasks are the total of all Planned Hours from all the occurrences. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>.
         </p>
         
         </td> 
         </tr> 
         </tbody> 
         </table>
      
   
      <!--<tr> 
      <td role="rowheader">Allocation</td> 
      <td> <p>If your Task Constraint is Calculated Work or Effort Driven, specify the <strong>Allocation %</strong> (allocation percentage) for each assignee. This is the amount of time from the schedule of the assignee that they can spend on this task. Changing the allocation percentage for an assignee will change the Planned Hours of a task. </p> <p>When the Task Constraint is Simple, you can specify the following:</p> 
         <ul> 
         <li> <p>Allocation Hours of each assignee.</p> </li> 
         <li> <p>Planned Hours of the task</p> </li> 
         <li> <p>Duration of the task</p> </li> 
         </ul> </td> 
      </tr> 
      <tr> 
      <td role="rowheader">Assignee's Role</td> 
      <td> <p>Select a role from the <strong>Assignee's Role</strong> drop-down menu when you selected a person as an assignee. This is the role that the assignee can fulfill on this task. </p> <p><b>TIP</b>
         Only the job roles associated with each assignee in their profile appear in the drop-down menu.</p> </td> 
         </tr>
         </tbody> 
         </table>**********************

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Task** box. 
      The Assignments area opens in the old experience. 
   
      ![Assignments section in the Edit Task box](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. (Conditional) Using the old experience, do the following: 

   1. Click **Search people, roles, or teams** and start typing the name of a user, role, or team that you want to assign to the task, then click it or press Enter when it displays on the list.

      >[!TIP]
      >
      >* If the user's name contains a special character, you must include the special character in the search field.
      >* You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
      >
      >* If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following: 
      >
      >* Reassign the work item to active resources. 
      >* Associate the users in a deactivated team with an active team and reassign the work item to the active team. 

   1. (Optional) Hover over an assignee's name, then click **Make Primary** to indicate whether an assignee is the primary assignee or the owner of the task. A team cannot be the primary assignee of a task. 
   1. (Optional) Update the following fields: 

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Duration Type</td> 
         <td> <p>This identifies the relationship between the following: </p> 
         <ul> 
         <li> <p>The number of resources assigned to a task </p> </li> 
         <li> <p>The total effort required to complete the task </p> </li> 
         <li> <p> The total duration of the task. </p> </li> 
         </ul> <p>Your Workfront administrator or a group administrator selects the default Duration Type setting for the tasks in your system or your group. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>. </p> <p>Duration Types enable you to set consistent resource assignments based on the needs of the task. For more information about the Duration Type of a task, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p> <p>Select from the following options: </p> 
         <ul> 
         <li> <p>Calculated Assignment </p> </li> 
         <li> <p> Calculated Work </p> </li> 
         <li> <p>Effort Driven </p> </li> 
         <li> <p>Simple</p> </li> 
         </ul> </td> 
      </tr> 
      <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
         <td role="rowheader">Duration per Occurrence</td> 
         <td> <p>This displays only on the parent of recurring tasks. It displays the duration of each recurring task, as defined when the task was created. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>. </p> <p> <b>NOTE</b> 
         
         Durations modified in individual recurring tasks do not display the value indicated in this field. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Duration</td> 
         <td> 
         <div> 
         <div> 
         <p>This is the amount of time that you allow a task to remain open before it is completed. </p> 
         <p><b>IMPORTANT</b>
         
         Because the task duration is typically the amount of time between the Planned Start and the Planned Completion Dates, it affects the timeline of the project.</p> 
         
         <p>To indicate the Duration of the task and the unit of time do the following:</p> 
         <ul> 
         <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Type the length of time and select from the units of time available in the drop-down menu.</p> <p><b>TIP</b></p>
         When you update the Duration of tasks in a task list, you can use the abbreviation for the unit of time. </p> </li> 
         </ul> 
         <p> You can choose from the regular time or elapsed time options in the following table: </p> 
         <table style="table-layout:auto"> 
         <col> 
         <col data-mc-conditions=""> 
         <tbody> 
         <tr> 
         <td>Unit of Time</td> 
         <td>Abbreviation</td> 
         </tr> 
         <tr> 
         <td>Minutes</td> 
         <td>M</td> 
         </tr> 
         <tr> 
         <td>Hours</td> 
         <td>H</td> 
         </tr> 
         <tr> 
         <td>Days. This is the default. </td> 
         <td>D</td> 
         </tr> 
         <tr> 
         <td>Weeks</td> 
         <td>W</td> 
         </tr> 
         <tr> 
         <td>Months</td> 
         <td>T</td> 
         </tr> 
         <tr> 
         <td>Elapsed Minutes</td> 
         <td>EM</td> 
         </tr> 
         <tr> 
         <td>Elapsed Hours</td> 
         <td>EH</td> 
         </tr> 
         <tr> 
         <td>Elapsed Days</td> 
         <td>ED</td> 
         </tr> 
         <tr> 
         <td>Elapsed Weeks</td> 
         <td>EW</td> 
         </tr> 
         <tr> 
         <td>Elapsed Months</td> 
         <td>ET</td> 
         </tr> 
         </tbody> 
      </table> 

         <p><b>NOTE</b>
            
         <p>Elapsed time is a unit of time for a task's Duration. It is the time between the Planned Start Date and the Planned Completion Date of a task that includes holidays, weekends, and time off. In other words, elapsed time is the passage of calendar days. 

         Regular time takes into account holidays, weekends, and time off and excludes them from the Duration of the task. For more information about task duration, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>. </p>
         </div> 
         </div> </td> 
         </tr> 
         <tr> 
         <td role="rowheader">Planned Hours</td> 
         <td> <p>Specify the number of Planned Hours for the task, in hours. This is the amount of actual time that it would take the assignees of the task to complete it. You can only specify the number of Planned Hours for a task when the Duration Type is set to Calculated Assignment. For more information about duration types, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p> 
         <b>NOTE</b>
         <p>
         When creating recurring tasks, the Planned Hours are those of each occurrence. The Planned Hours of the parent tasks are the total of all Planned Hours from all the occurrences. For information about creating recurring tasks, see <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Create recurring tasks</a>.
         </p>
         
         </td> 
         </tr> 
         <tr> 
         <td role="rowheader">Allocation</td> 
         <td> <p>If your Task Constraint is Calculated Work or Effort Driven, specify the <strong>Allocation %</strong> (allocation percentage) for each assignee. This is the amount of time from the schedule of the assignee that they can spend on this task. Changing the allocation percentage for an assignee will change the Planned Hours of a task. </p> <p>When the Task Constraint is Simple, you can specify the following:</p> 
            <ul> 
            <li> <p>Allocation Hours of each assignee.</p> </li> 
            <li> <p>Planned Hours of the task</p> </li> 
            <li> <p>Duration of the task</p> </li> 
            </ul> </td> 
         </tr> 
         <tr> 
         <td role="rowheader">Assignee's Role</td> 
         <td> <p>Select a role from the <strong>Assignee's Role</strong> drop-down menu when you selected a person as an assignee. This is the role that the assignee can fulfill on this task. </p> <p><b>TIP</b>
         
         Only the job roles associated with each assignee in their profile appear in the drop-down menu.</p> </td> 
            </tr> 
            </tbody> 
            </table>

1. Click **Save** or continue with the following sections.

<div class="preview">

#### Edit the Assignments area in the Preview environment-->