---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：タスクとプロジェクトの問題の詳細の発生元'
description: 問題がタスクまたはプロジェクトに変換されると、タスクまたはプロジェクトと問題との間に解決対象の関係が確立されます。 このビューには、タスクまたはプロジェクトが完了したときに自動的に完了する、問題の次のフィールドが表示されます — EDIT ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---

# 表示：元のタスクとプロジェクトの問題の詳細

問題がタスクまたはプロジェクトに変換されると、タスクまたはプロジェクトと問題との間に解決対象の関係が確立されます。 このビューには、タスクまたはプロジェクトが完了したときに自動的に完了する、問題の次のフィールドが表示されます。

* 名前
* エントリ日
* 予定完了日
* 実際の完了日
* リクエストタイプ
* 作成者名
* ユーザーに割り当て済み

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

詳しくは、 [表示：タスクとプロジェクトリストに元の問題情報を表示する](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タスクとプロジェクトの発生元の問題の詳細を表示します

1. タスクのリストまたはプロジェクトのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. 内&#x200B;**列のプレビュー** 領域を選択し、1 つ以外のすべての列を削除します。
1. 残りの列のヘッダーをクリックし、 **テキストモードに切り替え**.
1. テキストモード領域の上にマウスを移動し、 **クリックしてテキストを編集**.
1. 検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. クリック **ビューを保存**.
