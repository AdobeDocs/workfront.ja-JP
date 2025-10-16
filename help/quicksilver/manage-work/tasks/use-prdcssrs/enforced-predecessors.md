---
product-area: projects
navigation-topic: use-predecessors
title: 先行タスクを強制的に実行
description: 先行タスクとは、他のタスクの完了に依存するタスクのことです。先行タスクの関係は、タスクの開始日と完了日に影響し、最終的にはプロジェクトのタイムラインに影響を与えます。
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 94%

---

# 先行タスクを強制的に実行

<!-- Audited: 2/2024 -->

先行タスクとは、他のタスクの完了に依存するタスクのことです。先行タスクの関係は、タスクの開始日と完了日に影響し、最終的にはプロジェクトのタイムラインに影響を与えます。

先行タスクについて詳しくは、[タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

タスク間の先行タスクの関係を設定することで、依存タスクの開始と終了が、どのように先行タスクの開始と終了に依存するかを定義できます。これを行うには、異なる依存関係タイプを使用します。

依存関係タイプについて詳しくは、[タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)を参照してください。

## 強制的に実行される先行タスクの概要

>[!IMPORTANT]
>
>先行タスクの関係が優先されるようにするには、先行タスクを強制的に実行する必要があります。先行タスクを強制しなくても、依存タスクでは、依存関係タイプに関係なく、先行タスクの開始と終了とは別個に開始および終了できます。

プロジェクトに先行タスクを設定する際に、先行タスクの関係を強制的に実行できます。

先行タスクが強制的に実行された場合、後続タスクは先行タスクが完了するまで開始できません。例えば、タスク A とタスク B の間に終了と開始の関係を強制的に実行すると、タスク A が完了とマークされるまで、タスク B は開始できません（ステータスを「新規」の状態に維持し、「完了率」は 0％のままにする必要があります）。関係を強制的に実行は、すべての先行タスクタイプに適用されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p> 
   <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクおよびプロジェクトに対する権限の管理</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
      <p>New: Standard</p> 
      <p>OR</p>
      <p>Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>Manage permissions to the tasks and the project</p></td> 
  </tr> 
 </tbody> 
</table>-->

## タスクレベルで先行タスクを強制的に実行する

1. 先行タスクを強制的に実行する後続タスクに移動します。
1. 左側のパネルで **先行タスク** をクリックし、**先行タスクの追加** をクリックします。
1. （条件付き）プロジェクト間の先行タスクを追加する場合は、「**親プロジェクト**」フィールドのプロジェクト名を削除し、別のプロジェクトに置き換えます。
1. 「**タスク**」フィールドに先行タスクの名前を指定します。
1. この 2 つのタスクの間で&#x200B;**依存関係タイプ**&#x200B;を指定します。

   デフォルトの&#x200B;**依存関係タイプ**&#x200B;は&#x200B;**終了-開始**&#x200B;です。

1. 「**強制**」フィールドを選択して、先行タスクを強制的に実行します。
1. 「**保存**」をクリックします。

## タスクリストで先行タスクを強制的に実行する

1. プロジェクトのタスクリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューで「**標準ビュー**」を選択します。

1. 先行タスクとして指定するタスクの番号をメンタルメモに記録します。
1. 先行タスクを強制的に実行する後続タスクを検索します。
1. **先行タスク**&#x200B;列で、先行タスクの番号の入力を開始し、末尾に「e」を付けます。例えば、選択したタスクの先行タスクとしてタスク番号 1 を追加するには、「1e」と入力します。
1. Enter を押して、タスクの先行タスク情報を保存します。

   ![predecessor_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
