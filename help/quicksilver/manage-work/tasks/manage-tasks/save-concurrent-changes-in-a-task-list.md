---
product-area: projects
navigation-topic: manage-tasks
title: タスクリスト内での同時変更の保存の概要
description: リスト内でタスクを編集する際に、個別の保存設定を使用して、変更の保存を自動的にするか手動でするかどうかを指定できます。
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '497'
ht-degree: 100%

---

# タスクリスト内での同時変更の保存の概要

リスト内でタスクを編集する際に、個別の保存設定を使用して、変更の保存を自動的にするか手動でするかどうかを指定できます。

タスクリスト内のタスクの編集に関について詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)を参照してください。

2 人のユーザーが同じタスクで変更を加えている場合、競合が発生する場合があります。

タスクリスト内でタスクを編集する際には、以下の点を考慮してください。

* プロジェクトの更新の種類が自動、手動、または変更時の場合、変更内容を自動的に保存するように選択すると、Adobe Workfrontはタスクに対して行った変更を直ちに保存します。プロジェクトの更新の種類について詳しくは、[プロジェクトの更新の種類を選択](../../../manage-work/projects/manage-projects/select-project-update-type.md)を参照してください。
* Workfront は、作業中のリストに関する情報を毎分アップデートし、他のユーザーがシステム内の他の場所で行う変更を反映させます。これにより、常にタスクに関する最新の情報を取得できます。

複数のユーザーが同じタスクを編集する場合、以下のシナリオが考えられます。

* **1 人のユーザーがタスクリストに変更を自動的に保存し、別のユーザーが手動で変更を保存**：ユーザー B が（ユーザー A と）同一の複数のタスクの編集中に、ユーザー A が手動で変更を保存した場合、変更は自動的に保存されますが、ユーザー B が行なったライブの変更は、1 分ごとにユーザー A のリストで更新されます。2 人のユーザーが行った変更の間に競合が発生した場合、両名が変更を保存する前に、手動で保存しようとするユーザー（この場合はユーザー A）に警告メッセージが表示されます。警告メッセージに、競合する変更を含む項目が表示されます。この時点で、ユーザ A は、変更を保持する（ユーザ B による変更を上書きする）か、破棄する（ユーザ B による変更を保持する）かを選択できます。

>[!NOTE]
>
>行った変更を破棄する場合は、他のユーザーが行った編集と競合する変更だけでなく、すべての変更に適用されます。

* **複数のユーザーがタスクリストに手動で変更を保存**：リストのタスクに変更を加えている複数のユーザーが手動で同時に保存する場合、Workfront は、最初に保存を実行するユーザーによる変更を保存します。これらの変更を保存しても、競合が発生することはありません。次に Workfront は、他のすべてのユーザーによる変更と、既に保存されている情報とを比較し、他のユーザーが情報を保存する前に、競合する変更についての警告を表示します。

>[!IMPORTANT]
>
>他のすべての変更よりも、自分の変更を保持することを選択すると、自分が変更を加えたタスクが別のユーザーによって削除されない限り、すべての変更が保存されます。この場合、警告メッセージは、削除されたタスクに加えた変更が失われることを通知します。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
