---
product-area: projects
navigation-topic: convert-issues
title: Adobe Workfront での変換の問題の概要
description: イシューの送信後に、イシューを完了するために必要な作業が他にもある場合は、そのイシューをプロジェクトまたはタスクに変換することができます。
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '1383'
ht-degree: 89%

---

# Adobe Workfront での変換の問題の概要

イシューの送信後に、イシューを完了するために必要な作業が他にもある場合は、そのイシューをプロジェクトまたはタスクに変換することができます。

イシューのタスクへの変換について詳しくは、[Adobe Workfront でイシューをタスクに変換](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)を参照してください。

イシューのプロジェクトへの変換について詳しくは、[Adobe Workfront でイシューをプロジェクトに変換](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)を参照してください。

## イシューを変換する際の考慮事項

* Workfront 管理者またはグループ管理者は、イシューがプロジェクトまたはタスクに変換されたときに、イシューに発生すること、その解決策、および主要連絡先のアクセスに関する環境設定をすでに設定しています。これは、[システム全体のタスクとイシューの環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)で説明されています。
* Workfront は、変換時にイシューに関連する承認をすべて削除します。
* タスクまたはプロジェクトに変換すると、Workfront はイシューの解決オブジェクトを上書きします。新しいタスクまたはイシューは、変換後に新しいイシューの解決オブジェクトになります。
* 次の点に注意してください。

   * 変換中に、作成中のプロジェクトまたはタスクにイシューとその解決策を関連付けたままにするかどうかを尋ねられる場合があります。
   * イシューを保持すると、プロジェクト、タスク、またはイシューに変更が生じた場合や、Workfront でタイムラインが再計算された場合に、プロジェクトまたはタスクのステータスと完了率が、イシューのステータスと完了率を自動的に更新します。

* イシューをタスクまたはプロジェクトに変換すると、イシューに割り当てられたユーザーのホームエリアからイシューが削除されます。

* 問題を変換する場合、元の問題に対する権限は、変換後のオブジェクト（タスクまたはプロジェクト）には転送されません。

* テンプレートを使用してイシューをプロジェクトに変換する場合、テンプレートのほとんどの情報が新しいプロジェクトに転送されます。ただし、問題の情報の一部は、新しいプロジェクトにも転送できます。 詳しくは、 [テンプレートを使用してイシューをプロジェクトに変換する際のプロジェクトフィールドの概要](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) 」の節を参照してください。
* イシューの変換時に、すべてのドキュメントまたはその情報が、イシューの変換先となる新しいオブジェクトに移動されるわけではありません。ドキュメントまたはドキュメントリンクが添付されたイシューを変換する場合、次の項目が含まれます。

   * ドキュメント
   * Google Drive や SharePoint など、サードパーティのサービスへのドキュメントリンク。
   * バージョン
   * プルーフは、**元のイシューを保持し、その解決策をこのプロジェクトに関連付ける**&#x200B;オプションが選択されていない場合にのみ含まれます。
   * ドキュメントとドキュメントリンクが添付されたイシューを変換する場合、ドキュメント承認は含まれません。

* 変換時にイシューを残すことに決め、それにドキュメントが添付されている場合、ドキュメントとそのバージョンはプロジェクトまたはタスクにコピーされます。プルーフとドキュメント承認は、プロジェクトやタスクにコピーされません。
* 変換時にイシューを残さないことに決め、それにドキュメントが添付されている場合、ドキュメント、そのバージョン、およびプルーフはプロジェクトまたはタスクに転送されます。ドキュメント承認は、プロジェクトやタスクには転送されません。
* Google ドライブなどのサードパーティサービスから元のイシューにリンクされているドキュメントやフォルダーがある場合は、変換時にイシューを保持するかどうかに関係なく、そのリンクが新しいオブジェクトにコピーされます。
* イシューのコメントは、イシューから変換されたタスクまたはプロジェクトにもコピーされますが、タグ付きユーザーは転送されません。
* カスタムフォーム情報をイシューから変換先のプロジェクトまたはタスクに転送する場合は、イシューから転送する同じフィールドを含むプロジェクトまたはタスクのカスタムフォームがあることを確認してください。詳しくは、[オブジェクトの変換時にカスタムフォームデータを転送](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md)を参照してください。

## テンプレートを使用してイシューをプロジェクトに変換する際のプロジェクトフィールドの概要 {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

イシューをプロジェクトに変換する場合は、空のプロジェクトに変換するか、テンプレートを使用します。

詳しくは、[イシューを Adobe Workfront のプロジェクトに変換](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)を参照してください。

テンプレートを使用する場合、テンプレートに入力される一部のフィールドは、変換されたイシューから作成されたプロジェクトに転送されます。その他のフィールドは、変換されたイシューからプロジェクトに転送されます。

