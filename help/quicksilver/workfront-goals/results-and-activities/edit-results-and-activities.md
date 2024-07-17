---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront Goals での結果とアクティビティの編集
description: Adobe Workfront 管理者から Adobe Workfront Goals への適切なアクセス権が付与されたら、目標、結果およびアクティビティを作成および編集できるようになります。
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 89%

---

# Adobe Workfront Goals での結果とアクティビティの編集

Adobe Workfront 管理者から Adobe Workfront Goals への適切なアクセス権が付与されたら、目標、結果およびアクティビティを作成および編集できるようになります。

目標、結果、アクティビティの作成について詳しくは、次の記事を参照してください。

* [Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)
* [Adobe Workfront Goals での結果とアクティビティの編集に関する基本を学ぶ](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Adobe Workfront Goals の目標への結果の追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Adobe Workfront Goals の目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

## アクセス要件

以下が必要です。

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
   <p>新しいプランとライセンス構造の場合：
  <ul><li>究極の計画 </li>
  または
  <li>Prime プランまたは Select Adobe Workfront プランのAdobe Workfront Goals の追加ライセンス。 </li></ul> </p>
<p>現在のプランおよびライセンス構造の場合： 
<ul><li> プロまたはそれ以上 </li>
  <li>Workfront ライセンスに加えて、Adobe Workfront Goals ライセンス。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront プラン*</td>
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
 <td role="rowheader"><p>アクセスレベル</p></td>
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
   <td> <p>Workfront 管理者を含むすべてのユーザーには、メインメニューに「目標」エリアが含まれるレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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


1. **メインメニュー** ![](assets/main-menu-icon.png) をクリックして、「**目標**」をクリックします。
1. 目標リストで目標の名前をクリックし、目標ページを開きます。
1. 左パネルで「**進行状況インジケーター**」をクリックします。
1. 進行状況インジケーターリストで結果を選択し、**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。

   「結果を編集」ボックスが開きます。

   ![](assets/edit-result-box-unshimmed.png)

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
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. **メインメニュー** ![](assets/main-menu-icon.png) をクリックして、「**目標**」をクリックします。
1. 目標リストで目標の名前をクリックし、目標ページを開きます。
1. 左パネルで&#x200B;**進行状況インジケーター**&#x200B;をクリックします。
1. 進行状況インジケーターリストでアクティビティを選択し、**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。

   「アクティビティを編集」ボックスが開きます。

   ![](assets/edit-activity-box-unshimmed.png)

1. 次の情報を編集します。
   * **アクティビティの名前**：アクティビティの名前。目標の完了を示すために実行しなければならないアクティビティを説明する、わかりやすい名前を付けます。
   * **アクティビティの所有者：**&#x200B;アクティビティの所有者。所有者は、アクティブな Workfront ユーザーである必要があります。\
     「アクティビティ」フィールドについて詳しくは、[目標へのアクティビティの追加](../results-and-activities/add-activities-to-goals.md)を参照してください。
1. 「**保存**」をクリックします。


