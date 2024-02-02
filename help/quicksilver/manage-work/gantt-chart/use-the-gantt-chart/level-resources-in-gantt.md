---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: '[!UICONTROL ガントチャート]でのリソースの標準化'
description: ガントチャートでリソースを標準化する方法について説明します。
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: ht
source-wordcount: '592'
ht-degree: 100%

---

# [!UICONTROL ガントチャート]でのリソースの標準化

プロジェクトでのリソースの標準化には、次の 2 つの目的があります。

* 担当者に超過して配分された時間を自動的に調整する。
* プロジェクトの現実的なタスクスケジュールを自動的に作成する。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへの [!UICONTROL Edit] アクセス</p> <p><b>メモ</b>

まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトへの[!UICONTROL Manage]アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## リソースの標準化の概要

同じリソースを 2 つの異なるタスクに割り当てる場合は、リソースの標準化を使用して、タスクが同時に発生しないようにタスクのタイムラインを調整できます。

プロジェクトのリソースを標準化する場合は、次の点を考慮します。

* リソースの標準化は 1 つのプロジェクトにのみ適用され、[!DNL Adobe Workfront] では一度に複数のプロジェクトにわたってリソースを標準化することはできません。
* 「**[!UICONTROL 残存作業時間の優先]**」が「**[!UICONTROL 期間タイプ]**」として選択されている場合、[!DNL Workfront] はリソースを標準化しません。
* 複数のユーザーが同じタスクに割り当てられている場合、標準化はキャンセルされます。
* 「**[!UICONTROL タスクの制約]**」のタイプに対する条件は、リソースの標準化よりも優先されます。例えば、「[!UICONTROL タスクの制約]」として「**[!UICONTROL 固定日付]**」が選択されている場合、リソースの標準化によってタスクの日付が変更されることはありません。
* 先行タスク関係は、リソースの標準化よりも優先されます。
* [!UICONTROL ガントチャート]で標準化を調整するには、プロジェクトの「**[!UICONTROL リソースの標準化]**」を「**[!UICONTROL 手動]**」に設定する必要があります。プロジェクトに対する管理権限がある場合は、プロジェクトでこの設定を調整し、**[!UICONTROL プロジェクトの編集]**&#x200B;ボックスで「**[!UICONTROL 手動]**」ではなく「**[!UICONTROL 自動]**」を選択することで、システムに自動的にリソースを標準化させることができます。

  ![](assets/resource-leveling-mode-350x177.png)

* プロジェクト所有者またはタスク担当者は、タスクに標準化の遅延を導入して、タスクに追加の時間が必要になる可能性が高いことを示すことができます。タスクに標準化の遅延を追加する方法については、[タスク標準化の遅延の更新](../../../manage-work/tasks/task-information/task-leveling-delay.md)を参照してください。

## [!UICONTROL ガントチャート]でのリソース標準化の適用

タスクリストの[!UICONTROL ガントチャート]を使用して、リソースを標準化できます。

1. 標準化するプロジェクトに移動します。
1. **[!UICONTROL タスク]**&#x200B;エリアで、**[!UICONTROL ガントチャート]**&#x200B;アイコンをクリックします。

   「**[!UICONTROL 自動保存]**」オプションが有効になっていると、すべての変更は自動的に保存されます。これはデフォルトで有効になっています。

1. （オプション）**[!UICONTROL 計画]モード**&#x200B;のアイコンをクリックし、「**[!UICONTROL 手動保存／標準]**」または「**[!UICONTROL タイムラインの計画]**」を選択して、変更を手動で保存します。

   >[!TIP]
   >
   >「[!UICONTROL 自動保存]」オプションが有効になっている場合、[!UICONTROL ガントチャート]でリソースを標準化することはできません。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. **[!UICONTROL リソースの標準化]**&#x200B;ドロップダウンメニューをクリックします。

   ![Level_resouces.png](assets/level-resouces.png)

1. 次のオプションのいずれかを選択します。

   * **[!UICONTROL 今すぐ標準化]**：選択したタスクにリソースの標準化を適用します。
   * **[!UICONTROL 標準化のクリア]**：選択したタスクからリソースの標準化をすべて削除します。

   >[!NOTE]
   >
   >同じ期間に発生する複数のタスクにリソースが割り当てられている場合、リソース配分が超過することがあります。

1. （オプションかつ条件付き）「自動保存」オプションを無効にしてある場合、変更をキャンセルまたは複製するには、**[!UICONTROL 取り消し]**&#x200B;アイコンまたは&#x200B;**[!UICONTROL やり直し]**&#x200B;アイコンをクリックします。

   >[!TIP]
   >
   >以下のキーボードショートカットを使用すると、[!UICONTROL ガントチャート]上で変更を取り消したり、やり直したりできます。
   >
   >* [!DNL Mac]：取り消すには [!UICONTROL Command + Z] キーを使用し、やり直すには [!UICONTROL Command + Shift + Z] キーを使用します。
   >* Windows：取り消すには [!UICONTROL Ctrl + Z] キーを使用し、やり直すには [!UICONTROL Ctrl + Y] キーを使用します。


1. [!UICONTROL ガントチャート]の右上隅にある「**[!UICONTROL 保存]**」をクリックします。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
