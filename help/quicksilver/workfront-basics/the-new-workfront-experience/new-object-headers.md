---
content-type: overview
navigation-topic: the-new-workfront-experience
title: オブジェクトヘッダーの概要
description: ' [!DNL Adobe Workfront] 内のオブジェクトのヘッダーを確認すると、そのオブジェクトに関する情報が一目でわかります。ヘッダー内の情報には、オブジェクトの所有者、ステータスまたは完了率を含めることができます。'
feature: Get Started with Workfront
exl-id: 76e21df0-9272-4bfb-8a97-c16ae5f4b5dc
source-git-commit: 58dffc8a84c2bcaaf09dfc65c6555d57f0b2eeb4
workflow-type: tm+mt
source-wordcount: '3707'
ht-degree: 97%

---

# オブジェクトヘッダーの概要

[!DNL Adobe Workfront] 内のオブジェクトのヘッダーを確認すると、そのオブジェクトに関する情報が一目でわかります。

ヘッダーには、オブジェクト名に加えて、オブジェクトの所有者、ステータスまたは完了率を含めることができます。

[!DNL Workfront] は、ヘッダー内の可能な限りの領域をオブジェクト名に優先的に割り当てます。オブジェクト名が長すぎる場合は切り詰められます。オブジェクトの完全な名前を表示するには、そのオブジェクトにポインタを合わせます。

## オブジェクトのヘッダーへのアクセス

[!DNL Workfront] におけるオブジェクトのヘッダーへのアクセスは、そのヘッダーを持つすべてのオブジェクトで同一です。

例えば、プロジェクトのヘッダーにアクセスするには：

1. プロジェクトに移動します。\
   ページの上部にヘッダーが表示され、そこにプロジェクト名が含まれています。

   ![](assets/project-header-350x18.png)

## [!UICONTROL ホーム]ヘッダーの概要

ホームでは、次のヘッダーを使用できます。

* タスク：このヘッダーの使用方法について詳しくは、この記事の[タスクヘッダーの概要](#task-header-overview)を参照してください。
* イシュー：このヘッダーの使用方法について詳しくは、この記事の[イシューヘッダーの概要](#issue-header-overview)を参照してください。

## カスタマイズ可能なヘッダー

[!DNL Workfront] 管理者またはグループ管理者は、レイアウトテンプレートを使用して、プロジェクト、タスクおよびイシューのヘッダーをカスタマイズできます。

この記事では、プロジェクト、タスク、イシューを含む、すべてのオブジェクトのデフォルトヘッダーについて説明します。

オブジェクトのヘッダーに関する情報のカスタマイズについて詳しくは、[レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。


## プロジェクトヘッダーの概要

![](assets/project-header-350x18.png)

プロジェクトヘッダーには、デフォルトで次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">親オブジェクトを含むパンくずリスト</td> 
   <td>プロジェクトがプログラムまたはポートフォリオに関連付けられている場合、ヘッダーの左上隅のパンくずリストに表示されます。親オブジェクトの名前をクリックすると、その親オブジェクトが開きます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>紫色の [!UICONTROL Project] アイコン <img src="assets/nwe-projects-icon.png"> がプロジェクト名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プロジェクト名</td> 
   <td>ヘッダーのプロジェクト名は編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>「[!UICONTROL PROJECT]」というテキストが、ヘッダーのプロジェクト名の上に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">タスクのアクション領域</td> 
   <td> <p>アクション領域はプロジェクト名の横に表示されます。</p> <p> <img src="assets/nwe-general-actions-area.png"> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td>ヘッダーのプロジェクト完了率は編集できません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project Owner]</td> 
   <td> <p>ヘッダーの [!UICONTROL Project Owner] は編集できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Completion Date] </td> 
   <td> <p>プロジェクトが [!UICONTROL Completion Date] からスケジュールされている場合、ヘッダーのプロジェクト [!UICONTROL Planned Completion Date] と時刻を編集できます。プロジェクトが [!UICONTROL Start Date] からスケジュールされている場合、この情報はプロジェクトのタスクから更新されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Condition] </td> 
   <td> <p>プロジェクトの [!UICONTROL Condition Type] を手動に設定すると、ヘッダーのプロジェクト [!UICONTROL Condition] を更新できます。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>ヘッダーのプロジェクト [!UICONTROL Status] を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Approvals]エリア</td> 
   <td> <p>承認者の 1 人である場合は、次のアイコンを使用して、プロジェクトの承認を管理します。</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> </img> [!UICONTROL Approve]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> </img> [!UICONTROL Reject]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> </img> [!UICONTROL Recall]</p> <p>承認者でない場合は、[!UICONTROL More]アイコン <img src="assets/more-icon-for-approvals-area.png"> をクリックして、現在の承認ステップに関する情報を表示します。</p> <p>承認について詳しくは、<a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">承認プロセスの概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## タスクヘッダーの概要

