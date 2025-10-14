---
title: タスクの共有
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、タスクの表示や編集のアクセス権を付与できます。タスクへのアクセス権の付与について詳しくは、タスクへのアクセス権の付与を参照してください。
author: Courtney
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: eb4bf18407562b88bf0c946c905b202e5b62a5fe
workflow-type: tm+mt
source-wordcount: '1201'
ht-degree: 51%

---

# タスクの共有

Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、タスクの表示や編集のアクセス権を付与できます。タスクへのアクセス権の付与について詳しくは、[タスクへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)を参照してください。

ユーザーに付与されるアクセスレベルに加えて、共有するアクセス権を持つ特定のタスクを表示、参加または管理する権限をユーザーに付与することもできます。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

オブジェクトを共有するには、次の条件を満たしている必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：標準</p> 
   または
   <p>現在：ワーク以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>共有するオブジェクトに対する表示以上の権限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>共有するオブジェクトに対する表示またはそれ以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タスクを共有する際の考慮事項

以下の考慮事項に加えて、[オブジェクトに対する権限の共有の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

* タスクの作成者は、デフォルトでそのタスクの管理権限を持っています。
* タスクは個別に共有することも、一度に複数のタスクを一括して共有することもできます。\
  タスクの共有は、他のオブジェクトの共有と同じです。Workfront での項目の共有について詳しくは、[オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)を参照してください。

* タスクに次の権限を付与できます。

   * 表示
   * 管理
   * 参加
* タスクを共有すると、デフォルトでは、ユーザーはタスクに関連付けられたすべての子オブジェクトに対して同じ権限を継承します。 例えば、タスクに添付された子タスク、イシューおよびドキュメントに対して同じ権限を継承します。\
  Workfront のオブジェクトの階層について詳しくは、[Adobe Workfront のオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)を参照してください。

  Workfront 管理者は、ドキュメントがユーザーのアクセスレベルの上位のオブジェクトから権限を継承するかどうかを指定できます。ドキュメントに対する継承された権限の制限について詳しくは、[カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

* タスクから継承された権限を削除できます。\
  継承された権限をオブジェクトから削除する方法について詳しくは、[オブジェクトから権限の削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)を参照してください。

## タスクの共有方法

タスクは次の方法で共有できます。

* 手動（個別または一括）。

* 次の操作を実行すると、自動的に次の操作が行われます。

   * プロジェクト、プログラムまたはポートフォリオなど、タスクの任意の親オブジェクトに対する権限を指定します。タスクは、親オブジェクトから権限を継承します。オブジェクトに対する継承された権限の表示について詳しくは、[オブジェクトの継承された権限の表示](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)を参照してください。
   * タスクが存在するプロジェクトの作成に使用するテンプレートで、プロジェクト共有にエンティティを追加します。テンプレートからのプロジェクトの共有について詳しくは、[テンプレートの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)を参照してください。

   * プロジェクトの編集時に、プロジェクト内のすべてのタスクに対する権限を指定します。プロジェクトに対するユーザーの権限に基づいて、プロジェクト上のタスクへのアクセスを管理する方法について詳しくは、[プロジェクトの編集](../../manage-work/projects/manage-projects/edit-projects.md)の記事の [&#128279;](../../manage-work/projects/manage-projects/edit-projects.md#access) の節を参照してください。

  >[!TIP]
  >
  >ユーザーがプロジェクトのタスクに割り当てられたときに付与するタスク権限を指定しない場合、ユーザーはデフォルトでプロジェクトに付与されている権限と同じ権限を受け取ります。

## タスクの共有

1. 共有するタスクに移動します。

1. タスク名の右側にある「**共有**」をクリックします。 **共有 [ タスク名]** ダイアログボックスが開きます。

   ![&#x200B; 「タスクを共有」ボタン &#x200B;](assets/share-task-button.png)

1. **タスクへのアクセスの許可** フィールドに、タスクを共有するユーザー、チーム、役割、グループ、または会社の名前の入力を開始し、ドロップダウンリストに表示されたら名前をクリックします。

   >[!TIP]
   >
   >アクティブなユーザー、チーム、役割または会社とのみタスクを共有できます。


1. （オプション） **アクセスできるユーザー** ドロップダウンを選択し、タスクのアクセスレベルを選択します。

   * **招待されたユーザーのみがアクセスできます：** タスクに招待されたユーザーのみがタスクにアクセスできます（デフォルト）。
   * **システム内の全員が閲覧可能**：システム内のすべてのユーザーが、招待なしにタスクを閲覧できます。

1. ユーザー名の右側のドロップダウンをクリックし、このタスクの権限レベルを選択します。

   * **表示**：ユーザーは、タスクを確認し、共有できます。
   * **投稿**：ユーザーは、更新、情報の記録、小さな編集、タスクの共有を行うことができます（すべての表示権限も含まれます）。
   * **管理**：ユーザーは、管理者権限を持たずにタスクへのフルアクセス権を持ちます。これはアクセスレベルで付与されます（すべての表示権限と投稿権限も含まれます）。

1. （オプション）付与した権限レベルの横にある「詳細オプション」アイコンをクリックして、タスクに対する特定の権限を設定します。

   ![&#x200B; 設定済みの高度な権限オプション &#x200B;](assets/advanced-permission-options.png)

1. （オプション）タスクの子オブジェクトに対して継承された権限をオフにするには、**継承された権限** でインラインの **オフ** をクリックします。

1. （オプション）リンクを使用してタスクをすばやく共有するには、「**リンクをコピー**」をクリックして受信者に転送します。

1. **保存**&#x200B;をクリックします。


## タスクを一括共有

1. 共有するタスクを含むプロジェクトに移動します。

1. プロジェクトページの「**タスク**」タブで、共有する各タスクの左側にあるボックスを選択し、ページ上部にある **共有** アイコン ![&#x200B; 共有アイコン &#x200B;](assets/share-icon.png) をクリックします。 共有モーダルが開きます。

   ![&#x200B; タスクの一括共有 &#x200B;](assets/bulk-share-tasks.png)

1. **タスクへのアクセスの許可** フィールドに、タスクを共有するユーザー、チーム、役割、グループ、または会社の名前の入力を開始し、ドロップダウンリストに表示されたら名前をクリックします。

   >[!TIP]
   >
   >タスクを共有できるのは、アクティブなユーザー、チーム、役割または会社のみです。


1. （オプション） **アクセスできるユーザー** ドロップダウンを選択し、タスクのアクセスレベルを選択します。

   * **招待されたユーザーのみがアクセスできます：** タスクに招待されたユーザーのみがタスクにアクセスできます（デフォルト）。
   * **システム内の全員が表示可能**：システム内のすべてのユーザーが、招待なしにタスクを表示できます。


1. ユーザー名の右側にあるドロップダウンをクリックし、タスクの権限レベルを選択します。

   * **表示**：ユーザーは、タスクを確認し、共有できます。
   * **投稿**：ユーザーは、更新、情報の記録、小さな編集、タスクの共有を行うことができます（すべての表示権限も含まれます）。
   * **管理**：ユーザーは、管理者権限を持たないタスクへのフルアクセス権を持ちます。これらのアクセス権はアクセスレベルで付与されます（すべての表示権限と投稿権限も含まれます）。

1. （オプション）付与した権限レベルの横にある「詳細オプション」アイコンをクリックして、タスクに対する特定の権限を設定します。

   ![&#x200B; 設定済みの高度な権限オプション &#x200B;](assets/advanced-permission-options.png)

1. **保存**&#x200B;をクリックします。

## タスク権限

次の表に、ユーザーにタスクの表示、参加または管理を許可する際にユーザーに付与できる権限を示します。

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
   <th><strong>表示</strong> </th> 
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
   <td scope="row">先行タスクの追加</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">イシューを追加</td> 
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
   <td scope="row">タスクのコピー*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">タスクの移動*</td> 
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
   <td scope="row">予定日の変更</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">割り当ての受け入れ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">割り当て</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">カスタムフォームを添付</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">カスタムフィールドを編集</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">承認プロセスを作成</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">費用を追加／編集</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">財務情報を表示</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">アップデート／コメント</td> 
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

&#42;プロジェクトのアクセスレベルと権限で制御されます。
