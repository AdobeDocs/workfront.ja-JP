---
product-area: projects
navigation-topic: use-predecessors
title: タスクリストに先行タスク関係を作成する
description: 先行タスク（または先行タスクのみ）を使用して、他のタスクに依存するタスクを開始または完了するためにリンクできます。 例えば、招待（先行タスク）を送信する前に、パーティ（依存タスク）をホストしたくない場合などです。
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# タスクリストに先行タスク関係を作成する

先行タスク（または先行タスクのみ）を使用して、他のタスクに依存するタスクを開始または完了するためにリンクできます。 例えば、招待（先行タスク）を送信する前に、パーティ（依存タスク）をホストしたくない場合などです。

この記事では、タスクリストで先行タスクを作成する方法を説明します。

タスクの先行タスクは、Adobe Workfrontの次の領域で表示できます。

* [ 先行タスク ] 列のタスク一覧で、次の操作を行います。
* ガントチャートで
* 依存タスクの [ 先行タスク ] セクション

詳しくは、 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクおよびプロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 先行タスクの作成

1. プロジェクトに移動します。
1. クリック **タスク** をクリックします。
1. 現在のビューに **前任者** 列。

   ビューに [ 先行タスク ] 列が表示されない場合は、そのビューに変更するか、ビューに列を追加します。

1. 依存タスクとして指定するタスクを選択します。
1. 内側をクリック **先行タスク** 列。
1. 選択したタスクの先行タスクとして指定するタスク番号を入力し、 **入力**.

   先行タスクが完了とマークされると、先行タスクのアイコンが緑色に変わります。 これは、依存タスクの作業準備ができたことを示します。

   [ 先行タスク ] 列で使用できる関係の種類の詳細については、「 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 先行タスクの詳細を表示

先行タスクの詳細は、タスクリストからすばやく表示できます。

1. タスク一覧で、 **先行タスク** 列。

   先行タスクの詳細を示すボックスが表示されます。

   ![先行者の詳細](assets/predecessor-details-in-task-list.png)

   次の詳細が表示されます。

   **旧名称：** 参照される先行者の名前。 先行タスクのタスク番号が含まれます。 タスク名をクリックして開きます。 上記の例では、前者は「実稼動/実行/配信」です。

   **プロジェクト名：** 先行プロジェクトが存在するプロジェクトの名前。 先行プロジェクトがタスクと同じプロジェクトに属する場合は現在のプロジェクト、先行プロジェクトが別のプロジェクトに属する場合はクロスプロジェクトとして識別されます。 上記の例では、プロジェクト名は Digital Asset Production (Integrated) - Project です。 プロジェクト間の先行タスクの詳細については、 [プロジェクト間の先行タスクの作成](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   プロジェクトの詳細を展開して、プロジェクトの計画開始日と終了日、条件、ステータス、完了率、所有者を確認できます。 クロスプロジェクトの場合は、「 **プロジェクトを見る** をクリックして、プロジェクトを開きます。

   **ID:** 先行プロジェクトが存在するプロジェクトの参照番号。

   **予定開始：** 先行タスクの計画開始日。

   **計画終了：** 先行タスクの計画完了日。

   **先行タスクの数：** 参照先の先行タスクの数。 上記の例では、参照される先行リソースに 1 つの先行リソースが含まれています。

   **後続の人数：** 参照先の先行タスクの後続タスク（または依存タスク）の数。 上記の例では、参照される先行者には 1 つの後続者があります。
