---
product-area: projects
navigation-topic: manage-tasks
title: タスクの編集
description: 自分で作成したタスクに関する情報、または Contribute または Manage 権限を持っているタスクに関する情報を編集できます。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: ht
source-wordcount: '3712'
ht-degree: 100%

---

# タスクの編集

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


自分で作成したタスクに関する情報、または Contribute または Manage 権限を持っているタスクに関する情報を編集できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
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
    </ul> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## タスクの編集に関する制限

タスクを編集できない場合がある制限がいくつかあります。

タスクを編集する際は、次の点に注意してください。

* 「現在」ステータスのプロジェクトのタスクトリガーの通知の更新：タスクに割り当てられたユーザーが混乱するのを避けるには、プロジェクトのステータスが「現在」の場合に編集タスクをできる限り制限します。
* 承認プロセス内のタスクは編集できません。承認プロセスでのタスクのログ時間またはステータスの更新のみが可能です。

  ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* 完了、無効または承認保留中のステータスを持つプロジェクトのタスクに対するドキュメントの編集や追加は、Workfront 管理者またはグループ管理者がプロジェクト環境設定エリアでこの機能を有効にした場合にのみ行うことができます。プロジェクトの環境設定について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

* プロジェクトが「完了」、「無効」とマークされている、または「承認プロセス中」の場合、タスクに関する次の情報をいつでも編集できます。

   * 時間のログ記録
   * 既存の費用の編集
   * カスタムフォームの添付

## リスト内のタスクの編集

リストのビューに表示されるインライン編集フィールドを使用して、タスクのリスト内のタスク情報を編集できます。

リスト内のタスクの編集について詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)を参照してください。

## 概要を使用してリスト内のタスクを編集

概要パネルを使用して、リスト内のタスクを編集できます。概要パネルでのタスクの編集について詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)の「概要パネルでのタスクの編集」を参照してください。

## 「タスクを編集」ボックスでのタスクの編集

