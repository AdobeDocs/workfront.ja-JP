---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトタイムラインを再計算
description: タイムラインの再計算を使用すると、管理者は、プロジェクトに関連する様々な要因がプロジェクトのタイムラインに与える影響を確認できます。 プロジェクトのタイムラインは、計画日と予定日を指します。
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# プロジェクトタイムラインを再計算

タイムラインの再計算を使用すると、管理者は、プロジェクトに関連する様々な要因がプロジェクトのタイムラインに与える影響を確認できます。 プロジェクトのタイムラインは、計画日と予定日を指します。

スケジュール、人事のタイムオフ、およびプロジェクトの範囲外の他の項目に変更を加えても、プロジェクトのタイムラインに直ちには影響しません。 タイムラインを再計算すると、プロジェクトタイムラインに影響が出ます。 再計算が行われるまで、外部インフルエンスはプロジェクトに影響を与えません。

この記事では、タイムラインの再計算が発生する方法について説明します。

## アクセス要件

<!--drafted for P&P: 

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
タイムラインの自動再計算は、プロジェクトの作業に関わるユーザーに対して特別なアクセス権を付与することなくおこなわれます。

ただし、プロジェクトのタイムラインを手動で再計算するには、次のアクセス権が必要です。

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
   <td> <p>プロジェクトへのアクセスを編集</p> <p>システム管理者：システム内のすべてのプロジェクトのタイムラインを再計算する場合</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 自動再計算

