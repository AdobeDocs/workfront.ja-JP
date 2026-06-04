---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: システム タスクの状態
description: Workfront の 3 つのビルトインのシステムタスクステータスは必須です。つまり、ロック解除、名前変更および並べ替えはできますが、非表示や削除はできません。 組織のニーズに合わせて新しいシステムタスクステータスを追加することもできます。 タスクステータスの変更は通常は手動のプロセスですが、システムで発生している他の要因によっては、タスクのステータスが自動的に変更される場合もあります。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
TQID: https://experienceleague.adobe.com/FACmZvT5v00-FS0lOBCMh347ZqM6c-Upfq4ITymVpV0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 409
ht-degree: 94%

---

# システムタスクステータス

Workfront の 3 つのビルトインのシステムタスクステータスは必須です。つまり、ロック解除、名前変更および並べ替えはできますが、非表示や削除はできません。

組織のニーズに合わせて新しいシステムタスクステータスを追加することもできます。

タスクステータスの変更は、通常は手動のプロセスです。 ただし、システムで発生している他の要因によっては、タスクのステータスが自動的に変更される場合があり、その概要を以下のリストで説明します。

Workfront インスタンスには、次のタスクステータスが用意されています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>システムタスクステータス</th> 
   <th>このステータスが発生する状況</th> 
   <th>タスクがこのステータスの場合に発生するアクション</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新規（必須ステータス）</td> 
   <td>これは、新しく作成されたあらゆるタスクのデフォルトのステータスです。</td> 
   <td>プロジェクトのタスクが「進行中」のステータスにある場合、そのタスクはタスクに割り当てられているユーザーの「作業要求」タブに表示されます。 これで、ユーザーはタスクの作業を開始できます。</td> 
  </tr> 
  <tr> 
   <td>処理中（必須ステータス）</td> 
   <td>タスクをこのステータスにすると、そのタスクの作業が始まったことを示すことができます。</td> 
   <td> <p>タスクを「処理中」とマークすると、タスクの「実際の開始日」に値が表示されます。</p> <p>タスクの進捗は、タスクの完了率を手動で更新するまで記録されません。</p> </td> 
  </tr> 
  <tr> 
   <td>完了（必須ステータス）</td> 
   <td> <p>タスクの作業が完了したら、タスクを手動で「完了」とマークすることができます。</p> <p>タスクの「トラッキングモード」が「オートコンプリート」に設定されている場合、タスクは予定完了日に達すると自動的に「完了」とマークされます。</p> </td> 
   <td> <p>タスクが完了すると、タスクの完了率が 100％とマークされます。 タスクが完了すると、ホーム領域の担当者の「自分の作業」リストからタスクが削除されます。</p> <p>タスクを「完了」とマークすると、タスクに「実際の完了日」の値が表示されます。</p> <p><b>メモ</b>：タスクに未完了のイシューがある場合に、タスクのステータスを「完了」に変更すると、ステータスは自動的に「完了 - 保留中の問題」に変わります。</p> </td> 
  </tr> 
 </tbody> 
</table>
