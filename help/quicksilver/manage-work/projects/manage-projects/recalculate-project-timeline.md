---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトタイムラインの再計算
description: タイムラインの再計算を使用すると、管理者は、プロジェクトに関連する様々な要因がプロジェクトのタイムラインに与える影響を確認できます。プロジェクトのタイムラインは、予定日と見込み日を指します。
author: Alina
feature: Work Management
exl-id: ec5d9a07-e45a-4aa2-9f41-9421ca5d5920
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 58%

---

# プロジェクトタイムラインの再計算

<!--Audited: 06/2025-->

タイムラインの再計算を使用すると、管理者は、プロジェクトに関連する様々な要因がプロジェクトのタイムラインに与える影響を確認できます。プロジェクトのタイムラインは、予定日と見込み日を指します。

プロジェクトの範囲外でスケジュールや人員の休暇、その他の項目に変更を加えても、プロジェクトのタイムラインに直ちには影響しません。タイムラインを再計算すると、プロジェクトタイムラインに影響が出ます。再計算が行われるまで、外部の影響はプロジェクトに作用しません。

この記事では、タイムラインの再計算がどのように発生するかについて説明します。

プロジェクトの作業に関与するユーザーが特別なアクセス権を持っていなくても、タイムラインの自動再計算が行われます。 また、タイムラインを手動で再計算することもできます。

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
    <p>プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p>システム内のすべてのプロジェクトのタイムラインを再計算するシステム管理者</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対して権限を管理</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard </p> 
    <p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> <p>System administrator to recalculate timeline for all projects in the system</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 自動再計算

デフォルトでは、プロジェクトの範囲が変更された時、または毎晩、プロジェクトのタイムラインは自動的に毎日再計算されます。Workfront管理者は、「設定」の「プロジェクト環境設定」領域でタイムライン設定を管理して、毎晩またはスコープの変更ごとにタイムラインを自動計算するかどうかを決定します。 詳しくは、[プロジェクトのタイムライン再計算の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)を参照してください。

>[!IMPORTANT]
>
>* プロジェクトのタイムラインが 15 年を超える場合、そのプロジェクトの自動再計算は無効になり、手動更新タイプのみ選択できます。 プロジェクト上の日付を 15 年未満に変更した場合は、タイムラインを自動的に計算する前に 1 回手動で再計算する必要があります。
>* プレビューおよびカスタム更新サンドボックス環境の場合、夜間の再計算は無効になり、プロジェクトのタイムラインは自動的に再計算されません。 プレビューおよびカスタム更新サンドボックス環境のプロジェクトタイムラインを手動で再計算する必要があります。
>* プロジェクトが複雑な場合、タイムラインの自動再計算が行われない場合があります。
> 複雑なプロジェクトの例としては、複数の依存関係、多数のタスク、複数のプロジェクト間先行タスク、複数のタスクのインデントを含むプロジェクトなどがあります。
> Workfrontでは、プロジェクトページのプロジェクト名の右側に、プロジェクトタイムラインを手動で再計算する必要があることを示す警告を表示します。 プロジェクトの管理権限を持つユーザーのみが、タイムラインを手動で再計算できます。
>
>   ![](assets/project-warning-to-manually-recalculate-timeline.png)
>

