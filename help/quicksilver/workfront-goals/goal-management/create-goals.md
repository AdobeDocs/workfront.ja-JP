---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals での目標の作成
description: CEO、マネージャー、または個人の投稿者であっても、Adobe Workfront Goals で目標を作成し、自分の作業を、自分の目標や組織の戦略を概略化した目標に合わせることができます。
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 86%

---

# Adobe Workfront Goals での目標の作成

CEO、マネージャー、または個人の投稿者であっても、Adobe Workfront Goals で目標を作成し、自分の作業を、自分の目標や組織の戦略を概略化した目標に合わせることができます。

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
<p>目標の表示には表示権限以上が必要</p>
<p>目標に対する編集権限を管理</p>
<p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p>
</td>
</tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューに目標エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 目標作成のガイドライン

Workfront Goals を開始する前に、ベストプラクティスに関する推奨事項と、目標を効果的に管理するためのガイドラインをお読みになることをお勧めします。目標の作成と管理に関するガイドラインについて詳しくは、[Adobe Workfront Goals の概要](../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。

## 目標を作成

この記事では、Workfront Goals で戦略目標を作成する方法について説明します。ビジネスケースの目標の作成について詳しくは、[ビジネスケース目標を作成](../../manage-work/projects/define-a-business-case/create-business-case-goals.md)を参照してください。

次のいずれかの方法で戦略目標を作成できます。

* [ゼロから目標を作成](#create-a-goal-from-scratch)
* [既存の目標をコピー](#copy-an-existing-goal)
* [結果またはアクティビティを目標に変換](#convert-a-result-or-activity-to-a-goal)

### ゼロから目標を作成 {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
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

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. 右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**目標**」の順にクリックします。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   目標リストが表示されます。
1. 「**新しい目標**」をクリックします。

   「新しい目標」ボックスが表示されます。

   ![](assets/new-goal-box-unshimmed.png)

1. 次のフィールドに情報を入力します。
   * **目標名**：目標の名前を入力します。必須フィールドです。
   * **期間**：事前に定義された四半期または年を&#x200B;**期間**&#x200B;ドロップダウンフィールドから選択します。

     または

     「**カスタム日付を使用**」オプションを選択して、目標の「**開始**」および「**終了日**」を選択します。

     前年、今年、翌年とそれぞれの四半期が、事前定義されたオプションとして期間ドロップダウンフィールドにリストされます。

     目標の期間は、目標が完了すると予想される期間を示します。

   * **目標の所有者**：目標の所有者を示すために、ユーザー、チーム、グループ、または組織の名前の入力を開始します。デフォルトでは、目標の所有者が選択されています。
   * **説明**：目標に関する追加情報を入力します。
1. 「**目標を作成**」をクリックします。

   新しい目標が目標リストに一覧表示され、**ドラフト**&#x200B;のステータスになります。

   目標をアクティブ化し、作業を開始するには、目標を進行状況インジケーターに関連付ける必要があります。

   アクティブ化する目標を準備するには、次のうち 1 つ以上を実行します。
   * 結果を追加する

     結果の追加について詳しくは、[Adobe Workfront Goals で目標に結果を追加](../results-and-activities/add-results-to-goals.md)を参照してください。
   * アクティビティを追加する

     アクティビティの追加について詳しくは、[Adobe Workfront Goals の目標へのアクティビティの追加](../results-and-activities/add-activities-to-goals.md)を参照してください。
   * 別の目標を整合させる

     目標の整合について詳しくは、[Adobe Workfront Goals で目標をに結び付けて整合させる](../goal-alignment/align-goals-by-connecting-them.md)を参照してください。


### 既存の目標をコピーする {#copy-an-existing-goal}

既存の目標をコピーして、目標を作成できます。

目標のコピーについて詳しくは、[Adobe Workfront Goals で目標をコピー](../../workfront-goals/goal-management/copy-goals.md)を参照してください。

### 結果またはアクティビティを目標に変換 {#convert-a-result-or-activity-to-a-goal}

既存の目標の結果やアクティビティを目標に変換することで、目標を作成できます。新しい目標は、元の目標に一致するように調整されます。

結果とアクティビティを目標に変換する方法について詳しくは、[Adobe Workfront Goals で目標をに結び付けて整合させる](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)を参照してください。

