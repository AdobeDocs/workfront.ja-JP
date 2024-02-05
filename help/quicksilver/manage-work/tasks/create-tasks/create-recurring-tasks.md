---
product-area: projects
navigation-topic: create-tasks
title: 繰り返しタスクを作成
description: 単一のプロジェクトの一部として繰り返す必要のあるタスクに対して、繰り返しタスクを作成できます。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: 297e72ebb70c335078d65e7ed6e28862285d2fb1
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 93%

---

# 繰り返しタスクを作成

<!--Audited: 01/2024-->

単一のプロジェクトの一部として繰り返す必要のあるタスクに対して、繰り返しタスクを作成できます。

既存の繰り返しタスクの編集の影響を含む、繰り返しタスクの一般的な情報について詳しくは、[繰り返しタスクの概要](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>新規：標準</p> 
   <p>現在：作業以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対して、タスクを追加する機能以上を持つ参加権限</p> 
   <p>タスクを作成すると、タスクに対する「権限を管理」が自動的に付与される</p> 
   <p> タスク権限について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">タスクを共有</a>を参照してください。</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。 アクセス要件について詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 繰り返しタスクの作成

>[!NOTE]
>
>既存のタスクを変更して繰り返しタスクを作成することはできません。タスクはゼロから作成する必要があります。

1. 繰り返しタスクを作成するプロジェクトに移動し、左側のパネルの「**タスク**」セクションをクリックします。
1. 「**新規タスク**」をクリックします。

   新規タスクダイアログボックスが表示されます。

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. クリック **その他のオプション** 次に、 **タスク名** フィールドに入力します。
1. 新しいタスクを追加した場合と同じ方法で、タスクの更新を続行します。新しいタスクの追加について詳しくは、[プロジェクトでタスクを作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)を参照してください。

   >[!TIP]
   >
   >   新しい繰り返しタスクで表示される期間と予定時間数は、それぞれの繰り返しタスクの期間と予定時間数です。親タスクの期間は、最も早いタスクの予定開始日から最も遅いタスクの予定完了日までの時間です。親タスクの予定時間数は、すべてのタスクからのすべての予定時間数の合計です。

1. 左側のパネルにある「**概要**」をクリックします。
1. 「**繰り返しスケジュール**」セクションまで下にスクロールして、「**これを繰り返しタスクにする**」オプションを選択します。

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. **頻度**&#x200B;ドロップダウンリストで、タスクを実行する時間単位の数と時間単位の種類を選択します。次のオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>繰り返しタイプ</th> 
      <th>説明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>日</strong> </td> 
      <td> <p>選択した頻度に応じて、タスクは毎日、2 日ごと、3 日ごとなどに繰り返されます。最大 6 日ごとに繰り返すタスクを設定できます。デフォルト設定は 1 日です。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>稼働日</strong> </td> 
      <td> <p> タスクは、選択した頻度に応じて、毎日、2 稼働日ごと、3 稼働日ごとなどに繰り返されます。最大 6 稼働日ごとに繰り返すタスクを設定できます。</p> <p><a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールの作成</a>で説明しているように、このオプションでは、システム管理者が定義したデフォルトのスケジュールを使用します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>週</strong> </td> 
      <td> <p> タスクは、選択した頻度に応じて、毎週、2 週間ごと、3 週間ごとなどに繰り返されます。</p> <p>「<strong>イテレーション</strong>」フィールドで、各タスクを実行する曜日を選択します。複数の曜日を選択できます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>月</strong> </td> 
      <td> <p>タスクは、選択した頻度に応じて、毎月、2 か月ごと、3 か月ごとなどに繰り返されます。1 ～ 12 か月を選択できます。 </p> <p>「<strong>イテレーション</strong>」フィールドで、タスクを実行する際に次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>毎月のある特定の日付&lt;month date&gt;</strong> </p> <p>1 ～ 30 日までの日付を選択するか、「<strong>最後</strong>」を選択します。例えば、「毎月 30 日」を選択できます。 </p> </li> 
        <li> <p><strong>毎月 &lt;number&gt; &lt;day of the week&gt;</strong> </p> <p>最初のドロップダウンメニューで、月の週数を 1 ～ 4 の数値で選択できます。または、「最後」を選択できます。 </p> <p>2 番目のドロップダウンメニューでは、任意の曜日を選択できます。 </p> <p>例えば、「毎月第 2 火曜日」を選択できます。 </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >プロジェクトのスケジュールにスケジュール例外が関連付けられている場合、例外の期間中に繰り返しタスクを実行することはできません。スケジュールの例外期間中に発生する繰り返しタスクは、例外期間後の最初の営業日に開始するようにスケジュールされます。スケジュールの例外について詳しくは、[スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)の記事を参照してください。

1. 「**開始**」フィールドで、繰り返しタスクを開始する日時を選択します。
1. 「**終了**」フィールドで、繰り返しタスクを完了する日時を選択します

   または

   「**`<number>` 発生後**」を選択して、定期タスクの発生回数を指定します。Workfront は、このフィールドで指定した数と同じ回数の定期タスクを作成します。

1. 「**タスクを作成**」をクリックします。

   タスクリストが表示されます。定期タスクは親として作成され、繰り返しはすべてその子として作成されます。Workfront は、親に入力した名前の後に数字を付けて、子タスクの名前を自動生成しました。繰り返しタスクは、タスクリストの最後に配置されます。

   親の定期タスクから自動入力されるフィールドについて詳しくは、[定期タスクの概要](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md)を参照してください。

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. （オプション）各定期タスクを、プロジェクト内の他のタスクと同様に変更します。

   例えば、割り当て、先行タスク、期間を追加し、カスタムフィールドを含むタスクに関するその他の情報を変更できます。

   >[!IMPORTANT]
   >
   >子を個別に変更した後に親の繰り返しを変更すると、子同士の間、または子と親の間で情報が異なる場合があります。詳しくは、[定期タスクの概要](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md)を参照してください。
