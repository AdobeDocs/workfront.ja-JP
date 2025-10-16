---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 作業量の概要
description: 作業量の概要
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '1474'
ht-degree: 99%

---

# 作業量の概要

<!--Audited: 01/2024-->

<!--
(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more)
-->

プロジェクトマネージャーは、プロジェクトでのタスクの完了に必要な作業量を見積もる方法を決定できます。次のいずれかのインジケーターを使用して、タスクの完了に必要な作業量を見積もります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">予定時間数</td> 
   <td> <p> タスクに割り当てられたリソースがタスクを完了するのに要する時間数を示す、手動の数値エントリまたは Adobe Workfront の計算値です。 </p> <p>予定時間数に関して次の点を考慮します。 </p> 
    <ul> 
     <li>これはデフォルトのメソッドです。 </li> 
     <li>予定時間数は、期間タイプが「予定割り当て時間」または「シンプル」のタスクに対してのみ更新できます。 </li> 
    </ul> <p>予定時間数について詳しくは、<a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">予定時間数の概要</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">作業量 </td> 
   <td> <p>タスクの完了に 1 日あたりの作業量が小、中、大のどれになるかを定義する手動のラベルです。<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>作業量に関して、次の点を考慮します。</p> 
    <ul> 
     <li>このフィールドは、シンプル期間タイプのタスクでのみ使用できます。 </li> 
     <li>このラベルの使用を有効にして、プロジェクトレベルで関連付けられる作業時間の割合を定義できます。 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

この記事では、作業量とは何か、およびタスクの作業量を見積もる際に、作業量をどのように使用するかについて説明します。

>[!NOTE]
>
>予定時間数と作業量が相互に影響し合います。予定時間数を更新すると作業量が更新され、作業量を更新すると、タスクの予定時間数が更新できます。

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
   <td> <p>標準</p>
   <p>プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトとタスクへのアクセス権を編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトおよびそのタスクに対する権限を管理する</p>  </td> 
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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current: Plan </p>
   Or
   <p>New: Standard </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>Edit access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project and its tasks</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 作業量を使用する際の考慮事項

