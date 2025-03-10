---
product-area: projects
navigation-topic: create-tasks
title: サブタスクの作成
description: Adobe Workfrontでは、タスクに親子関係を設定できます。 子タスクはサブタスクと呼ばれます。メインタスクをサブタスクにすることで、タスクリストにサブタスクを作成できます。サブタスクをメインタスクにすることもできます。
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 82%

---

# サブタスクを作成

<!-- Audited: 01/2025 -->

Adobe Workfrontでは、タスクに親子関係を設定できます。 子タスクはサブタスクと呼ばれます。メインタスクをサブタスクにすることで、タスクリストにサブタスクを作成できます。サブタスクをメインタスクにすることもできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>新規：標準</p>
   <p>現在：ワーク以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクの追加以上の機能を備えたプロジェクトおよび親タスクに、参加権限を付与</p> <p>タスクを作成すると、タスクに対する管理権限が自動的に付与されます。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## サブタスクを作成

タスクリストまたはタスクの「サブタスク」セクションからサブタスクを作成できます。

### タスクリストからサブタスクを作成 {#create-subtasks-from-the-task-list}

1. サブタスクを作成するプロジェクトに移動します。
1. 左パネルの「**タスク**」セクションをクリックします。
1. （条件付き）子タスクにするタスクが、親にするタスクの直下にまだ存在しない場合は、タスクリスト内の適切な場所にドラッグ&amp;ドロップします。
1. サブタスクにするタスクを選択し、以下のいずれかの操作を行います。

   * **インデント**&#x200B;アイコン![](assets/indent-icon-nwe-33x29.png)をクリックし、選択したタスクを、その直上にあるタスクのサブタスクにします。
   * 標準の英語 QWERTY キーボードを使用する場合は、キーボードの Option + >（Mac）または Alt + >（Windows）を押します。他の言語では、Option +（Mac）または Alt +（Windows）コマンドを使用してインデントすることができます。

     >[!TIP]
     >
     >インライン編集でタスクを編集する際には、キーボードショートカットは機能しません。その場合は、インデントアイコン ![](assets/indent-icon-nwe-33x29.png) を使用して、サブタスクを作成します。

   * 親タスクとして指定したいタスクの上に、タスクをドラッグ＆ドロップします。

     >[!NOTE]
     >
     >タスクの一覧がタスク番号で並べられている場合、およびタスクリストにグループが適用されていない場合にのみ、タスクのインデントを設定できます。

### タスクのサブタスクセクションからサブタスクを作成 {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>Workfrontまたはグループ管理者が、レイアウトテンプレートを使用して、環境内の「サブタスク」セクションを削除している可能性があります。

1. サブタスクを作成するプロジェクトに移動します。
1. 左側のパネルで「**タスク**」セクションをクリックします。
1. サブタスクを作成するタスクの名前をクリックします。
1. 左側のパネルで「**サブタスク**」セクションをクリックします（存在する場合）。
1. 「**新規タスク**」をクリックします。

   [プロジェクトでのタスクの作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)の記事の手順に従って、サブタスクの作成を続行します。

1. **タスクを作成** をクリックします。

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
