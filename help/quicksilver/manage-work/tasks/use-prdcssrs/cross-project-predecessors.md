---
product-area: projects
navigation-topic: use-predecessors
title: プロジェクト間の先行タスクの作成
description: プロジェクト間の先行タスクとは、別のプロジェクト内の別のタスク（後続タスクと呼ばれます）が依存するタスクです。 先行タスクとは、依存（後続）タスクよりも優先されるタスクです。 たとえば、依存タスクを開始する前に、先行タスクを [ 完了 ] とマークする必要がある依存関係を作成できます。
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# プロジェクト間の先行タスクの作成

<!--Audited: 12/2023-->

プロジェクト間の先行タスクとは、別のプロジェクト内の別のタスク（後続タスクと呼ばれます）が依存するタスクです。 先行タスクとは、依存（後続）タスクよりも優先されるタスクです。 たとえば、依存タスクを開始する前に、先行タスクを [ 完了 ] とマークする必要がある依存関係を作成できます。

Adobe Workfrontを使用すると、1 つのプロジェクト内の先行タスクが許可されるのと同じように、他のプロジェクト内のタスクに依存するタスクを設定できます。

>[!INFO]
>
>例えば、掘削会社には 1 つのバックホーしかなく、2 つのプロジェクトにはバックホーを使用する必要があるタスクがあります。 プロジェクトマネージャは、最初のプロジェクトのタスクを、2 番目のプロジェクトのタスクの先行タスクにすることができます。 これは、最初のプロジェクトが終了したときに、2 つ目のプロジェクトでバックホーの使用を開始できることを示しています。

プロジェクト間の先行タスクを通じてプロジェクトをリンクする場合、プライマリプロジェクトの日付（先行タスクがある日付）は、セカンダリプロジェクト（後続タスクがある日付）に影響します。

>[!TIP]
>
>セカンダリプロジェクトの更新日を表示するには、プロジェクトのタイムラインを再計算する必要があります。 タイムラインの再計算について詳しくは、 [プロジェクトのタイムライン再計算の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

先行関係の詳細については、「 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## アクセス要件

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
  <td> <p>新規：標準 </p>
 <p>または</p> 
<p>現在：プラン </p> 
</td> 
 </tr>   <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>タスクおよびプロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクト間の先行タスクを作成する

1. 後続のタスク（依存タスク）に移動します。
1. クリック **先行タスク** をクリックします。
1. クリック **先行タスクを追加します。**
1. Adobe Analytics の **親プロジェクト** [ ] フィールドに、現在のタスクの先行タスクにするタスクを含むプロジェクトの名前を入力します。
1. 名前がドロップダウンリストに表示されたら、その名前をクリックします。
1. Adobe Analytics の **タスク** フィールドに、現在のタスクの先行タスクにするタスクの名前を入力します。
1. 先行タスクと依存タスクの間の関係を定義するには、次の情報を指定します。

   * **依存関係の種類：** 先行タスクと依存タスクの関係を選択します。 既定の関係は [ 終了 — 開始 ] です。これは、依存タスクを開始する前に先行タスクを終了する必要があることを意味します。 様々な依存タイプについて詳しくは、 [タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **ラグ：** 依存タスクが開始できるまで、強制先行タスクの完了後に経過する必要がある時間を指定します。 各種のラグの詳細については、 [ラグタイプの概要](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **強制：** このオプションを選択した場合、2 つのタスク間の依存関係を、ユーザーが早期にタスクを開始したことで回避することはできません。 たとえば、タスク A とタスク B の間に関係を強制すると、タスク A が完了するまでタスク B は開始できません。 先行タスクの適用の詳細については、「 [先行タスクの実行](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     このオプションを選択しない場合、依存関係はユーザーに対する提案のように扱われます。 例えば、ユーザーはタスク A が完了する前にタスク B を開始できます。

1. 「**保存**」をクリックします。

   プロジェクト間の先行タスクを持つタスクには、先行タスクが属するプロジェクトの参照番号と、タスクの番号がコロンで区切られて、タスクリストの [ 先行タスク ] 列に表示されます。

   ![プロジェクト間の先行者](assets/cross-project-predecessor-in-list-view.png)

   先行タスクが完了とマークされると、先行タスクのアイコンが緑色に変わります。 これは、依存タスクの作業準備ができたことを示します。

   この値の上にマウスポインターを置くと、先行プロジェクト、日付に関する詳細情報が表示されます。 [ 詳細 ] ボックスの [ プロジェクト間の先行タスク ] をクリックして、タスクを開きます。

   前任者のプロジェクトの詳細を表示するには、ホバーウィンドウの上部をクリックします。

   クリック **プロジェクトを見る** 前任者のプロジェクトを開く。

   ![プロジェクト間の先行者の詳細](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   The **プロジェクトを見る** [ ] オプションは、プロジェクト間の先行タスクを表示する場合にのみ表示されます。

