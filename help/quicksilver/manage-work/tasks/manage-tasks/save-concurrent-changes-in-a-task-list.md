---
product-area: projects
navigation-topic: manage-tasks
title: タスクリスト内の同時変更の保存の概要
description: リストのタスクを編集する際に、別の保存設定を使用して、リストのタスクを編集する際に、手動で変更を自動的に保存するかどうかを指定できます。
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# タスクリスト内の同時変更の保存の概要

リストのタスクを編集する際に、別の保存設定を使用して、リストのタスクを編集する際に、手動で変更を自動的に保存するかどうかを指定できます。

タスクリスト内のタスクの編集について詳しくは、 [リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

2 人のユーザーが同じタスクで変更を加えている場合、競合が発生することがあります。

タスクリスト内のタスクを編集する際は、次の点に注意してください。

* [ 更新の種類 ] が [ 自動 ]、[ 自動 ]、または [ 変更時 ] の場合、変更内容を自動的に保存するように選択すると、Adobe Workfrontはタスクに加えた変更を直ちに保存します。 プロジェクトの更新タイプについては、 [プロジェクトの更新タイプを選択](../../../manage-work/projects/manage-projects/select-project-update-type.md).
* Workfrontは、作業中のリストに関する情報を毎分更新し、他のユーザーがシステム内の他の場所で行う変更を反映します。 これにより、常にタスクに関する最新の情報を取得できます。

複数のユーザーが同じタスクを編集する場合、次のシナリオが存在します。

* **1 人のユーザーがタスクリストに変更を自動的に保存し、別のユーザーが手動で変更を保存します**:ユーザー B が同じタスクの編集中に、ユーザー A が手動で変更を保存し、自動的に変更を保存すると、ユーザー B が行ったライブの変更は、1 分ごとにユーザー A のリストに更新されます。 2 人のユーザーが行った変更の間に競合が発生した場合、ユーザーが手動で保存した（ユーザー A）場合、変更を保存する前に警告メッセージが表示されます。 警告メッセージに、競合する変更を含む項目が表示されます。 この時点で、ユーザ A は、変更を保持する（ユーザ B による変更を上書きする）か、破棄する（ユーザ B による変更を保持する）かを選択できます。

>[!NOTE]
>
>行った変更を破棄する場合は、他のユーザーが行った編集と競合する変更だけでなく、すべての変更に適用されます。

* **複数のユーザーがタスクリストに手動で変更を保存しています**:リスト内のタスクに変更を加えている複数のユーザーが手動で同時に保存する場合、Workfrontは最初に保存したユーザーによる変更を保存します。 これらの変更を保存しても、競合が発生することはありません。 次に、Workfront は、他のすべてのユーザーによる変更と既に保存された情報を比較し、情報を保存する前に、他のユーザーに対する競合する変更に関する警告を表示します。

>[!IMPORTANT]
>
>変更を他のすべての変更に対して保持する場合は、変更を加えたタスクが別のユーザーによって削除されていない限り、すべての変更が保存されます。 この場合、削除したタスクに加えた変更が失われたことを示す警告メッセージが表示されます。

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