* プロジェクトタスクの予定時間数が 0 で、プロジェクトで「作業量を使用してタスクの予定時間数を自動的に計算」設定を有効にすると、それらに関連付けられた作業量のデフォルトレベルは中になります。シンプルな期間タイプのタスクでは、予定時間数が自動的に更新されます。詳しくは、この記事の[作業量のレベル](#levels-of-work-effort)の節を参照してください。
* プロジェクトタスクの予定時間数が 0 より大きく、プロジェクトで「作業量を使用してタスクの予定時間数を自動的に計算」設定を有効にすると、シンプルな期間タイプのタスクの予定時間数を変更せずに、予定時間数に応じて作業量のレベルが更新されます。詳しくは、この記事の [Workfront が予定時間に基づいて作業量を計算する方法](#how-workfront-calculates-work-effort-based-on-planned-hours)の節を参照してください。
* プロジェクトタスクの予定時間数が 0 で、プロジェクトで「作業量を使用してタスクの予定時間数を自動的に計算」設定を有効にすると、作業量のレベルが中から小または大に更新されて、予定時間数も更新されます。詳しくは、この記事の [Workfront が作業量に基づいて予定時間数を計算する方法](#how-workfront-calculates-planned-hours-based-on-work-effort)の節を参照してください。
* タスクを編集し、同時にタスクの「予定時間数」と「作業量」フィールドの両方を変更すると、予定時間数は指定した値で更新されますが、作業量の値は更新された予定時間数に基づいて計算されます。
* タスクの作業量の値を更新すると、期間は予定時間数に基づいて自動計算されなくなります。シンプルな期間タスクを期間が計算する方法について詳しくは、[期間タイプの概要：シンプル](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)を参照してください。
* タスクの期間タイプをシンプルから他のタイプに変更すると、タスクの「作業量」フィールドが非表示になります。予定時間数は変更されません。
* 親タスクの作業量レベルは更新できません。親タスクの作業量レベルは、すべての子タスクの合計であるタスクの予定時間数に基づいて自動的に計算されます。親タスクについて詳しくは、[サブタスクを作成](../../../manage-work/tasks/create-tasks/create-subtasks.md)を参照してください。

## 予定時間数ではなく作業量の使用を有効にする

1. プロジェクトに移動し、**その他**&#x200B;メニュー ![](assets/more-icon.png) をクリックして、「**編集**」をクリックします。
1. 「**タスク設定**」をクリックし、「**作業量を使用してタスクの予定時間数を自動的に計算**」オプションを選択します。デフォルトでは、このオプションは選択されていません。

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   プロジェクトで作業量の使用を有効にする方法について詳しくは、[プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md)の記事の「タスク設定」の節を参照してください。

1. 左側のパネルで「**タスク**」をクリックし、タスクの名前を選択してアクセスします。
1. **その他**&#x200B;メニュー ![](assets/more-icon.png) をクリックして、「**編集**」をクリックします。タスクにシンプルな期間タイプが含まれていることを確認します。

   >[!TIP]
   >
   >タスクの作業量は、「タスクの詳細」セクションでも更新できます。

1. **概要**&#x200B;エリアで、「作業量」ドロップダウンメニューをクリックして、タスクを完了するのに必要な作業量を修正します。

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   タスクの「作業量」フィールドを更新する方法について詳しくは、次の記事を参照してください。

   * [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)記事の「概要」セクション
   * [タスクの詳細の概要エリアでタスク情報を管理](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## 作業量のレベル {#levels-of-work-effort}

プロジェクトマネージャーは、プロジェクトに対して 3 つのレベルの作業量を指定できます。各作業レベルは、ユーザーがタスクを完了するのに必要な 1 日の時間の割合を表します。

作業量のレベルを設定する際には、「このタスクに割り当てられたユーザーが時間内に完了するために 1 日に費やすべき時間はどれくらいか」という質問を自分に問いかける必要があります。

次の表に、作業量のレベルと、対応するデフォルトの割合を示します。プロジェクトマネージャーは、組織のニーズに合わせて割合を更新できます。これは、プロジェクトの編集時に行います。プロジェクトの編集の詳細については、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

Workfront 管理者は、設定のプロジェクト環境設定エリアで「稼働日の標準的な時間数」を定義します。これは、作業時間と見なされる 1 日の時間です。Workfront のインスタンスに対するプロジェクト環境設定の構成について詳しくは、[システム全体のプロジェクト環境設定の構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

>[!NOTE]
>
>以下の例では、Workfront 管理者が勤務 1 日あたりの標準的な時間数の値を 8 時間に設定していると仮定します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>作業量のレベル</td> 
   <td>割合（％）の値</td> 
  </tr> 
  <tr> 
   <td>小 </td> 
   <td>タスクを完了するための小規模な作業レベルは、勤務 1 日あたりの標準的な時間数の 25％に設定されます。つまり、このレベルの作業量を割り当てたタスクは、1 日で完了するのに最大 2 時間かかる必要があります。 <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>中</td> 
   <td> <p>タスクを完了するための中レベルの作業量は、稼働日の標準的な時間数の 50％に設定されます。これは、このレベルの作業量が割り当てられたタスクが 1 日で完了するのにかかる時間は 2 時間以上 6 時間未満であることを意味します。<code>(0.50*80=4)</code> </p> <p>メモ：プロジェクトで作業量を使用してタスクの予定時間数の自動計算を行う設定が有効になっている場合、この設定が有効になる前の予定時間が 0 時間のタスクのデフォルト設定です。これにより、タスクの予定時間数が 4 時間に更新されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>大</td> 
   <td>タスクを完了するための大規模な作業レベルは、勤務 1 日あたりの標準的な時間数の 75％に設定されます。これは、このレベルの作業量が割り当てられたタスクが 1 日で完了するには 6 時間以上かかることを意味します。 <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Workfront が作業量に基づいて予定時間数を計算する方法 {#how-workfront-calculates-planned-hours-based-on-work-effort}

プロジェクトで「作業量を使用してタスクの予定時間数を自動的に計算」する設定を有効にすると、Workfront は次の式を使用してシンプルな期間タイプのタスクの予定時間数を計算します。

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

例えば、期間が 3 日で、作業量が中程度のタスクの予定時間数は 12 時間です。

```
Planned Hours = 3*4=12
```

ここで、稼働日の標準的な時間数の値は 8 時間です。

>[!TIP]
>
>タスクを複数のリソースに割り当てると、タスクの期間の 1 日ごとに、各リソースに対して予定時間が均等に配分されます。

## Workfront が予定時間に基づいて作業量を計算する方法 {#how-workfront-calculates-work-effort-based-on-planned-hours}

作業量の使用を有効にして、プロジェクトのタスクの予定時間数の設定を自動的に計算し、既にタスクの予定時間数を持つか、タスクの予定時間数を編集する場合、Workfront は作業量の値を更新します。

Workfront では、次の式を使用して、予定時間数に従って作業量のレベルを更新します。

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

例えば、期間が 2 日のタスクがあり、予定時間数を 8 時間から 20 時間に更新すると、タスクの作業量は中から大に更新されます。

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## タスクとプロジェクトの作業量の検索

* [プロジェクトの作業量](#work-effort-for-projects)
* [タスクの作業量](#work-effort-for-tasks)

### プロジェクトの作業量 {#work-effort-for-projects}

プロジェクトの「作業量」セクションは、次のエリアにあります。

* プロジェクトの編集ボックスのタスク設定エリア

### タスクの作業量 {#work-effort-for-tasks}

タスクの「作業量」フィールドは、次のエリアにあります。

* タスクの編集ボックスの概要エリア
* 「タスクの詳細」セクションの概要エリア（作業時間エリア内）
* タスクリストまたはレポート
