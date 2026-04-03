---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: プロジェクトのクリティカルパスの概要
description: プロジェクトのクリティカルパスの決定は、Adobe Workfront が、プロジェクトのタイムラインに影響を与える可能性のある、プロジェクト内の一連のタスクにフラグ付けする自動的な方法で行われます。プロジェクトのタイムラインに影響を与える可能性のあるタスクは、クリティカルパスタスクとしてフラグ付けされます。
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 49%

---

# プロジェクトのクリティカルパスの概要

<!-- Audited: 5/2025 -->

プロジェクトのクリティカルパスを決定することは、Adobe Adobe Workfrontが、プロジェクトのタイムラインに影響を与える可能性のある、プロジェクトの一連のタスクに自動的にフラグを立てる方法のひとつです。 プロジェクトのタイムラインに影響を与える可能性のあるタスクには、クリティカルパスのタスクとしてフラグが付けられます。

次の機能は、プロジェクトのクリティカルパスに影響を与える可能性があります。

* プロジェクトの作業分割構造。

  詳しくは、[ プロジェクトの作業分割構造の決定](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)を参照してください。

* 各タスクが完了するまでに要する時間（期間）。
* タスク間の依存関係。

  次の点に注意してください。

   * クリティカルパス上のタスクに先行タスクの関係がある場合、先行タスクまたは後続タスクの日付の変更が依存関係に直接影響する場合、その先行タスクと後続タスクもクリティカルパス上にあります。

     >[!TIP]
     >
     >タスクの後継タスクの日付が、依存タスクの日付やプロジェクトの日付に直接影響を与えない場合、後継タスクはクリティカルパスに存在しません。
     >
     >
     >![ クリティカルパス上にSuccessorがありません](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * サブタスクがクリティカルパスタスクとして識別される場合、予測開始日と親タスクの時間がサブタスクの時間と同じ場合、親タスクもクリティカルパスタスクとして識別されます。

これらの機能を考慮し、最も早いタスクとプロジェクトの終了を決定するタスクの間の最長パスを使用して、クリティカルパスが計算されます。クリティカルパスの計算では、プロジェクトを長引かせることなく各タスクを開始および終了できる最も早い時間と最も遅い時間が考慮されます。このプロセスは、どのタスクが「クリティカル」（かつ最も長いパスに属する）か、どのタスクが「合計浮動小数」（プロジェクトを長引かせることなく遅延できる）かを決定します。

クリティカルパスでのタスクのアクティビティの遅延は、プロジェクトの見込み完了日に直接影響します（クリティカルパスに浮動小数はありません）。

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
   <td> 
   <p>標準<p>
   <p>Work またはそれ以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクに対する表示以上のアクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する表示以上の権限 </p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
Old:

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
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on a task </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## クリティカルパスの表示

Workfront アプリケーションの次のエリアで、クリティカルパスに属するタスクを表示できます。

* [ガントチャートでクリティカルパスを表示](#view-the-critical-path-in-the-gantt-chart)
* [タスクリストまたはレポートでクリティカルパスを表示](#view-the-critical-path-in-a-task-list-or-report)

### ガントチャートでクリティカルパスを表示 {#view-the-critical-path-in-the-gantt-chart}

ガントチャートのクリティカルパスにタスクを表示する手順は、次の通りです。

{{step1-to-projects}}

1. プロジェクトリストで、プロジェクトを選択します。

1. 左側のパネルで、**タスク**&#x200B;をクリックします。 「**タスク**」タブが開きます。

1. タスクリストの右上隅にある「**ガントチャート**」アイコンをクリックします。

   ![gantt_chart_icon__1_.png](assets/gantt-icon.png)

1. ガントチャートのセクションの右上隅にある「**オプション**」アイコン「![ オプションアイコン ](assets/options-icon.png)」をクリックし、表示されるドロップダウンで「**クリティカルパス**」オプションを選択します。 クリティカルパス上のタスクでは、タイムラインの上に赤い線が表示されるようになりました。

   ![crtitical_path_on_gant__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### タスクリストまたはレポートでクリティカルパスを表示 {#view-the-critical-path-in-a-task-list-or-report}

タスクのリストのクリティカルパスにあるタスクを表示する手順は、次の通りです。

{{step1-to-projects}}

1. プロジェクトリストで、プロジェクトを選択します。

1. 左側のパネルで、**タスク**&#x200B;をクリックします。 「**タスク**」タブが開きます。

1. **表示** アイコン ![表示アイコン ](assets/view-icon.png)をクリックし、**ステータス**&#x200B;を選択します。 クリティカルパス上のタスクには、リストの&#x200B;**フラグ**&#x200B;列に&#x200B;**クリティカルパス** フラグが表示されます。

   または

   **フィルター** アイコン ![ フィルターアイコン ](assets/filters-icon.png)をクリックし、**以上の新しいフィルター**&#x200B;を選択します。
1. 最初のフィールドに「*重要です*」と入力し、リストの「**タスク**」セクションに表示されたら選択します。

   ![ タスクはクリティカルフィルター](assets/task-is-critical.png)

1. 2番目のドロップダウンメニューで「**Is true**」が選択されていることを確認します。

   ![は真のドロップダウンです](assets/critical-path-filter.png)

1. フィルターパネルを閉じます。 タスクリストには、クリティカルパス上のタスクのみが表示されるようになりました。
