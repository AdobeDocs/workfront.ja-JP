---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: ラグタイプの概要
description: '[ ラグ ] は、依存タスクが開始できるまで、強制的な先行タスクの完了後に経過する必要がある時間（正のラグ）、または依存タスクが先行タスクの開始前に開始できる時間（負のラグ）です。'
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: a2d3032b32d321c0089839dafad6c9b3c5ba153a
workflow-type: tm+mt
source-wordcount: '1519'
ht-degree: 0%

---

# ラグタイプの概要

[ ラグ ] は、先行タスクの計画完了から、依存タスクが開始できるまでの時間（正のラグ）、または依存タスクが先行タスクの開始前に開始できる時間（負のラグ）です。

後続タスクの計画日、予定日、および推定日は、先行タスクの遅延と計画日、予定日、および推定開始日（完了）を考慮して計算されます。

## アクセス要件

<!--drafted - replace table at P&P:

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
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>タスクおよびプロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タスクのラグとラグのタイプを示す

タスクの先行関係を定義する際に、タスクのラグタイプを指定できます。

* [タスクの [ 先行タスク ] セクションにラグの種類を指定する](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [タスクリストのラグの種類を示す](#indicate-lag-types-in-a-task-list)

### タスクの [ 先行タスク ] セクションにラグの種類を指定する {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. 先行タスクとラグの種類を定義するタスクに移動します。
1. クリック **先行タスク** をクリックします。 クリックする必要がある場合があります **表示を増やす**&#x200B;を、 **先行タスク**.
1. クリック **先行タスクを追加**.
1. （オプション）プロジェクト間の先行タスクを追加する場合は、 **親プロジェクト** 別のプロジェクトでの名前。
1. 先行タスクの名前を入力し、一覧に表示されたら選択します。
1. を選択します。 **依存タイプ**.

   先行依存タイプの詳細については、「 [タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. を指定します。 **ラグ** 金額に数値を使用します。 負の値を指定して、負の値のラグを示すことができます。
1. 前任者に示すラグのタイプを識別するには、次のオプションから選択します。

   * **日**
   * **カレンダーの日数**
   * **パーセント**
   * **曜日**
   * **曜日（ゼロ以外）**

     これらのラグの種類とその計算方法の詳細については、「 」の項を参照してください。 [ラグタイプの概要](#lag-types-overview) 」を参照してください。

1. 「**保存**」をクリックします。

### タスクリストのラグの種類を示す  {#indicate-lag-types-in-a-task-list}

1. タスクリストに移動し、 **標準** 表示元： **表示** ドロップダウンメニュー。

1. 内側をクリック **先行タスク** 先行タスクと遅延金額を指定するタスクに対応する列。
1. スペースを含めずに、次のように入力します。

   * 選択したタスクの先行タスクとして指定するタスクの数
   * タスク間で指定する依存関係の種類の省略形

     依存関係タイプの略語の詳細は、 [タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * 次のいずれか **+** 正の遅れまたは **-** マイナスの遅れに対して

   * ラグの量
   * 使用するラグタイプの略語。

     ラグタイプの省略形の詳細については、「 [ラグタイプの概要](#lag-types-overview) 」を参照してください。

   たとえば、タスクに先行タスクと正の遅延が 2 日間あることを示すには、次のように入力します。  `1fs+2d` （「先行タスク」列内）

1. キーボードの Enter キーをクリックして、タスクに対する変更を保存します。

## ラグタイプの概要 {#lag-types-overview}

遅い時間が必要なタスクの例として、木を木に切って木を材木にすることが考えられます。 切りたての木を切る前にしばらく乾かさなければならない場合は、木を切って木を木に切り込む間に時間がかかります。

次の表に、ラグの種類と各タイムの時間を示す方法を示します。

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>値</strong> </p> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>日（d または de）</p> </td> 
   <td> <p>依存関係によってリンクされた 2 つのタスク間の遅延は、稼働日数で測定されます。 これはデフォルトのラグタイプです。 </p> <p>たとえば、2 つの稼働日ラグが設定され、先行タスクが金曜日に終了する場合、依存タスクは水曜日に開始されます。 週末は、ラグの一部としてカウントされません。 </p> <p>注意：日の最大ラグ制限は 366 です。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>カレンダーの日数（c または ce）</p> </td> 
   <td> <p>2 つのタスク間の遅延は、休日や週末を含むカレンダー日で測定されます。 </p> <p>注意：このラグタイプでは非稼働日がラグの一部としてカウントされますが、依存タスクは非稼働日には開始できません。 このラグタイプにより、依存タスクが非稼働日に開始される場合、依存タスクの計画開始日は次の稼働日にスケジュールされます。 </p> <p>たとえば、2 つの暦日ラグを持つ終了日と開始日の依存関係があり、先行タスクが木曜日に終了する場合、依存タスクは日曜日ではなく月曜日に開始されます。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>パーセント（p または pe）</p> </td> 
   <td> <p>遅延は、先行タスクを完了する推定時間のパーセンテージで表されます。 </p> <p>たとえば、10 日間の先行タスクに 20%の遅延がある終了 — 開始依存関係がある場合、先行タスクのタスク期間の 20%を表す日数が計算され、それが遅延として使用されます。 この場合、タスクの完了から 2 日後になります。 </p>

<p><b>メモ</b></p> パーセントの最大ラグ制限は 2000%です。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>曜日（w または we） </p> </td> 
   <td> <p>2 つのタスク間の遅延は、先行タスクの計画完了日を含む週の曜日を示すことで測定されます。</p> <p>このラグタイプでは、各曜日は数値に関連付けられます。</p> 
    <ul> 
     <li>日曜日=1</li> 
     <li>月曜日=2</li> 
     <li>火曜日=3</li> 
     <li>水曜日=4</li> 
     <li>木曜日=5</li> 
     <li>金曜日=6</li> 
     <li>土曜日=7</li> 
    </ul> <p>後続の計画開始日が現在の週の火曜日になり、火曜日が先行の計画完了日より前になることを示す場合は、次の式を使用して後続のコードを作成します。 </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>メモ</b></p>

後続タスクの開始日が特定の火曜日に計算され、その日が現在の週に渡された場合、後続タスクの予定開始日は、可能な場合は次の週の同じ日（火曜日）になります。 </p> <p>ラグが現在の週の土曜日に発生し、土曜日が先行者の計画完了日より後であることを示す場合は、次の式を使用して後続者をコード化します。</p> <p><code>4fs+7w</code> </p> <p>土曜日が非稼働日の場合は、次の日（正の遅れを示す）が後続の計画開始日として選択されます。 </p>

<p>これは、スケジュールの例外には適用されません。 日付もスケジュール例外で、後続の開始日がその日に計算される場合は、前任者の式で指定された曜日である、最も近い使用可能な日付を検索します。</p>

<p>たとえば、開始日が特定の火曜日に計算され、その日がスケジュールの例外で、先行タスクのラグが正の場合、次の火曜日（稼働日も含む）を後続タスクの開始日として選択します。 ラグが負の場合は、前の火曜日が開始日として選択されます。</p>

<p>過去または将来の週を示すには、ラグタイプの日の数の前に数値を追加します。 </p> <p>例えば、10 週間前の月曜日を指定する場合、次のコードを使用して後続のユーザーを指定できます。</p> <p><code>4fs-102w</code> </p> <p>「10」は 10 週間前を表し、「2」は月曜日に割り当てられた番号を表します。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>曜日非ゼロ（k または ke）</p> </td> 
   <td> <p>2 つのタスク間の遅延は、先行タスクの時間が指定した曜日に終了する場合を除き、 Day of the Week lag タイプと同じように測定されます。 次に、ラグタイムが隣接する週 (+/-) に計算されます。 </p> <p>この場合、ラグタイムは 0 にはできません。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ネガティブなラグの概要

負の値のラグを使用して、先行タスクの終了前にタスクを開始する必要性または能力を指定できます。

負のラグを使用する場合は、次のルールを考慮してください。

* 負の遅延は、タスクの開始日/終了日を、プロジェクトの予定開始日/終了日の前または後に強制することはできません。 これらの日付は、プロジェクトの「スケジュールの開始日」フィールドで指定します。

  この場合、次の点に注意してください。

   * プロジェクトを「完了日から」にスケジュールします。
   * プロジェクトの最後のタスクは、[ タスクの終了日 ] の制約を使用する必要があります。 プロジェクト上のすべてのタスクを考慮するために、タスクに十分な期間を割り当てることをお勧めします。 残りのタスクは、 As As Possible 制約と適切に連携します。

* タスクで [ 終了 — 開始 ] 先行タスク関係を使用すると、エラーメッセージが表示される場合があります。

  この場合、次の点に注意してください。

   * タスク間に [ 終了 ] と [ 終了 ] の先行タスク関係を設定します。
   * 後続のタスクの期間は、タスク間の遅延日数の意図した数以上にする必要があります。
