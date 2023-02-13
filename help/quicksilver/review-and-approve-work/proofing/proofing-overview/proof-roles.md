---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: 配達確認の役割の概要
description: 配達確認の役割を使用すると、個々の配達確認に対する権限を付与できます。 配達確認の役割は、配達確認の権限プロファイルとは異なります。 配達確認権限プロファイルの詳細については、「配達確認権限プロファイルの概要」を参照してください。
author: Courtney
feature: Digital Content and Documents
exl-id: 258213af-0081-412e-bf6b-cdeb75d52966
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 2%

---

# 配達確認の役割の概要

配達確認の役割を使用すると、個々の配達確認に対する権限を付与できます。 配達確認の役割は、配達確認の権限プロファイルとは異なります。 配達確認権限プロファイルについて詳しくは、 [配達確認権限プロファイルの概要](../../../review-and-approve-work/proofing/proofing-overview/permission-profiles.md).

## 配達確認の役割

配達確認の役割は、ユーザーが配達確認のレビューに招待されたときに、個々の配達確認のユーザーに付与されます。 Workfront Pro+プランをお持ちの場合は、作業用またはプランのライセンスを持つユーザーに校正ロールを付与できます。 Workfront Premium レガシープランをご利用の場合は、指定された校正ライセンスを持つユーザーに校正の役割を付与できます。 詳しくは、 [Workfrontの校正機能へのアクセス](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

>[!NOTE]
>
>新しいWorkfrontプランのユーザーは、システム内の任意のユーザーに作成者またはモデレーターの役割を付与できます。 レガシープランのユーザーは、システム内の配達確認ライセンスを持つすべてのユーザーに、作成者またはモデレーターの役割を付与できます。

配達確認の役割は、特定の配達確認に関してレビュー担当者が実行できるアクションを定義します。

**例：** レビュー担当者の役割が割り当てられている場合は、マークアップとコメントを追加して配達確認を確認するように求められますが、配達確認を承認または拒否するオプションはありません。

特定の配達確認の役割は、レビュー担当者に対して（アカウントプロファイルがない場合でも）編集権限を付与し、コメントに対するアクションの追加、新しいバージョンの作成、配達確認へのレビュー担当者の追加などの追加機能を使用できます。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>配達確認を表示</strong> </p> </th> 
   <th> <p><strong>マークアップを追加</strong> </p> </th> 
   <th> <p><strong>コメントを追加</strong> </p> </th> 
   <th> <p><strong>返信がない場合は自分のコメントを編集</strong> </p> </th> 
   <th> <p><strong>決定を下す</strong> </p> </th> 
   <th> <p><strong>他のユーザーが行ったコメントを削除</strong> </p> </th> 
   <th>コメントを解決</th> 
   <th>コメントにアクションを適用</th> 
   <th> <p><strong>配達確認を編集</strong> </p> </th> 
   <th>他のユーザーと配達確認を共有</th> 
   <th>新しいバージョンを作成</th> 
   <th> <p><strong>ホーム領域での承認リクエストの表示</strong> </p> </th> 
   <th>新しいレビュー担当者を追加</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>読み取り専用</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>レビュアー</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>承認者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>レビュアーと承認者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>作者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>調整者</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
