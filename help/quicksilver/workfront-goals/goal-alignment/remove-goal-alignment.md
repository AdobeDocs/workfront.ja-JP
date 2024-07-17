---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Adobe Workfront Goals での目標の整合性の削除
description: 2 つの目標を接続しても意味がない場合は、それらの目標間の整合性を削除できます。
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 90%

---

# Adobe Workfront Goals での目標の整合性の削除

2 つの目標を接続しても意味がない場合は、それらの目標間の整合性を削除できます。

目標の整合について詳しくは、次の記事を参照してください。

* [目標を Adobe Workfront 目標に結び付けて整合させる](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [結果とアクティビティを目標に変換して目標を連携](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## アクセス要件

以下が必要です。

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
 <td role="rowheader">Adobe Workfront プラン*</td>
 <td>
 <p>新規ライセンス：コントリビューター以上</p>
 または
 <p>現在のライセンス：リクエスト以上</p> </td>
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
  <p>目標の表示には表示権限以上が必要</p>
  <p>目標に対する編集権限を管理</p>
  <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p>
  </td>
 </tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者を含むすべてのユーザーには、メインメニューに「目標」エリアが含まれるレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 前提条件

開始するには、まず以下が必要です。

* 親目標に、1 つ以上の子目標が関連付けられている。子の目標は、目標の進捗状況インジケーターです。

## 目標の整合性の削除に関する考慮事項

2 つの目標間の整合性を削除する際は、次の点を考慮してください。

* 親目標をアクティブに保つには、別の目標、アクティビティ、または結果が関連付けられている必要があります。
* 関連付けられた子目標が、親目標の唯一の進捗インジケーターである場合、関連付けられた子目標は削除できません。
* 子目標は、親目標との整合を外すと、スタンドアロンの目標になります。

## 目標の整合性の削除

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Workfront の&#x200B;**目標**&#x200B;エリアにアクセスし、目標の名前をクリックして、目標のページを開きます。
1. 親目標の目標ページで、左パネルの&#x200B;**進行状況インジケーター**&#x200B;をクリックします。

   ![](assets/remove-goal-alignment-from-list-unshimmed.png)

1. **タイプ：目標**&#x200B;グループ化を選択し、目標を選択して、リストの上の&#x200B;**連携解除**&#x200B;アイコン![](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png)をクリックします。

   連携解除ボックスが表示されます。

1. 「**連携解除**」をクリックし、選択した目標を親から切断します。

   目標はスタンドアロンの目標になり、元の目標の進捗状況インジケーターとして表示されなくなります。接続解除された目標の進行状況は、元の目標の進行状況に影響を与えなくなりました。

   成功メッセージがページの右上隅に表示され、目標が連携解除されたことを確認できます。