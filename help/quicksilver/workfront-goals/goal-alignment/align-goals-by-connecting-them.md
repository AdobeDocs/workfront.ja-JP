---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 目標をAdobe Workfront目標に結び付けて整列させる
description: 個人の目標を持つ個人の投稿者の場合は、組織の戦略の大きなコンテキストで自分の目標の進捗を効果的に表示するために、チームの目標に合わせて目標を調整することができます。
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# 目標をAdobe Workfront目標に結び付けて整列させる


個人の目標を持つ個人の投稿者の場合は、組織の戦略の大きなコンテキストで自分の目標の進捗を効果的に表示するために、チームの目標に合わせて目標を調整することができます。

組織の全員が目標を組織の目標に合わせて決めれば、個人の貢献やチームの取り組みが、より大きな企業レベルの優先事項に進むためにどのように役立つかを明確に確認できます。 目標を揃えるためのベストプラクティスについて詳しくは、 [Adobe Workfront目標の目標揃えの概要](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Adobe Workfront目標で目標を結び付けるには、次の 2 つの方法があります。

* 目標を相互に結び付けることで、目標間の整列を作成できます。

* 2 つの目標を手動で整列させたり、既存の目標の結果やアクティビティを別の目標に変換したりできます。 変換された結果またはアクティビティが、元の目標の子目標になります。

>[!IMPORTANT]
>
>目標には、合計 1000 個の進行状況インジケーターを設定できます。

この記事では、目標を相互に結び付けることで、目標を整列させる方法について説明します。 結果とアクティビティを目標に変換して目標を調整する方法について詳しくは、 [結果とアクティビティを目標に変換して目標を揃える](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## アクセス要件

<!--drfated for the P&P release: 

You must have the following:

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

## 目標を相互に結び付けて整列させる

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. 整列する 2 つの目標を作成します。 目標の作成について詳しくは、 [Adobe Workfront目標での目標の作成](../../workfront-goals/goal-management/create-goals.md).
1. （オプション）整列させる目標をアクティブ化します。 ステータスが「ドラフト」、「アクティブ」または「非アクティブ」の目標を整列できます。 目標のアクティブ化について詳しくは、 [Adobe Workfront目標で目標を有効化](../../workfront-goals/goal-management/activate-goals.md).
1. 別の目標（親目標）に整列させる目標（子目標）に移動し、その名前をクリックして目標ページを開きます。

   >[!INFO]
   >
   >たとえば、目標 2 が目標 1 の進行状況に影響を与えたい場合は、目標 2 に進む必要があります。

1. クリック **目標の詳細** をクリックします。

1. 内 **親目標情報** 領域、クリック **追加** 内 **親目標** 親目標がない場合はフィールド

   または

   別の名前を選択するには、親目標の名前をクリックします。

1. 既存の目標の名前を **親目標** フィールドに値を入力し、リストに表示されるときに選択します。 同じ期間または将来の期間に属する目標のみがリストに表示されます。

1. クリック **変更を保存**.

   （目標 2）から始めた目標は、それに合わせた親目標（目標 1）の子目標になります。\
   「目標の位置合わせ」セクションで、目標 2 を目標 1 の 2 次として連結した位置合わせ目標が表示されます。
子目標は、親目標の進捗状況が更新されると、親目標の「進捗状況インジケーター」セクションに表示されます。

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. （オプション）目標の整列セクションで目標を表示するには、Workfrontの目標領域に移動し、 **目標の整列** 」セクションを使用して、 [ 目標の位置合わせ ] セクションの詳細については、 [Adobe Workfront目標の目標の目標揃えセクションに移動](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. （オプション）いずれかの目標に、進行状況を示すアクティビティと結果を追加します。 アクティビティと結果の追加について詳しくは、次の記事を参照してください。

   * [Adobe Workfront目標での目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Adobe Workfront目標の目標に結果を追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. （オプション）組織の全体的な戦略とは関係なくなったと考える場合に、2 つの目標の整合を解除します。 目標間の位置揃えの削除について詳しくは、 [Adobe Workfront目標の目標の整合を削除](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

