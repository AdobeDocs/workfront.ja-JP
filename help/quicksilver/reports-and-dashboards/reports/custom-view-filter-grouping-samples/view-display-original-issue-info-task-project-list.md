---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '表示：タスクとプロジェクトリストに元の問題情報を表示'
description: 問題をリスト内のタスクとプロジェクトに変換した後、タスクとプロジェクトリストのビューに元の問題の情報を表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 235156b6-a9b6-484e-b126-54874da705c8
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 4%

---

# 表示：タスクとプロジェクトの一覧に元の問題情報を表示します

問題をリスト内のタスクとプロジェクトに変換した後、タスクとプロジェクトリストのビューに元の問題の次の情報を表示できます。

* 変換済みイシュー名
* 変換済みのイシューのエントリ日
* 変換された問題の発行者名

標準の Report Builder を使用したビューの作成について詳しくは、 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

![task_and_project_list_with_original_issue_info.png](assets/task-and-project-list-with-original-issue-info-350x59.png)

プロジェクトとタスクリストに関する追加の問題情報を含める方法の詳細については、「 [表示：タスクとプロジェクトの問題の詳細の発生元](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-originating-issue-details-tasks-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: no longer needed - all fields are now in the UI</p>
<p>Applying this view is identical for tasks and projects.</p>
<p>To apply this view to a task list:</p>
<ol>
<li value="1">Go to a list of tasks which have been converted from issues</li>
<li value="2">From the <strong>View</strong> drop-down menu, select <strong>New View</strong>.</li>
<li value="3">In the<strong>Column Preview</strong> area, eliminate all columns except for one.</li>
<li value="4">Click the header of the remaining column, then click<strong>Switch to Text Mode</strong>.</li>
<li value="5">Mouse over the text mode area, and click <strong>Click to edit text</strong>.</li>
<li value="6"> <p>Remove the text you find in the <strong>Text Mode</strong> box, and replace it with the following code:</p>
<div class="codeSnippet">
<a class="codeSnippetCopyButton" role="button">Copy</a>
<div class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False">
<pre><code>column.0.descriptionkey=name<br>column.0.isInlineEditable=false<br>column.0.link.linkproperty.20.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.displayname=Converted Issue Name<br>column.1.linkedname=convertedOpTask<br>column.1.textmode=true<br>column.1.valuefield=convertedOpTaskName<br>column.1.valueformat=HTML<br>column.2.displayname=Converted Issue Entry Date<br>column.2.textmode=true<br>column.2.valuefield=convertedOpTaskEntryDate<br>column.2.valueformat=HTML<br>column.3.displayname=Originator Name<br>column.3.textmode=true<br>column.3.valuefield=convertedOpTaskOriginator:name<br>column.3.valueformat=HTML</code></pre>
</div>
</div> </li>
<li value="7"> Click <strong>Save View</strong>. </li>
</ol>
</div>
-->
