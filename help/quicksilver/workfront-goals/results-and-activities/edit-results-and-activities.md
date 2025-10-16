---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront Goals での結果とアクティビティの編集
description: Adobe Workfront 管理者から Adobe Workfront Goals への適切なアクセス権が付与されたら、目標、結果およびアクティビティを作成および編集できるようになります。
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 81%

---

# Adobe Workfront Goals での結果とアクティビティの編集

Adobe Workfront 管理者から Adobe Workfront Goals への適切なアクセス権が付与されたら、目標、結果およびアクティビティを作成および編集できるようになります。

目標、結果、アクティビティの作成について詳しくは、次の記事を参照してください。

* [Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)
* [Adobe Workfront Goals での結果とアクティビティの編集に関する基本を学ぶ](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Adobe Workfront Goals の目標への結果の追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Adobe Workfront Goals の目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

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
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
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

## 結果とアクティビティの編集に関する考慮事項

<!--
According to Vazgen, access levels will add more considerations.)
-->

* 作成した目標や管理権限を持つ目標に属している結果やアクティビティを編集できます。
* Workfront Goals のアクティビティとして、目標に関連付けられているプロジェクトの進行状況を編集することはできません。プロジェクトのタスクが完了すると、プロジェクトの進行状況が更新されます。プロジェクトを切断すると、目標からプロジェクトを削除できます。詳しくは、[Adobe Workfront Goals の目標からの結果、アクティビティ、プロジェクトの削除](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md)の記事のプロジェクトの切断の節を参照してください。

  >[!NOTE]
  >
  >次のプロジェクト情報がプロジェクトレベルで更新されると、Workfront Goals は該当する情報を目標レベルで自動的に更新します。
  >
  >   
  >   
  >   * プロジェクト所有者
  >   * プロジェクト名
  >   * プロジェクトの完了率
  >   
  >   
  >プロジェクトを目標に接続する方法について詳しくは、[Adobe Workfront Goals の目標へのプロジェクトの追加](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)を参照してください。

* 結果やアクティビティが目標の進行状況に関係なくなった場合は、目標から削除できます。削除した結果とアクティビティは復元できません。結果とアクティビティの削除について詳しくは、[Adobe Workfront Goals の目標からの結果、アクティビティ、プロジェクトの削除](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md)を参照してください。
* 過去を含めた任意の期間で、目標に関連付けられた結果やアクティビティを編集できます。
* 結果とアクティビティを編集すると設定が更新されますが、進行状況は更新されません。結果とアクティビティの進行状況を更新する必要があります。目標、結果およびアクティビティの進行状況の更新について詳しくは、[Adobe Workfront Goals の目標の進行状況の更新](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md)を参照してください。

## 結果を編集

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![Results gear icon](assets/results-gear-icon-options-350x85.png)

1. Click **Edit** to edit the following information:

   | Field |Description|
   |---|---|
   | Name |The name of the result. |
   | Owner |The owner of result.  |
   | Value |How you measure the progress of the result. |
   | Initial |The original value of the result. |
   | Target |The desired value when the result is completed. |

1. Click **Save**.
-->


1. **メインメニュー**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**目標** をクリックします。
1. 目標リストで目標の名前をクリックし、目標ページを開きます。
1. 左パネルの「**進行状況インジケーター**」をクリックします。
1. 「進捗インジケーター」リストで結果を選択し、**編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。

   「結果を編集」ボックスが開きます。

   ![ 結果を編集ボックス ](assets/edit-result-box-unshimmed.png)

1. 次の情報を編集します。
   * **結果名**：結果の名前。目標を完了するために取得しなければならない結果を示す、わかりやすい名前を付けます。
   * **結果の所有者**：結果の所有者。所有者は、アクティブな Workfront ユーザーである必要があります。
   * **値のタイプ**：結果の進行状況の測定方法。
   * **初期値**：結果の元の値。
   * **ターゲット値**：結果が完了したときの望ましい値。
「結果」フィールドについて詳しくは、[目標への結果の追加](../results-and-activities/add-results-to-goals.md)を参照してください。
1. 「**保存**」をクリックします。

## アクティビティを編集

<!--
Editing activities differs depending on which environment you use.

### Edit activities in the Production environment

>[!TIP]
>
>You cannot edit the Activity Type after you saved an activity on a goal.

1. Go to the goal for which you want to edit an activity and click the goal name to open the **Goal Details** panel.
1. Click **Activities**.
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![Activities gear icon](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. **メインメニュー**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**目標** をクリックします。
1. 目標リストで目標の名前をクリックし、目標ページを開きます。
1. 左パネルの「**進行状況インジケーター**」をクリックします。
1. 「進捗インジケーター」リストでアクティビティを選択し、**編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。

   「アクティビティを編集」ボックスが開きます。

   ![ アクティビティを編集ボックス ](assets/edit-activity-box-unshimmed.png)

1. 次の情報を編集します。
   * **アクティビティの名前**：アクティビティの名前。目標の完了を示すために実行しなければならないアクティビティを説明する、わかりやすい名前を付けます。
   * **アクティビティの所有者：**&#x200B;アクティビティの所有者。所有者は、アクティブな Workfront ユーザーである必要があります。\
     「アクティビティ」フィールドについて詳しくは、[目標へのアクティビティの追加](../results-and-activities/add-activities-to-goals.md)を参照してください。
1. 「**保存**」をクリックします。


