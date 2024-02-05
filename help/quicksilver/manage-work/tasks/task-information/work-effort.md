---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 作業量の概要
description: 作業量の概要
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 74%

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
     <li>「期間タイプ」が「計算割当」または「簡易」のタスクに対してのみ、手動で計画時間を更新できます。 </li> 
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
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在：プラン </p>
   または
   <p>新規：標準 </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベルの設定</td> 
   <td> <p>プロジェクトとタスクへのアクセス権を編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトおよびそのタスクに対する権限を管理する</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 作業量を使用する際の考慮事項

* プロジェクトタスクの予定時間数が 0 で、プロジェクトで「作業量を使用してタスクの予定時間数を自動的に計算」設定を有効にすると、それらに関連付けられた作業量のデフォルトレベルは中になります。単純な期間タイプのタスクでは、計画時間が自動的に更新されます。 詳しくは、  [作業量のレベル](#levels-of-work-effort) 」を参照してください。
* プロジェクトタスクの計画時間が 0 より大きく、[ 作業時間を使用してプロジェクトの計画時間を自動的に計算する ] 設定を有効にした場合、作業時間のレベルは、[ 簡易期間タイプの計画時間 ] タスクの量を変更せずに、計画時間数に応じて更新されます。 詳しくは、 [Workfrontが計画時間に基づいて作業工数を計算する方法](#how-workfront-calculates-work-effort-based-on-planned-hours) 」を参照してください。
* プロジェクトタスクの予定時間数が 0 で、プロジェクトで「作業量を使用してタスクの予定時間数を自動的に計算」設定を有効にすると、作業量のレベルが中から小または大に更新されて、予定時間数も更新されます。詳しくは、この記事の [Workfront が作業量に基づいて予定時間数を計算する方法](#how-workfront-calculates-planned-hours-based-on-work-effort)の節を参照してください。
* タスクを編集し、同時にタスクの「予定時間数」と「作業量」フィールドの両方を変更すると、予定時間数は指定した値で更新されますが、作業量の値は更新された予定時間数に基づいて計算されます。
* タスクの作業量の値を更新すると、期間は予定時間数に基づいて自動計算されなくなります。シンプルな期間タスクを期間が計算する方法について詳しくは、[期間タイプの概要：シンプル](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)を参照してください。
* タスクの「期間の種類」を「シンプル」から「その他」に変更すると、「作業量」フィールドはタスクで非表示になります。 予定時間数は変更されません。
* 親タスクの作業量レベルは更新できません。 親タスクの作業量レベルは、すべての子タスクの積み上げであるタスクの計画時間数に基づいて自動的に計算されます。 親タスクについて詳しくは、[サブタスクを作成](../../../manage-work/tasks/create-tasks/create-subtasks.md)を参照してください。

## 予定時間数ではなく作業量の使用を有効にする

1. プロジェクトに移動し、 **その他** メニュー ![](assets/more-icon.png)を選択し、次に **編集**.
1. 「**タスク設定**」をクリックし、「**作業量を使用してタスクの予定時間数を自動的に計算**」オプションを選択します。デフォルトでは、このオプションは選択されていません。

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   プロジェクトで作業量の使用を有効にする方法について詳しくは、[プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md)の記事の「タスク設定」の節を参照してください。

1. 左側のパネルで「**タスク**」をクリックし、タスクの名前を選択してアクセスします。
1. 次をクリック： **その他** メニュー ![](assets/more-icon.png)を選択し、次に **編集**. タスクにシンプルな期間タイプが含まれていることを確認します。

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

次の表に、作業量のレベルと、対応するデフォルトの割合を示します。プロジェクトマネージャーは、組織のニーズに合わせて割合を更新できます。これは、プロジェクトの編集時に行います。 プロジェクトの編集の詳細については、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

Workfrontの管理者は、「セットアップ」の「プロジェクトの環境設定」領域で、1 日あたりの標準時間を定義します。 これは、作業時間と見なされる 1 日の時間です。Workfront のインスタンスに対するプロジェクト環境設定の構成について詳しくは、[システム全体のプロジェクト環境設定の構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

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
   <td> <p>タスクを完了するための中レベルの労力は、「通常の作業時間」（1 作業日あたりの時間）の 50%に設定されます。 つまり、このレベルの作業量を割り当てたタスクが 1 日で完了するまでに 2 時間以上 6 時間未満かかる必要があります。 <code>(0.50*80=4)</code> </p> <p>メモ：プロジェクトで作業量を使用してタスクの予定時間数の自動計算を行う設定が有効になっている場合、この設定が有効になる前の予定時間が 0 時間のタスクのデフォルト設定です。これにより、タスクの予定時間数が 4 時間に更新されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>大</td> 
   <td>タスクを完了するための大規模な作業レベルは、勤務 1 日あたりの標準的な時間数の 75％に設定されます。つまり、このレベルの作業量を割り当てたタスクは、1 日で完了するのに 6 時間以上かかる必要があります。 <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Workfront が作業量に基づいて予定時間数を計算する方法 {#how-workfront-calculates-planned-hours-based-on-work-effort}

[ 作業時間の使用 ] を有効にしてプロジェクトのタスクの計画時間数を自動的に計算すると、Workfrontは次の数式を使用して、[ 簡易期間の種類 ] のタスクの計画時間数を計算します。

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

例えば、期間が 3 日で、作業量が中程度のタスクの予定時間数は 12 時間です。

```
Planned Hours = 3*4=12
```

ここで、「標準時間（1 稼働日あたり）」の値は 8 時間です。

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

* 「プロジェクトを編集」ボックスの「タスク設定」領域

### タスクの作業量 {#work-effort-for-tasks}

タスクの「作業量」フィールドは、次のエリアにあります。

* タスクの編集ボックスの概要エリア
* 「タスクの詳細」セクションの概要エリア（作業時間エリア内）
* タスクリストまたはレポート
