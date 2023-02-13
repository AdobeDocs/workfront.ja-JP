---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront目標で結果とアクティビティを編集
description: Adobe Workfront管理者からAdobe Workfront目標への正しいアクセス権が付与されたら、目標、結果およびアクティビティを作成および編集できます。
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 1%

---

# Adobe Workfront目標で結果とアクティビティを編集

Adobe Workfront管理者からAdobe Workfront目標への正しいアクセス権が付与されたら、目標、結果およびアクティビティを作成および編集できます。

目標、結果、アクティビティの作成について詳しくは、次の記事を参照してください。

* [Adobe Workfront目標での目標の作成](../../workfront-goals/goal-management/create-goals.md)
* [Adobe Workfront目標の結果とアクティビティの概要](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Adobe Workfront目標の目標に結果を追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Adobe Workfront目標での目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

## アクセス要件

<!--drafted for P&P release: replace the table below with this: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->
以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リクエスト以上</p> <p>詳しくは、 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfrontライセンスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、 Adobe Workfront Goals の追加ライセンスを購入する必要があります。 </p> <p>詳しくは、 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront目標の使用要件</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>目標へのアクセスを編集</p> <p><b>メモ</b>

<p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、以下を参照してください。</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront目標へのアクセス権の付与</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <div> 
     <p>目標に対する権限の管理</p> 
     <p>目標の共有について詳しくは、 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront目標での目標の共有</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 前提条件

を起動する前に、次の条件を満たす必要があります。

* メインメニューの目標領域を含むレイアウトテンプレート。

## 結果とアクティビティを編集する際の考慮事項

<!--
According to Vazgen, access levels will add more considerations.)
-->

* 作成した目標に属する結果やアクティビティ、または管理する権限を持つ目標を編集できます。
* 目標に関連するプロジェクトの進捗状況は、Workfront目標のアクティビティとして編集できません。 プロジェクトのタスクが完了すると、プロジェクトの進行状況が更新されます。 プロジェクトを切断することで、ゴールからプロジェクトを削除できます。 詳細については、この記事の「プロジェクトの切断」の節を参照してください [Adobe Workfront目標の目標から結果、アクティビティ、プロジェクトを削除](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).

   >[!NOTE]
   >
   >次のプロジェクト情報がプロジェクトレベルで更新されると、Workfront目標は目標レベルで自動的に更新します。
   >
   >   
   >   
   >   * プロジェクト所有者
   >   * プロジェクト名
   >   * プロジェクトの完了率

   >   
   >   
   >プロジェクトを目標に接続する方法について詳しくは、 [Adobe Workfront目標の目標へのプロジェクトの追加](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* 目標の進捗状況と関係がなくなった場合は、目標から結果やアクティビティを削除できます。 削除した結果とアクティビティは復元できません。 結果およびアクティビティの削除について詳しくは、 [Adobe Workfront目標の目標から結果、アクティビティ、プロジェクトを削除](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).
* 目標に関連付けられた結果やアクティビティは、過去を含め、任意の期間から編集できます。
* 結果やアクティビティを編集すると、設定が更新され、進行状況は更新されません。 結果とアクティビティの進行状況を更新する必要があります。 目標、結果およびアクティビティの進捗状況の更新について詳しくは、 [Adobe Workfront目標での目標の進捗状況の更新](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

## 結果を編集

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![](assets/results-gear-icon-options-350x85.png)

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


1. 次をクリック： **メインメニュー** ![](assets/main-menu-icon.png)を、 **目標**.
1. 「目標リスト」で目標の名前をクリックし、目標ページを開きます。
1. クリック **進行状況指標** をクリックします。
1. 進行状況インジケーターリストで結果を選択し、 **編集** アイコン ![](assets/edit-icon.png).

   「結果を編集」(Edit Result) ボックスが開きます。

   ![](assets/edit-result-box-unshimmed.png)

1. 次の情報を編集します。
   * **結果名**:結果の名前。 目標を完了するために取得する必要がある結果を示すわかりやすい名前を付けます。
   * **結果の所有者**:結果の所有者。 所有者は、アクティブなWorkfrontユーザーである必要があります。
   * **値のタイプ**:結果の進行状況を測定する方法。
   * **初期値**:結果の元の値。
   * **ターゲット値**:結果が完了したときの目的の値。
結果フィールドについて詳しくは、 [目標に結果を追加](../results-and-activities/add-results-to-goals.md).
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
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. 次をクリック： **メインメニュー** ![](assets/main-menu-icon.png)を、 **目標**.
1. 「目標リスト」で目標の名前をクリックし、目標ページを開きます。
1. クリック **進行状況指標** をクリックします。
1. 「進行状況指標」リストでアクティビティを選択し、 **編集** アイコン ![](assets/edit-icon.png).

   「アクティビティを編集」ボックスが開きます。

   ![](assets/edit-activity-box-unshimmed.png)

1. 次の情報を編集します。
   * **アクティビティ名**:アクティビティの名前。 目標が完了したことを示すために実行する必要があるアクティビティを示すわかりやすい名前を付けます。
   * **アクティビティ所有者：** アクティビティの所有者。 所有者は、アクティブなWorkfrontユーザーである必要があります。\
      アクティビティフィールドについて詳しくは、 [目標へのアクティビティの追加](../results-and-activities/add-activities-to-goals.md).
1. 「**保存**」をクリックします。


