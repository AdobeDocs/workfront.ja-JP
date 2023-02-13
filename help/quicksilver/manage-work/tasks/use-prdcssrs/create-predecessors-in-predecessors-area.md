---
product-area: projects
navigation-topic: use-predecessors
title: '[ 先行タスク ] 領域を使用して先行タスク関係を作成する'
description: 先行タスク（または先行タスクのみ）を使用して、他のタスクに依存するタスクを開始または完了するためにリンクできます。 例えば、招待（先行タスク）を送信する前に、パーティ（依存タスク）をホストしたくない場合などです。
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# [ 先行タスク ] 領域を使用して先行タスク関係を作成する

先行タスク（または先行タスクのみ）を使用して、他のタスクに依存するタスクを開始または完了するためにリンクできます。 例えば、招待（先行タスク）を送信する前に、パーティ（依存タスク）をホストしたくない場合などです。

この記事では、タスク内の [ 先行タスク ] タブを使用して先行タスクを設定する方法を示します。

タスクの一覧で先行タスクを設定する方法については、 [タスクリストに先行タスク関係を作成する](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

タスクの先行タスクは、Adobe Workfrontの次の領域で表示できます。

* 依存タスクの [ 先行タスク ] セクション
* ガントチャート内
* [ 先行タスク ] 列のタスク一覧

先行タスクの詳細については、 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクおよびプロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タスクの先行タスクの作成

1. 依存タスクとして指定するタスクに移動し、「 **先行タスク** をクリックします。

   クリックが必要になる場合があります **さらに表示**&#x200B;を、 **先行タスク**.

1. クリック **+前任者を追加**.
1. （オプション）プロジェクト間の先行タスクを追加するには、 **親プロジェクト** フィールドに別のプロジェクトを入力し、先行タスクとして使用する 1 つまたは複数のタスクの名前を入力します。

   プロジェクト間の先行タスクの追加の詳細については、 [プロジェクト間の先行タスクの作成](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. 先行タスクとして指定する 1 つまたは複数のタスクの名前を入力します。

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. を選択します。 **依存タイプ**.

   タスクの依存タイプの詳細については、 [タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. を指定します。 **ラグ** 金額（日単位）。

   ラグタイプの詳細については、を参照してくださ&#x200B;い。 [ラグタイプの概要](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. 選択 **強制** 2 つのタスク間の先行関係を強制する場合。

   先行タスクの適用の詳細については、 [先行タスクを適用](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. 「**保存**」をクリックします。
