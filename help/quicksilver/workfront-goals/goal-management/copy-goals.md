---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals で目標をコピーする
description: Adobe Workfront Goals の目標をコピーして目標を作成できます。元の目標情報の一部は新しい目標に転送されます。
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 86%

---

# Adobe Workfront Goals の目標をコピー

<!--Audited for P&P only: 4/2025-->

Adobe Workfront Goals の目標をコピーして目標を作成できます。元の目標情報の一部は新しい目標に転送されます。

## アクセス要件

>[!NOTE]
>
>過去にこのパッケージを購入したことがある会社は、Adobe Workfront Goals を引き続き使用する場合があります。 詳細については、アカウント担当者にお問い合わせください。
>
>Adobe Workfront Goals は購入できなくなりました。

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront パッケージ</p> </td> 
   <td> 
   <p>Adobe WorkfrontUltimate</p>
   </td> 
  </tr> 
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront プラン</td>
 <td>
 <p>投稿者以上</p>
 <p>リクエスト以上</p></td>
 </tr>
 <tr>
 <td role="rowheader">アクセスレベル設定</td>
 <td> <p>Goals への編集アクセス権</p> </td>
 </tr>
 <tr>
 <td role="rowheader">オブジェクト権限</td>
 <td>
  <div>
  <p>目標の表示には表示権限以上が必要</p>
  <p>目標に対する編集権限を管理</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>システム管理者を含むすべてのユーザーには、メインメニューの目標エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## 目標のコピーに関する考慮事項

目標をコピーする前に、アクセスレベルで目標を編集する権限が必要です。目標へのアクセス権の付与について詳しくは、[Adobe Workfront Goals へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)を参照してください。

既存の目標をコピーする理由の一部を次に示します。

* 期間（四半期または年）の終わりに、次の期間のために同じ目標を再作成する場合。
* 期間の終わりに、目標を完了できず、別の期間でその目標に取り組む場合。
* 複数のチームメンバーが同じ目標を持ち、それぞれに対して 1 つずつ作成する必要がある場合。

>[!TIP]
>
>目標は任意のステータスでコピーできます。目標ステータスについて詳しくは、[Adobe Workfront Goals の目標ステータスの概要](../../workfront-goals/goal-management/goal-status-overview.md)を参照してください。

目標をコピーする際は、次の点を考慮してください。

* 目標に関する情報もすべて新しい目標にコピーされます。
* 既存の目標の結果をコピーするように選択できます。結果の名前は新しい目標に転送されますが、既存の目標に関する結果の現在の進行状況は新しい目標にコピーされません。コピーした結果は、デフォルトで同じ所有者に割り当てられます。

  >[!NOTE]
  >
  >元の所有者が Workfront から削除または非アクティブ化にされた場合、新しい結果がログインユーザーに割り当てられます。

* 目標をコピーする際に、目標のアクティビティをコピーすることはできません。

## 目標をコピー

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >   
   >* Add a Result
   >   
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. 目標に移動して **詳細** メニュー ![ 詳細アイコン ](assets/more-icon.png) をクリックし、「**目標をコピー**」をクリックします。

   ![ 目標ボックスをコピー ](assets/copy-goal-box-unshimmed.png)

1. コピーした目標に関する次の情報を更新します。
   * **目標名**：新しい目標の名前。コピーされた目標のデフォルト名は、「Copy of &lt;元の目標>」です。
   * **期間**：目標を達成する期間。ドロップダウンメニューから期間を選択します。

     または

     「**カスタム日付を有効にする**」を選択して、目標の&#x200B;**開始日**&#x200B;と&#x200B;**終了日**&#x200B;のカスタム日付を指定します。「カスタム日付を有効にする」設定は、デフォルトでは無効になっています。

     >[!TIP]
     >
     >   「カスタム日付を有効にする」をオフにすると、元の目標の期間に戻ります。

      * **目標の所有者**：目標の所有者。ユーザー、チーム、グループ、会社のいずれかを指定できます。デフォルトは、元の目標の所有者です。
      * **説明**：目標に関する追加情報。
      * **結果をコピー**：現在の目標の結果をコピーした目標に転送する場合は、このオプションを選択します。これにより、元の結果が複製され、コピーしたゴールに添付されます。コピーしたゴールの結果には、元のゴールの結果と同じ所有者、名前、測定値が含まれます。

        >[!NOTE]
        >
        >* 元の結果の進行状況は、コピーされた目標には転送されません。
        >* 元の所有者が Workfront から削除または非アクティブ化にされた場合、新しい結果がログインユーザーに割り当てられます。

1. 「**目標をコピー**」をクリックします。

   元の目標と同様の目標が作成され、ステータスはドラフトになります。

   >[!NOTE]
   >
   >元の目標から結果をコピーしていない場合は、まず新しい目標を進捗状況インジケーターに関連付けてから、目標をアクティブ化して達成に向けて作業を開始する必要があります。
   >目標と進捗インジケーターの関連付けについて詳しくは、次の記事を参照してください。
   >* [Adobe Workfront Goals の目標に結果を追加](../results-and-activities/add-results-to-goals.md)
   >* [Adobe Workfront Goals の目標にアクティビティを追加](../results-and-activities/add-activities-to-goals.md)
   >* [目標を Adobe Workfront Goals に結び付けて連携](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >目標のアクティブ化について詳しくは、[目標をアクティブ化](../goal-management/activate-goals.md)を参照してください。