![](assets/task-header-350x18.png)

タスクヘッダーには、デフォルトで次の情報が含まれています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">親オブジェクトを含むパンくずリスト</td> 
   <td> <p>タスクの親オブジェクトがパンくずリストに表示されます。親オブジェクトの名前をクリックすると、その親オブジェクトが開きます。</p> <p>詳細情報は、<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">パンくずリストの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>緑色の [!UICONTROL Task] アイコン <img src="assets/nwe-tasks-icon.png"> が、タスク名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">タスクの名前</td> 
   <td>ヘッダーのタスク名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>ヘッダー内のタスク名の上に「[!UICONTROL TASK]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">タスクのアクション領域</td> 
   <td> <p>タスク名の横に、[!UICONTROL actions]エリアが表示されます。</p> <p> <img src="assets/nwe-dependency-action-area.png"> </p> <p>「依存関係」アイコンが表示された場合は、アイコンをクリックして、タスクの先行タスクまたは後続タスクを表示できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td>ヘッダーでタスクの完了率を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td>タスクの割り当て先は、ヘッダーで編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Work on It] ボタン、[!UICONTROL Done] ボタン、または [!UICONTROL Start Task] ボタン</p> </td> 
   <td> <p>タスクが割り当てられている場合は、[!UICONTROL Work on It] <span>ボタン、または [!UICONTROL Start Task] </span> ボタンをクリックして、現在タスクに取り組んでいることを示します。または、[!UICONTROL Done] ボタンをクリックして、タスクが完了したことを示します。</p> <p><span>[!UICONTROL Work On It] ボタンを [!UICONTROL Start Task] ボタンに置き換える方法については、<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">[!UICONTROL Work On It] ボタンを [!UICONTROL Start Task] ボタンに置き換える</a></span>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Completion Date]</td> 
   <td> <p>ヘッダーで、タスクの[!UICONTROL Planned Completion Date]<span>および時刻</span>を編集できます。</p> <p>ヒント：[!UICONTROL Commit Date]はヘッダーに表示されません。このレポートは、[!UICONTROL Details]ページで表示できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>ヘッダーで、タスクの[!UICONTROL Status]を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Approvals]エリア</td> 
   <td> <p>あなたが承認者の場合は、次のアイコンを使用してタスクの承認を管理します。</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> </img> [!UICONTROL Approve]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> </img> [!UICONTROL Reject]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> </img> [!UICONTROL Recall]</p> <p>承認者でない場合は、[!UICONTROL More]アイコン <img src="assets/more-icon-for-approvals-area.png"> をクリックして、現在の承認ステップに関する情報を表示します。</p> <p>承認について詳しくは、<a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">承認プロセスの概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## イシューヘッダーの概要

![](assets/issue-header-350x19.png)

