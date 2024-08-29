---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront Goals で目標に結果を追加する方法
description: 結果は、目標の進捗を測定します。結果、アクティビティや整合された目標を目標に関連付けないと、目標をアクティブ化できず、目標に対する進捗を記録できません。
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 88%

---

# Adobe Workfront Goals で目標に結果を追加する方法

結果は、目標の進捗を測定します。結果、アクティビティや整合された目標を目標に関連付けないと、目標をアクティブ化できず、目標に対する進捗を記録できません。

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
  <ul><li>究極の計画 </li></ul>
   </p>
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
 <td> <p>Goals への編集アクセス権</p>  </td>
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

## 前提条件

開始するには、まず以下が必要です。

* メインメニューの Workfront Goals 領域を含んだレイアウトテンプレート。
* 既存の目標。

  目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。

>[!IMPORTANT]
>目標には、合計 1000 件以上のアクティビティ、結果、プロジェクト、整合された目標を含めることはできません。

## 目標に結果を追加

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. メインメニュー ![](assets/main-menu-icon.png) をクリックし、続いて「**目標**」をクリックします。

1. **目標リスト**&#x200B;で目標の名前をクリックし、目標ページを開きます。
1. 左側のパネルの「**進捗状況インジケーター**」をクリックします。
1. **新規進捗状況インジケーター**&#x200B;ドロップダウンメニューを展開し、「**結果を作成**」をクリックします。

   新規結果ボックスが開きます。

   ![](assets/new-result-box-unshimmed.png)

1. 結果の名前を「**結果名**」フィールドに入力します。必須フィールドです。
1. （オプション）結果を別のユーザーに割り当てる場合は、「**結果の所有者**」フィールドから自分の名前を削除します。デフォルトでは、アクティビティを作成したユーザーが所有者となります。

   >[!NOTE]
   >
   >チーム、グループや会社を結果の所有者として割り当てることはできません。

1. 「**どのように結果を測定したいですか？」で、以下のように行います。** エリアで、以下の情報を指定します。
   * **値のタイプ**：結果の進捗を測定する方法を示します。進捗状況は、数値、パーセント値、または通貨額で測定することができます。

     次の表に示すオプションから値のタイプを選択します。

     | 値のタイプ | 説明 |
     |---------------------------------------------------------|------------------|
     | 数値 | 数値 |
     | % | 割合（%） |
     | CN¥、DKK、KR、Mex$、R、R$、zł、£、¥、€、₹、฿、MYR、₪、$ | 通貨の値 |

   * **初期値**：結果の進捗状況が記録される前の、結果が最初に持つ値。
   * **ターゲット値**：結果が完了したとみなされる時点での、その結果が達成しようとする値。
1. 「**結果を作成**」をクリックします。

   結果は、目標ページの結果グループの下の「進捗状況インジケーター」セクションに表示されます。

   目標をアクティブ化した後で、結果の進捗状況を更新すると、目標の進捗状況も自動的に更新されます。目標のアクティブ化について詳しくは、[Adobe Workfront Goals で目標をアクティブ化](../goal-management/activate-goals.md)を参照してください。
