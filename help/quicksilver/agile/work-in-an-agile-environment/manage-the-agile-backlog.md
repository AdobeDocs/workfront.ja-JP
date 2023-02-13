---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: アジャイルバックログの管理
description: タスクと問題は、チームが使用しているアジャイルな方法に応じて、アジャイルなチームに割り当て、そのチームのバックログにストーリーとして追加できます。
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: b855f032b24079ff27435fb833cd3ed8a382a77c
workflow-type: tm+mt
source-wordcount: '1376'
ht-degree: 0%

---

# アジャイルバックログの管理

以下の作業項目は、チームが使用するアジャイルな方法に応じて、アジャイルチームに割り当て、ストーリーとしてチームのバックログに追加できます。

* **[!UICONTROL スクラムアジャイルチーム]:** タスクと問題は、アジャイルチームに割り当て、バックログに追加できます。
* **[!UICONTROL かんばんアジャイルチーム]:** タスクをアジャイルチームに割り当て、バックログに追加できます。 ユーザーは、「 [[!UICONTROL バックログを追加] かんばん委員会に](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). チームは、このバックログを使用して作業キューに優先順位を付け、管理します。

タスクまたは問題は、任意の場所からチームに割り当てることができます（その後、チームバックログに追加されます） [!DNL Adobe Workfront]. 例えば、1 つのチームに複数のプロジェクトから作業割り当てを割り当てることができます。

>[!NOTE]
>
>複数のチームをバックログ項目に追加した場合、タスクまたは問題は、主チームのバックログにのみ表示されます。 主なチームが最初に割り当てられたチームです。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以降</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>[!UICONTROL ストーリーが存在するプロジェクトへの [!UICONTROL 管理 ] アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## バックログに関するストーリーの作成と管理

* [ストーリーの並べ替え](#reorder-stories)
* [[!UICONTROL 改行] 下の話](#break-down-stories)
* [ストーリーを編集](#edit-stories)
* [バックログに新しいストーリーを作成](#create-new-stories-on-the-backlog)
* [バックログからイテレーションまたはかんばんボードにストーリーを移動](#move-stories-from-the-backlog-to-an-iteration-or-kanban-board)

### ストーリーの並べ替え {#reorder-stories}

ドラッグ&amp;ドロップを使用して、バックログリスト内のストーリーを並べ替えることができます。

1. ストーリーの並べ替えを行うアジャイルバックログに移動します。
1. 内 **[!UICONTROL 表示]** ドロップダウンメニューで、 **[!UICONTROL バックログ]** を含むビューまたはカスタムビュー **[!UICONTROL 注文]** 列。

   >[!NOTE]
   >
   >タスクまたは問題にアジャイルチームが割り当てられ、プロジェクトのステータスが「現在」と等しくない場合、バックログには表示されません。 ただし、[ 注文 ] 列のバックログ数には影響します。

1. 1 つ以上のストーリーを選択し、ストーリーをバックログに表示する順序にドラッグします。\
   ![バックログ項目をドラッグ&amp;ドロップ](assets/agile-backlog-drag-and-drop.png)

### ストーリーの分類 {#break-down-stories}

バックログ内のストーリーのサイズは異なるので、ユーザーはそれらを反復で使用可能なサイズに分類できます。 ストーリーを分類すると、ストーリーが表すタスクにサブタスクが作成され、バックログの元のタスクが置き換えられます。 親タスクまたはそのサブタスクをアジャイルチームに割り当てることはできますが、両方を同時にチームに割り当てることはできません。

>[!NOTE]
>
>ストーリーを分類する際は、次の制限事項を考慮してください。
>
>* 分類できるのは、タスクを表すストーリーのみです。 問題を表すストーリーを分類することはできません。
>* ストーリーは、プロジェクトに関連付けられている場合にのみ分類できます。



ストーリーを分類するには：

1. 分類するストーリーが含まれているバックログに移動します。
1. 分類するストーリーを選択し、「 **[!UICONTROL ストーリーを分類]**.\
   この [!UICONTROL ストーリーを分類] ダイアログボックスが表示されます。\
   ![ストーリーを分類ダイアログ](assets/backlog-breakdown-dialog.png)

1. ストーリーの名前と推定値を指定し、ストーリーの準備ができているかどうかを選択します。
1. クリック **[!UICONTROL ストーリーを追加]** 元の物語から別の物語を作り出す
1. 「**[!UICONTROL 保存]**」をクリックします。

### ストーリーを編集 {#edit-stories}

ストーリーは、 [!UICONTROL ストーリー] または [!UICONTROL 問題] プロジェクト内のタスクや問題を一括編集する場合と同様に、「バックログ」タブが表示されます。詳しくは、 [タスクを一括編集](../../manage-work/tasks/manage-tasks/edit-tasks.md#editing-tasks-in-bulk) in [タスクを編集](../../manage-work/tasks/manage-tasks/edit-tasks.md) および [問題の編集](../../manage-work/issues/manage-issues/edit-issues.md#bulk-editing-issues) in [問題の編集](../../manage-work/issues/manage-issues/edit-issues.md).

## バックログに新しいストーリーを作成 {#create-new-stories-on-the-backlog}

バックログから直接ストーリーを作成するか、既存のタスクまたはイシューをアジャイルチームに割り当てることで、バックログに新しいストーリーを作成できます。

* [バックログからストーリーを作成](#create-a-story-from-the-backlog)
* [アジャイルチームにタスクまたはイシューを割り当てる](#assign-a-task-or-issue-to-an-agile-team)

### バックログからストーリーを作成 {#create-a-story-from-the-backlog}

バックログからストーリーを作成すると、ストーリーはタスクまたはタスクとしてプロジェクト内に作成されます。 バックログからストーリーをイシューとして作成することはできません。

バックログからストーリーを作成する手順は、次のとおりです。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL チーム]**.

1. （オプション） **[!UICONTROL チームの切り替え]** アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png)をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 選択 **[!UICONTROL バックログ]** を左側のパネルからクリックします。
1. タスクを作成するかイシューを作成するかに応じて、次のいずれかの操作を実行します。

   * **タスクを作成するには：** クリック **[!UICONTROL ストーリー]**.

   * **イシューを作成するには：** クリック **[!UICONTROL 問題]**.

1. クリック **[!UICONTROL 新しいストーリー]** または **[!UICONTROL 新しい問題]**.

1. 次の情報を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL ストーリー名 ]</strong></td>
      <td> ストーリーの名前を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 説明 ]</strong></td>
      <td>（オプション）ストーリーの説明を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 準備完了 ]</strong></td>
      <td> ストーリーを反復に追加する準備ができているかどうかを選択します。 この設定は情報提供のみを目的としています。 この設定のステータスに関係なく、ストーリーを反復に追加できます。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 予測 ]</strong></td>
      <td>ストーリーのポイントまたは時間単位の推定値を指定します。 見積もりはバーンダウンチャートに影響を与えます。 反復のバーンダウンチャートは、各ストーリーに正確な推定が含まれる場合にのみ正確です。 （ポイントの見積もりを指定する場合は、各ポイントが表す時間数をチーム設定で既に指定している必要があります）。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 親プロジェクト ]</strong></td>
      <td>このストーリーを作成するプロジェクトの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。<br>プロジェクトのステータスは [!UICONTROL Current] に設定する必要があります。 プロジェクトのステータスが [!UICONTROL Current] 以外の場合は、ドロップダウンメニューに表示されません。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 親タスク ]</strong></td>
      <td>（オプション）このストーリーが従属する親タスクの名前を入力し、ドロップダウンリストに表示されたら、名前をクリックします。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL カスタムForms]</strong></td>
      <td> （オプション）このストーリーに追加するカスタムフォームを選択します。</td>
     </tr>
    </tbody>
   </table>