イシューヘッダーには、デフォルトで次の情報が含まれています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">親オブジェクトを含むパンくずリスト</td> 
   <td> <p>イシューの親オブジェクトがパンくずリストに表示されます。親オブジェクトの名前をクリックすると、その親オブジェクトが開きます。</p> <p>詳細情報は、<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">パンくずリストの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>ピンク色の[!UICONTROL Issue]アイコン <img src="assets/nwe-issues-icon.png"> が、イシュー名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">イシューの名前</td> 
   <td>ヘッダーのイシュー名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>ヘッダー内のイシュー名の上に「[!UICONTROL ISSUE]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">イシューのアクションエリア</td> 
   <td> <p>イシューの名前の横に、[!UICONTROL actions]エリアが表示されます。</p> <p> <img src="assets/nwe-dependency-action-area.png"> </p> <p>[!UICONTROL Dependency] アイコンが表示された場合は、アイコンをクリックして、イシューの先行タスクまたは後続タスクを表示できます。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td> <p>ヘッダーからイシューの完了率を編集できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td>ヘッダーからイシューの担当者を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work on It]、[!UICONTROL Done]、<span> または [!UICONTROL Start Issue] ボタン </span></td> 
   <td>イシューを担当する場合は、[!UICONTROL Work on It] <span> または [!UICONTROL Start Issue] </span> ボタンをクリックして現在イシューの処理中であることを示します。または、[!UICONTROL Done] ボタンをクリックしてイシューの完了を示します。<span>[!UICONTROL Work On It] ボタンを [!UICONTROL Start Task] ボタンに置き換える方法について詳しくは、</span><span href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">[!UICONTROL Work On It] ボタンを [!UICONTROL Start] ボタンに置き換える</a></span><span> を参照してください。</span></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Completion Date]</td> 
   <td> <p>ヘッダーのイシュー [!UICONTROL Planned Completion Date] <span>および時刻</span>を編集できます。</p> <p>ヒント：[!UICONTROL Commit Date]はヘッダーに表示されません。このレポートは、[!UICONTROL Details]ページで表示できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>ヘッダーのイシュー [!UICONTROL Status] を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Approvals]エリア</td> 
   <td> <p>あなたが承認者の場合は、次のアイコンを使用して、イシューの承認を管理します。</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> [!UICONTROL Approve]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> [!UICONTROL Reject]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> [!UICONTROL Recall]</p> <p>承認者でない場合は、[!UICONTROL More] アイコン <img src="assets/more-icon-for-approvals-area.png"> をクリックして、現在の承認ステップに関する情報を表示します。</p> <p>承認について詳しくは、<a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">承認プロセスの概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## プログラムヘッダーの概要

![](assets/program-header-350x18.png)

プログラムヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">ポートフォリオ名を含むパンくずリスト</td> 
   <td> <p>[!UICONTROL Portfolio]には、[!UICONTROL Program]のヘッダーからアクセスできます親オブジェクトの名前をクリックすると、その親オブジェクトが開きます。</p> <p>詳細情報は、<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">パンくずリストの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>オレンジ色の [!UICONTROL Program] アイコン <img src="assets/nwe-programs-icon.png"> は、プログラム名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プログラムの名前</td> 
   <td>ヘッダーのプログラム名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>プログラムが [!UICONTROL Active] とマークされている場合は、ヘッダーのプログラム名の上に「[!UICONTROL PROGRAM]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクティベーションステータス</td> 
   <td> <p>プログラムが非アクティブ化されている場合、ヘッダー内のプログラム名の上に「[!UICONTROL PROGRAM DEACTIVATED]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プログラムのアクションエリア</td> 
   <td> <p>プログラム名の横に、[!UICONTROL actions] エリアが表示されます。</p> <p> <img src="assets/nwe-general-actions-area.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td> <p>ヘッダーのプログラムの [!UICONTROL Percent CompletePercent Complete] は編集できません。この情報は、プログラムのプロジェクトから更新されます。</p> <p>ヒント：デフォルトでは、プログラムの完了率は、そのプログラムに属する [!UICONTROL Current] または [!UICONTROL Approved Status] 内のプロジェクトの完了率の値の平均です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Manager]</td> 
   <td> <p>ヘッダーの [!UICONTROL Program Manager] を編集できます。これは、[!UICONTROL Program Owner] と同じです。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Completion Date]</td> 
   <td>ヘッダーのプログラム[!UICONTROL Planned Completion Date]は編集できません。この情報は、プログラム内のプロジェクトの[!UICONTROL Planned Completion Date]から更新されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Active Projects Condition]</td> 
   <td>これは、プログラム内のアクティブなプロジェクトのうち、[!UICONTROL Condition]が[!UICONTROL On Target]、[!UICONTROL At Risk]または[!UICONTROL In Trouble]に設定されている割合を計算したものです。</td> 
  </tr> 
 </tbody> 
</table>

## ポートフォリオヘッダーの概要 {#portfolio-header-overview}

![](assets/portfolio-header-350x19.png)

