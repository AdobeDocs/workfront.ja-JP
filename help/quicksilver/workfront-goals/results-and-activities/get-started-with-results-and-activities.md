---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront Goals の結果とアクティビティについての基本を学ぶ
description: 目標をアクティブ化するには、結果、アクティビティまたは連携した目標を目標に追加する必要があります。これにより、目標のステータスがドラフトからアクティブに更新され、目標に関する進捗の記録が開始されます。
author: Alina
feature: Workfront Goals
exl-id: 64fa0aef-cb92-465a-9b74-d863fc232fd1
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: ht
source-wordcount: '812'
ht-degree: 100%

---

# Adobe Workfront Goals の結果とアクティビティについての基本を学ぶ

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
>この記事で説明している機能を使用するには、組織に以下が必要です。
>
>* Pro 以上の [Adobe Workfront プラン](https://www.workfront.com/plans)。
>* Workfront ライセンスに加えて、Adobe Workfront Goals ライセンス。
>
>  Workfront Goals ライセンスについては、Workfront のアカウントマネージャーにお問い合わせください。
>
>Workfront Goals へのアクセス権について詳しくは、[Workfront Goals の使用要件](../../workfront-goals/goal-management/access-needed-for-wf-goals.md)を参照してください。


目標を作成すると、その目標のステータスは「ドラフト」になります。目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。

目標に関する進行状況の記録を開始するには、目標をアクティブ化する必要があります。目標をアクティブ化してそのステータスを「アクティブ」に変更するには、まず目標に次の情報を追加する必要があります。

* 結果
* アクティビティ
* プロジェクト
* 連携した目標

目標は、これらの項目の少なくとも 1 つを追加すると、アクティブ化できます。目標の結果とアクティビティを更新して、目標の進捗を示す必要があります。


>[!IMPORTANT]
>
> 目標は、アクティビティ、結果、プロジェクト、連携された目標を、合計 1000 件以上持つことはできません。</span>

この記事では、アクティビティと結果の概要を説明します。目標の連携については、[Adobe Workfront Goals での目標の連携](../../workfront-goals/goal-alignment/goal-alignment.md)を参照してください。プロジェクトを目標に接続する方法について詳しくは、[Adobe Workfront Goals の目標へのプロジェクトの追加](../results-and-activities/connect-projects-to-goals-overview.md)を参照してください。

## 結果の概要

<!--
<p> This will have additional types in the future - add another section for types?)</p>
-->

結果は、目標の進捗状況やどのくらい達成に近づいているかを測定します。目標の所有者は、結果を所有することもできます。目標に対する結果は、別のユーザーに割り当てられる場合もあります。

目標への結果の追加について詳しくは、[Adobe Workfront Goals の目標への結果の追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)を参照してください。

自分の目標または組織の他のエンティティに属する目標に結果を追加できます。

結果を操作する際は、次の点に注意してください。

* 「目標がいつ完了するかをどうやって知るのか？」という質問に答えるようにします。
* 結果は指標です。結果の進行状況を示すために、次のオプションから選択できます。

  <!--
  this might change (jira, Salesforce, etc))
  -->

   * 通貨
   * 数値
   * パーセンテージ

結果の詳細については、[結果、アクティビティ、プロジェクトの類似点](#similarities-between-results-activities-and-projects)の節で、結果とアクティビティの類似点リストを参照してください。

## アクティビティの概要

<!--
This will have additional types in the future - add another section for types?
-->

アクティビティは、結果と同様に、具体的かつ測定可能で、通常、完了率の指標を含みます。目標の所有者は、目標に関連付けられたアクティビティを所有することもできます。また、目標に関するアクティビティが別のユーザーに割り当てられている場合もあります。

目標へのアクティビティの追加について詳しくは、[Adobe Workfront Goals の目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)を参照してください。

アクティビティを目標に関連付ける際は、次の点を考慮してください。

* 「目標が完了したら何を達成するのか？」という質問に答えるようにします。
* アクティビティは、完了または未完了という観点から考えることができるカスタムエントリです。手動で更新して、これまでに完了したアクティビティの割合を示す必要があります。

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

結果とアクティビティの詳細については、この記事の[結果、アクティビティ、プロジェクトの類似点](#similarities-between-results-activities-and-projects)の節で、結果とアクティビティの類似点リストを参照してください。

## 結果、アクティビティ、プロジェクトの類似点 {#similarities-between-results-activities-and-projects}

結果、アクティビティ、プロジェクトは目標の進捗状況の指標です。

プロジェクトの管理方法と、結果およびアクティビティの管理方法には、いくつかの違いがあります。目標へのプロジェクトの追加について詳しくは、[Adobe Workfront Goals の目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)を参照してください。目標に接続されているプロジェクトについては、[Adobe Workfront Goals の目標にプロジェクトを追加する](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)を参照してください。

結果、アクティビティ、プロジェクトに加えて、目標に、子の目標を関連付けることもできます。また、子の目標は、目標の進捗状況指標の一種です。詳しくは、[Adobe Workfront Goals で目標をに結び付けて整合させる](../goal-alignment/align-goals-by-connecting-them.md)を参照してください。また、子目標の進捗状況指標の進捗状況は、親目標の進捗状況を左右します。

次の表に、目標のインジケーターとしての、結果、アクティビティ、プロジェクトの類似点と相違点を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b><p>機能</p></b></td> 
   <td><b><p>結果</p></b></td> 
   <td><b><p>アクティビティ</p></b></td> 
   <td> <p><strong>プロジェクト</strong> </p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td><span style="font-weight: normal;">Workfront インターフェイスでオブジェクト名をカスタマイズできます</span> </td> 
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
   <td>そのうちの 1 つを複数の目標に関連付けることができます。</td> 
   <td> </td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>目標の進行状況を計算する際には、その進捗状況が考慮されます。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>レポートは、Workfront Goals で手動で更新する必要があります</td> 
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
   <td>ユーザーにのみ割り当てることができ、チーム、グループ、会社には割り当てることはできません。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>具体的かつ測定可能で、通常は進行状況を示す設定数値が含まれます。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>開始値と終了値の間の値の範囲が提供され、これらの値を達成するにはどの程度近いかを示します。終了値に近い値は、目標の進捗状況の値を計算します。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
 </tbody> 
</table>
