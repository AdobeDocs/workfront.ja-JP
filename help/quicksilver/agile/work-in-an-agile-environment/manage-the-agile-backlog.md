---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: アジャイルバックログの管理
description: チームが使用するアジャイル手法に応じて、タスクとイシューをアジャイルチームに割り当て、そのチームのバックログにストーリーとして追加できます。
author: Jenny
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 69%

---

# アジャイルバックログの管理

チームが使用するアジャイル手法に応じて、次の作業項目をアジャイルチームに割り当て、そのチームのバックログにストーリーとして追加できます。

* **[!UICONTROL アジャイルチームのスクラム ]:** タスクとイシューは、アジャイルチームに割り当てられ、バックログに追加できます。
* **[!UICONTROL かんばんアジャイルチーム ]:** タスクをアジャイルチームに割り当て、バックログに追加できます。 [[!UICONTROL  バックログの追加 ] をかんばんボードに対して ](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md) で説明しているように、ユーザーは Agile ストーリーボードから直接バックログを表示できます。 チームはこのバックログを使用し、作業キューに優先順位を付けて管理します。

タスクまたはイシューは、[!DNL Adobe Workfront] の任意の場所からチームに割り当てることができます（その後、チームバックログに追加されます）。例えば、1 つのチームに複数のプロジェクトから作業割り当てを割り当てることができます。

>[!NOTE]
>
>複数のチームをバックログ項目に追加した場合、タスクまたはイシューは、プライマリチームのバックログにのみ表示されます。プライマリチームは、最初に割り当てられたチームです。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>Work またはそれ以上</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>ストーリーが含まれるプロジェクトへのアクセスの管理 </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## バックログでのストーリーの作成と管理

