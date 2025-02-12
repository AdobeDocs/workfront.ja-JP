---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: タスクおよび問題を委任
description: 不在時に割り当てられた作業を、一時的にデリゲートできます。この記事では、タスクとイシューの割り当てをデリゲートする方法について説明します。
author: Alina
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 79%

---

# タスクおよびイシューのデリゲート

<!-- Audited: 10/2024 -->


<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote this as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

不在時に割り当てられた作業を、一時的にデリゲートできます。

タスクとイシューの割り当てや承認をデリゲートできます。この記事では、タスクとイシューの割り当てをデリゲートする方法について説明します。

作業のデリゲートに関する一般情報について詳しくは、[作業のデリゲートの概要](../../manage-work/delegate-work/delegate-work-overview.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

>[!IMPORTANT]
>
>* 委任者として選択したユーザーには、デリゲートを依頼するユーザーのタスクやイシューに対する権限と同じ権限が付与されます。
>* 権限は、アクセスレベル内で機能する必要があり、デリゲートされたユーザーのアクセスレベルが、デリゲートを依頼するユーザーのアクセスレベルより低い場合もあります。
>
>   
>   例えば、デリゲートされるユーザーがアクセスレベルでタスクに対する表示アクセス権のみを持ち、デリゲートを依頼するユーザーがデリゲートするタスクに対して管理権限を持っている場合、デリゲートされるユーザーには、デリゲートされるタスクに対して管理権限が付与されます。ただし、ユーザーはデリゲートされたタスクに対して、デリゲートを依頼したユーザーと同じアクションを実行することはできません。不在時にタスクを更新できるようにするには、システム管理者にタスクに対する編集アクセス権をリクエストする必要があります。
>
>   
>   システム管理者がアクセスレベルを変更する方法については、[カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。
>
>* デリゲーションが既に開始した後に割り当てられた項目の場合、[!DNL Workfront] が新しく割り当てられた項目を委任者と共有するまで、項目が割り当てられてから最大 1 時間かかる場合があります。


この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>新規：コントリビューター以上</p><p>または</p><p>現在：Review 以上</p>

>[!NOTE]
>
>リクエストライセンスを持っている場合は、作業に割り当てられることができますが、他のユーザーに対して作業をデリゲートすることはできません。[!DNL Workfront] では、作業をレビュー、リクエスト、コントリビューターの各ユーザーに割り当てることはお勧めしません。

</tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびイシューに対する編集アクセス権 
     </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>割り当てられているタスクまたはイシューに対する表示権限またはそれ以上の権限</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## 前提条件

この記事で説明するアクティビティを実行する前に、次の点を確認する必要があります。

* [!DNL Workfront] またはグループの管理者が、[!DNL Workfront] ーザーインスタンスの [!UICONTROL **設定**] 領域の [!UICONTROL  タスクとイシューの環境設定 ] セクションで [!UICONTROL  ユーザーがタスクとイシューを委任することを許可 ] 設定を有効にしました。

  詳しくは、[システム全体のタスクとイシューの環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

## タスクとイシューを別のユーザーにデリゲート

作業を他のユーザーにデリゲートする前に、ユーザーと連絡を取り、作業項目の委任者に指定される旨を伝えることをお勧めします。作業をデリゲートする前に、口頭での承認を求め、自分の不在中に相手が作業を完了させるために必要な時間があることを確認します。

タスクとイシューのデリゲートに関する一般情報について詳しくは、[タスクとイシューのデリゲートの概要](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md)を参照してください。

タスクやイシューを他のユーザーにデリゲートするには、次の手順に従います。

1. [!UICONTROL **ホーム**] エリアに移動します。
1. [!UICONTROL **マイ作業**]、[!UICONTROL **マイタスク**] または [!UICONTROL **マイイシュー**] ウィジェットが [!UICONTROL **ホーム**] に追加されていることを確認します。

   詳しくは、[ ホームでのウィジェットの追加、編集、削除 ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md) を参照してください。

1. [!UICONTROL **マイ作業**]、[!UICONTROL **マイタスク**] または [!UICONTROL **マイイシュー[!UICONTROL ** ウィジェットの左上隅にある **]委任**] をクリックします。

   ![ 委任ボタン ](assets/delegate-button-on-my-work-widget.png)

1. 次を更新します。

   * [!UICONTROL **タスクおよびイシューのデリゲート先**]：タスクおよびイシューをデリゲートするユーザーの名前を入力し、リストに表示されたら選択します。選択できるユーザーは 1 名のみです。

     委任者として選択したユーザーには、デリゲートしたタスクやイシューに対する権限と同じ権限が付与されます。

   * [!UICONTROL **開始日**]：作業項目のデリゲーションを開始する日付をカレンダーから選択します。

     >[!TIP]
     >
     >開始日に過去の日付を指定することはできません。

   * [!UICONTROL **終了日なし**]：デリゲーションの終了日を指定しない場合は、このオプションを選択します。

   * [!UICONTROL **終了日**]：デリゲーションを停止する日付をカレンダーから選択します。

     >[!TIP]
     >
     >「終了日」フィールドを空のままにし、「終了日なし」オプションを選択していない場合、デリゲーションは現在の日に対してのみ設定されます。

     ![ 展開された代理ボックス ](assets/delegate-box-expanded-in-home.png)
     <!--check screen shot - submitted bug for casing-->

1. 「[!UICONTROL **保存**]」をクリックします。

   次が発生します。

   * 作業は指定したユーザーにデリゲートされます。選択した時間枠に日付が設定された未完了のタスクまたはイシュー（デリゲーションが有効になった後に新しく割り当てられたものを含む）は、デリゲートされます。

     >[!TIP]
     >
     >   デリゲーションの時間枠内に日付が設定された完了済みの作業項目は、デリゲートされません。


   * 画面の下部に、別のユーザーへの作業の委任が有効になったことを確認するメッセージが表示されます。デリゲートされたユーザーの名前が確認メッセージに表示されます。

   * [!DNL Workfront] で割り当てが表示できるほとんどの領域で、タスクとイシューが他のユーザーにデリゲートされたことを示すメッセージが表示されます。委任者の名前が含まれていないエリアについて詳しくは、[作業のデリゲートの概要](delegate-work-overview.md)を参照してください。

   * [!UICONTROL **ホーム**]&#x200B;領域の「[!UICONTROL **デリゲート**]」ボタンが「[!UICONTROL **デリゲーションを編集**]」に変更されます。これは、デリゲーションが実行されていることを示します。
     <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
      </MadCap:conditionalText>
      -->

     ![ デリゲーションを編集ボタン ](assets/edit-delegation-button-on-my-work-widget.png)

   * イベント通知と個人通知が有効になっている場合は、デリゲーションの確認メールも送信されます。

   * イベント通知が有効になっている場合、委任者として選択したユーザーには、デリゲーションに関するメールが届きます。

     個人のメール通知を有効にする方法について詳しくは、[自身のメール通知の変更](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)を参照してください。

## デリゲーションを編集または停止

終了日を選択した場合は、デリゲーションの有効期限を指定するか、手動で停止することができます。また、デリゲーションの日付が変更された場合は、デリゲーションの時間枠を変更することもできます。

1. [!UICONTROL **ホーム**] 領域に移動して、次のいずれかのウィジェットで [!UICONTROL **委任を編集**]**をクリックします。自分の作業**、**自分のタスク**、または **自分の問題**。
1. [!UICONTROL  タスクおよび問題の委任を停止 ] ボックスで、次のいずれかの操作を行います。
   * 「[!UICONTROL **開始日**]」または「[!UICONTROL **終了日**]」を変更します
   * 「[!UICONTROL **デリゲーションを停止**]」をクリックします

   >[!TIP]
   >
   >    デリゲーションが既に開始している場合は、デリゲーションの「終了日」のみを編集できます。

   ![ 委任を停止ボタン ](assets/stop-delegation-box-new-home-tasks-and-issues.png)

1. （条件付き）「[!UICONTROL **保存**]」をクリックして新しいデリゲーション日を保存します

   または

   確認ボックスの「[!UICONTROL **デリゲーションを停止**]」をクリックして、デリゲーションの停止を確定します。

   これで、デリゲーションの日付が更新されたか、デリゲーションが停止し、デリゲートされたユーザーがタスクとイシューから削除されました。タスクおよびイシューに対する権限は、そのまま残ります。

## デリゲートされた作業と委任者情報を検索

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

タスクとイシューをデリゲートする場合、[!DNL Workfront] には、デリゲートされた作業や委任者を確認できる領域がいくつかあります。

* [「割り当て」ボックスで委任者を検索](#locate-delegates-in-the-assignments-box)
* [[!UICONTROL ホーム]でデリゲートされた作業を検索](#locate-delegated-work-in-home)


### 「[!UICONTROL 割り当て]」ボックスで委任者を検索

システム管理者またはグループ管理者がシステムで作業のデリゲーションを有効にした場合、「[!UICONTROL 割り当て]」ボックスには、アクセスできるすべての場所に次のタブが表示されます。

* [!UICONTROL **割り当て**]：タスクまたはイシューに割り当てられたユーザーがここに表示されます。
* [!UICONTROL **デリゲーション**]：タスクまたはイシューの担当者が委任者として指定したユーザーがここに表示されます。

次の領域で「[!UICONTROL 割り当て]」ボックスにアクセスできます。

* タスクまたはイシューのヘッダー

  タスクまたはイシューのヘッダーの「[!UICONTROL 割り当て]」フィールドが、「[!UICONTROL 割り当てとデリゲーション]」に変更されます。

  ![ タスクヘッダーの割り当てと委任パネル ](assets/assignments-and-delegates-panel-in-task-header.png)

* タスクまたはイシューを手動で割り当てる際の[!UICONTROL ワークロードバランサー]

  ![ バランサーの割り当てと委任パネル ](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> タスクまたはイシューの「編集」ボックスの「[!UICONTROL 割り当て]」セクションでは、委任者を表示できません。

タスクまたはイシューがデリゲートされたものの、「[!UICONTROL デリゲーション]」サブタブが空の場合は、次のシナリオのいずれかが存在する可能性があります。

* タスクまたはイシューに割り当てられていません。
* タスクまたはイシューの日付がデリゲーションの時間枠外です。

>[!TIP]
>
>デリゲートされたタスクやイシューの予定時間数または実際の時間数は、デリゲートされたユーザーの[!UICONTROL ワークロードバランサー]や [!DNL Resource Planner] などのリソース管理ツールでは考慮されません。これらの時間数は、割り当てられたユーザーにのみ関連付けられます。

### [!UICONTROL ホーム]でデリゲートされた作業を検索

1. [!UICONTROL **担当作業**] ウィジェットの [!UICONTROL **ホーム**] エリアに移動します。
1. 「フィルター」ドロップダウンメニューをクリックし、次のオプションを 1 つ以上選択します。
   * [!UICONTROL **デリゲート済み**]：自分にデリゲートされた、または自分がデリゲートしたタスクやイシューを表示します。
   * [!UICONTROL **自分にデリゲート済み**]：別のユーザーが自分にデリゲートしたタスクとイシューを表示します。
   * [!UICONTROL **自分がデリゲート済み**]：自分が他のユーザーにデリゲートしたタスクとイシューを表示します。

     ![ 委任されたタスクと問題フィルター ](assets/delegated-tasks-and-issues-new-home-filter.png)

1. （オプション） [!UICONTROL **並べ替え**] ドロップダウンメニューをクリックして、次の条件でリストを並べ替えます。
   * [!UICONTROL  期限 ]. これはデフォルトの並べ替えオプションです。
   * [!UICONTROL 名前]
   * [!UICONTROL 完了率]
   * [!UICONTROL ステータス]
1. （オプション） [!UICONTROL **マイ作業**] ウィジェットの右上にあるグループ化ドロップダウンメニューを展開し、次のいずれかの条件でグループ化します。
   * なし。 これはデフォルトのグループ化オプションです。
   * [!UICONTROL プロジェクト]
   * [!UICONTROL ステータス]
   * [!UICONTROL  期限日 ]

1. 委任した項目または委任された項目を表示するには、次のいずれかを表示します。

   * 他のユーザーに委任した項目については、タスクまたは問題のステータスで [!UICONTROL **委任先**] の後に委任名を見つけます。

   * 自分に委任された項目の場合は、タスクまたは問題のステータスの [!UICONTROL **委任者**] の後に、担当者の名前を見つけます。

     >[!TIP]
     >
     >    デリゲーションが今日以降の日付に開始するように設定されている場合は、デリゲーションの開始日も[!UICONTROL 作業リスト]に表示されます。委任された項目は、グループのタイプに応じて、[!UICONTROL 作業リスト]に対して選択したグループ化に表示されます。例えば、[!UICONTROL 予定完了日]によってグループ化した場合、委任された項目は予定完了日と一致するグループ化に表示されます。
