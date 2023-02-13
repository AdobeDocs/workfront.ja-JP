---
title: タスクの共有
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront管理者は、アクセスレベルを割り当てる際に、タスクの表示や編集のアクセス権を付与できます。 タスクへのアクセス権の付与の詳細については、「タスクへのアクセス権の付与」を参照してください。
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 4%

---

# タスクの共有

Adobe Workfront管理者は、アクセスレベルを割り当てる際に、タスクの表示や編集のアクセス権を付与できます。 タスクへのアクセス権の付与の詳細については、 [タスクへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

ユーザーに付与されるアクセスレベルに加えて、共有する特定のタスクを表示、投稿、管理する権限をユーザーに付与することもできます。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。

## タスクを共有する際の考慮事項

以下の考慮事項に加えて、 [オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* タスクの作成者には、デフォルトでタスクの管理権限が付与されています。
* タスクは個別に共有することも、一度に複数のタスクを一括して共有することもできます。\
   タスクの共有は、他のオブジェクトの共有と同じです。 Workfrontでの項目の共有について詳しくは、 [オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* タスクに次の権限を付与できます。 

   * ビュー
   * 管理
   * 参加\
      ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* タスクを共有する場合、デフォルトでは、ユーザーはタスクに関連付けられたすべての子オブジェクトに同じ権限を継承します。 例えば、タスクに添付された子タスク、タスク、ドキュメントに対して同じ権限を継承します。\
   Workfrontのオブジェクトの階層について詳しくは、  [Adobe Workfrontのオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   Workfrontの管理者は、ドキュメントがユーザーのアクセスレベルの上位のオブジェクトから権限を継承するかどうかを指定できます。 ドキュメントに対する継承された権限の制限について詳しくは、 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* タスクから継承された権限を削除できます。\
   継承された権限をオブジェクトから削除する方法について詳しくは、  [オブジェクトから権限を削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## タスクを共有する方法

タスクは次の方法で共有できます。

* 手動（個別または一括）。 タスクを手動で共有することは、Workfrontで他のオブジェクトを共有する場合と似ています。

   Workfrontでのオブジェクトの共有について詳しくは、  [オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 次の操作を実行すると、自動的に実行されます。

   * タスクの任意の親オブジェクトに対する権限を指定します。プロジェクト、プログラム、またはポートフォリオ。 タスクは、親オブジェクトから権限を継承します。 オブジェクトに対する継承された権限の表示については、 [オブジェクトの継承された権限の表示](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * タスクが存在するプロジェクトの作成に使用するテンプレートで、プロジェクト共有にエンティティを追加します。 テンプレートからプロジェクトを共有する方法については、 [テンプレートの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * プロジェクトの編集時に、プロジェクト内のすべてのタスクに対する権限を指定します。 プロジェクトに対するユーザーの権限に基づいて、プロジェクト上のタスクへのアクセスを管理する方法については、 [](../../manage-work/projects/manage-projects/edit-projects.md#access) 記事のセクション [プロジェクトを編集](../../manage-work/projects/manage-projects/edit-projects.md).
   >[!TIP]
   >
   >ユーザーがプロジェクト上のタスクに割り当てられる際に、どのタスク権限を持たせるかを指定しない場合、ユーザーはデフォルトで、プロジェクト上の同じ権限を受け取ります。

## タスク権限

次の表に、ユーザーにタスクの表示、投稿、管理を許可する際にユーザーに付与できる権限を示します。

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>アクション</strong> </th> 
   <th><strong>管理</strong> </th> 
   <th><strong>参加</strong> </th> 
   <th><strong>ビュー</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">タスクを追加</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">先行タスクを追加</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">問題を追加</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">タスクを削除</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>一般タスクの編集<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">タスクステータスの変更</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">タスク制約の編集</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">タスクの表示</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">ドキュメントを追加</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">タスクをコピー*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">タスクを移動*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">時間の記録</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">計画日の変更</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">割り当てを承認</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">割り当てを行う</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">カスタムフォームを添付</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">カスタムフィールドの編集</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">承認プロセスの作成</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">タスクを承認</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">財務情報を編集*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">費用の追加/編集</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">財務情報の表示</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">更新/コメント</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">共有</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">システム全体で共有</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;プロジェクトのアクセスレベルと権限で制御します。