タスクの編集エリアまたはタスクの詳細エリアを使用してタスクを編集できます。次の手順では、「タスクを編集」ボックスでタスクを編集する方法を説明します。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. **プロジェクト**&#x200B;をクリックし、プロジェクトの名前をクリックして開きます。
1. 左側のパネルの&#x200B;**タスク**&#x200B;をクリックします。
1. 編集するタスクをクリックします。
1. （オプション）タスクに関する限定的な情報を編集するには、左側のパネルで「**タスクの詳細**」をクリックします。

   ![](assets/nwe-task-details-expanded-350x273.png)

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

   1. （オプション）すべてのエリアを折りたたむには、右上隅の&#x200B;**すべて折りたたむ**&#x200B;アイコン ![](assets/collapse-all-icon.png) をクリックします。
   1. （オプションおよび条件付き）エリアが折りたたまれている場合、各エリアの横にある&#x200B;**右向き矢印** ![](assets/right-pointing-arrow.png) をクリックして、編集するエリアを展開します。
   1. 「タスクの詳細」タブでの情報の編集について詳しくは、次の記事を参照してください。

      * [「タスク詳細概要」領域でのタスク情報の管理](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [タスクの詳細セクションでのタスクの財政の管理](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. （オプション）タスクにカスタムフォームが添付されていない場合は、「**カスタムフォームの追加**」フィールドに値を入力を開始し、リストに表示されたらフォームを選択して、「**変更を保存**」をクリックします。
   1. （オプション）**書き出し**&#x200B;アイコン ![](assets/export.png) をクリックして概要とカスタムフォーム情報を PDF ファイルに書き出し、「**書き出し**」をクリックします。次の中から選択します。

      * すべてを選択（1 つ以上のカスタムフォームが添付されている場合にのみ表示）
      * 概要
      * 1 つまたは複数のカスタムフォームの名前

      PDF ファイルがお使いのコンピューターにダウンロードされます。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      詳しくは、[カスタムフォームとオブジェクトの詳細を書き出す](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)を参照してください。

1. （条件付き）タスクに関するすべての情報を編集するには、タスクに対する管理権限を持つユーザーとして、タスク名の横で&#x200B;**その他**&#x200B;メニュー ![](assets/more-icon.png)「**編集**」の順にクリックします。

   または

   タスクのリストから、タスクを選択し、**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。

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

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者がレイアウトテンプレートを設定する方法に応じて、タスクを編集ボックスのフィールドが並べ替えられたり、表示されなかったりする場合があります。詳しくは、[レイアウトテンプレートを使用して詳細ビューをカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

### タスク名 {#task-name}

1. 上記の説明に従って、タスクの編集を開始します。
1. 左側のパネルで&#x200B;**タスク名**&#x200B;をクリックします。

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. タスクの名前をアップデートします。

1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

### 概要 {#overview}

1. 上記の説明に従って、タスクの編集を開始します。
1. 左側のパネルで「**承認**」をクリックします。

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

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
      <td> <p>タスクが開発のどのような段階にあるかを示す、タスクのステータスを選択します。</p> <p><b>ヒント</b>

   タスクのステータスを、タスクのヘッダーでアップデートできます。 </p> </td>
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
       </ul> <p>Workfront 管理者が選択したプロジェクト設定に応じて、優先順位の名前が異なる場合があります。タスクの優先度について詳しくは、<a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">タスクの優先度をアップデート</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">「タスクの日付と制約事項」セクション</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タスクの制約</td> 
      <td> <p>タスクをいつ完了する必要があるかを、タスクの制約を指定して決定します。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
      <li> <p><span>固定日付</span> </p> <p>「<strong>予定開始日</strong>」および「<strong>予定完了日</strong>」を指定します。 </p> </li> 
      <li> <p><span>指定日に開始</span> </p> <p>「<strong>予定開始日</strong>」を指定します。 </p> </li> 
      <li> <p><span>指定日に終了</span> </p> <p>「<strong>予定完了日</strong>」を指定します。 </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>できるだけ早く</span></p> </li> 
      <li> <p><span>できるだけ遅く</span></p> </li> 
      <li> <p><span>最も早い空き時間</span></p> </li> 
      <li> <p> <span>最も遅い空き時間</span></p> </li> 
      <li> <p><span>指定日までに開始</span> </p> </li> 
      <li> <p>予定開始日を指定します。</p> </li> 
      <li> <p><span>指定日以後に開始</span> </p> <p>「<strong>予定開始日</strong>」を指定します。 </p> </li> 
      <li> <p> <span>これよりも遅く</span>終了しない</p> <p>「<strong>予定完了日</strong>」を指定します。 </p> </li> 
      <li> <p> <span>これよりも早く</span>終了しない</p> <p><strong>予定完了日</strong>の指定</p> </li> 
       </ul> <p>タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスクの制約の概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">コミット日時</td> 
      <td> <p>これは、タスクに割り当てられたユーザーがそのタスクの完了期限として約束する日付です。これは、予定完了日とは異なる場合があります。担当者のみがこのフィールドを編集できます。Workfront でのコミット日について詳しくは、<a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">コミット日の概要</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定開始日時</td> 
      <td> <p>タスクの開始がいつに予定されているか。タスクの予定開始日が設定され、次のような様々な要因の影響を受けます。</p> 
       <ul> 
      <li>タスクの開始予定日に関するシステム全体の環境設定に応じて、プロジェクトの新規タスクの開始日は、デフォルトで本日またはプロジェクトの開始日になります。<span>プロジェクトに関連付けられたグループのグループ管理者も、グループに対してこの環境設定を指定できます。</span>システムレベルまたはグループレベルのタスクの環境設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">システム全体のタスクとイシューの環境設定の指定</a>を参照してください。</li> 
      <li>タスクの先行タスクに応じて、予定開始日は、先行タスクの終了後（または先行タスク関係によっては開始後）の次の設定可能な日付として Workfront によって選択されます。先行タスクの関係について詳しくは、<a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">タスクの先行タスクの概要</a>を参照してください。</li> 
      <li>タスクの制約が「固定日付」または「指定日に開始」のいずれかである場合、プロジェクトマネージャーまたはタスク責任者は、予定開始日を手動で設定できます。タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスクの制約の概要</a>を参照してください。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定完了日時</td> 
      <td> <p>タスクの計画時に予想される完了日。予定完了日は、次のようなさまざまな要因によって設定できます。</p> 
       <ul> 
      <li>予定完了日は、予定開始日にタスクの期間を加算することによって、予定開始日から計算されます。プロジェクトマネージャーまたは Workfront 管理者がタスクの期間を指定すると、予定完了日の更新がトリガーされます。予定日が変更される原因の多くは、タスクの期間の更新です。</li> 
      <li>タスクの制約が「固定日付」か「指定日に終了」のいずれかである場合、プロジェクトマネージャーまたはタスク責任者は、予定完了日を手動で設定できます。タスクの制約について詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスクの制約の概要</a>を参照してください。</li> 
      <li>タスクの期間タイプが変更され、同時にタスクのリソース数が変更されると、予定完了日も変更されます。期間のタイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>を参照してください。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の開始日時</td> 
      <td> <p>タスクの実際の開始日を指定します。タスクのステータスを「進行中」に変更すると、デフォルトは通常、自動的に設定されます。実際の開始日は、プロジェクトマネージャーまたはタスク責任者が手動で変更することもできます。 </p> </td> 
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
      <li> <p>タスクの期間タイプが「シンプル」である。 </p> <p><b>ヒント</b>

   タスクの期間タイプを変更すると、このフィールドは淡色表示になります。 </p> </li>
   <li>プロジェクトマネージャーが、プロジェクトの「作業量を使うとタスクの予定時間数を自動的に計算できます」フィールドを有効にしてある。 </li> 
      </ul> 
      <p>次のオプションから選択します。</p> 
      <ul> 
      <li>小</li> 
      <li>中 <span style="font-weight: normal;">（これは新規タスクのデフォルト値です）</span></li> 
      <li>大</li> 
      </ul> 
      <p><b>メモ</b>

   工数を更新すると、タスクの予定時間数が更新される可能性があります。プロジェクトの更新タイプが「自動」の場合、更新は即時に行われます。プロジェクトの更新タイプが「手動」の場合、更新された予定時間数を確認するにはタイムラインを再計算する必要があります。 </p>

   <p>予定時間数ではなく作業量を使用してタスク量を見積もる方法について詳しくは、<a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>を参照してください。 </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックするか、次の節に進みます。

### 割り当て {#assignments}

1. 上記の説明に従って、タスクの編集を開始します。
1. 左側のパネルで「**割り当て**」をクリックします。

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. 「**ユーザー、役割、チームを検索する**」をクリックして、タスクに割り当てるユーザー、役割またはチームの名前の入力を開始し、リストに表示されたらクリックするか Enter キーを押します。

   >[!NOTE]
   >
   >ユーザーの名前に特殊文字が含まれている場合は、その特殊文字を検索フィールドに含める必要があります。

   >[!TIP]
   >
   >複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
   >
   >非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
   >
   >* 作業アイテムをアクティブなリソースに再割り当てする。
   >* 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。

1. （オプション）担当者がタスクのプライマリ担当者かどうかを指定するには、名前の隣にある&#x200B;**所有者**&#x200B;ラジオボタンを選択します。チームをタスクのプライマリ担当者にすることはできません。
1. （条件付きおよびオプション）次のフィールドを更新します。

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
       </ul> <p>システムまたはグループのタスクに対する期間タイプのデフォルト設定は、Workfront 管理者 <span> またはグループ管理者 </span> が選択します。プロジェクトのデフォルトの設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>を参照してください。 </p> <p>期間タイプを使用すると、タスクのニーズに基づいて一貫したリソース割り当てを設定できます。タスクの期間タイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間タイプの概要</a>を参照してください。 </p> <p>次のオプションから選択します。 </p> 
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
      <td>日。これがデフォルトです。 </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>週</td> 
      <td>W</td> 
      </tr> 
      <tr> 
      <td>月</td> 
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
   <td> <p>タスクの予定時間数を時間単位で指定します。タスクの担当者がタスクを完了するのにかかる実際の時間です。タスクの予定時間数を指定できるのは、期間タイプが予定割り当て時間に設定されている場合のみです。期間のタイプについて詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>を参照してください。</p> 
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

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. 「**カスタムフォームを追加**」をクリックし、タスクに関連付けるカスタムフォームまたはフォームを選択します。このフィールドでカスタムフォームを選択できるようにするには、まずカスタムフォームを作成する必要があります。アクティブなカスタムフォームのみがリストに表示されます。

   カスタムフォームの作成について詳しくは、[カスタムフォームを作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。1 つのタスクに最大 10 個のカスタムフォームを追加することができます。

1. （条件付き）カスタムフォームをタスクに添付した場合は、フォーム上の任意のフィールドを編集します。タスクを保存する前に、すべての必須フィールドを指定する必要があります。

   >[!NOTE]
   >
   >Workfront 管理者がカスタムフォーム内のセクションに権限を設定する方法によっては、特定のカスタムフォーム上の同じフィールドを誰もが表示または編集できるわけではありません。カスタムフォームのセクション内のフィールドを編集する権限は、タスク自体に対する権限によって異なります。タスク権限の設定については、[タスクの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)を参照してください。

1. 「**保存**」をクリックするか、以降のセクションの編集を続けます。

### 財務 {#finance}

1. [タスクを編集](#Edit2)の節の説明に従って、タスクの編集を開始します。
1. 左側のパネルで「**財務**」をクリックします。

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

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
       </ul> <p>コストの追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。システムまたはグループのタスクに対するデフォルトのコストタイプ設定は、Workfront 管理者またはグループ管理者が選択します。プロジェクトのデフォルトの設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクトの環境設定を指定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">収益タイプ</td> 
      <td> <p>タスクの収益タイプを指定します。これにより、タスクの時間数に基づいて、タスクの収益の計算方法が決まります。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
      <li> <p> 請求不可 </p> </li> 
      <li> <p>ユーザー (毎時) </p> </li> 
      <li> <p>役割（毎時） </p> </li> 
      <li> <p>固定 (毎時) </p> </li> 
      <li> <p>ユーザー (毎時)（上限付き） </p> </li> 
      <li> <p>役割（毎時）（上限付き） </p> </li> 
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

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

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
      <td> <p>平準化の遅延を時間単位で指定します。 </p> <p> 平準化の遅延について詳しくは、<a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">タスクの平準化の遅延をアップデート</a>を参照してください。 </p> </td> 
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

1. 「**保存**」をクリックします。

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## タスクヘッダーでのタスクの編集（制限あり）

タスクヘッダーでは、わずかですが情報を編集できます。

システム管理者またはグループ管理者は、タスクヘッダーに表示されるフィールドをカスタマイズできます。詳しくは、[レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

デフォルトでは、次のフィールドがプロジェクトヘッダーに含まれています。

* タスク名
* 完了率
* 割り当て
* 予定完了日時

  >[!CAUTION]
  >
  >一部のタスクの制約やその他の依存関係が原因で、このフィールドを編集できない場合があります。タスクの制約については、[タスクの制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)を参照してください。

* ステータス
* 現在の承認プロセスで承認者として設定されている場合、承認の決定を行う

## タスクを一括編集

リスト内のタスクに加えた変更を自動的に保存する場合は、リスト内のタスクを一括で編集し、そのすべての情報を同時に更新できます。

タスクの一括保存について詳しくは、[リスト内のタスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)の記事で「タスクを一括編集」の節を参照してください。