ポートフォリオヘッダーに含まれる情報は、以下のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>青い[!UICONTROL Portfolio]アイコン <img src="assets/nwe-portfolios-icon.png"> がポートフォリオ名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ポートフォリオ名</td> 
   <td>ヘッダーのポートフォリオ名は編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>ポートフォリオがアクティブとマークされている場合、ヘッダーのポートフォリオ名の上に「[!UICONTROL PORTFOLIO]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクティベーションステータス</td> 
   <td> <p>ポートフォリオが非アクティブ化されている場合、ヘッダーのポートフォリオ名の上に「[!UICONTROL PORTFOLIO DEACTIVATED]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ポートフォリオの[!UICONTROL actions]エリア</td> 
   <td> <p>ポートフォリオ名の横に、[!UICONTROL actions]エリアが表示されます。</p> <p> <img src="assets/nwe-general-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
   <td>ヘッダーの[!UICONTROL Portfolio Manager]は編集できます。これは、[!UICONTROL Portfolio Owner]と同じです。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL On Time]</td> 
   <td>ポートフォリオ内のプロジェクトのうち、現在目標通りであるプロジェクトの割合を計算したものです。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL On Budget]</td> 
   <td>ポートフォリオ内のプロジェクトのうち、現在予算通りであるプロジェクトの割合を計算したものです。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aligned]</td> 
   <td>ポートフォリオ内のプロジェクトのうち、ポートフォリオと一致しているプロジェクトの割合を計算したものです。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ROI]</td> 
   <td>ポートフォリオ内のすべてのプロジェクトの[!UICONTROL Return on Investment]を計算したものです。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Net Value]</td> 
   <td>これは、ポートフォリオ内のすべてのプロジェクトの[!UICONTROL Net Value]を計算したものです。</td> 
  </tr> 
 </tbody> 
</table>

## テンプレートヘッダーの概要 {#template-header-overview}

![](assets/template-header-350x18.png)

テンプレートヘッダーに表示される情報は、以下のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>緑色の[!UICONTROL Template]アイコン <img src="assets/nwe-templates-icon.png"> がテンプレート名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">テンプレート名</td> 
   <td>ヘッダーのテンプレート名は編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>テンプレートがアクティブとマークされている場合、ヘッダーのテンプレート名の上に「[!UICONTROL TEMPLATE]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクティベーションステータス</td> 
   <td> <p>テンプレートが非アクティブ化されている場合、ヘッダーのテンプレート名の上に「[!UICONTROL TEMPLATE DEACTIVATED]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">テンプレートのアクションエリア</td> 
   <td> <p>テンプレート名の横に、アクションエリアが表示されます。</p> <p> <img src="assets/nwe-general-actions-area.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Template Owner]</td> 
   <td>ヘッダーの [!UICONTROL Template Owner] フィールドは編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Duration]</td> 
   <td>テンプレートの期間です。ヘッダーのこのフィールドは編集できません。</td> 
  </tr> 
 </tbody> 
</table>

## テンプレートのタスクヘッダーの概要

![](assets/template-task-header-350x18.png)

テンプレートのタスクヘッダーに表示される情報は、以下の通りです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">親オブジェクトのパンくずリスト</td> 
   <td> <p>テンプレートのタスクの親オブジェクトがパンくずリストに表示されます。親オブジェクトの名前をクリックすると、その親オブジェクトが開きます。</p> <p>詳しくは、<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">パンくずリストの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>緑色の [!UICONTROL Task] アイコン <img src="assets/nwe-tasks-icon.png"> がテンプレートのタスク名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">テンプレートのタスク名</td> 
   <td>ヘッダーのテンプレートのタスクの名前を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>「[!UICONTROL TEMPLATE TASK]」というテキストが、ヘッダー内のテンプレートのタスクの名前の上に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">テンプレートのタスクのアクションエリア</td> 
   <td> <p>アクションエリアはテンプレートのタスクの名前の横に表示されます。</p> <p> <img src="assets/nwe-general-actions-area.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td>ヘッダーでテンプレートのタスクの [!UICONTROL Assignments] を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Completion Day]</td> 
   <td>テンプレートの期間の、テンプレートのタスクが完了する必要がある日です。</td> 
  </tr> 
 </tbody> 
</table>

## 請求記録ヘッダーの概要

![](assets/billing-record-header-nwe-350x19.png)

