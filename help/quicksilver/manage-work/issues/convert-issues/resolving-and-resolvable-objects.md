---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: 解決オブジェクトと解決可能オブジェクトの概要
description: 解決可能オブジェクトとは、解決策が解決オブジェクトに結び付けられているイシューです。解決オブジェクトは、プロジェクト、タスクまたは別のイシューです。
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '1761'
ht-degree: 49%

---

# 解決オブジェクトと解決可能オブジェクトの概要

<!-- Audited: 5/2025 -->

解決可能オブジェクトとは、解決策が解決オブジェクトに結び付けられているイシューです。解決オブジェクトは、プロジェクト、タスクまたは別のイシューです。

イシューをタスクまたはプロジェクトに変換すると、そのイシューはタスクまたはプロジェクトの解決可能オブジェクトになります。

イシューを解決オブジェクト（タスク、プロジェクトまたはイシュー）に手動でリンクすることもできます。詳しくは、[イシューの解決策を他のイシュー、タスクまたはプロジェクトに手動で結び付ける](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md)を参照してください。

このシナリオでは、元のイシューがタスク、プロジェクト、イシューの解決可能オブジェクトになります。

## 解決可能オブジェクトを処理するために Adobe Workfront を設定 {#set-up-adobe-workfront-to-handle-resolvable-objects}

Workfront の管理者またはグループ管理者は、システム内またはグループ内の解決可能オブジェクトの処理方法を決定できます。

解決可能オブジェクトをタスクまたはプロジェクトに変換するときにそのオブジェクトを保持するか、タスクまたはプロジェクトを作成したら削除するかを選択できます。 イシューの変換中にこれらの設定を変更できるように選択すると、イシューを変換するユーザーが、変換中にイシューを保持するか削除するかを選択できるようになります。

>[!NOTE]
>
>解決可能オブジェクトとは常に、その解決策とステータスが、関連付けられた解決オブジェクトの解決策とステータスに依存する可能性があるイシューです。解決オブジェクトとは、イシュー、タスクまたはプロジェクトです。

解決可能オブジェクトを処理するための環境設定の指定について詳しくは、[システム全体のタスクとイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: drafted and just pointed the user to the article linked above)&nbsp;</p>
<p>To establish the system default for what happens to the issue as it is being converted to a task or a project:</p>
<ol>
<li value="1">Log in to Workfront as a Workfront administrator <span>or group administrator.</span></li>
<li value="2"> <p>  From the main menu, click <strong>Setup</strong>. </p> <p> <img src="assets/qs-main-menu-expanded-with-menu-highlight-350x521.png" style="width: 350;height: 521;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Expand <strong>Project Preferences</strong>.</li>
<li value="4">Click <strong>Tasks & Issues</strong>.</li>
<li value="5">Go to the <strong>Issues</strong> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings:
<ul>
<li><p><strong>Automatically update Resolvable Issue status when the status of the Resolving Object changes:</strong> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <strong>Keep the original issue and tie its resolution to the task</strong> or<strong>project</strong> must be selected.</p>
<ul>
<li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
<li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
</note></li>
</ul></li>
<li><strong>When converting an issue to a TASK...:</strong> The settings in this section determine what happens during the conversion process from issue to task:
<ul>
<li><strong>Keep the original issue and tie its resolution to the task:</strong> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
<li><strong>Allow Primary Contact to have access to the task:</strong> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
</ul></li>
<li><strong>When converting an issue to a PROJECT...:</strong> The settings in this section determine what happens during the conversion process from issue to project:
<ul>
<li><strong>Keep the original issue and tie its resolution to the project:</strong> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
<li><strong>Allow Primary Contact to have access to the project:</strong> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
</ul></li>
</ul></li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## プロジェクトまたはタスクへの変換時の解決可能オブジェクトの処理

Workfront 管理者またはグループ管理者がシステムレベルまたはグループレベルのイシューの環境をどのように設定したかに応じて、イシューをプロジェクトまたはタスクに変換する際に、解決可能オブジェクトに処理できる可能性があります。

次のシナリオが存在します。

