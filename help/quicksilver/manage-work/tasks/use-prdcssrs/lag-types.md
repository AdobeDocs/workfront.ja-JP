---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: ラグタイプの概要
description: ラグとは、強制的な先行タスクの完了後、依存タスクの開始までに経過する必要がある時間（正のラグ）、または先行タスクの開始前に依存タスクを開始できる時間（負のラグ）のことです。
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: bec625b70b39fec9f9a6d4f7b48023702de43675
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 78%

---

# ラグタイプの概要

<!-- Audited: 01/2024 -->

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクおよびプロジェクトに対する権限の管理</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## タスクのラグとラグタイプを指定

タスクと先行タスクの関係を定義する際に、タスクのラグタイプを指定できます。

### タスクの「先行タスク」セクションにラグタイプを指定 {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. 先行タスクとラグタイプを定義するタスクに移動します。
1. 左側のパネルで「**先行タスク**」をクリックします。「**さらに表示**」、「**先行タスク**」の順にクリックする場合もあります。
1. 「**先行タスクの追加**」をクリックします。
1. （オプション）プロジェクト間先行タスクを追加する場合は、**親プロジェクト**&#x200B;の名前を別のプロジェクトの名前に置き換えます。
1. 先行タスクの名前を入力し、一覧に表示されたら選択します。
1. 「**依存関係タイプ**」を選択します。

   先行タスクの依存関係タイプについて詳しくは、[タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)を参照してください。

