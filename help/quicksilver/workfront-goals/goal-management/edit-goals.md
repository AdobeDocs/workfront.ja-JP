---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals で目標を編集する
description: 既存の目標を、任意の期間およびステータスで編集できます。
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 76%

---

# Adobe Workfront Goals の目標の編集

<!--Audited for P&P only: 10/2025-->

既存の目標を、任意の期間およびステータスで編集できます。

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
 <td role="rowheader">Adobe Workfront プラン</td>
 <td>
 <p>投稿者以上</p>
<p>リクエスト以上</p></td>
 </tr>
  <tr>
 <td role="rowheader">アクセスレベル設定</td>
 <td> <p>Goals への編集アクセス権</p> </td>
 </tr>
 <tr data-mc-conditions="">
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

## 目標の編集に関する考慮事項

* ステータスが「クローズ」の目標は編集できません。
* 任意の期間から目標を編集できます。

  過去の目標に関する次の情報を編集できます。

   * 名前
   * 期間
   * ステータス

     >[!TIP]
     >
     >目標がクローズの場合、その目標を再度開くと、進捗の完了率が再計算されます。クローズされた目標を編集することはできません。

   * 説明
   * 結果とアクティビティ

## 目標を編集

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. **メインメニュー** アイコン ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png) をクリックしてから、**目標** をクリックします。\
   目標のリストが表示されます。
1. 目標をクリックします。\
   目標ページが表示されます。

   ![&#x200B; 目標ページ &#x200B;](assets/goal-page-unshimmed.png)

1. 目標の情報を編集するには、次のいずれかを行います。
   * 目標ヘッダーに表示されるフィールドをクリックして更新します。ヘッダーの一部のフィールドは編集できません。
   * 目標名の右側にある **その他のアイコン**![&#x200B; その他のアイコン &#x200B;](assets/more-icon.png) をクリックし、**編集** をクリックします。
   * 左側のパネルで **目標の詳細** をクリックし、右上隅の **編集アイコン**![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックしてから、**すべて編集** をクリックします。 「目標の詳細」セクションのフィールドを更新します。

     >[!IMPORTANT]
     >
     >上記のエリアに表示されるフィールドの一部は編集できません。Workfront は一部のフィールドを計算しますが、このようなフィールドは読み取り専用です。

1. （条件付き）前の手順で選択した内容に応じて、目標に関する次の情報を更新します。

   * 目標ヘッダーの次の情報を更新し、Enter キーを押して変更を保存します。
      * **目標名**：目標の名前をクリックし、新しい名前を入力します。
      * **所有者**：所有者の名前をクリックして、ユーザー、チーム、グループまたは会社の名前を入力し、リストに表示されたら選択します。1 つの目標に対して所有者を 1 名だけ指定できます。
   * 目標の編集ボックスで次の情報を更新し、「**保存**」をクリックします。
      * **目標名**
      * **期間**：クリックして目標の期間を更新\
        または\
        「**カスタム日付を使用**」を選択して、目標の&#x200B;**開始**&#x200B;および&#x200B;**終了日**&#x200B;の日付を指定します。

        >[!TIP]
        >
        >「**カスタム日付を有効にする**」の選択を解除し、目標の元の期間に戻ります。

      * **目標の所有者**
      * **説明**：目標に関する情報を追加または更新します。
   * 「目標の詳細」セクションの情報を更新または確認します。詳しくは、[Adobe Workfront Goals の「目標の詳細」セクションでの目標の更新](../goal-management/update-goals-in-goal-details-panel.md)を参照してください。

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. （オプション）左側のパネルの「**進捗状況インジケーター**」をクリックして、目標に結果、アクティビティまたはプロジェクトを追加します。進捗状況インジケーターを追加することで、目標の進捗を確実にトラックできます。
詳しくは、次の記事を参照してください。
   * [Adobe Workfront Goals の目標へのアクティビティの追加](../results-and-activities/add-activities-to-goals.md)
   * [Adobe Workfront Goals の目標への結果の追加](../results-and-activities/add-results-to-goals.md)
   * [Adobe Workfront Goals の目標へのプロジェクトの追加](../results-and-activities/connect-projects-to-goals-overview.md)。


</div>
