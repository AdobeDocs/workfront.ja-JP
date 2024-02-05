---
product-area: projects
navigation-topic: create-tasks
title: サブタスクを作成
description: Workfront では、タスクに親子関係を設定できます。子タスクはサブタスクと呼ばれます。メインタスクをサブタスクにすることで、タスクリストにサブタスクを作成できます。サブタスクをメインタスクにすることもできます。
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: d71ee30378c39975366f4f257e3f7b17aba0c0ae
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 91%

---

# サブタスクを作成

<!-- Audited: 1/2024 -->

Workfront では、タスクに親子関係を設定できます。子タスクはサブタスクと呼ばれます。メインタスクをサブタスクにすることで、タスクリストにサブタスクを作成できます。サブタスクをメインタスクにすることもできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> 
   <p>新規：標準</p>
   <p>現在：作業以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクの追加以上の機能を備えたプロジェクトおよび親タスクに、参加権限を付与</p> <p>タスクの作成後、タスクに対する「管理」権限が自動的に付与されます。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## サブタスクを作成

サブタスクは、タスクリストまたはタスクのサブタスクセクションから作成できます。

### タスクリストからサブタスクを作成 {#create-subtasks-from-the-task-list}

1. サブタスクを作成するプロジェクトに移動します。
1. 左パネルの「**タスク**」セクションをクリックします。
1. （条件付き）親にしたいタスクの直下に、子タスクにしたいタスクがまだ配置されていない場合は、そのタスクをタスクリスト内の適切な場所にドラッグします。
1. サブタスクにするタスクを選択し、以下のいずれかの操作を行います。

   * **インデント**&#x200B;アイコン![](assets/indent-icon-nwe-33x29.png)をクリックし、選択したタスクを、その直上にあるタスクのサブタスクにします。
   * 標準の英語 QWERTY キーボードを使用する場合は、キーボードの Option + >（Mac）または Alt + >（Windows）を押します。他の言語では、Option +（Mac）または Alt +（Windows）コマンドを使用してインデントすることができます。

     >[!TIP]
     >
     >インライン編集でタスクを編集する際には、キーボードショートカットは機能しません。その場合は、インデントアイコン ![](assets/cs1.png) を使用して、サブタスクを作成します。

   * 親タスクとして指定したいタスクの上に、タスクをドラッグ＆ドロップします。

     >[!NOTE]
     >
     >タスクの一覧がタスク番号で並べられている場合、およびタスクリストにグループが適用されていない場合にのみ、タスクのインデントを設定できます。

### タスクのサブタスクセクションからサブタスクを作成 {#create-subtasks-from-the-task-subtasks-section}

1. サブタスクを作成するプロジェクトに移動します。
1. 左側のパネルで「**タスク**」セクションをクリックします。
1. サブタスクを作成するタスクの名前をクリックします。
1. 左側のパネルで「**サブタスク**」セクションをクリックします。
1. 「**新規タスク**」をクリックします。

   [プロジェクトでのタスクの作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)の記事の手順に従って、サブタスクの作成を続行します。

1. 「**タスクを保存**」をクリックします。

## サブタスクをメインタスクにする

1. サブタスクをメインタスクにするプロジェクトに移動します。
1. 左側のパネルで「**タスク**」セクションをクリックします。
1. メインタスクにしたいサブタスクを選択します。
1. **アウトデント**&#x200B;アイコン ![](assets/outdent-icon-nwe-31x29.png) をクリックし、サブタスクをメインタスクにします。

   または

   標準の英語 QWERTY キーボードで、Option + &lt;（Mac）または Alt + &lt;（Windows）を押します。他の言語では、Option + コマンドが使用される場合があります。（Mac）または Alt +。（Windows）インデントを解除する。

   >[!NOTE]
   >
   >タスクのリストがタスク番号で並べ替えられていて、タスクリストにグループ化が適用されていない場合にのみ、タスクのインデントを解除できます。
