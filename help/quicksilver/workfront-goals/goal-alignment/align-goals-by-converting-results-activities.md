---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 結果とアクティビティを目標に変換して目標を連携
description: 2 つの目標を手動で連携させたり、既存の目標の結果やアクティビティを別の目標に変換したりできます。変換された結果やアクティビティは、元の目標の子目標になります。2 つの目標を手動で連携させる方法について詳しくは、目標を Adobe Workfront Goals に結び付けて連携を参照してください。
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 89%

---

# 結果とアクティビティを目標に変換して目標を連携

2 つの目標を手動で連携させたり、既存の目標の結果やアクティビティを別の目標に変換したりできます。変換された結果やアクティビティは、元の目標の子目標になります。
2 つの目標を手動で連携させる方法について詳しくは、[目標を Adobe Workfront Goals に結び付けて連携](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)を参照してください。

## アクセス要件


<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront プラン</td>
 <td>
 <p>任意</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront ライセンス*</td>
 <td>
 <p>新規ライセンス：コントリビューター以上</p>
 または
 <p>現在のライセンス：リクエスト以上</p> <p>詳しくは、<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront ライセンスの概要</a>を参照してください。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">製品*</td>
 <td>
 <p> 新製品の要件は、次のいずれかです。 </p>
<ul>
<li>Select または Prime Adobe Workfront プランと、追加のAdobe Workfront Goals ライセンス。</li>
<li>Workfront Goals をデフォルトで含む究極のWorkfront プラン。 </li></ul>
 <p>または</p>
 <p>現在の必要な製品：Workfront プランとAdobe Workfront Goals の追加ライセンス。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">アクセスレベル</td>
 <td> <p>Goals への編集アクセス権</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">オブジェクト権限</td>
 <td>
  <div>
  <p>目標の表示には表示権限以上が必要</p>
  <p>目標に対する編集権限を管理</p>
  <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューに目標エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. 目標に変換する結果またはアクティビティがある目標に移動します。
1. 目標のページで、左側のパネルの「**進捗インジケーター**」をクリックします。
1. 進捗インジケーターのリストで結果またはアクティビティを選択し、**目標に変換**&#x200B;アイコン ![](assets/convert-to-goal-icon-unshimmed.png) をクリックします。「目標に変換」ボックスが開きます。

   ![](assets/convert-to-goal-box-unshimmed.png)
1. 次の情報を更新します。
   * **目標名**：デフォルトでは、新しい目標は、元の結果やアクティビティと同じ名前になります。
   * **期間**：デフォルトでは、新しい目標の期間は現在の四半期になります。「**カスタム日付を有効にする**」設定を選択して、新しい目標のカスタム期間を定義します。
   * **目標の所有者**：デフォルトでは、目標の新しい所有者は、元の結果またはアクティビティの所有者になります。
   * **説明**：新しい目標に関する詳細情報を追加します。
1. 「**保存**」をクリックします。

   これで、結果またはアクティビティが、元の目標の子目標に変換されます。その後、元の目標の進捗状況インジケーターリストに目標として表示されます。



