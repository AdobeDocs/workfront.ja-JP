---
user-type: administrator
product-area: system-administration;projects
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: キックスタートシナリオ：シンプルなプロジェクトとタスクのインポートの準備
description: キックスタートのメソッドを使用して、基本的なプロジェクトとタスクの読み込みに使用できる設定とコントロールについて詳しく説明します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c095ce9d-b189-449b-bd13-2633837697ed
TQID: https://experienceleague.adobe.com/--8-vO2RCBBbSZ2gfFl5RurpGviyK7sW6NauyoHKFhE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1402
ht-degree: 79%

---

# キックスタートのシナリオ：シンプルなプロジェクトおよびタスクの読み込みの準備

キックスタート方式を使用した基本的なプロジェクトとタスクの読み込みで使用できる設定とコントロールについて詳しく説明します。

## シナリオ

実装チームは、これらのデータをシステムに手動で入力するのではなく、アクティブなプロジェクトのプロジェクト情報とタスク情報をインポートします。

* [プロジェクト](#projects)
* [タスクリスト](#task-list)

### プロジェクト {#projects}

次の表には、4 つのプロジェクトおよびキックスタートのファイル形式にマッピングする必要がある基本的な詳細が表示されています。

このシナリオでは、ユーザーが既に Adobe Workfront に読み込まれていることを前提とします。 ユーザーがまだ Workfront に存在しない場合は、別の名前を使用するか、このシナリオより前にユーザーと共にキックスタートのシナリオを完了します。

1. Workfront を実装します。

   | 予定開始日 | 今日 |
   |---|---|
   | プロジェクトマネージャー | Jennifer Campbell |
   | プロジェクトスポンサー | Marc Lewis |
   | グループ | マーケティング |
   | 会社 | *YourCompany* |

   {style="table-layout:auto"}

1. HR システムを実装します。

   | 予定開始日 | 20XX年7月14日 |
   |---|---|
   | プロジェクトマネージャー | Pam Reynolds |
   | プロジェクトスポンサー | Marc Lewis |
   | グループ | マーケティング |
   | 会社 | *YourCompany* |

   {style="table-layout:auto"}

1. ドキュメント管理システムを実装します。

   | 予定開始日 | 20XX年8月23日 |
   |---|---|
   | プロジェクトマネージャー | Jennifer Campbell |
   | プロジェクトスポンサー | Ray Andrews |
   | グループ | IT |
   | 会社 | *YourCompany* |

   {style="table-layout:auto"}

1. 新しいカレンダーシステムを実装します。

   | 予定開始日 | 20XX年9月6日 |
   |---|---|
   | プロジェクトマネージャー | Pam Reynolds |
   | プロジェクトスポンサー | Ray Andrews |
   | グループ | IT |
   | 会社 | *YourCompany* |

   {style="table-layout:auto"}

### タスクリスト {#task-list}

次のタスクリストは、プロジェクトの非常に簡略化されたタスクリストを表示します。 プロジェクト間の唯一の違いは、各プロジェクトの開始日と進行状況です。

親タスクは、子タスクの期間、作業内容および完了率を継承します。 サマリータスクになるために、これらの値を設定する必要はありません。

>[!NOTE]
>
>このシナリオで示す手順は、[キックスタートのシナリオ：会社、グループ、役割およびユーザーのキックスタートの準備](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-company-group-role-user-prep.md)で提供される手順ほど明確ではありません。 会社シートおよびグループのシートから値を検索してコピーする方法を既に学習していることを前提としているため、これらの手順については説明しますが、具体的には説明しません。

1. 設定を行います。
1. ユーザーを読み込みます。

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
      <td role="rowheader">ワーク</td> 
      <td>1 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront：0%</p> <p>時間：0%</p> <p>ドキュメント：100%</p> <p>カレンダー：100%</p> </td> 
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
      <td role="rowheader">ワーク</td> 
      <td>1 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront：0%</p> <p>時間：0%</p> <p>ドキュメント：100%</p> <p>カレンダー：100%</p> </td> 
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
      <td role="rowheader">ワーク</td> 
      <td>4 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront：0%</p> <p>時間：0%</p> <p>ドキュメント：100%</p> <p>カレンダー：25%</p> </td> 
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
      <td role="rowheader">ワーク</td> 
      <td>4 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront：0%</p> <p>時間：0%</p> <p>ドキュメント：50%</p> <p>カレンダー：100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 継続的なサポートポリシーを作成します。

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
      <td role="rowheader">ワーク</td> 
      <td>4 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront：0%</p> <p>時間：0%</p> <p>ドキュメント：50%</p> <p>カレンダー：0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. ロールアウトします。

   | 先行 | 1、6、7 |
   |---|---|

   {style="table-layout:auto"}

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
      <td role="rowheader">ワーク</td> 
      <td>2 時間</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>Workfront：0%</p> <p>HR：0%</p> <p>ドキュメント：0%</p> <p>カレンダー：0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

## テンプレートのダウンロード

キックスタートのページに移動します。 会社、グループ、プロジェクト、タスク、ユーザーの各オブジェクトを選択します。 「既存のデータを含める」チェックボックスを選択します（これにより、会社 ID、グループ ID、ユーザー ID を素早く参照します）。 「ダウンロード」ボタンをクリックします。

## プロジェクト詳細の入力

ダウンロードした Workfront.xlsx ファイルを開きます。 「PROJ」プロジェクトシートに移動します。

![PROJ プロジェクトセット](assets/im2.png)
Workfrontでプロジェクトを作成済みでない限り、空にする必要があります。

![空のプロジェクトシート ](assets/im10.png)

次のプロジェクトフィールドの値を設定します。

* **IsNew列を設定**
isNew列の3 ～ 6行にTRUEを入力します。
* **一意のIDを設定**
ID列の各行に一意のIDを入力します。通常、1から始まる整数は、新しいレコードを作成するときに適切に機能します。
* **プロジェクト名を設定**
setName列に各プロジェクトの名前を入力します。
* **プロジェクトスケジュールの設定**

  setScheduleID フィールドにプロジェクトで使用するスケジュールの ID を 入力します。

* **プロジェクトの予定開始日の設定**

  setPlannedStartDate 列の日時に、プロジェクトを開始する日時を入力します。 空のままにすると、Workfrontは、ブラウザーのタイムゾーンに従って、現在の日付とその日の午前 0 時のタイムスタンプを使用してプロジェクトを読み込みます。

* **タスク番号の設定**
setTaskNumber列に値を入力して、タスクがプロジェクト計画に表示される順序を制御します。
* **プロジェクトの日付を指定します。**
setPlannedStartDate列に、各プロジェクトの予定開始日を入力します。
* **その他の必要な詳細を設定します。**
必要に応じて、説明や現在の状況など、その他の詳細を入力します。グループ グループ シートで各プロジェクトのグループ IDを検索し、各プロジェクトのsetGroupID列に入力します。CMPY会社シートでプロジェクトの会社IDを検索し、setCompanyID列に入力します。USER User シートで各プロジェクト所有者のユーザーIDを検索し、setOwnerID列に入力します。ユーザーユーザーシートで各プロジェクトスポンサーのユーザーIDを検索し、setSponsorID列に入力します。

![値を設定](assets/im9.png)

>[!NOTE]
>
>ステータスフィールドと優先度フィールドの許容値は、Workfront のワークフロー設定エリアで、各オブジェクトのステータスと優先度の環境設定を参照することで確認できます。

## 入力タスクの詳細

キックスタートを使用してプロジェクトを読み込む際に、プロジェクトのタスクに関する情報を追加できます。

ダウンロードした Workfront.xlsx ファイルを開きます。 **「TASK」タスクシートに移動します。**

Workfront で既にタスクを作成している場合を除き、このシートは空白にしておく必要があります。

![ タスクシート ](assets/im8.png)

![空のタスクシート ](assets/im7.png)

![ タスクシート列](assets/im6.png)

タスクをマッピングする最も簡単な方法は、（特に、各プロジェクトでタスクが同じ場合）一度に 1 つのプロジェクトです。 その後、最初のプロジェクトのタスクプランをコピーし、後続のプロジェクトのタスクプランを少し調整できます。 残りの手順では、Workfront プロジェクトの実装のみのタスクを作成することを前提としています。 シナリオに従って、1 つのプロジェクトにつき 9 つのタスクを読み込むので、isNew 列の 3 行目から 11 行目までに TRUE を入力します。

次のタスクフィールドに値を設定します。

* **セット ID**
ID列の各行に一意のIDを入力します。
* **セット名**
setName列にタスク名を入力します。
* **プロジェクト IDの確認**
「Workfrontを実装」プロジェクト用に設定したIDを入力します。PROJ プロジェクトシートを確認して、正しいIDであることを確認します。
* **ユーザーを設定**
ユーザーユーザーシートに移動して、各タスクに割り当てられたユーザーのIDを検索し、setAssignedToID列のそれぞれのセルにこれらの値を入力します。
* **タスク関係の特定**
タスク 2 ～ 5の場合は、setParentID列に1を入力します。 9 番目のタスクには、setParentID 列に 8 を入力します。 setPredecessorString 列に、各先行タスクのタスク番号を入力します。 このシナリオの 8 番目のタスクなどのように、タスクに複数の先行タスクがある場合、各先行タスク ID を区切るために、コンマを使用する必要があります。 「先行タスク関係の作成」の記事で説明されている簡略表記法を使用して、非終了 - 開始関係に間隔を置いて先行タスクを定義できます。
* **期間を設定**
setDuration フィールドにタスクの時間数、日数、週数、月数を入力して、各タスクの期間を設定します。 次に、setDurationUnit フィールドに期間単位を入力します。

  |   | 入力可能値 |
  |---|---|
  | 分 | M |
  | 時間 | H |
  | 日 | D |
  | 週 | W |
  | か月 | T |

  分は時間単位の小数として表すこともできます（例：分 = 5 時間）

* 各タスクの作業量を setWorkRequired フィールドに設定します。 次に、setWorkUnit フィールドに作業単位を入力します。 「要求された作業」値が期間と異なる場合は、setDurationType フィールドに A を入力する必要もあります。

  | 期間タイプ | 入力可能値 |
  |---|---|
  | 予定割り当て時間 | A |
  | 予定作業 | W |
  | 残存作業時間の優先 | D |
  | シンプル | S |

* 各タスクの setPercentComplete フィールドに、完了率の整数表記を入力します。 この値には、パーセント記号（%）を含めないでください。
* 必要に応じて、作成する各タスクの説明とその他の詳細を含めます。

  ![詳細を追加](assets/im5.png)

* 先行タスク関係に基づいているので、setPlannedStartDate 列と setTaskConstraint 列は、このプロジェクトのタイムラインの作成には使用されません。 その代わりに、各タスクの日付を入力できます。 その場合は、setTaskConstraint 列に有効なタスク制約も指定してください。 このフィールドの有効な値について詳しくは、タスク制約の記事と関連記事を参照してください。

  このシナリオの場合、読み込む他のプロジェクトのタスクを作成する最も簡単な方法は、定義したタスクをコピーし、下の 12 行目以降にペーストすることです。 続いて、以下を行います。

   1. ID 列の値を付け直します。
   1. setProjectID 列を、次に行うプロジェクトに設定した値に更新します。
   1. setParentID 値と setPredecoderString 値を更新して、このプロジェクトのタスクに割り当てた新しい ID が反映されるようにします。
   1. タスクの割り当てと完了率を更新します。
   1. 次回のプロジェクトのタスクに対して、これらの手順を繰り返します。

* **Excel ファイルの読み込み**

  [キックスタートテンプレートを使用した Adobe Workfront へのデータの読み込み](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)で示されている手順に従います。