* [プロジェクトタイムラインの自動再計算](#automatic-recalculation-of-project-timelines)
* [プロジェクトタイムラインの自動再計算を引き起こすアクション](#actions-that-trigger-an-automatic-recalculation-of-project-timelines)



### プロジェクトタイムラインの自動再計算 {#automatic-recalculation-of-project-timelines}

Workfrontでは、次のすべての条件を満たすプロジェクトのタイムラインが毎日再計算されます。

* 現在のステータスがある。
* プロジェクトの更新の種類が [ 自動 ] または [ 自動および変更時 ] に設定されています。

  詳しくは、[ プロジェクト更新タイプの概要 ](../../../manage-work/projects/planning-a-project/project-update-type-overview.md) を参照してください。

* 過去 3 か月以内の最終更新日がある。 Workfront管理者は、このデフォルトの機能を変更できます。 詳しくは、[プロジェクトのタイムライン再計算の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)を参照してください。

* プロジェクト タイムラインの最終計算日が、現在のカレンダーの日付の範囲内にありません。 つまり、プロジェクトタイムラインの最終計算日が、現在の日付の 00:00 より前になります。

プロジェクトのタイムラインを更新する頻度を設定できます。プロジェクトのタイムラインが更新されると、プロジェクトに加えられた変更に基づいて再計算されます。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or changes made to another project that the timeline is dependent on
</MadCap:conditionalText>
-->


<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: above, the last part is drafted because of this: I don't think this is right because we told people that in the case of cross-project predecessors, the timeline must be calculated manually for the successor to see the updates in the predecessor's project. Drafting for now.)</p>
-->

詳しくは、[プロジェクトの更新タイプを選択](../../../manage-work/projects/manage-projects/select-project-update-type.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: content moved to the article linked above)</p>
<p>You can configure how the timeline for your project is updated:</p>
<ol>
<li value="1">Go to the project for which you want to configure how the timeline is updated.</li>
<li value="2"> <p>  Click the <strong>More</strong> icon <img src="assets/more-icon.png"> to the right of the project name, then click  <strong>Edit</strong>. </p> <p>The <strong>Edit Project</strong> dialog box is displayed.</p> </li>
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

### プロジェクトタイムラインの自動再計算を引き起こすアクション {#actions-that-trigger-an-automatic-recalculation-of-project-timelines}

プロジェクトの存続期間中の様々な範囲の変更により、以下のアクションを含めて、プロジェクトのタイムラインが自動的に再計算されます。

* タスクのステータスの更新。
* タスクを別のプロジェクトに移動。
* タスクの予定日または予定完了日の更新。
* 期間タイプ、タスクの制約、またはタスクの担当者数の更新。
* 先行タスクの関係の更新。
* タスクへの承認の追加によって、タスクの予定完了日にも時間を追加。\
  承認設定について詳しくは、[グローバル承認設定の指定](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)を参照してください。

## 手動再計算 {#manual-recalculation}

プロジェクト所有者は、個々のプロジェクトのタイムラインを手動で再計算できます。Workfront の管理者は、Workfront のすべてのタイムラインを手動で再計算できます。

* [個々のプロジェクトのタイムラインを再計算するか、一括して再計算](#recalculate-timelines-for-individual-projects-or-in-bulk)
* [「プロジェクトを編集」ボックスでタイムラインを手動で一括再計算](#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box)
* [システム内のすべてのプロジェクトのタイムラインを再計算（Workfront 管理者のみ）](#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only)

### 個々のプロジェクトのタイムラインを再計算するか、一括して再計算 {#recalculate-timelines-for-individual-projects-or-in-bulk}

プロジェクトのタイムラインは、プロジェクトページ、またはプロジェクトリストやレポートから、Workfront で再計算できます。

1. タイムラインを再計算するプロジェクトに移動して、プロジェクト名の左側にある **その他** アイコン ![ その他メニュー ](assets/qs-more-menu.png) をクリックします。

   または

   プロジェクトリストまたはレポートに移動して、1 つまたは複数のプロジェクトを選択し、リストの上部にある **その他** アイコン ![ その他メニュー ](assets/qs-more-menu.png) をクリックします。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >プロジェクトの複雑さによっては、最適なパフォーマンスを確保するためにタイムラインを一括で再計算する際に、多数のプロジェクトを選択しないことをお勧めします。 プロジェクトが複雑になりすぎる原因として、複数の依存関係や割り当て、大量のカスタムフィールドなどが挙げられます。

1. **タイムラインを再計算** をクリックします。 タイムラインが再計算され、成功メッセージが画面に表示されます。

   >[!TIP]
   >
   >タイムラインの再計算が完了する前は、予定日または見込み日の一部が淡色表示になる場合があります。これは、再計算がまだ終わっておらず、日程が変更される可能性があることを意味します。

### 「プロジェクトを編集」ボックスでタイムラインを手動で一括再計算 {#manually-recalculate-timelines-in-bulk-in-the-edit-projects-box}

複数のプロジェクトのタイムラインを一括編集することで、手動で再計算することができます。

>[!TIP]
>
>プロジェクトの複雑さによっては、最適なパフォーマンスを確保するために、大量に編集する際に多数のプロジェクトを選択しないことをお勧めします。 プロジェクトが複雑になりすぎる原因として、複数の依存関係や割り当て、大量のカスタムフィールドなどが挙げられます。

1. プロジェクトのリストに移動します。
1. リスト内の複数のプロジェクトを選択し、「**編集**」をクリックします。
1. 「**設定**」をクリックし、「**タイムラインを再計算**」を選択します。

1. 「**変更を保存**」をクリックします。

### システム内のすべてのプロジェクトのタイムラインを再計算（Workfront 管理者のみ） {#recalculate-timelines-for-all-projects-in-the-system-workfront-administrators-only}

Workfront の管理者は、「タイムラインを再計算」の診断を実行して、Workfront システム内のすべてのタイムラインを直ちに再計算できます。これにより、すべてのプロジェクトマネージャーは、予定日と見込み日の両方に対する外部の変更の影響を即座に確認できます。

Workfront サイト全体のタイムラインの再計算の詳細については、「プロジェクトのタイムライン再計算の設定 [ のWorkfront インスタンス全体のタイムラインの再計算の節を参照してください ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)

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
<li> <p><strong>Automatic and On Change:</strong> This is the default setting. The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.  <br>This is the recommended setting as it ensures that the project timeline is always up to date.</p> <p>When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed. </p> <p> <img src="assets/dates-dimmed-when-insline-editing-350x146.png" style="width: 350;height: 146;"> </p> <p>This indicates that the recalculation is not yet finished, and the dates are subject to change. </p> </li>
<li><strong>Change Only:</strong> The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur. <br>You might want to select this option if you are concerned about system performance and if changes rarely occur in the project or in other projects that the timeline is dependent on.</li>
<li> <p><strong>Automatic Only:</strong> The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.</p> <note type="note">
A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.
</note> </li>
<li><strong>Manual Only:</strong> The project timeline is updated only when you select the option to <strong>Recalculate Timelines</strong>, as described in the section "Manual Recalculation" in the article <a href="#" class="MCXref xref selected">Recalculate project timelines</a>.<br>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</li>
</ul>
</div>
-->
