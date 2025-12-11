---
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront でのビューの作成または編集
description: ビューを使用して、画面に表示する情報のタイプをカスタマイズできます。Adobe Workfront では、複数のタイプのビューを使用できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 63%

---

# Adobe Workfront でのビューの作成または編集

<!-- Audited: 11/2024 -->

ビューを使用して、画面に表示する情報のタイプをカスタマイズできます。Adobe Workfront では、複数のタイプのビューを使用できます。

この記事では、リストおよびレポートの標準ビューを作成および編集する方法について説明します。

詳しくは、[Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)を参照してください。

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
   <td role="rowheader">Adobe Workfront プラン</strong></td> 
   <td> 
    <p>投稿者以上</p>
    <p>リクエスト以上</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポートのビューを作成するために、レポート、ダッシュボード、カレンダーへの編集アクセス権</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートのビューを作成または編集するために、レポートに対する管理権限</p> <p>編集するために、ビューに対する管理権限</p>
   </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## ビューの作成またはカスタマイズ

ビューの作成またはカスタマイズの手順は、標準ビュー、アジャイル ビュー、ボード ビューのどちらを作成またはカスタマイズするかによって異なります。

* [標準ビューを作成またはカスタマイズ](#create-or-customize-a-standard-view)
* [アジャイルビューを作成またはカスタマイズ](#create-or-customize-an-agile-view)

### 標準ビューを作成またはカスタマイズ {#create-or-customize-a-standard-view}

標準ビューを新規作成するか、以前作成した既存の標準ビューをカスタマイズすることができます。

1. ビューを作成またはカスタマイズするリストの&#x200B;**表示**&#x200B;ドロップダウンメニューをクリックします。

1. 「**+新規ビュー**」ボタンをクリックして、新規ビューを作成します。
または
編集する既存のビューの右側にマウスポインターを置くと表示される **編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。
**ビューをカスタマイズ**&#x200B;ダイアログボックスが表示されます。

1. 「**列のプレビュー**」セクションで、以下のいずれかを行います。

   * 列のタイトルをクリックし、新しいフィールドを選択して、列の値を変更します。
   * 「**列を追加**」をクリックして列を追加し、追加する列の名前を入力し、ドロップダウンリストに表示されたらクリックします。
   * 列のタイトルを新しい場所にドラッグして、列の表示順序を調整します。

   * [**列の設定**] 領域で、[**この列の集計方法**] をクリックし、列でのデータの表示方法を選択します。 このオプションは、次の列タイプで使用できます。
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>日付フィールド</strong></td> 
           <td><ul>
           <li>最大</li>
         <li>最小</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>通貨フィールド</strong></td> 
           <td><ul>
           <li>カウント</li>
         <li>合計</li>
           <li>平均</li>
         <li>最大</li>
           <li>最小</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>文字列フィールドとブール値フィールド</strong></td> 
           <td><ul><li>カウント</li></ul>
           <p>メモ：値は常に true または false なので、Workfrontは通常、ブール値フィールドをカウントで要約することはお勧めしません。</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >グループ化の次のフィールドの値を要約する場合、親オブジェクト（親タスクなど）に次の例外が適用されます：
     >   
     > * 「実績時間数」を除くすべての数値および通貨フィールド（たとえば、「予定/実績労力コスト」、「予定/実績費用コスト」、「予定/実績コスト」、「予定時間数」）は、子タスクとスタンドアロンタスクのみの値を要約します。 親タスクの値や親の親の値は集計されません。
     > * 実績時間では、メインの親タスクとスタンドアロン・タスクの値が要約されます。親タスクまたは子タスクの親の数値は要約されません。
     > * 数値および通貨値のカスタム データ フィールドには、親、子、親の親、およびスタンドアロン タスクのすべてのタスクが要約されます。
     >
     >レポートでのグループ化の使用について詳しくは、[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

      * （オプション）**「詳細」オプション**&#x200B;をクリックして、列に以下の情報を指定します。

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>カスタム列ラベル</strong></td> 
           <td><p>列のカスタムラベルを指定します。このラベルは、デフォルトのラベルを置き換えます。 互換性の問題を回避するには、UTF-8 文字のみを使用することをお勧めします。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>フィールド形式</strong></td> 
           <td>列のフィールドに値を表示する形式を選択します。</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>ダッシュボードにこのカラムを表示</strong></td> 
           <td><p>このオプションを選択すると、レポートが別のレポートと並べて表示される際に、この列がダッシュボードに表示されます。このオプションを選択しない場合、レポートが並べて表示されるダッシュボードでレポートを表示する際に、この列は表示されません。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>カラムのルール</strong></td> 
           <td><p>「<strong>+この列にルールを追加」をクリックして </strong> 列のルールを定義します。 ルールを追加した後、そのルールに一致するフィールドの表示方法について、フィールドとテキストのスタイルを定義できます。ルールの定義が完了したら、「<strong>ルールを追加</strong>」をクリックします。</p></td> 
          </tr> 
         </tbody> 
        </table>

        レポートのビューを条件付きで書式設定する方法について詳しくは、[テキストモードでの条件付き書式の使用](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)の記事を参照してください。

1. （条件付き）**「詳細」オプション**&#x200B;をクリックした場合は、「**完了**」をクリックします。

1. 「**ビューを保存**」をクリックしてビューを新規作成するか、現在のビューを変更して置き換えます。\
   または\
   「**新規ビューとして保存**」をクリックして、変更を新規ビューとして保存します。

   >[!TIP]
   >
   >「**新規ビューとして保存**」は、ビルトインの Workfront ビューをカスタマイズした場合に使用できる唯一のオプションです。

   アクセス権によって、ビューの保存方法が決まります。最初にビューを作成した場合は、変更を保存できます。それ以外の場合は、バージョンを保存するよう求められます。ビューに加えた変更は、そのビューを共有しているユーザーに影響を与えることに注意してください。

### アジャイルビューを作成またはカスタマイズ {#create-or-customize-an-agile-view}

アジャイルビュー（ボードビューとも呼ばれます）は、プロジェクト上のタスクとイシューのリストに対してのみ表示されます。

これらは事前に設定されていますが、特定の設定を変更できます。

アジャイル ビューまたはボード ビューの詳細については、「[ アジャイル ビューでプロジェクトを管理する ](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)」を参照してください。

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
