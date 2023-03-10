---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: システムタスクのステータス
description: Workfrontの 3 つの組み込みのシステムタスクステータスが必要です。つまり、タスクのロック解除、名前変更、並べ替えは可能ですが、非表示や削除はできません。 また、組織のニーズに合わせて新しいシステムタスクステータスを追加することもできます。 タスクのステータスの変更は、通常は手動のプロセスですが、システムで発生している他の要因に応じて、タスクのステータスが自動的に変更される場合があります。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# システムタスクのステータス

Workfrontの 3 つの組み込みのシステムタスクステータスが必要です。つまり、タスクのロック解除、名前変更、並べ替えは可能ですが、非表示や削除はできません。

また、組織のニーズに合わせて新しいシステムタスクステータスを追加することもできます。

通常、タスクのステータスの変更は手動のプロセスです。 ただし、システムで発生している他の要因に応じて、タスクのステータスが自動的に変更される場合は、次のリストで時間の概要を示します。

Workfrontインスタンスには、次のタスクステータスが用意されています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>システムタスクステータス</th> 
   <th>このステータスが発生した場合</th> 
   <th>タスクがこのステータスの場合に発生するアクション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新規（必須ステータス）</td> 
   <td>これは、新しく作成されたすべてのタスクのデフォルトのステータスです。</td> 
   <td>タスクのステータスが「現在」のプロジェクトの場合、タスクはタスクに割り当てられているユーザーの「作業要求」タブに表示されます。 これで、ユーザーはタスクの作業を開始できます。</td> 
  </tr> 
  <tr> 
   <td>処理中（必須ステータス）</td> 
   <td>タスクをこのステータスに配置して、そのタスクの作業が開始したことを示すことができます。</td> 
   <td> <p>タスクを「進行中」とマークすると、タスクの「実績開始日」に値が表示されます。</p> <p>タスクの進捗状況は、タスクの完了率を手動で更新するまで記録されません。</p> </td> 
  </tr> 
  <tr> 
   <td>完了（必須ステータス）</td> 
   <td> <p>タスクの作業が完了したら、タスクを手動で完了とマークすることができます。</p> <p>タスクの「追跡モード」が「自動完了」に設定されている場合、タスクは計画完了日に達すると自動的に「完了」とマークされます。</p> </td> 
   <td> <p>タスクが完了すると、タスクの完了率が 100%とマークされます。 タスクが完了すると、[ ホーム ] 領域の担当者の作業リストからタスクが削除されます。</p> <p>タスクを [ 完了 ] に設定すると、タスクに [ 実績完了日 ] の値が表示されます。</p> <p><b>注意</b>:タスクに未完了のタスクが含まれ、タスクのステータスを「完了」に変更すると、ステータスは自動的に「完了 — 保留中のタスク」に変わります。</p> </td> 
  </tr> 
 </tbody> 
</table>