デフォルトでは、プロジェクトの範囲が変更されたとき、または毎晩、プロジェクトのタイムラインは自動的に毎日再計算されます。 Workfrontの管理者は、設定の「プロジェクトプリファレンス」領域の「タイムライン」設定を管理することで、毎晩、またはスコープの変更ごとに、タイムラインを自動的に計算するかどうかを決定します。 詳しくは、 [プロジェクトのタイムライン再計算の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

>[!NOTE]
>
>プロジェクトのタイムラインが 15 年を超える場合、そのプロジェクトの自動再計算は無効になります。 15 年を超えるプロジェクトに対して選択できるのは、「更新タイプ」の「手動」のみです。 プロジェクト上の日付を 15 年未満に変更した場合は、タイムラインを自動的に計算する前に 1 回手動で再計算する必要があります。

* [プロジェクトタイムラインの自動再計算](#automatic-recalculation-of-project-timelines)
* [プロジェクトタイムラインの自動再計算をトリガーするアクション](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)

### プロジェクトタイムラインの自動再計算 {#automatic-recalculation-of-project-timelines}

Adobe Workfrontでは、次の条件がすべて満たされたプロジェクトのタイムラインが毎日再計算されます。

* ステータスが「現在」
* プロジェクトの更新タイプが [ 自動 ] または [ 自動 ] に設定され、[ 変更時 ] に設定されている

   プロジェクトの更新タイプの詳細については、 [プロジェクト更新タイプの概要](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

* 過去 3 ヶ月以内の最終更新日がある\
   Workfront管理者は、 [プロジェクトのタイムライン再計算の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

* プロジェクトタイムラインの最終計算日が現在のカレンダー日内にありません。 つまり、プロジェクトタイムラインの最終計算日が現在の日の 00:00 より前になっています。

プロジェクトのタイムラインを更新する頻度を設定できます。 プロジェクトタイムラインを更新すると、プロジェクトに加えた変更に基づいて再計算されます。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

詳しくは、 [プロジェクトの更新タイプを選択](../../../manage-work/projects/manage-projects/select-project-update-type.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click&nbsp; <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
<li value="3"> <p>Click<strong>Settings.</strong><br><img src="assets/screen-shot-2013-09-18-at-10.36.16-am-350x347.png" alt="" style="width: 350;height: 347;"></p> </li>
<li value="4">In the <strong>Update Type</strong> drop-down list, select from the following options:<br><strong>- Automatic and On Change:</strong> (Default setting) The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night. <br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.
<div>
<p><img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"></p>
</div><br>This indicates that the recalculation is not yet finished, and the dates are subject to change. <br><strong>- Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.<br>You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br><strong>- Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on.<br><note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note><br><strong>- Manual Only:</strong> The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="#manual-recalculation" class="MCXref xref">Manual recalculation</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).<br>For more information about the project Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a><note type="note">
If the timeline of a project is longer than 15 years, the automatic recalculation is disabled. If you change the dates on the project to less than 15 years, you must manually recalculate your timeline one time before it is calculated automatically.
</note></li>
<li value="5">Click <strong>Save Changes.</strong></li>
</ol>
</div>
-->

### プロジェクトタイムラインの自動再計算をトリガーするアクション {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

プロジェクトのライフサイクルの様々な範囲の変更により、以下の操作を含め、プロジェクトのタイムラインが自動的に再計算されます。

* タスクのステータスを更新しています。
* タスクを別のプロジェクトに移動する。
* タスクの計画日または計画完了日を更新します。
* 期間の種類、タスクの制約、またはタスクの担当者数を更新する。
* タスクの先行関係を更新しています。
* タスクに承認を追加して、タスクの計画完了日にも時間を追加します。\
   承認設定について詳しくは、 [グローバル承認設定の指定](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

## 手動で再計算 {#manual-recalculation}

プロジェクト所有者は、個々のプロジェクトのタイムラインを手動で再計算できます。 Workfrontの管理者は、Workfrontのすべてのタイムラインを手動で再計算できます。

* [個々のプロジェクトのタイムラインを再計算するか、一括して再計算します](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [「プロジェクトを編集」ボックスでタイムラインを手動で一括再計算する](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [システム内のすべてのプロジェクトのタイムラインを再計算する (Workfront管理者のみ )](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### 個々のプロジェクトのタイムラインを再計算するか、一括して再計算します {#recalculate-timelines-for-individual-projects-or-in-bulk}

プロジェクトのタイムラインは、プロジェクトページ、またはプロジェクトリストやレポートから、Workfrontで再計算できます。

1. タイムラインを再計算するプロジェクトに移動し、 **詳細** アイコン ![](assets/qs-more-menu.png) プロジェクト名の左

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   または

   プロジェクトリストまたはレポートに移動して、1 つまたは複数のプロジェクトを選択し、 **詳細** アイコン ![](assets/qs-more-menu.png) をクリックします。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >プロジェクトの複雑さに応じて、最適なパフォーマンスを確保するためにタイムラインを一括で再計算する場合は、多数のプロジェクトを選択しないことをお勧めします。 プロジェクトが複雑すぎる可能性があるものには、複数の依存関係や割り当て、または多数のカスタムフィールドがあるものがあります。

1. クリック **タイムラインを再計算**.

   タイムラインが再計算されると、再計算が成功したことを示すメッセージが表示されます。

   >[!TIP]
   >
   >タイムラインの再計算が完了する前は、計画済みまたは推定日付の一部が淡色表示になる場合があります。 つまり、再計算はまだ完了しておらず、日付が変更される場合があります。

### 「プロジェクトを編集」ボックスでタイムラインを手動で一括再計算する {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

複数のプロジェクトのタイムラインを一括編集することで、手動で再計算することができます。

>[!TIP]
>
>プロジェクトの複雑さに応じて、最適なパフォーマンスを確保するために、大量のプロジェクトを一括編集する際には選択しないことをお勧めします。 プロジェクトが複雑すぎる可能性があるものには、複数の依存関係や割り当て、または多数のカスタムフィールドがあるものがあります。

1. プロジェクトのリストに移動します。
1. リスト内の複数のプロジェクトを選択し、「 **編集**.
1. クリック **設定**&#x200B;を選択し、「 **タイムラインを再計算**.

1. クリック **変更を保存**.

### システム内のすべてのプロジェクトのタイムラインを再計算する (Workfront管理者のみ ) {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfrontの管理者は、「タイムラインを再計算」の診断を実行して、Workfrontシステム内のすべてのタイムラインを直ちに再計算できます。 これにより、すべてのプロジェクトマネージャは、計画日と予定日の両方に対する外部の変更の影響を即座に確認できます。

Workfrontサイト全体のタイムラインの再計算の詳細については、「 Workfrontインスタンス全体のタイムラインを再計算する」の節を参照してください。 [プロジェクトのタイムライン再計算の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Project Update Types</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to thisa rticle: /Content/Manage work/Projects/Planning a Project/project-update-type-overview.htm)</p>
<p>For information about how to update the project's Update Type, see <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>. </p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<p>You can select how each project calculates its timeline by choosing between the following Update Types:</p> <note type="important">
If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.
</note>
<ul>
<li> <p><strong>Automatic and On Change:</strong>&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp; <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong>&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong>&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong>&nbsp;The project timeline is updated only&nbsp;when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in&nbsp;the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
