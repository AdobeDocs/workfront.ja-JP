---
product-area: templates
keywords: タスク，デフォルト，自動化，作成
navigation-topic: templates-navigation-topic
title: テンプレートタスクの編集
description: テンプレートを作成した後、テンプレートタスクに関する情報を編集できます。 テンプレートタスクで更新する情報は、テンプレートを使用してプロジェクトを作成した後、またはテンプレートをプロジェクトに添付した後に、プロジェクトタスクに関連付けられます。
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '2470'
ht-degree: 6%

---

# テンプレートタスクの編集

テンプレートを作成した後、テンプレートタスクに関する情報を編集できます。 テンプレートタスクで更新する情報は、テンプレートを使用してプロジェクトを作成した後、またはテンプレートをプロジェクトに添付した後に、プロジェクトタスクに関連付けられます。

テンプレートの作成について詳しくは、 [プロジェクトテンプレートの作成](../../../manage-work/projects/create-and-manage-templates/create-template.md).

## アクセス要件

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
   <td role="rowheader">AdobeWorkfrontlicense*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>テンプレートへのアクセスを編集</p> <p>注意：正しいアクセス権を持っていても、テンプレートタスクを編集できない場合は、Workfront管理者にアクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong> </td> 
   <td> <p>テンプレートの権限を管理します。 </p> <p>テンプレートタスクに対する Contribute 以上の権限。</p> <p>オブジェクトへのアクセス要求については、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセスレベルを確認するには、Workfront管理者に問い合わせてください。

## 前提条件

始める前に、

* テンプレートを作成します。

   テンプレートの作成について詳しくは、 [プロジェクトテンプレートの作成](../../../manage-work/projects/create-and-manage-templates/create-template.md).

## テンプレートタスクの編集

「テンプレートタスクの編集」領域または「テンプレートタスクの詳細」領域を使用して、テンプレートタスクを編集できます。 次の手順では、「テンプレートタスクの編集」ボックスでタスクを編集する方法を説明します。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **テンプレート**.
1. テンプレートの名前をクリックして開きます。
1. クリック **テンプレートタスク** をクリックします。
1. リスト内のテンプレートタスクの名前をクリックして、テンプレートタスクを開きます。
1. （条件付き）テンプレートタスクに関する限定的な情報を編集するには、 **テンプレートタスクの詳細** 左側のパネルで、「詳細」セクションの領域に移動して、各領域の情報を編集します。
1. （オプション） **すべて折りたたむ** アイコン ![](assets/collapse-all-icon.png) をクリックします。
1. 「詳細」セクションの情報を編集するには、 **編集** アイコン ![](assets/edit-icon.png)をクリックし、下のいずれかの領域から選択するか、 **すべてを編集** すべての領域で情報を編集するには、次の手順に従います。

   * 概要
   * カスタムフォーム

      税関フォームの名前は、オブジェクトにカスタムフォームが添付されている場合にのみ表示されます。

   * 財務
   >[!TIP]
   >
   >[ 詳細 ] 領域に表示されるすべてのフィールドの詳細については、下の [ テンプレートの編集 ] タスクボックスを使用して、すべてのフィールドを編集し続けます。

1. （条件付き）テンプレートタスクに関するすべての情報を編集するには、 **詳細** メニュー ![](assets/qs-more-icon-on-an-object.png) テンプレートタスクの名前の横にある「 **編集**.

   この **テンプレートタスクの編集** ボックスが表示されます。

   >[!TIP]
   >
   >また、リスト内のテンプレートタスクを選択し、「編集」をクリックして、「テンプレートタスクの編集」ボックスを開くこともできます。

   ![](assets/edit-template-tasks-box-classic-350x356.png)

