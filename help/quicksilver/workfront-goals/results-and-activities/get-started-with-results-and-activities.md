---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront目標の結果とアクティビティの概要
description: 目標をアクティブ化するには、結果、アクティビティまたは整列した目標を目標に追加する必要があります。 これにより、目標のステータスがドラフトからアクティブに更新され、目標に関する進捗の記録が開始されます。
author: Alina
feature: Workfront Goals
exl-id: 64fa0aef-cb92-465a-9b74-d863fc232fd1
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Adobe Workfront目標の結果とアクティビティの概要

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>この記事で説明する機能を使用するには、以下が必要です。
>
>* プロ以上 [Adobe Workfrontプラン](https://www.workfront.com/plans).
>* Workfrontライセンスに加えて、Adobe Workfront Goals ライセンスが必要です。
>
>  Workfront Goals ライセンスについて詳しくは、Workfrontのアカウントマネージャーにお問い合わせください。
>
>Workfront Goals へのアクセスについて詳しくは、 [Workfront目標の使用要件](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


目標を作成すると、その目標のステータスは「ドラフト」になります。 目標の作成について詳しくは、 [Adobe Workfront目標での目標の作成](../../workfront-goals/goal-management/create-goals.md).

目標に関する進行状況の記録を開始するには、目標の記録を有効にする必要があります。 目標をアクティブ化し、そのステータスを「アクティブ」に変更するには、まず目標に次の情報を追加する必要があります。

* 結果
* アクティビティ
* プロジェクト
* 整列した目標

これらの項目の少なくとも 1 つを追加した後、目標をアクティブ化できます。 目標の結果とアクティビティを更新して、目標の進捗を示す必要があります。


>[!IMPORTANT]
>
> 目標には、合計 1000 個を超えるアクティビティ、結果、プロジェクト、または整列した目標を含めることはできません。</span>

この記事では、アクティビティと結果の概要を説明します。 目標の調整について詳しくは、 [Adobe Workfront目標の目標の調整](../../workfront-goals/goal-alignment/goal-alignment.md). プロジェクトを目標に接続する方法について詳しくは、 [Adobe Workfront目標の目標へのプロジェクトの追加](../results-and-activities/connect-projects-to-goals-overview.md).

## 結果の概要

<!--
<p> This will have additional types in the future - add another section for types?)</p>
-->

結果は、目標の進捗状況や達成に近い状況を測定します。 目標の所有者は、結果を所有することもできます。 目標に対する結果は、別のユーザーに割り当てられる場合もあります。

目標に結果を追加する方法について詳しくは、 [Adobe Workfront目標の目標に結果を追加](../../workfront-goals/results-and-activities/add-results-to-goals.md).

組織の他のエンティティに属する独自の目標または目標に結果を追加できます。

結果を扱う際は、次の点に注意してください。

* 「目標がいつ完了したかを知るにはどうすればよいですか？」という質問に答えます。
* 指標指標です。 結果の進行状況を示すために、次のオプションから選択できます。

   <!--
  this might change (jira, Salesforce, etc))
  -->

   * 通貨
   * 数値
   * 百分率

結果の詳細については、の節で、結果とアクティビティの類似性のリストを参照してください [結果、アクティビティ、プロジェクトの類似点](#similarities-between-results-activities-and-projects) 」を参照してください。

## アクティビティの概要

<!--
This will have additional types in the future - add another section for types?
-->

アクティビティ（結果など）は、具体的かつ測定可能で、通常、完了率の指標が含まれます。 目標の所有者は、目標に関連付けられたアクティビティを所有することもできます。 また、目標に関するアクティビティが別のユーザーに割り当てられている場合もあります。

アクティビティを目標に追加する方法について詳しくは、 [Adobe Workfront目標での目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

アクティビティを目標に関連付ける際は、次の点を考慮してください。

* 「目標が達成されたら、何を達成するか」という質問に答えます。
* アクティビティは、完了または不完全という点でより多くを考慮できるカスタムエントリです。 これまで完了したアクティビティの割合を示すために、指標を手動で更新する必要があります。

<!--
* You can associate the following activities with goals:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Manual progress bar </td> 
     <td> <p>Custom entries that can be thought of more in terms of complete or incomplete. They must be manually updated.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><p>Project</p></td> 
     <td> <p>Existing projects that you have at least permissions to View and are not in a status of Dead. They are updated automatically, based on the progress of their work items. </p> <p>The projects must exist before associating them with the goal. You can associate a project with multiple goals. For information about adding projects to goals, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</p>
     <p><span class="preview">In the Preview environment, projects are separate progress indicators, independent from activities. Adding projects to a goal in the Preview environment is different from adding activities. For more information, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</span></p>
      </td> 
    </tr> 
   </tbody> 
  </table>
-->
<!--drafted for goal redesign: For THE PRODUCTION RELEASE: remove the projects in this article altogether.-->

結果とアクティビティの詳細については、の節で、結果とアクティビティの類似点のリストを参照してください。 [結果、アクティビティ、プロジェクトの類似点](#similarities-between-results-activities-and-projects) 」を参照してください。

## 結果、アクティビティ、プロジェクトの類似点 {#similarities-between-results-activities-and-projects}

結果、アクティビティおよびプロジェクトは目標の進捗状況インジケーターです。

プロジェクトの管理方法と、結果およびアクティビティの管理方法には、いくつかの違いがあります。 目標にプロジェクトを追加する方法について詳しくは、 [Adobe Workfront目標での目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 目標に関連するプロジェクトについて詳しくは、 [Adobe Workfront目標の目標へのプロジェクトの追加](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

結果、アクティビティ、プロジェクトに加えて、子の目標を目標に関連付けることもできます。 また、子の目標は、目標の進捗状況インジケーターの一種でもあります。 詳しくは、 [目標をAdobe Workfront目標に結び付けて整列させる](../goal-alignment/align-goals-by-connecting-them.md). また、子目標の進捗状況インジケーターの進捗状況は、親目標の進捗状況を左右します。

次の表に、目標指標として、結果、アクティビティおよびプロジェクトの類似点と相違点を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b><p>機能</p></b></td> 
   <td><b><p>件の結果</p></b></td> 
   <td><b><p>アクティビティ</p></b></td> 
   <td> <p><strong>プロジェクト</strong> </p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td><span style="font-weight: normal;">Workfrontインターフェイスでオブジェクト名をカスタマイズできます</span> </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>過去の目標に追加できます。</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>複数の結果、アクティビティまたはプロジェクトを同じ目標に関連付けることができます。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>1 つの目標を複数の目標に関連付けることができます。</td> 
   <td> </td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>目標の進捗を計算する際には、その進捗状況が考慮されます。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>レポートは、Workfront目標で手動で更新する必要があります</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>目標の終了日に完了する予定です</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ユーザーにのみ割り当てることができ、チーム、グループ、会社には割り当てることができません。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>具体的で測定可能で、通常、進行状況を示す設定数が含まれます。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>開始値と終了値の間の値の範囲が提供され、これらの値を達成するにはどの程度近いかを示します。 終了値に近い値は、目標の進捗状況を計算します。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
 </tbody> 
</table>