* [ストーリーの並べ替え](#reorder-stories)
* [ストーリーの[!UICONTROL 分類]](#break-down-stories)
* [ストーリーの編集](#edit-stories)

### ストーリーの並べ替え {#reorder-stories}

ドラッグ＆ドロップを使用して、バックログリスト内のストーリーを並べ替えることができます。

1. ストーリーを並べ替えるアジャイルバックログに移動します。
1. **[!UICONTROL ビュー]**&#x200B;ドロップダウンメニューで、**[!UICONTROL バックログ]**&#x200B;ビュー、または&#x200B;**[!UICONTROL 注文]**&#x200B;列を含むカスタムビューを選択します。

   >[!NOTE]
   >
   >タスクまたは問題にアジャイルチームが割り当てられ、プロジェクトが現在と同じステータスでない場合、バックログには表示されません。 ただし、注文列のバックログ数には影響します。

1. 1 つ以上のストーリーを選択し、バックログに表示する順にドラッグします。
   ![バックログ項目のドラッグ＆ドロップ](assets/agile-backlog-drag-and-drop.png)

### ストーリーの分類 {#break-down-stories}

バックログ内のストーリーのサイズは異なるので、ユーザーは反復で使用可能なサイズにストーリーを分類できます。ストーリーを分類すると、ストーリーが表すタスクにサブタスクが作成され、バックログの元のタスクが置き換えられます。アジャイルチームに親タスクまたはそのサブタスクを 1 つ割り当てることができますが、両方を同時にチームに割り当てることはできません。

>[!NOTE]
>
>ストーリーを分類する際は、次の制限事項を考慮してください。
>
>* 分類できるのは、タスクを表すストーリーのみです。イシューを表すストーリーは分類できません。
>* ストーリーは、プロジェクトに関連付けられている場合にのみ分類できます。


ストーリーを分類するには：

1. 分類するストーリーが含まれているバックログに移動します。
1. 分類するストーリーを選択し、「ストーリーを分類 **[!UICONTROL をクリックし]** す。
[!UICONTROL ストーリーを分類]ダイアログボックスが表示されます。
   ![ストーリーを分類ダイアログ](assets/backlog-breakdown-dialog.png)

1. ストーリーの名前と見積りを指定し、ストーリーの準備ができたかどうかを選択します。
1. 元のストーリーから別のストーリーを作成するには、「**[!UICONTROL ストーリーを追加]**」をクリックします。
1. 「**[!UICONTROL 保存]**」をクリックします。

### ストーリーの編集 {#edit-stories}

プロジェクト内のタスクや課題を一括で編集するのと同じように、「バックログ」の「[!UICONTROL ストーリー]」タブまたは「[!UICONTROL イシュー]」タブからストーリーを直接編集できます。詳しくは、[タスクの編集](../../manage-work/tasks/manage-tasks/edit-tasks.md)の[タスクの一括編集](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk)と、[イシューの編集](../../manage-work/issues/manage-issues/edit-issues.md)を参照してください。

## バックログでの新しいストーリーの作成 {#create-new-stories-on-the-backlog}

バックログから直接ストーリーを作成するか、アジャイルチームに既存のタスクまたはイシューを割り当てることで、バックログに新しいストーリーを作成できます。

* [バックログからストーリーを作成する](#create-a-story-from-the-backlog)
* [アジャイルチームにタスクまたはイシューを割り当てる](#assign-a-task-or-issue-to-an-agile-team)

### バックログからストーリーを作成する {#create-a-story-from-the-backlog}

バックログからストーリーを作成すると、ストーリーはプロジェクト内のタスクまたはイシューとして作成されます。

バックログからストーリーを作成する手順は、次のとおりです。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックして、「**[!UICONTROL チーム]**」をクリックします。

1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームの切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索し、表示されたら選択します。

1. 左パネルから「**[!UICONTROL バックログ]**」を選択します。
1. タスクを作成するかイシューを作成するかに応じて、次のいずれかの操作を実行します。

   * **タスクを作成するには：**「**[!UICONTROL ストーリー]**」をクリックします。

   * **イシューを作成するには：**[!UICONTROL 「]**イシュー**」をクリックします。

1. 「**[!UICONTROL 新規ストーリー]**」または「**[!UICONTROL 新規イシュー]**」をクリックします。

1. 次の情報を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td> ストーリーの名前を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>（オプション）ストーリーの説明を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td> ストーリーをイテレーションに追加する準備ができているかどうかを選択します。この設定は情報提供のみを目的としています。この設定のステータスに関係なく、ストーリーをイテレーションに追加できます。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>ストーリーのポイントまたは時間単位の推定値を指定します。見積もりはバーンダウンチャートに影響を与えます。イテレーションのバーンダウンチャートは、各ストーリーに正確な見積もりが含まれる場合にのみ正確です。（ポイントの見積もりを指定する場合は、各ポイントが表す時間数をチーム設定で既に指定している必要があります。）</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>このストーリーを作成するプロジェクトの名前の入力を開始し、ドロップダウンリストに表示されたら名前をクリックします。<br>プロジェクトのステータスは [!UICONTROL Current] に設定する必要があります。プロジェクトのステータスが [!UICONTROL Current] 以外の場合は、ドロップダウンメニューには表示されません。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>（オプション）このストーリーが従属する親タスクの名前の入力を開始し、ドロップダウンリストに表示されたら、名前をクリックします。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> （オプション）このストーリーに追加するカスタムフォームを選択します。</td>
     </tr>
    </tbody>
   </table>

1. 「**[!UICONTROL ストーリーを保存]**」をクリックします。

### アジャイルチームにタスクまたはイシューを割り当てる {#assign-a-task-or-issue-to-an-agile-team}

アジャイルチームにタスクまたはイシューを割り当てることができます。 割り当て後、タスクまたはイシューはチームバックログに新しいストーリーとして表示されます。

アジャイルチームにタスクまたはイシューを割り当てるには：

1. 割り当てるタスクを含むプロジェクトに移動します。
1. リストからタスクまたはイシューを選択します。
1. 「**[!UICONTROL 編集]**」をクリックします。
1. 「**[!UICONTROL 割り当て]**」をクリックします。
1. （オプション）既存の担当者を削除します。
1. 「**[!UICONTROL 割り当て先を追加]**」をクリックします。
1. タスクまたはイシューに割り当てるアジャイルチームの名前の入力を開始し、ドロップダウンリストに表示されたらチーム名をクリックします。
1. 「**[!UICONTROL 変更を保存]**」をクリックします。
タスクまたはイシューがチームのバックログで利用できるようになりました。

## バックログ内にストーリーを移動またはバックログからストーリーを移動

* [バックログからイテレーションまたはボードへのストーリーの移動](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [既存のストーリーをバックログに移動する](#move-existing-stories-to-the-backlog)
* [バックログからストーリーを書き出す](#export-stories-from-the-backlog)

### バックログからイテレーションまたはボードへのストーリーの移動

1. アジャイルチームのバックログに移動します。
1. 反復またはかんばんボードに移動するストーリーを選択し、**[!UICONTROL 詳細]**/**[!UICONTROL 移動先]** をクリックします。
ストーリーを [!UICONTROL  かんばん ] ボードに移動すると、「[!UICONTROL  ストーリーをかんばん ] ボードに移動」が表示されます。
ストーリーをある反復に移動させる場合、[!UICONTROL ストーリーを反復に移動]ダイアログボックスが表示されます。
   ![ストーリーを移動ダイアログ](assets/agile-backlog-addtoiteration.png)

1. 次のいずれかの操作を行います。

   * **スクラムチームの場合：**「**[!UICONTROL 反復の選択]**」フィールドで、ストーリーを移動する反復を選択します。

   * **かんばんチームの場合：**「**[!UICONTROL かんばんボードの選択]**」フィールドで、チームの[!UICONTROL かんばん]ボードを選択します。（かんばんチームは 1 つの[!UICONTROL かんばん]ボードのみを持つことができます。）

1. 「**[!UICONTROL ストーリーを移動]**」をクリックします。

### 既存のストーリーをバックログに移動 {#move-existing-stories-to-the-backlog}

チームがまだストーリーに取り組む準備ができていないと判断した場合は、ストーリーをバックログに移動できます。

詳しくは、[ アジャイルストーリーの移動 ](../../agile/work-in-an-agile-environment/move-an-agile-story.md) を参照してください。

### バックログからストーリーの書き出し {#export-stories-from-the-backlog}

バックログから直接 1 つ以上のストーリー（タスクやイシューを含む）を書き出すことができます。

[データの書き出し](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)の説明に従って、[!DNL Workfront] でその他のデータを書き出すのと同じ方法でバックログからストーリーを書き出します。