請求記録のヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">親オブジェクトのパンくずリスト</td> 
   <td> <p>請求記録の親オブジェクトがパンくずリストに表示されます。親オブジェクトの名前をクリックすると、その親オブジェクトが開きます。</p> <p>詳しくは、<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">パンくずリストの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>青色の [!UICONTROL Billing Record] アイコン <img src="assets/nwe-billing-record-icon-57x55.png" style="width: 57;height: 55;"> が、請求記録の名前の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">請求記録の名前</td> 
   <td>ヘッダーの請求記録の名前を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>「[!UICONTROL BILLING RECORD]」というテキストが、ヘッダー内の請求記録の名前の上に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">請求記録のアクションエリア</td> 
   <td> <p>請求記録の名前の横に [!UICONTROL More] メニュー <img src="assets/more-menu.png"> が表示され、次のオプションを選択できます。</p> 
    <ul> 
     <li> <p>[!UICONTROL Edit]</p> </li> 
     <li> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Billing Record Total]</td> 
   <td>請求記録の合計金額です。このフィールドは編集できません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Billing Date]</td> 
   <td>請求記録の作成時に手動で変更された場合を除き、請求レコードが作成された日付です。[!UICONTROL Billing Date] のヘッダーを編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td> <p>請求記録のステータスが [!UICONTROL Billed] の場合、その記録は編集できません。</p> <p>ヘッダーの請求記録のステータスを編集できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーヘッダーの概要

![](assets/user-header-350x20.png)

ユーザーヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">ユーザーのプロフィール画像</td> 
   <td>ヘッダーのプロフィール画像を更新することはできません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザーの名前とタイトル</td> 
   <td> <p> ユーザーのタイトルは、名前の上にすべて大文字で表示されます。ヘッダーのユーザーの名前は編集できません。</p> </td> 
  </tr> <!--
   <tr> 
    <td role="rowheader">Name of the object type</td> 
    <td> <p>The name of the object type does not display.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">アクティベーションステータス</td> 
   <td> <p>ユーザーが非アクティブ化されている場合、ヘッダー内のすべてのテキストとプロフィール画像がグレー表示になります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザーのアクションエリア</td> 
   <td> <p>ユーザーの名前の横に、アクションエリアが表示されます。</p> <p> <img src="assets/nwe-general-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">メールアドレス</td> 
   <td>ヘッダーのメールアドレスは編集できません。これは通常、ユーザー名でもあります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">電話番号</td> 
   <td>ヘッダーの電話番号は編集できません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">チーム</td> 
   <td> <p>ユーザーが所属するチームを表示できます。チームのアバターの上でマウスを移動すると、チームの名前が表示されます。ヘッダーのチームは編集できません。</p> </td> 
  </tr> 
 </tbody> 
</table>

## チームヘッダーの概要

![](assets/team-header-350x23.png)

チームのヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>紫色の [!UICONTROL Team] アイコン <img src="assets/nwe-teams-icon.png"> が、チーム名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">チームの名前</td> 
   <td>ヘッダーでチーム名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>「[!UICONTROL TEAM]」というテキストがヘッダー内のチーム名の上に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">チームのアクションエリア</td> 
   <td> <p>チーム名の横に、[!UICONTROL actions] エリアが表示されます。</p> <p> <img src="assets/nwe-switch-team-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">チームメンバーのプロファイル画像</td> 
   <td>チームメンバーのプロフィール写真。画像の上にマウスを移動すると、ユーザーの名前が表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">説明</td> 
   <td>これは、チームのメンバーに関する簡単な説明です。ヘッダーのチームの説明は編集できません。</td> 
  </tr> 
 </tbody> 
</table>

## イテレーションヘッダーの概要

![](assets/iteration-header-350x19.png)

イテレーションヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>オレンジ色の [!UICONTROL Iteration] アイコン <img src="assets/nwe-iteration-icon-58x58.png" style="width: 58;height: 58;"> がイテレーション名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">イテレーションの名前</td> 
   <td>ヘッダーのイテレーション名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>「[!UICONTROL ITERATION]」というテキストが、ヘッダー内のイテレーション名の上に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">イテレーションのアクションエリア</td> 
   <td> <p>ヘッダーの右上隅に、アクションエリアが表示されます。</p> <p> <img src="assets/nwe-iteration-action-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">所有者</td> 
   <td>これは、イテレーションの [!UICONTROL Owner] です。ヘッダーの [!UICONTROL Owner] は編集できません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeline]</td> 
   <td>[!UICONTROL Timeline] は、このイテレーションの開始日と終了日を示します。ヘッダーの [!UICONTROL Timeline] は編集できません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team]</td> 
   <td>ヘッダー内のイテレーションのチームは編集できません。チーム名をクリックすると、チームページに移動します。</td> 
  </tr> 
 </tbody> 
</table>

## グループヘッダーの概要

![](assets/nwe-group-header-350x20.png)

グループのヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>オレンジ色の [!UICONTROL Group] アイコン <img src="assets/nwe-group-icon.png"> が、グループ名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">グループの名前</td> 
   <td>ヘッダーのグループ名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>ヘッダー内のグループ名の上に、「[!UICONTROL GROUP]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">グループの [!UICONTROL actions] エリア</td> 
   <td> <p>グループ名の横にある [!UICONTROL More] メニュー <img src="assets/more-menu.png"> が表示され、次のオプションを選択できます。</p> 
    <ul> 
     <li> <p>[!UICONTROL Edit]</p> </li> 
     <li> <p>[!UICONTROL Copy]</p> </li> 
     <li> <p>[!UICONTROL Delete]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Business Leader]</td> 
   <td>ヘッダーの [!UICONTROL Business Leader] を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Licenses in use] </td> 
   <td> <p>「[!UICONTROL Licenses in use]」ボックスに、グループおよびそのサブグループ内の [!UICONTROL Plan] および [!UICONTROL Work] ライセンスユーザーの数が表示されます。数字をクリックすると、5 種類のライセンスに関する情報が表示されます。</p> <p>詳しくは、<a href="../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md" class="MCXref xref">新しい [!DNL Adobe Workfront] エクスペリエンスでグループに割り当てられ、使用されているライセンス数を表示する</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group Administrators]</td> 
   <td>ヘッダーのグループ管理者を編集できます。</td> 
  </tr> 
 </tbody> 
</table>

## ドキュメントヘッダーの概要

![](assets/document-header-350x19.png)

ドキュメントヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">親オブジェクトを含むパンくずリスト</td> 
   <td> <p>ドキュメントの親オブジェクトがパンくずリストに表示されます。親オブジェクトの名前をクリックすると、その親オブジェクトが開きます。</p> <p>詳しくは、<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">パンくずリストの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>青色の [!UICONTROL Document] アイコン <img src="assets/nwe-documents-icon-53x50.png" style="width: 53;height: 50;"> が、ドキュメント名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ドキュメントの名前</td> 
   <td>ヘッダーのドキュメント名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>「[!UICONTROL DOCUMENT]」というテキストは、ヘッダーのドキュメント名の上に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ドキュメントのアクションエリア</td> 
   <td> <p>ドキュメント名の横に、アクションエリアが表示されます。</p> <p> <img src="assets/nwe-doc-version-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">承認の [!UICONTROL Decision] エリア</td> 
   <td> [!UICONTROL 決定 ] 領域は、ドキュメントヘッダーの右上隅に表示されます。この領域は、承認フェーズと、承認者、レビュー担当者、またはその両方によって異なります。 <ul><li> <p>承認者の場合は、次のアイコンを使用してドキュメントの承認を管理できます。</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> [!UICONTROL Approve]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> [!UICONTROL Recall]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> [!UICONTROL Reject]</p> <p>承認の決定について詳しくは、 <a href="../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">作業の承認</a>.</li><li><p>レビュー担当者の場合は、「レビューを完了」ボタンをクリックして、ドキュメントをレビューしたことを示すことができます。</p><p>ドキュメントのレビューについて詳しくは、 <a href="../../review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-a-document.md" class="MCXref xref">ドキュメントのレビュー</a>.</p></li><li>それ以外の場合は、この領域にはドキュメントの現在のレビューおよび承認ステータスが表示されます。</li><ul></p> </td> 
  </tr> 
 </tbody> 
</table>

## 会社ヘッダーの概要 {#company-header-overview}

![](assets/company-header-350x20.png)

会社のヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>青色の [!UICONTROL Company] アイコン <img src="assets/nwe-company-icon.png"> が、会社名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">会社の名前</td> 
   <td>ヘッダーの会社の名前を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>「[!UICONTROL COMPANY]」というテキストが、ヘッダーの会社名の上に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">会社のアクションエリア</td> 
   <td> <p>会社の名前の横に [!UICONTROL More] メニュー <img src="assets/more-menu.png"> が表示され、次のオプションを選択できます。</p> 
    <ul> 
     <li> <p>[!UICONTROL Edit]</p> </li> 
     <li> <p>[!UICONTROL Delete Company]</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## プランヘッダーの概要

![](assets/nwe-plan-header-350x34.png)

プランは、[!DNL Workfront Scenario Planner] のオブジェクトです。[!DNL Scenario Planner] について詳しくは、[ [!DNL Scenario Planner]  の概要](../../scenario-planner/scenario-planner-overview.md)を参照してください。

プランヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">計画に戻る</td> 
   <td>このリンクをクリックすると、[!UICONTROL Plans] リストに移動します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>青色の [!UICONTROL Plan] アイコン <img src="assets/nwe-plan-icon-65x62.png" style="width: 65;height: 62;"> が、プラン名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プランの名前</td> 
   <td>ヘッダーのプラン名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>ヘッダーのプラン名の上に「[!UICONTROL PLAN]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プランのアクションエリア</td> 
   <td> <p>プランの名前の横に、アクションエリアが表示されます。</p> <p> <img src="assets/nwe-general-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">追加のプラン領域</td> 
   <td> <p>プラン名とアクションエリアの下で、次の操作を実行できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Show conflicts]</strong>：この切替スイッチをクリックすると、イニシアチブ内の競合の表示と非表示が切り替わります。</p> </li> 
     <li> <p><strong>[!UICONTROL Compare scenarios]</strong>：このリンクをクリックすると、作成したシナリオの比較が並んで表示されます。</p> </li> 
     <li> <p><strong>[!UICONTROL Scenario selection]</strong>：このドロップダウンメニューでは、シナリオをコピーするか、別のシナリオを選択して表示できます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">担当業務の情報</td> 
   <td>「[!UICONTROL Job Role]」ボックスで、必要とされる担当業務の数と比較して、プランで使用可能な担当業務数を確認できます。ボックスをクリックすると、使用可能な担当業務を調整できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Financial] 情報</td> 
   <td>「[!UICONTROL Financial]」ボックスに、プランの予算、コストおよび稼働率の割合が表示されます。ボックスをクリックすると、予算金額を調整し、人件費をプランに含めるかどうかを決定できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Net Value]</td> 
   <td>「[!UICONTROL Net Value]」ボックスに、計画に入力した予算とコストに基づいて、計画の純価が表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared with]情報</td> 
   <td>計画の表示や管理を行うアクセス権を持つユーザーは、ヘッダーの右上隅に表示されます。プロフィール画像の上にポインタを合わせると、名前が表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Go to Publish]</td> 
   <td>[!UICONTROL Go to Publish]をクリックすると、表示中のシナリオのイニシアチブにリンクされたプロジェクトを作成または更新できます。</td> 
  </tr> 
 </tbody> 
</table>


## 目標ヘッダーの概要

![](assets/goal-header.png)

会社が Workfront Goals にアクセスできる場合は、戦略的目標を作成できます。[!DNL Workfront Goals] について詳しくは、[ [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md) の基本を学ぶを参照してください。

目標ヘッダーには、次の情報が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>ヘッダー情報</th> 
   <th>メモ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">オブジェクトアイコン </td> 
   <td> <p>紫色の [!UICONTROL Goal] アイコン <img src="assets/goal-icon.png" > が目標名の左側に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">目標の名前</td> 
   <td>ヘッダーの目標名を編集できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトタイプ名</td> 
   <td> <p>ヘッダーの目標名の上に、「[!UICONTROL GOAL]」というテキストが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">目標のアクションエリア</td> 
   <td> <p>目標の名前の横に、アクションエリアが表示されます。</p> <p> <img src="assets/nwe-general-actions-area.png"> </p>
   目標のアクションエリアで、次のアクションを実行できます。
   <ul><li>[!UICONTROL Edit]</li>
   <li>[!UICONTROL Copy goal]</li>
   <li>[!UICONTROL Delete goal]</li>
   <li>[!UICONTROL Share]</li>
   <li>[!UICONTROL Activate]または[!UICONTROL Deactivate]</li>
   <li>[!UICONTROL Close]または[!UICONTROL Reopen]</li>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Progress]</td> 
   <td>進捗目標の割合、目標の達成率を示します。目標の進捗を更新することはできません。Workfront は、目標に関する各進捗インジケーターの進捗状況に基づいて計算します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Owner]</td> 
   <td>これは目標の所有者です。目標所有者を手動で更新できます。ユーザー、チーム、グループまたは組織を目標所有者にすることができます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Period]</td> 
   <td>目標を完了する必要がある時間枠。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Condition]</td> 
   <td>目標条件は、目標が予定通りに完了できるかどうか、遅れているかを示します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>目標がアクティブ、新規またはクローズ済みかを示します。目標のステータスを手動で更新できません。詳しくは、<a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals]</a> の目標ステータスの概要を参照してください。</td> 
  </tr> 
 </tbody> 
</table>