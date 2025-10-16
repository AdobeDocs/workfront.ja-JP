---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 結果とアクティビティを目標に変換して目標を連携
description: 2 つの目標を手動で連携させたり、既存の目標の結果やアクティビティを別の目標に変換したりできます。変換された結果やアクティビティは、元の目標の子目標になります。2 つの目標を手動で連携させる方法について詳しくは、目標を Adobe Workfront Goals に結び付けて連携を参照してください。
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 79%

---

# 結果とアクティビティを目標に変換して目標を連携

<!--Audited P&P only: 4/2025-->

2 つの目標を手動で連携させたり、既存の目標の結果やアクティビティを別の目標に変換したりできます。変換された結果やアクティビティは、元の目標の子目標になります。
2 つの目標を手動で連携させる方法について詳しくは、[目標を Adobe Workfront Goals に結び付けて連携](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)を参照してください。

## アクセス要件

>[!NOTE]
>
>過去にこのパッケージを購入したことがある会社は、Adobe Workfront Goals を引き続き使用する場合があります。 詳細については、アカウント担当者にお問い合わせください。
>
>Adobe Workfront Goals は購入できなくなりました。

+++展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<td> <p>Adobe Workfront パッケージ</p> </td> 
   <td> 
   <p>Adobe WorkfrontUltimate</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront プラン</p> </td> 
   <td> <p>投稿者以上</p> 
     <p>要求者以上</p> </td> 
  </tr>

<td><p>アクセスレベル設定</p> </td> 
   <td> <p>Goals への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td> <p>オブジェクト権限 </p> </td> 
   <td> <p>目標に対する権限の管理</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>システム管理者を含むすべてのユーザーには、メインメニューの目標エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
 </tbody> 
</table>

詳しくは、[Workfrontへのアクセス要件ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

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
   <p> New product requirement: Workfront</p>
   Or
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

## 前提条件

開始するには、まず以下が必要です。

* 既存の結果とアクティビティを含む既存の目標。

  目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。

>[!IMPORTANT]
>
>目標には、最大 1000 個の進捗インジケーターを設定できます。

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## 結果やアクティビティを目標に変換する際の考慮事項

結果やアクティビティの範囲が予想よりも大きくなって、目標となる方が理にかなっている場合があります。既存の目標の結果やアクティビティを新しい目標に変換できます。これは、目標を連携させるためのボトムアップアプローチです。

結果やアクティビティを目標に変換する際は、次の点を考慮してください。

* 変換された結果またはアクティビティが元の目標の子目標になり、2 つの目標が連携します。
* 元の目標に関する追加の結果やアクティビティがない場合、新しく作成された目標は、元の目標の単一の進捗インジケーターになります。子の目標に対する進捗をトラックするには、結果とアクティビティを追加する必要があります。
* 結果またはアクティビティを目標に変換すると、元に戻せなくなります。変換すると、新しい子目標を再び親目標の結果やアクティビティにすることはできなくなります。

## 結果またはアクティビティを目標に変換

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![Convert to goal](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. 目標に変換する結果またはアクティビティがある目標に移動します。
1. 目標のページで、左側のパネルの「**進捗インジケーター**」をクリックします。
1. 進捗インジケーターのリストで結果またはアクティビティを選択し、進捗インジケーターリストの上部にある **目標に変換** アイコン ![&#x200B; 目標に変換 &#x200B;](assets/convert-to-goal-icon-unshimmed.png) をクリックします。 「目標に変換」ボックスが開きます。

   ![&#x200B; 目標に変換ボックス &#x200B;](assets/convert-to-goal-box-unshimmed.png)
1. 次の情報を更新します。
   * **目標名**：デフォルトでは、新しい目標は、元の結果やアクティビティと同じ名前になります。
   * **期間**：デフォルトでは、新しい目標の期間は現在の四半期になります。「**カスタム日付を有効にする**」設定を選択して、新しい目標のカスタム期間を定義します。
   * **目標の所有者**：デフォルトでは、目標の新しい所有者は、元の結果またはアクティビティの所有者になります。
   * **説明**：新しい目標に関する詳細情報を追加します。
1. 「**保存**」をクリックします。

   これで、結果またはアクティビティが、元の目標の子目標に変換されます。その後、元の目標の進捗状況インジケーターリストに目標として表示されます。