1. **ラグ**&#x200B;の日数を数値でを指定します。負の値を指定すれば、負の値のラグを示すことができます。
1. 次のオプションから、先行タスクに指定するラグのタイプ選択します。

   * **日数**
   * **カレンダーの日数**
   * **パーセント**
   * **曜日**
   * **曜日（ゼロ以外）**

     これらのラグの種類とその計算方法の詳細については、「 」の項を参照してください。 [ラグのタイプ](#lag-types) 」を参照してください。

1. 「**保存**」をクリックします。

### タスクリストでラグタイプを指定  {#indicate-lag-types-in-a-task-list}

1. タスクリストに移動し、 **標準** 表示。

1. 先行タスクとラグの量を指定するタスクに対応した「**先行タスク**」列内をクリックします。
1. スペースを含めずに、次のように入力します。

   * 選択したタスクの先行タスクとして指定するタスクの数
   * タスク間の依存関係タイプを示す略語

     依存関係タイプの略語について詳しくは、[タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)を参照してください。

   * 正のラグには **+**、負のラグには **-**

   * ラグの量
   * 使用するラグタイプの略語

     ラグタイプの省略形の詳細については、「 [ラグのタイプ](#lag-types) 」を参照してください。

   たとえば、タスクに先行タスクと正の遅延が 2 日間あることを示すには、次のように入力します。 `1fs+2d` （「先行タスク」列内）

1. キーボードの Enter キーを押して、タスクに対する変更を保存します。

## ラグのタイプ {#lag-types}

タスクに遅延時間が必要なことは、木を製材するすることに例えられます。伐採したばかりの木を製材する前にしばらく乾かさなければならない場合は、木を切ってから材木にするまで遅延時間が生じます。

次の表に、ラグタイプと各タイプの量を示す方法を示します。

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
   <td> <p>依存関係によってリンクされた 2 つのタスク間の遅延は、稼働日数で測定されます。これはデフォルトのラグタイプです。 </p> <p>例えば、稼働日数が 2 日のラグを伴う終了 - 開始依存関係がある場合、先行タスクが金曜日に終了すると、依存タスクは水曜日に開始されます。週末は、ラグの一部としてカウントされません。 </p> <p>メモ：ラグの日数の上限は 366 です。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>カレンダーの日数（c または ce）</p> </td> 
   <td> <p>2 つのタスク間の遅延は、休日や週末を含むカレンダーの日数で測定されます。 </p> <p>メモ：このラグタイプでは非稼働日がラグの一部としてカウントされますが、依存タスクは非稼働日には開始できません。このラグタイプにより、依存タスクが非稼働日に開始される場合、依存タスクの予定開始日は次の稼働日にスケジュールされます。 </p> <p>例えば、カレンダーの日数が 2 日のラグを伴う終了 - 開始依存関係がある場合、先行タスクが木曜日に終了すると、依存タスクは日曜日ではなく月曜日に開始されます。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>パーセント（p または pe）</p> </td> 
   <td> <p>遅延は、先行タスクを完了するための推定時間のパーセンテージで表されます。 </p> <p>たとえば、10 日間の先行タスクに 20%の遅延がある終了 — 開始依存関係がある場合、前任者のタスク期間の 20%を表す日数が計算され、それが遅延として使用されます。 この場合は、タスクの完了から 2 日後になります。 </p>

<p><b>メモ</b></p> パーセントの場合、ラグの上限は 2000％です。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>曜日（w または we） </p> </td> 
   <td> <p>2 つのタスク間の遅延は、先行タスクの予定完了日が含まれる週の曜日を示すことで測定されます。</p> <p>このラグタイプの場合、各曜日は次のように数値に関連付けられます。</p> 
    <ul> 
     <li>日曜日 = 1</li> 
     <li>月曜日 = 2</li> 
     <li>火曜日 = 3</li> 
     <li>水曜日 = 4</li> 
     <li>木曜日 = 5</li> 
     <li>金曜日 = 6</li> 
     <li>土曜日 = 7</li> 
    </ul> <p>後続タスクの予定開始日が今週の火曜日に当たり、火曜日が先行タスクの予定完了日より前であることを示す場合は、次の式を使用して後続タスクをコード化します。 </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>メモ</b></p>

後続タスクの開始日が特定の火曜日に計算され、その日が現在の週に渡された場合、後続タスクの予定開始日は、可能な場合は次の週の同じ日（火曜日）になります。 </p> <p>ラグが現在の今週の土曜日に当たり、土曜日が先行タスクの予定完了日より後であることを示す場合は、次の式を使用して後続タスクをコード化します。</p> <p><code>4fs+7w</code> </p> <p>土曜日が非稼働日の場合は、その次の稼動日（正のラグを示す）が後続タスクの予定開始日として選択されます。 </p>

<p>これは、スケジュール例外には適用されません。ある日付がスケジュール例外で、後続タスクの開始日の計算結果がその日になる場合、システムは、先行タスクの式で指定された曜日に当たる最も近い稼働日を検索します。</p>

<p>例えば、開始日の計算結果が特定の火曜日になり、その日がスケジュール例外で、先行タスクのラグが正の場合、その次の火曜日（その日が稼働日の場合）が後続タスクの開始日として選択されます。ラグが負の場合は、その前の火曜日が開始日として選択されます。</p>

<p>過去または将来の週を示すには、ラグタイプの曜日番号の前に数値を付け加えます。 </p> <p>例えば、10 週間前の月曜日を指定する場合、次のコードを使用して後続タスクの先行タスクを示すことができます。</p> <p><code>4fs-102w</code> </p> <p>10 は 10 週間前を表し、2 は月曜日に割り当てられた数字です。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>曜日非ゼロ（k または ke）</p> </td> 
   <td> <p>2 つのタスク間の遅延は、先行タスクの時間が指定された同じ曜日に終了する場合を除き、曜日ラグタイプと同じように測定されます。その場合、ラグタイムは隣接する週（+/-）まで計算されます。 </p> <p>この場合、ラグタイムは 0 にはできません。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 負のラグ

負のラグを使用して、先行タスクの終了前にタスクを開始する必要性、または開始できることを指定できます。

負のラグを使用する場合は、次のルールを考慮してください。

* 負の遅延は、タスクの開始日/終了日を、プロジェクトの予定開始日/終了日の前または後に強制することはできません。 これらの日付は、プロジェクトの「スケジュールの基点」フィールドで指定します。

  この場合、次の点を考慮してください。

   * プロジェクトを完了日からスケジューリングします。
   * プロジェクトの最後のタスクでは、タスクの制約の必須終了日を使用する必要があります。プロジェクト上のすべてのタスクを考慮し、タスクに十分な期間を割り当てることをお勧めします。残りのタスクは、「できるだけ早く」の制約を使うと適切に機能します。

* タスクに対して「終了 - 開始」先行タスク関係を使用すると、エラーメッセージが表示される場合があります。

  この場合、次の点を考慮してください。

   * タスク間に「終了 - 終了」先行タスク関係を設定します。
   * 後続タスクの期間は、タスク間のラグ日数以上でなければなりません。