* Workfrontまたはグループの管理者が、元の問題を保持してその解決をタスクに、元の問題を保持してその解決を選択したプロジェクトに結び付け、「変換中にこれらの設定を変更できるようにする」を選択していない場合、イシューをタスクまたはプロジェクトに変換する際には、これらの設定を変更できません。\
  ![ プロジェクト環境設定のイシュー領域 ](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* Workfrontまたはグループの管理者が、元のイシューを保持してその解決をタスクに結び付け、元のイシューを保持してその解決を選択または未選択のプロジェクトに結び付け、「変換中にこれらの設定を変更できるようにする」を選択した場合、イシューをタスクまたはプロジェクトに変換する際にこれらの設定を変更できます。\
  ![ イシューを保持するオプション ](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

イシューのタスクやプロジェクトへの変換について詳しくは、[Adobe Workfront でのイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Tie the resolution of an issue to a project, task or </h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: created new article for this section; draft when the article is live and see if you need to make a link from this one to the new article) </p>
<div>
<p>You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue. <br>For more information about how the status of the Resolving Object affects the Resolvable Object, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p>
<p>You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this. </p>
<p>To tie the resolution of an issue to the resolution of a project, task, or issue:</p>
<ol>
<li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li>
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p>  </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li>
<li value="4">At the bottom of the form,  click in the <strong>Resolved By</strong> field,  and select from the following types of resolving objects:
<ul>
<li><strong>Project</strong></li>
<li><strong>Task</strong></li>
<li><p><strong>Issue</strong></p></li>
</ul><p>The field for the resolving object displays. </p></li>
<li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li>
<li value="6">Click <strong>Save</strong>&nbsp;<strong>Changes</strong>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
One project, task, or issue may have multiple issues as Resolvable Objects.
</note></li>
</ol>
</div>
</div>
-->

## 解決可能オブジェクトのステータスと解決オブジェクトのステータスを同期 {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* [解決オブジェクトがイシューの場合にステータスを同期](#synchronize-statuses-when-the-resolving-object-is-an-issue)
* [解決オブジェクトがタスクまたはプロジェクトの場合にステータスを同期](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### 解決オブジェクトがイシューの場合にステータスを同期 {#synchronize-statuses-when-the-resolving-object-is-an-issue}

イシューが別のイシューに手動で関連付けられている場合、2 番目のイシューのステータス（オブジェクトの解決）には、最初のイシューのステータス（解決可能なオブジェクト）の変化がトリガーされます。 1 つ目のイシューのステータスは、2 つ目のイシューの変更後のステータスと一致します。これは、デフォルトのイシューステータスとカスタムのイシューステータスの両方に当てはまります。

### 解決オブジェクトがタスクまたはプロジェクトの場合にステータスを同期 {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

イシューがタスクまたはプロジェクトの解決可能オブジェクトである場合、タスクおよびプロジェクトのステータスの変更は、イシューのステータスの変更をトリガーします。この場合、デフォルトステータスはカスタムステータスとは異なる方法でトリガーされます。

プロジェクトのカスタムステータスが、イシューステータスへの変更をトリガーしないデフォルトのステータスと等しい場合、プロジェクトステータスの変更は、イシューのステータスの変更をトリガーしません。

* [解決オブジェクトのデフォルトステータスと解決可能オブジェクトのデフォルトステータスを同期](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [解決オブジェクトのカスタムステータスと解決可能オブジェクトのカスタムステータスを同期](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### 解決オブジェクトのデフォルトステータスと解決可能オブジェクトのデフォルトステータスを同期 {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

「解決オブジェクトのステータスが変更されたとき、解決可能なイシューのステータスを自動的に更新」オプションが選択されているかどうかに関係なく、解決オブジェクト （プロジェクトまたはタスク）でデフォルトのステータスが変更されるたびに、解決可能オブジェクト （イシュー）のステータスが適切に変更されます。 このような変更をトリガーするために、デフォルトステータスのみがすでにマッピングされています。

次のデフォルトのタスクステータスは、イシューがタスクの解決オブジェクトとして設定されている場合のデフォルトのイシューステータスを次のようにトリガーします。

| **タスクステータス** | **イシューステータス** |
|---|---|
| 新規 | 新規 |
| 処理中 | 処理中 |
| 完了 | クローズ |

次のデフォルトのプロジェクトステータスは、イシューがプロジェクトの解決可能オブジェクトとして設定されている場合のデフォルトのイシューステータスを次のようにトリガーします。 一部のプロジェクトステータスでは、イシューステータスに対する変更がトリガーされません。 イシューは、プロジェクトが次のいずれかのステータスに変化する前のステータスを保持します。

| **プロジェクトステータス** | **イシューステータス** |
|---|---|
| プラン | 新規 |
| 現在 | 処理中 |
| 保留中 | 保留中 |
| リクエスト日 | イシューステータスの変更をトリガーしません。 |
| 承認済み | イシューステータスの変更をトリガーしません。 |
| 却下 | イシューステータスの変更をトリガーしません。 |
| アイデア | イシューステータスの変更をトリガーしません。 |
| 停止 | クローズ |
| 完了 | クローズ |

>[!NOTE]
>
>イシューのステータスがクローズ済み（タスクまたはプロジェクトのクローズの結果）になった後、タスクやプロジェクトのステータスがクローズ後に何に変更されるかに関係なく、イシューはクローズ状態のままになります。

#### 解決オブジェクトのカスタムステータスと解決可能オブジェクトのカスタムステータスを同期 {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

タスクまたはプロジェクトのステータスをカスタムステータスに変更すると、次の 2 つの条件を満たす場合にのみ、イシューのステータスがカスタムイシューステータスに変更されます。

* 「解決オブジェクトのステータスが変更された」オプションが選択されている場合は、解決可能なイシューのステータスを自動的に更新します。 詳しくは、「解決可能なオブジェクトを処理するためのAdobe Workfrontの設定 [ を参照してください ](#set-up-adobe-workfront-to-handle-resolvable-objects)。

* プロジェクトまたはタスクのカスタムステータスは、イシューのカスタムステータスと同じ 3 文字コードです。

イシューと、プロジェクトまたはタスクの両方で、同じキーを使用してカスタムステータスを作成できます。プロジェクトまたはタスク（解決オブジェクトとして）がカスタムステータスに変更されると、その変更はイシューステータスにも反映されます。 ステータスキーは、イシューとプロジェクトまたはタスクのステータスで同じにする必要があります。

例えば、「現在」と同じ 3 文字のコード LCD を使用して「起動済み」という名前のプロジェクトのカスタムステータスを作成するとします。 次に、「プロジェクトが起動済み」という名前のイシューカスタムステータスと、レターコード LCD （処理中と同じ）を作成します。 プロジェクトを起動済みとしてマークすると、イシューのステータスが自動的にプロジェクト起動済みに変更されます。 「オブジェクトの解決の状態が変更されたとき、解決可能問題の状態を自動的に更新する」設定が有効になっていない場合、代わりに、問題の状態が進行中に変更されます。

カスタムステータスの作成について詳しくは、[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

## 解決オブジェクトの完了率を、解決可能オブジェクトの完了率と同期します。

イシューがタスクまたはプロジェクトによって解決された場合、次のいずれかが発生すると、イシューの完了率が解決可能なイシューに対して更新されます。

* 誰かがタスクまたはプロジェクトに対する変更を保存したとき。
* プロジェクトのタイムラインが再計算される場合。

問題が別の問題によって解決された場合、問題のいずれかが更新されると、完了率が更新されます。

## タスクまたはプロジェクト上で解決可能オブジェクトの検索

>[!NOTE]
>
>この節の手順を実行するには、少なくとも、タスクおよびプロジェクトへの表示アクセス権と、表示する解決可能オブジェクトを含むタスクまたはプロジェクトへの表示権限が必要です。

解決オブジェクトを見つける方法は、タスクとプロジェクトで同じです。

1. イシューを変換して作成したプロジェクトまたはタスクに移動します。
1. ページの左側で、「**タスクの詳細**」または「**プロジェクトの詳細** タブを選択します。
1. 「**概要**」セクションの下部で、タスクまたはプロジェクトの解決可能オブジェクトが表示されている **この解決済み** フィールドを見つけます。

   ![ この「解決」フィールド ](assets/this-resolves-field.png)

   >[!NOTE]
   >
   >イシューは他のイシューに変換することはできませんが、イシューの解決に手動で関連付けることができます。 プロジェクト、タスクまたはイシューは、解決可能オブジェクトとして複数のイシューを持つことができます。プロジェクト、タスクまたはイシューが解決されると、解決可能オブジェクト（イシュー）も解決されます。解決可能イシューは、解決したプロジェクト、タスクまたはイシューを再び開いた場合でも、クローズドのままになります。

## リスト内の解決オブジェクトに関するイシューの特定

イシューの一覧で、**ステータスアイコン**&#x200B;列または&#x200B;**フラグ**&#x200B;列でステータスアイコンを見つけることで、解決オブジェクトとしてラベル付けされているイシューをこのアイコンで特定できます。

![ 解決中のオブジェクト ](assets/resolving-icon.png)

## レポートでの解決可能オブジェクトおよび解決オブジェクト情報の表示

プロジェクト、タスクまたはイシューのビューまたはレポートに、解決可能オブジェクトまたは解決オブジェクトに関する情報を表示できます。

表示できるフィールドと、そのフィールドを表示できるビューを次の表に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>表示されるフィールド</strong> </th> 
   <th><strong>問題ビュー</strong> </th> 
   <th><strong>タスク ビュー</strong> </th> 
   <th><strong>プロジェクト ビュー</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong> 解決可能あり </strong>：プロジェクトまたはタスクに解決可能な問題が関連付けられている場合は True 値を表示し、関連付けられていない場合は False 値を表示します。</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong>元のイシュー名、元のイシューのエントリ日、発信元名</strong>：元のイシューの名前とエントリ日のほか、元のイシューを作成したユーザーの名前を、カスタマイズされたテキストモードビューに表示します。<br> 詳しくは、<a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref"> 表示：タスクまたはプロジェクトリストに元のイシュー情報を表示する </a> を参照してください。<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>解決可能</strong>：プロジェクト／タスクレポートまたはリストのテキストモードカスタムビューにすべての解決可能オブジェクトのリストを表示します。</p> <p>詳しくは、<a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref"> 表示：タスクまたはプロジェクトレポートでの解決可能なオブジェクト </a> を参照してください。</p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong> 変換済みイシューの作成者 </strong>：後でタスクに変換されたイシューを最初にログに記録したユーザーに関する情報を表示します。 </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong> プロジェクトの解決 </strong>：元のイシューから変換された、またはイシューの解決オブジェクトとして手動で指定された解決プロジェクトに関する情報を表示します。</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong> タスクの解決 </strong>：元のイシューから変換された、またはイシューの解決オブジェクトとして手動で指定された解決タスクに関する情報を表示します。</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong> イシューの解決 </strong>：手動でイシューの解決オブジェクトとして指定された、イシューの解決に関する情報を表示します。</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
