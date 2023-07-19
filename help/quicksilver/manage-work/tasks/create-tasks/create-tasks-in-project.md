---
product-area: projects
navigation-topic: create-tasks
title: プロジェクトでのタスクの作成
description: プロジェクト内でタスクを作成できるのは、プロジェクトを作成した後だけです。
author: Alina
feature: Work Management
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: f8d596121f90d4f0c57e65cc415d1df87c14730c
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 1%

---

# プロジェクトでのタスクの作成

プロジェクト内でタスクを作成できるのは、プロジェクトを作成した後だけです。

例えば、プロジェクトを作成した後に、タスクを追加して変更し、プロジェクト計画を整理することができます。 プロジェクトの作成について詳しくは、 [プロジェクトの作成](../../../manage-work/projects/create-projects/create-project.md).

プロジェクトに含まれていない個人用タスクの作成について詳しくは、この記事の「個人用タスクの作成」の節を参照してください [ホーム領域から作業項目を作成する](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

この記事では、タスクを一から作成する方法について説明します。 次の方法でタスクを作成することもできます。

* 既存のタスクをコピーまたは複製する。 詳しくは、 [タスクのコピーと複製](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* タスクをプロジェクト間で移動する。 詳しくは、 [タスクを移動](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## アクセス要件

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td><p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 タスクへのアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">タスクへのアクセス権の付与</a>. Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクを追加する機能以上を持つ、プロジェクトに権限を付与する</p> <p>タスクを作成すると、タスクに対する「権限を管理」が自動的に付与されます</p> <p> タスク権限について詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">タスクの共有 </a>. </p> <p>追加の権限のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトでのタスクの作成

1. タスクを作成するプロジェクトに移動します。
1. クリック **タスク** をクリックします。
1. （条件付き）現在、アジャイルビューでタスクリストを表示している場合、 **リスト表示** アイコン ![](assets/list-view-in-agile-view-for-tasks.png) をクリックして、タスクリストを表示します。
1. （オプション） **プランモード** アイコン ![](assets/nwe-plan-mode-icon-task-list.png) を選択し、 **手動で保存**&#x200B;次に、 **標準** または **タイムライン計画**. これにより、 **自動保存** オプションを選択します。このオプションはデフォルトで有効になっています。

   ![](assets/nwe-autosave-off-manual-highlighted-350x58.png)

   >[!TIP]
   >
   >「手動保存」を選択すると、変更を元に戻すことができます。

1. 次のいずれかの操作を行って、新しいタスクを作成します。

   * クリック **新規タスク** タスクリストの最上部に
   * クリック **タスクをさらに追加** タスクリストの下部

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. （条件付き）クリックした場合 **新規タスク** 次の操作を実行します。

   1. 内のフィールドの制限付きリストで、任意のフィールドを指定します。 **新規タスク** ボックスに移動し、 **タスクを作成** タスクをすばやく作成する場合は、をクリックします。

      または

      タスクのすべてのフィールドを更新するには、 **その他のオプション** 開く **タスクを作成** ボックス

      ![](assets/nwe-create-task-small-screen-350x272.png)

      この **タスクを作成** ボックスが開きます。

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >Workfront管理者がレイアウトテンプレートを設定する方法によっては、「タスクを作成」ボックスのフィールドに環境内の異なるフィールドが表示される場合があります。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. 「タスクを作成」ボックスの左パネルで、次の領域に関する情報を指定します。

      * タスク名
      * 概要
      * 割り当て
      * カスタムフォーム
      * 財務
      * 設定

        タスクに関連するすべてのフィールドを定義する方法については、 [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. （条件付きおよびオプション）タスクを繰り返し実行する場合は、 **繰り返し頻度** フィールドに入力します。 繰り返しタスクの作成について詳しくは、 [繰り返しタスクの作成](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. （オプション）「 **ドキュメント** 左側のパネルでドキュメントを新しいタスクに添付し、 **ファイルの追加またはリンク** を使用して、コンピューター、別のサービス、またはコンピューターまたは別のサービスからドキュメントやフォルダーをタスクに追加します。

1. （条件付き）クリックした場合 **タスクをさらに追加** 手順 5 で、インライン編集を使用してタスク情報の入力を開始し、Enter キーを押します。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   特に、複数のタスクをリストに追加する場合は、このオプションを使用することをお勧めします。

   ![](assets/ctp4-350x26.png)

1. （条件付き）次のいずれかの操作を行います。

   * クリックした場合 **新規タスク** 手順 5 で、をクリックします。 **タスクを作成** 変更を保存し、プロジェクトに新しいタスクを追加します。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * クリックした場合 **タスクをさらに追加** 手順 5 で、次の操作を実行します。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. ブラウザー内の任意の場所をクリックして変更を送信するか、Enter キーを押します。
      1. （オプション）タスクリストで、新しく作成したタスクを選択し、 **インデント**.

         これにより、新しいタスクが前のタスクの子またはサブタスクになります。

         子タスクの詳細については、 [タスクの概要](../../../manage-work/tasks/task-information/tasks-overview.md).

      1. （条件付き） **自動保存** 押した後のオプション **タスクをさらに追加**&#x200B;を使用する場合、次の操作を実行できます。

         * クリック **取り消し** 最後の変更を元に戻す場合、または **キャンセル** をクリックして、タスクリストに加えたすべての変更を元に戻します。
         * 以前に **取り消し**&#x200B;をクリックし、 **やり直し** をクリックして、最後にキャンセルした変更を再適用します。
         * クリック **保存** をクリックして、タスクリストに対する変更を保存します。
