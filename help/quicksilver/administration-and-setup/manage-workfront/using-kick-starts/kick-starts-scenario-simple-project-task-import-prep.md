---
user-type: administrator
product-area: system-administration;projects
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: キック開始シナリオ — シンプルなプロジェクトとタスクのインポートの準備
description: Kick Start メソッドを使用して、基本的なプロジェクトとタスクの読み込みに使用できる設定とコントロールについて詳しく説明します。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c095ce9d-b189-449b-bd13-2633837697ed
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 9%

---

# キック開始シナリオ：シンプルなプロジェクトとタスクのインポートの準備

Kick Start メソッドを使用して、基本的なプロジェクトとタスクの読み込みに使用できる設定とコントロールについて詳しく説明します。

## シナリオ

実装チームは、アクティブなプロジェクトのプロジェクトとタスクの情報を、システムに手動で入力するのではなく、読み込む方が望ましいです。

* [プロジェクト](#projects)
* [タスクリスト](#task-list)

### プロジェクト {#projects}

次の表に、4 つのプロジェクトと、Kick Start ファイル形式にマッピングする必要がある基本的な詳細を示します。

このシナリオでは、ユーザーが既にAdobe Workfrontに読み込まれていることを前提としています。 ユーザーがまだWorkfrontにいない場合は、別の名前を使用するか、このシナリオより前にユーザーと共に「キック開始シナリオ」を完了します。

1. Workfrontを実装します。

   | 予定開始日 | 今日 |
   |---|---|
   | プロジェクト マネージャ | ジェニファーキャンベル |
   | プロジェクト スポンサー | マーク・ルイス |
   | グループ | マーケティング |
   | 会社 | *会社* |

   {style=&quot;table-layout:auto&quot;}

1. HR システムを実装します。

   | 予定開始日 | 20XX 年 7 月 14 日 |
   |---|---|
   | プロジェクト マネージャ | パムレイノルズ |
   | プロジェクト スポンサー | マーク・ルイス |
   | グループ | マーケティング |
   | 会社 | *会社* |

   {style=&quot;table-layout:auto&quot;}

1. ドキュメント管理システムを実装します。

   | 予定開始日 | 20XX 年 8 月 23 日 |
   |---|---|
   | プロジェクト マネージャ | ジェニファーキャンベル |
   | プロジェクト スポンサー | Ray Andrews |
   | グループ | IT |
   | 会社 | *会社* |

   {style=&quot;table-layout:auto&quot;}

1. 新しいカレンダーシステムを実装します。

   | 予定開始日 | 20XX 年 9 月 7 日 |
   |---|---|
   | プロジェクト マネージャ | パムレイノルズ |
   | プロジェクト スポンサー | Ray Andrews |
   | グループ | IT |
   | 会社 | *会社* |

   {style=&quot;table-layout:auto&quot;}

### タスクリスト {#task-list}

次のタスクリストは、プロジェクトの非常に簡略化されたタスクリストを表示します。 プロジェクト間の唯一の違いは、各プロジェクトで行われる開始日と進捗です。

親タスクは、子タスクの期間、作業時間、および完了率を継承します。 サマリータスクになるために、これらの値を設定する必要はありません。

>[!NOTE]
>
>このシナリオで示す手順は、 [キック開始シナリオ：会社、グループ、役割、およびユーザーのキックスタートの準備](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-company-group-role-user-prep.md). この前提は、会社およびグループのシートから値を検索してコピーする方法を既に学習していることです。そのため、これらの手順については説明しますが、具体的には概要は説明しません。

1. 設定.
1. ユーザーをインポートします。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">割り当て先</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">親タスク</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>1 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業</td> 
      <td>1 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>ドキュメント：100%</p> <p>カレンダー：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 権限を設定します。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">割り当て先</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">親タスク</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">先行</td> 
      <td>2</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>1 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業</td> 
      <td>1 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>ドキュメント：100%</p> <p>カレンダー：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. グループを作成します。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">割り当て先</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">親タスク</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">先行</td> 
      <td>4</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>2 日間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業</td> 
      <td>4 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>ドキュメント：100%</p> <p>カレンダー：25%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. トレーニングを準備します。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">割り当て先</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>2 日間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業</td> 
      <td>4 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>ドキュメント：50%</p> <p>カレンダー：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 継続的なサポートポリシーを構築します。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">割り当て先</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>2 日間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業</td> 
      <td>4 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront:0%</p> <p>HR:100%</p> <p>ドキュメント：50%</p> <p>カレンダー：0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. ロールアウト。

   | 先行 | 1, 6, 7 |
   |---|---|

   {style=&quot;table-layout:auto&quot;}

1. ユーザーをトレーニングします。

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">割り当て先</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">親タスク</td> 
      <td>8</td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td>1 日</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業</td> 
      <td>2 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront:0%</p> <p>HR:0%</p> <p>ドキュメント：0%</p> <p>カレンダー：0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

## テンプレートをダウンロード

「キック開始」ページに移動します。 会社、グループ、プロジェクト、タスク、およびユーザーの各オブジェクトを選択します。 「既存のデータを含める」チェックボックスをオンにします（会社 ID、グループ ID、ユーザー ID をすばやく参照するには、このチェックボックスをオンにします）。 「ダウンロード」ボタンをクリックします。

## 入力プロジェクトの詳細

先ほどダウンロードしたWorkfront.xlsx ファイルを開きます。 「PROJ プロジェクト」シートに移動します。

![](assets/im2-350x14.png)\
Workfrontで既にプロジェクトを作成している場合を除き、空にする必要があります。\
![](assets/im3-350x37.png)

>[!NOTE]
>
>スプレッドシートの [ ペインをフリーズ ] ツールを使用するか、不要な列を非表示にしたり、削除したりして、シートを使いやすくします。 ただし、後で使用する必要のある列や列を削除しないように注意してください。

![](assets/im10-350x42.png)

次のプロジェクトフィールドの値を設定します。

* **isNew 列を設定**
isNew 列の行 3 ～ 6 に TRUE を入力します。
* **一意の ID を設定**
ID 列の各行に一意の ID を入力します。通常、新しいレコードを作成する際には、1 から始まる整数が適切に機能します。
* **プロジェクト名を設定**
各プロジェクトの名前を setName 列に入力します。
* **プロジェクトスケジュールを設定**

   プロジェクトで使用するスケジュールの ID を setScheduleID フィールドに入力します

* **プロジェクトの計画開始日を設定**

   setPlannedStartDate 列に、プロジェクトを開始する日時と日時を入力します。 空のままにした場合、Workfrontは、現在の日付と、その日の午前 0 時のタイムスタンプを持つプロジェクトを、ブラウザーのタイムゾーンに従って読み込みます。

* **タスク番号の設定**
setTaskNumber 列に値を入力して、プロジェクト計画でのタスクの表示順序を制御します。
* **プロジェクトの日付を指定します。**
各プロジェクトの計画開始日を setPlannedStartDate 列に入力します。
* **他の必要な詳細を設定します。**
必要に応じて、説明や現在のステータスなど、その他の詳細を入力します。 GROUP Group シートで各プロジェクトのグループ ID を検索し、各プロジェクトの setGroupID 列に入力します。 CMPY Company シートでプロジェクトの会社 ID を検索し、setCompanyID 列に入力します。 「ユーザー」シートで各プロジェクト所有者のユーザー ID を検索し、setOwnerID 列に入力します。 USER User シートで各プロジェクトスポンサーのユーザー ID を検索し、setSponsorID 列に入力します。

![](assets/im9-350x24.png)

>[!NOTE]
>
>「ステータス」フィールドと「優先度」フィールドに指定できる値は、Workfrontの「ワークフロー設定」領域で各オブジェクトのステータスと優先度の環境設定を確認することで確認できます。

## 入力タスクの詳細

キックスタートを使用してプロジェクトを読み込む際に、プロジェクトのタスクに関する情報を追加できます。

先ほどダウンロードしたWorkfront.xlsx ファイルを開きます。 **[ タスク ] シートに移動します。**

Workfrontで既にタスクを作成している場合を除き、このシートは空にする必要があります。

![](assets/im8-350x14.png)

![](assets/im7-350x43.png)

![](assets/im6-350x16.png)

タスクをマッピングする最も簡単な方法は、一度に 1 つのプロジェクトです（特に、各プロジェクトでタスクが同じ場合）。 その後、最初のプロジェクトのタスクプランをコピーし、後続のプロジェクトのタスクプランを少し調整できます。 残りの手順では、Workfrontプロジェクトのみのタスクを作成することを前提としています。 シナリオに従って、1 つのプロジェクトにつき 9 つのタスクをインポートするので、isNew 列の行 3 ～ 11 に TRUE を入力します。

次のタスクフィールドの値を設定します。

* **ID の設定**
ID 列の各行に一意の ID を入力します。
* **名前を設定**
setName 列にタスク名を入力します。
* **プロジェクト ID を確認**
Workfrontプロジェクトの実装用に設定した ID を入力します。「 PROJ Project 」シートを確認し、PROJ が正しい ID であることを確認します。
* **ユーザーの設定**
[ ユーザー ] シートに移動して、各タスクに割り当てられたユーザーの ID を検索し、 setAssignedToID 列の各セルにこれらの値を入力します。
* **タスクの関係の特定**
タスク 2 ～ 5 について、 setParentID 列に 1 を入力します。 タスク 9 の場合、setParentID 列に 8 を入力します。 setPredecessorString 列に、各先行タスクのタスク番号を入力します。 タスクに複数の先行タスクがある場合（このシナリオのタスク 8 など）、各先行タスク ID を区切るにはコンマを使用する必要があります。 先行タスクは、「先行タスクの作成」の記事の短縮形を使用して、非終了 — 開始関係のラグを使用して定義できます。
* **期間を設定**
各タスクの期間を設定するには、 setDuration フィールドにタスクの時間数、日数、週数、月数を入力します。 次に、 setDurationUnit フィールドに期間の単位を入力します。

   |  | 許容値 |
   |---|---|
   | 分 | 月 |
   | 時間 | H |
   | 日 | 削 |
   | 週 | 水 |
   | 月 | 火 |

   分は、1 時間の分数として表すこともできます（例：分= 5 時間）

* 各タスクの作業量を、「 setWorkRequired 」フィールドで設定します。 次に、 setWorkUnit フィールドに作業単位を入力します。 作業に必要な値がデュレーションと異なる場合は、 setDurationType フィールドに A を入力する必要もあります。

   | 期間タイプ | 許容値 |
   |---|---|
   | 算出した割り当て | ア |
   | 算出した作業 | 水 |
   | 作業優先 | 削 |
   | シンプル | 選択 |

* 各タスクの setPercentComplete フィールドに、完了率の整数表現を入力します。 この値にパーセント記号 (%) を含めないでください。
* 必要に応じて、作成する各タスクの説明とその他の詳細を含めます。

   ![](assets/im5-350x35.png)

* setPlannedStartDate 列と setTaskConstraint 列は、先行関係に依存しているので、このプロジェクトのタイムラインの構築には使用されません。 代わりに、各タスクに日付を入力できます。 その場合は、 setTaskConstraint 列に有効なタスク制約も指定してください。 このフィールドの有効な値の詳細については、タスク制約と関連記事を確認してください。

   このシナリオの場合、インポートする他のプロジェクトのタスクを構築する最も簡単な方法は、定義したタスクをコピーし、12 行目から下に貼り付けることです。 その後、以下をおこないます。

   1. ID 列の値の番号を変更します。
   1. setProjectID 列を、次のプロジェクトに設定した値に更新します。
   1. このプロジェクトのタスクに割り当てられた新しい ID を反映するように、setParentID 値と setPredecoderString 値を更新します。
   1. タスクの割り当てと完了率を更新します。
   1. 次のプロジェクトのタスクに対して、これらの手順を繰り返します。

* **Excel ファイルをインポート**

   次に示す指示に従います。 [キックスタートテンプレートを使用してAdobe Workfrontにデータを読み込む](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