次の表に、プロジェクト情報と、その情報がテンプレートから転送されるか、イシューから転送されるかを示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>説明</td> 
   <td> <p>イシューの説明は、新しいプロジェクトに転送されます。 </p> <p> イシューに説明がない場合、テンプレートの説明がプロジェクトに転送されます。 </p> <p>イシューの場合とテンプレートの場合の両方で「説明」フィールドが空の場合、プロジェクトのフィールドは空になります。 </p> </td> 
  </tr> 
  <tr> 
   <td>ステータス</td> 
   <td>テンプレート上のグループに選択されたデフォルトのステータス。テンプレートがグループに関連付けられていない場合、プロジェクトのステータスは、Workfront 管理者が設定のプロジェクト環境設定エリアで設定したデフォルトのステータスに設定されます。詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定を指定</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td>優先度</td> 
   <td>テンプレートから転送します。 </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>イシューの URL が新しいプロジェクトに転送されます。 </p> <p> イシューで URL が指定されていない場合、テンプレートの URL がプロジェクトに転送されます。 </p> <p>イシューの場合とテンプレートの場合の両方で「URL」フィールドが空白の場合、プロジェクトのフィールドは空白になります。 </p> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト状況タイプ</td> 
   <td>テンプレートから転送します。</td> 
  </tr> 
  <tr> 
   <td>プロジェクトの状況</td> 
   <td>設定エリアの Workfront 管理者が決定した、システムレベルのデフォルト環境設定に一致します。詳しくは、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">カスタム条件をプロジェクトのデフォルトとして設定</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td>スケジュールの基点</td> 
   <td>テンプレートから転送します。</td> 
  </tr> 
  <tr> 
   <td>プロジェクトの日付</td> 
   <td> 
    <ul> 
     <li> <p><b>予定開始日</b>：テンプレートスケジュールのタイムゾーンに従って、テンプレートスケジュールの作業時間に基づく最も近い作業時間を事前に選択する必要があります。「スケジュール元」フィールドが「完了から」に設定されている場合、このフィールドは無効になっています。 </p> </li> 
     <li> <p><b>完了予定日</b>：テンプレートスケジュールのタイムゾーンに従って、テンプレートスケジュールの作業時間に基づく最も近い作業時間を事前に選択する必要があります。「スケジュールの基点」フィールドが「開始日」に設定されている場合、このフィールドは無効になっています。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ</td> 
   <td>テンプレートから転送します。 それ以外の場合、このフィールドは空白になります。</td> 
  </tr> 
  <tr> 
   <td>プログラム</td> 
   <td>テンプレートから転送します。 それ以外の場合、このフィールドは空白になります。</td> 
  </tr> 
  <tr> 
   <td>グループ</td> 
   <td><p> 次のシナリオが存在します。</p>
     <ul><li>変換中にグループが指定された場合、そのグループがプロジェクトのグループになります</li>
     <li>テンプレートを使用してプロジェクトに変換し、テンプレートにグループが存在し、変換時にグループを指定しない場合、テンプレートのグループが新しいプロジェクトのグループになります</li>
      <li> テンプレートにグループがなく、変換時にグループを指定しない場合、元のイシューのプロジェクトのグループが新しいプロジェクトのグループになります</li> </ul>
      </td> 
  </tr> 
  <tr> 
   <td>会社</td>    
   <td>  テンプレートから転送します。それ以外の場合、このフィールドは空白になります。</td>

</tr> 
  <tr> 
   <td>プロジェクト所有者</td> 
   <td>テンプレートの「テンプレート所有者」フィールドから転送します。それ以外の場合は、変換処理を実行するログイン中のユーザーに設定されます。 </td> 
  </tr> 
  <tr> 
   <td>プロジェクトスポンサー</td> 
   <td>テンプレートの「テンプレートスポンサー」フィールドから転送します。それ以外の場合、このフィールドは空白になります。</td> 
  </tr> 
  <tr> 
   <td>リソースマネージャー</td> 
   <td>テンプレートから転送します。それ以外の場合、このフィールドは空白になります。</td> 
  </tr> 
  <tr> 
   <td>タスク設定</td> 
   <td>テンプレートから転送します。</td> 
  </tr> 
  <tr> 
   <td>イシュー設定</td> 
   <td>テンプレートから転送します。 </td> 
  </tr> 
  <tr> 
   <td>アクセス</td> 
   <td> <p>テンプレートの「アクセス」セクションからの転送。 </p> </td> 
  </tr> 
  <tr> 
   <td>承認</td> 
   <td>テンプレートから転送します。イシューに関連付けられている承認は、変換中に削除されます。 </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p>  </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p>  </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## プロジェクトとタスクに関する元のイシュー情報を表示 {#view-original-issue-information-on-projects-and-tasks}

元のイシューの情報は、プロジェクトとタスクのリストとレポート、またはプロジェクトの詳細領域で表示できます。レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

変換後のプロジェクトとタスクで、どのイシューフィールドが表示されるかを次の表に示します。

| イシューフィールド | プロジェクトまたはタスクフィールド | プロジェクトリストまたはレポート | プロジェクト詳細領域 | タスクリストまたはレポート | タスク詳細領域 |
|---|---|---|---|---|---|
| イシュー名 | 変換済みイシュー名 | ✔ | ✔ | ✔ | ✔ |
| プライマリ連絡先 | 変換済みイシューの発信元名 | ✔ | `✔` | ✔ |   |
| エントリ日 | 変換済みのイシューのエントリ日 | ✔ |   | ✔ |   |


>[!CAUTION]
>
>イシューのプライマリ連絡先が変更された場合、またはイシューの変換後にイシューのリンクがプロジェクトまたはタスクから解除された場合は、変換済みイシューの発信元名は更新されず、イシューの変換時に元のプライマリ連絡先が表示されます。