1. 次のセクションのいずれかで、情報の指定を検討します。

   * [概要](#overview)
   * [財務](#finance)
   * [設定](#settings)
   * [割り当て](#assignments)
   * [カスタムフォーム](#custom-forms)
   * [コメント](#comment)

### 概要 {#overview}

1. 前述のように、テンプレートタスクの編集を開始します。
1. クリック **概要**.

   ![edit_task_overview.png](assets/edit-task-overview-350x438.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名前</strong> </td> 
      <td>テンプレートタスクの名前を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td>テンプレートタスクに関する追加情報を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>テンプレートタスクに関する情報に関連する Web リンクを指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先度</strong> </td> 
      <td> <p>これは、テンプレートタスクを優先順位付けできる視覚的なフラグです。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>なし</strong> </p> </li> 
        <li> <p><strong>低</strong> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">標準</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">高</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">緊急</span> </p> </li> 
       </ul> <p>Workfront管理者が選択したプロジェクトの環境設定によっては、優先度の名前が異なる場合があります。 優先度の編集の詳細については、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">優先度の作成とカスタマイズ</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>期間タイプ</strong> </td> 
      <td> <p>このテンプレートから作成される将来のタスクの期間のタイプは、このようになります。 <br>期間タイプは、次の間の関係を識別します。</p> <p> — タスクに割り当てられたリソースの数</p> <p> — タスクの完了に必要な総作業量</p> <p> — タスクの総期間。 </p> <p>期間タイプを使用すると、タスクのニーズに基づいて一貫したリソースの割り当てを設定できます。 タスクの期間の種類について詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプの概要</a>.</p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">算出した割り当て</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">算出した作業</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">作業優先</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">シンプル</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>期間</strong> </td> 
      <td> <p>「今後のタスクの期間」を分、時間、日、週または月単位で指定します。 このテンプレートから作成される将来のタスクの期間は、ここで指定した期間になります。</p> <p>デフォルトで、Workfrontは期間を日数単位で測定します。 タスクを完了するまでに、タスクを未完了のままにしておく時間です。 タスクの期間は、 <strong>期間のタイプ</strong> のタスクが <strong>シンプル</strong>、または <strong>タスク制約</strong> が <strong>固定日付</strong>.</p> <p>重要：通常、期間は、テンプレートタスクの「計画開始日」から「計画完了日」までの時間です。このため、テンプレートのタイムラインに影響を与えます。 これにより、テンプレートから作成される今後のプロジェクトのタイムラインが決まります。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>予定時間数</strong> </td> 
      <td> <p>このテンプレートで作成されたプロジェクトの将来のタスクの予定時間数を指定します。 タスクの担当者がタスクを完了するのにかかる実際の時間です。 タスクの予定時間数は、<strong>期間のタイプ</strong> が <strong>計算された割り当て</strong>. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">作業量 </td> 
      <td> <p><span>タスクの完了に必要な労力の量。 プロジェクトマネージャは、タスクの完了に必要な作業量を見積もる際に、予定時間の代わりにこのフィールドを使用することにします。 このフィールドは、次の条件を満たした場合にのみ表示されます。</span> </p> 
       <ul> 
        <li> <p><span>テンプレートタスクには「シンプルな期間」タイプがあります。</span> </p> <p>ヒント： <span>タスクの期間の種類を更新すると、このフィールドは非表示になります。</span> </p> </li> 
        <li><span>プロジェクトマネージャーが、テンプレートの「作業時間を使用して計画時間を計算する」フィールドを有効にしています。</span> </li> 
       </ul> 
       <div> 
        <p> 次のオプションから選択します。</p> 
        <ul> 
         <li>小</li> 
         <li>中 <span style="font-weight: normal;">（これは新しいタスクのデフォルト値です）</span></li> 
         <li>大</li> 
        </ul> 
       </div> <p>計画時間ではなく作業量を使用して作業量を見積もる方法については、 <span href="work-effort.md"><a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a></span>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>タスクの制約</strong> </td> 
      <td> <p>このテンプレートから作成されたプロジェクトのタスクには、この制約が適用されます。 タスク制約は、タスクを完了する必要があるタイミングを識別します。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li><strong>固定日付</strong>. を指定します。 <strong>計画開始</strong> および <strong>計画完了日。</strong></li> 
        <li><strong>指定日に開始</strong>. を指定します。 <strong>計画開始日。</strong></li> 
        <li><strong>指定日に終了</strong>. を指定します。 <strong>計画完了日</strong>.</li> 
        <li><strong>できるだけ早く</strong> </li> 
        <li><strong>できるだけ遅く</strong> </li> 
        <li style="font-weight: bold;"><strong>最も早い空き時間</strong> </li> 
        <li style="font-weight: bold;"><strong>最も遅い空き時間</strong> </li> 
        <li>指定日までに開始. を指定します。 <strong>計画開始日</strong>.</li> 
        <li><strong>指定日以後に開始</strong>. を指定します。 <strong>計画開始日</strong>.</li> 
        <li><strong>これよりも遅く終了しない</strong>. を指定します。 <strong>計画完了日</strong>.</li> 
        <li><strong>これよりも早く終了しない</strong>. を指定します。 <strong>計画完了日</strong>.</li> 
       </ul> <p>タスク制約の詳細については、 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">開始日</span><span style="font-weight: normal;">（オプションおよび条件付き）</span> </td> 
      <td> <p> テンプレートタスクの開始日は、タスク制約が次のいずれかの場合にのみ指定できます。</p> 
       <ul> 
        <li>指定日に開始</li> 
        <li>次の日までに開始</li> 
        <li>指定日までに開始</li> 
        <li>固定日付</li> 
       </ul> <p>これは、タスクが開始される将来のプロジェクトのタイムライン内の日付に対応します。 その他のすべての制約について、Workfrontはタスク間の先行タスクの依存関係に基づいて開始日を計算します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完了日</strong><span style="font-weight: normal;"> （オプションおよび条件付き）</span> </td> 
      <td> <p> テンプレートタスクの完了日は、タスク制約が次のいずれかの場合にのみ指定できます。</p> 
       <ul style="list-style-type: circle;"> 
        <li>指定日に終了</li> 
        <li>次よりも前に完了</li> 
        <li>これよりも遅く終了しない</li> 
        <li>固定日付</li> 
       </ul> <p>これは、タスクが完了する将来のプロジェクトのタイムライン内の日付に対応します。 その他のすべての制約について、Workfrontは、期間と先行者の依存関係に基づいて完了日を計算します。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   クリック **変更を保存**.

### 財務 {#finance}

1. 上記の説明に従ってタスクの編集を開始します。
1. クリック **金融**.

   ![edit_task_finance.png](assets/edit-task-finance-350x216.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>コストの種類</strong> </td> 
      <td> <p>将来のタスクのコストタイプを指定します。 これにより、タスクの時間数に基づいて、タスクのコストの計算方法が決まります。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>コストなし</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>固定 (毎時)</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>ユーザー (毎時)</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>役割 (毎時)</span> </p> </li> 
       </ul> <p>コストの追跡について詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>収益タイプ</strong> </td> 
      <td> <p>将来のタスクの収益タイプを指定します。 これにより、タスクの時間数に基づいて、タスクの売上高の計算方法が決まります。</p> <p style="font-weight: normal;">次のオプションから選択します。 </p> 
       <ul> 
        <li> <p style="font-weight: normal;">請求不可</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー (毎時)</p> </li> 
        <li> <p style="font-weight: normal;">役割 (毎時)</p> </li> 
        <li> <p style="font-weight: normal;">固定 (毎時)</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー (毎時) (上限付き)</p> </li> 
        <li> <p style="font-weight: normal;">役割 (毎時) (上限付き)</p> </li> 
        <li> <p style="font-weight: normal;">ユーザー (毎時) + 固定</p> </li> 
        <li> <p style="font-weight: normal;">役割 (毎時) + 固定</p> </li> 
        <li> <p style="font-weight: normal;">固定収益</p> </li> 
       </ul> <p>売上高の追跡について詳しくは、 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と売上高の概要</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   クリック **変更を保存**.

### 設定 {#settings}

1. 上記の説明に従ってタスクの編集を開始します。
1. クリック **設定**.

   ![](assets/edit-template-tasks-settings-classic-350x231.png)

1. 次のいずれかを更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>追跡モード</strong> </td> 
      <td> <p>今後のタスクの進捗状況の追跡方法を指定します。 </p> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>ユーザーが更新する必要あり</strong> </p> </li> 
        <li> <p><strong>予定通り</strong> </p> </li> 
        <li> <p><strong>遅延警告を無視</strong> </p> </li> 
        <li> <p><strong>自動完了</strong> </p> </li> 
        <li> <p><strong>先行タスク</strong> </p> </li> 
       </ul> <p>タスクのトラッキングモードについて詳しくは、 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">タスクトラッキングモードの概要</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>承認プロセス</strong> </td> 
      <td> <p>テンプレートタスクに関連付ける承認プロセスを選択します。 Workfront管理者は、テンプレートタスクに関連付ける前に、システムレベルのタスク承認プロセスを定義する必要があります。 <span>承認プロセスへの管理者アクセス権を持つユーザーは、グループ固有の承認プロセスを作成することもできます。</span> 承認プロセスの作成について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業項目の承認プロセスの作成</a>.</p> <p>承認プロセスを追加する際は、次の点を考慮してください。 </p> 
       <ul> 
       <li>アクティブな承認プロセスのみがリストに表示されます。 </li> 
       <li> <p>システム全体およびグループ固有の承認プロセスがリストに表示されます。 テンプレートの承認プロセス以外のグループに関連付けられている承認プロセスは、リストに表示されません。</p> <p>重要：テンプレートに関連付けられているグループが変更されると、グループ固有の承認プロセスが単一使用の承認プロセスになります。 プロジェクトのグループに対する変更や承認プロセスの変更が承認設定に及ぼす影響について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループと承認プロセスの変更が、割り当てられた承認プロセスに及ぼす影響</a>. </p> </li> 
       <li> <p>単一使用の承認プロセスを追加した場合は、「&lt;custom&gt;」と入力します。 詳しくは、 <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">新規または既存の承認プロセスと作業の関連付け</a>. </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>--> </li> 
       <li> <p>テンプレートタスクを一括編集する場合は、次のシナリオが存在します。</p> 
       <ul> 
       <li> <p>同じテンプレートグループからテンプレートタスクを選択すると、システムレベルとグループレベルの両方の承認プロセスがこのフィールドに表示されます。</p> </li> 
       <li> <p>別のテンプレートグループからテンプレートタスクを選択すると、このフィールドにはシステムレベルの承認プロセスのみが表示されます。</p> </li> 
       <li> <p>テンプレートタスクに 1 回限りの承認プロセスが添付されている場合、そのプロセスはシステムレベルで置き換えられます <span>またはグループレベルの承認プロセス</span> を選択します。 </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>リマインダー通知</strong> </td> 
      <td> <p>テンプレートタスクに添付するリマインダー通知を選択します。 このテンプレートから作成されたプロジェクトの今後のタスクに添付されます。 タスクでリマインダー通知を選択するには、システム管理者がリマインダー通知を設定する必要があります。 リマインダー通知の設定の詳細については、 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">リマインダー通知の設定</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   クリック **変更を保存**.

### 割り当て {#assignments}

1. 上記の説明に従ってタスクの編集を開始します。
1. クリック **割り当て**.

   ![assignments_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. クリック **担当者を追加** 新しい担当者をテンプレートタスクに追加します。 ユーザー、役割またはチームをタスクに割り当てることができます。 1 つのタスクに複数の担当者を割り当てることができます。 今後のタスクには、このテンプレートタスクから作成された場合と同じリソースが割り当てられます。
1. （オプション）複数の担当者がいる場合は、 **所有者** タスク所有者またはタスク担当者と見なされるユーザーまたは役割を示すラジオプライマリボタン。 Workfrontは、テンプレートタスクに割り当てた最初のユーザーまたはジョブの役割を、所有者またはプライマリの担当者としてマークします。
1. （条件付きおよびオプション）タスク制約が計算作業量または労力主導型の場合は、 **配分%** （割り当て率）を割り当てます。 担当者がこのタスクに費やすことができる、担当者のスケジュールからの時間です。 担当者の割り当て率を変更すると、タスクの予定時間が変更されます。
1. （条件付きおよびオプション）タスク制約が「単純」の場合は、 **時間** 各担当者の

   または

   合計数を指定 **予定時間** テンプレートタスク用。 これにより、すべての担当者間で合計時間が均等に配分されます。

1. （条件付きおよびオプション）タスク制約が「単純」の場合は、 **期間** 日単位のテンプレートタスクです。 これは、このテンプレートから作成されるタスクの期間になります。
1. （オプション） **担当者の役割** ドロップダウンメニュー。 これは、担当者がこの将来のタスクで実行できる役割です。 プロファイル内の各担当者に関連付けられているジョブの役割のみがドロップダウンメニューに表示されます。
1. （オプション）変更する情報に応じて、以降のセクションを引き続き編集します。

   または

   クリック **変更を保存**.

### カスタムフォーム {#custom-forms}

タスクをプロジェクトに追加する際にタスクに自動的に添付されるデフォルトのカスタムフォームを定義できます。 デフォルトのタスクカスタムフォームを含むようにプロジェクトを設定する方法については、この記事の「タスク」の節を参照してください [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 上記の説明に従ってタスクの編集を開始します。 テスト
1. クリック **カスタムForms**.

   ![custom_forms_edit_task.png](assets/custom-forms-edit-task-350x136.png)

1. テンプレートタスクに関連付ける 1 つ以上のカスタムフォームを選択します。 カスタムフォームをこのフィールドで選択できるようにするには、事前にカスタムフォームを作成する必要があります。 リストには、アクティブなカスタムフォームのみが表示されます。 カスタムフォームの作成について詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)テンプレートタスクには、最大 10 個のカスタムフォームを追加できます。 フォームは、テンプレートから作成されたタスクに自動的に追加されます。
1. （条件付きおよびオプション）カスタムフォームをテンプレートタスクに添付する場合、フォーム上の任意のフィールドを編集します。 テンプレートタスクを保存する前に、すべての必須フィールドを指定する必要があります。

   >[!NOTE]
   >
   >Workfront管理者がカスタムフォームのセクションに対して権限を設定した方法に応じて、すべてのユーザーが特定のカスタムフォームの同じフィールドを表示または編集できるわけではありません。 カスタムフォームのセクション内のフィールドを編集する権限は、テンプレートタスクに対する権限と今後のタスクに応じて異なります。\
   >カスタムフォームのセクションに対する権限の設定について詳しくは、 [カスタムフォームの共有](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).\
   >タスク権限の設定については、 [タスクの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).\
   >テンプレート権限の設定について詳しくは、 [テンプレートの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. （オプション）変更する情報に応じて、次のセクションを引き続き編集します。

   または

   クリック **変更を保存**.

### コメント {#comment}

1. 上記の説明に従ってタスクの編集を開始します。
1. クリック **コメント**.

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. テンプレートタスクの更新ストリームに表示するコメントを、「使用可能」フィールドで指定します。 このコメントは、テンプレートとテンプレートタスクに対する表示アクセス権を持ち、メモの表示アクセス権を持つすべてのユーザーに対して表示されます。
1. クリック **変更を保存**.

   変更は、このテンプレートタスクに対して送信されます。

   このテンプレートからプロジェクトを作成する場合、テンプレートタスクに適用したすべての設定が、プロジェクトタスクの設定になります。