1. クリック **[!UICONTROL ストーリーを保存]**.

### アジャイルチームにタスクまたはイシューを割り当てる {#assign-a-task-or-issue-to-an-agile-team}

アジャイルチームにタスクまたはイシューを割り当てることができます。 割り当て後、タスクまたは問題はチームバックログの新しいストーリーとして表示されます。

アジャイルチームにタスクまたはイシューを割り当てるには、次の手順に従います。

1. 再割り当てするタスクを含むプロジェクトに移動します。
1. リストからタスクまたはイシューを選択します。
1. クリック **[!UICONTROL 編集]**.
1. クリック **[!UICONTROL 割り当て]**.
1. （オプション）既存の担当者を削除します。
1. クリック **[!UICONTROL 担当者を追加]**.
1. タスクまたはイシューに割り当てるアジャイルチームの名前を入力し、ドロップダウンリストに表示されたらチーム名をクリックします。
1. クリック **[!UICONTROL 変更を保存]**.\
   タスクまたは問題がチームのバックログで利用できるようになりました。

## バックログからイテレーションまたは+ボードにストーリーを移動 {#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [既存のストーリーをバックログに移動](#move-existing-stories-to-the-backlog)
* [バックログからストーリーをエクスポート](#export-stories-from-the-backlog)

1. アジャイルチームのバックログに移動します。
1. 反復またはかんばんボードに移動するストーリーを選択し、 **[!UICONTROL 詳細]** > **[!UICONTROL 移動先]**.\
   ストーリーを [!UICONTROL かんばん] ボード、 [!UICONTROL ストーリーをかんばんに移動] ボードが表示されます。\
   ストーリーを反復する場合、 [!UICONTROL ストーリーを反復に移動] ダイアログボックスが表示されます。\
   ![ストーリーを移動ダイアログ](assets/agile-backlog-addtoiteration.png)

1. 次のいずれかの操作を行います。

   * **スクラムチームの場合：** 内 **[!UICONTROL 反復を選択]** 「 」フィールドで、ストーリーを移動する反復を選択します。

   * **かんばんチームの場合：** 内 **[!UICONTROL かんばんボードの選択]** フィールドでチームを選択 [!UICONTROL かんばん] ボード。 ( かんばんチームは 1 つのみを持つことができます [!UICONTROL かんばん] ボード )

1. クリック **[!UICONTROL ストーリーを移動]**.

### 既存のストーリーをバックログに移動 {#move-existing-stories-to-the-backlog}

チームがまだストーリーに取り組む準備ができていないと判断した場合は、ストーリーをバックログに移動できます。

詳しくは、 [俊敏なストーリーを移動](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### バックログからストーリーをエクスポート {#export-stories-from-the-backlog}

バックログから直接 1 つ以上のストーリー（タスクやイシューを含む）を書き出すことができます。

別のデータを書き出すのと同じ方法で、バックログからストーリーを書き出します。 [!DNL Workfront]( [データを書き出し](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
