---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '表示：タスクとプロジェクトの問題の詳細の発生'
description: 問題がタスクまたはプロジェクトに変換されると、タスクまたはプロジェクトと問題との間に解決対象の関係が確立されます。 このビューには、タスクまたはプロジェクトが完了したときに自動的に完了する、イシューのフィールドが表示されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 3%

---

# 表示：タスクとプロジェクトの問題の詳細の発生元

問題がタスクまたはプロジェクトに変換されると、タスクまたはプロジェクトと問題との間に解決対象の関係が確立されます。 このビューには、タスクまたはプロジェクトが完了したときに自動的に完了する、問題の次のフィールドが表示されます。

* 名前
* エントリ日
* 予定完了日
* 実際の完了日
* リクエストタイプ
* 作成者名
* ユーザーに割り当て済み

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

詳しくは、 [表示：タスクとプロジェクトの一覧に元の問題情報を表示します](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>ビューの変更をリクエスト </p>
   <p>レポートを変更する計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タスクとプロジェクトの発生元の問題の詳細を表示します

1. タスクのリストまたはプロジェクトのリストに移動します。
1. 次から： **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. Adobe Analytics の&#x200B;**列のプレビュー** 領域を選択し、1 つ以外のすべての列を削除します。
1. 残りの列のヘッダーをクリックし、 **テキストモードに切り替え**.
1. テキストモード領域の上にマウスを移動し、 **クリックしてテキストを編集**.
1. 検索したテキストを削除します。 **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>column.0.textmode=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.descriptionkey=name<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.width=150<br>column.1.displayname=Resolvables (Issues)<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(resolvables).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={name}<br>column.1.valueformat=HTML<br>column.2.displayname=Resolvables Entry Date<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(resolvables).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={entryDate}<br>column.2.valueformat=HTML<br>column.3.displayname=Resolvables Due Date<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(resolvables).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Resolvables Actual Completion Date<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(resolvables).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={actualCompletionDate}<br>column.4.valueformat=HTML<br>column.5.displayname=Resolvables Request Type<br>column.5.listdelimiter=<br><br>column.5.listmethod=nested(resolvables).lists<br>column.5.textmode=true<br>column.5.type=iterate<br>column.5.valueexpression={opTaskType}<br>column.5.valueformat=HTML<br>column.6.displayname=Resolvables Originator<br>column.6.listdelimiter=<br><br>column.6.listmethod=nested(resolvables).lists<br>column.6.textmode=true<br>column.6.type=iterate<br>column.6.valueexpression={owner}.{name}<br>column.6.valueformat=HTML<br>column.7.descriptionkey=assignedto<br>column.7.linkedname=assignedTo<br>column.7.listsort=nested(assignedTo).string(name)<br>column.7.namekey=assignedto<br>column.7.querysort=assignedTo:name<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.textmode=true<br>column.7.valuefield=assignedTo:name<br>column.7.valueformat=HTML<br>column.7.width=150</code></pre>

1. クリック **ビューを保存**.
