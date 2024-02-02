---
product-area: projects
navigation-topic: use-the-gantt-chart
title: タスクリストのガントチャートにおける情報の更新
description: タスクリストのガントチャートには、プロジェクトまたはテンプレートのタスクに関する詳細が表示されます。
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: e2f6eada24b4e48bce58189ec16447eda89f4a09
workflow-type: ht
source-wordcount: '1036'
ht-degree: 100%

---

# タスクリストの[!UICONTROL ガントチャート]における情報の更新

タスクリストの[!UICONTROL ガントチャート]には、プロジェクトまたはテンプレートのタスクに関する詳細が表示されます。

テンプレートでは、タスクリストの[!UICONTROL ガントチャート]は、テンプレートのタスクリストでタスクレベルで行われた更新を反映します。テンプレートに関連付けられている[!UICONTROL ガントチャート]は編集できません。

プロジェクトでは、タスクリストの[!UICONTROL ガントチャート]でタスク情報を直接更新できます。

この記事では、タスクリストの[!UICONTROL ガントチャート]で直接実行できる下記の操作について説明します。

* タスク期間の変更
* 先行タスク関係の作成または削除
* タスクの開始日と終了日の変更
* 完了率の更新
* プロジェクトリソースの標準化

## アクセス要件

この記事の手順に従うには、以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトとタスクへの[!UICONTROL Edit]アクセス権</p> <p>メモ：それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されていないかどうかを [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトとタスクへの[!UICONTROL Manage]アクセス権 </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## タスク期間の変更

1. 変更するプロジェクトに移動します。
1. 左パネルの「**[!UICONTROL タスク]**」をクリックします。

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. **[!UICONTROL ガントチャート]**&#x200B;アイコンをクリックします。

   ![ガントチャートアイコンのクリック](assets/click-gantt-chart-icon.png)

   「**[!UICONTROL 自動保存]**」オプションが有効になっていると、すべての変更は自動的に保存されます。これはデフォルトで有効になっています。

1. （オプション）**[!UICONTROL 計画モード]**&#x200B;アイコンをクリックし、「手動保存」オプションの「**[!UICONTROL 標準]**」または「**[!UICONTROL タイムラインの計画]**」を選択して、変更を手動で保存します。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. タスクのタイムラインにポインタを合わせて、タイムラインインジケーターを別の日付までドラッグします。
1. タスクの正しい新しい完了日で、インジケーターをドロップします。
1. （オプションおよび条件付き）変更の手動保存を選択した場合、変更をキャンセルまたは再現するには、**[!UICONTROL 取り消し]**&#x200B;アイコンまたは&#x200B;**[!UICONTROL やり直し]**&#x200B;アイコンをクリックします。

   >[!TIP]
   >
   >ガントチャートの変更の取り消しややり直しには、次のキーボードショートカットを使用できます。
   >
   >   
   >   
   >   * [!DNL Mac]：[!UICONTROL Command + Z] キーを取り消しに、[!UICONTROL Command + Shift + Z] キーをやり直しに使用します。
   >   * [!DNL Windows]：[!UICONTROL Ctrl + Z] キーを取り消しに、[!UICONTROL Ctrl + Y] キーをやり直しに使用します。
   >   
   >

1. [!UICONTROL ガントチャート]の右上隅にある「**[!UICONTROL 保存]**」をクリックします。

## 先行タスク関係の作成または削除

1. 変更するプロジェクトに移動します。
1. **[!UICONTROL タスク]**&#x200B;エリアで、**[!UICONTROL ガントチャート]**&#x200B;アイコンをクリックします。

   「**[!UICONTROL 自動保存]**」オプションがデフォルトで選択されており、この場合、すべての変更が自動的に保存されます。

   ![ガントチャートアイコンのクリック](assets/click-gantt-chart-icon.png)

1. （オプション）**[!UICONTROL 計画モード]**&#x200B;アイコンをクリックし、「手動保存」オプションの「**[!UICONTROL 標準]**」または「**[!UICONTROL タイムラインの計画]**」を選択して、変更を手動で保存します。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 先行タスク関係を作成するには、タスクの開始点をクリックし、タスクの終了点までドラッグします。
1. 先行タスク関係を削除するには、2 つのタスクを接続する先行タスクラインをクリックして選択し、キーボードの **[!UICONTROL Delete]** キーを押します。\
   ![Delete_predecessor.png](assets/delete-predecessor-350x152.png)

1. （オプションおよび条件付き）変更の手動保存を選択した場合、変更をキャンセルまたは再現するには、**[!UICONTROL 取り消し]**&#x200B;アイコンまたは&#x200B;**[!UICONTROL やり直し]**&#x200B;アイコンをクリックします。

   >[!TIP]
   >
   >ガントチャートの変更の取り消しややり直しには、次のキーボードショートカットを使用できます。
   >
   >   
   >   
   >   * [!DNL Mac]：[!UICONTROL Command + Z] キーを取り消しに、[!UICONTROL Command + Shift + Z] キーをやり直しに使用します。
   >   * [!DNL Windows]：[!UICONTROL Ctrl + Z] キーを取り消しに、[!UICONTROL Ctrl + Y] キーをやり直しに使用します。
   >   
   >

1. 「**[!UICONTROL 保存]**」をクリックします。

## タスクの開始日と終了日の変更

1. 変更するプロジェクトに移動します。
1. **[!UICONTROL タスク]**&#x200B;エリアで、**[!UICONTROL ガントチャート]**&#x200B;アイコンをクリックします。

   「**[!UICONTROL 自動保存]**」オプションが有効になっていると、すべての変更は自動的に保存されます。これはデフォルトで有効になっています。

   ![ガントチャートアイコンのクリック](assets/click-gantt-chart-icon.png)

1. （オプション）**[!UICONTROL 計画モード]**&#x200B;アイコンをクリックし、「手動保存」オプションの「**[!UICONTROL 標準]**」または「**[!UICONTROL タイムラインの計画]**」を選択して、変更を手動で保存します。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. タスクの中央にポインタを合わせ、多方向矢印を見つけます。
1. タスクをクリックし、目的の日付までドラッグします。

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. タスクの制約に影響を与えるような変更をタスクの日付に対して行う場合、「**[!UICONTROL 承諾]**」をクリックして、タスクの制約の変更を承認します。

   >[!NOTE]
   >
   >タスクに次の制約のいずれかがある場合、プロジェクトが[!UICONTROL 開始日]からスケジュールされていれば、システムは「[!UICONTROL タスクの制約]」を[!UICONTROL 指定日以後に開始]に更新し、プロジェクトが[!UICONTROL 完了日]からスケジュールされていれば、[!UICONTROL これよりも遅く終了しない]に更新します。
   >
   >   
   >   
   >   * [!UICONTROL できるだけ早く]
   >   * [!UICONTROL できるだけ遅く]
   >   * [!UICONTROL 最も早い空き時間]
   >   * [!UICONTROL 最も遅い空き時間]
   >   
   >   
   >場合によっては、先行タスク関係が原因でタスクの開始を早めることができないことがあり、タスクの移動ができません。

1. （オプションおよび条件付き）変更の手動保存を選択した場合、変更をキャンセルまたは再現するには、**[!UICONTROL 取り消し]**&#x200B;アイコンまたは&#x200B;**[!UICONTROL やり直し]**&#x200B;アイコンをクリックします。

   >[!TIP]
   >
   >[!UICONTROL ガントチャート]の変更の取り消しややり直しには、次のキーボードショートカットを使用できます。
   >
   >   
   >   
   >   * [!DNL Mac]：[!UICONTROL Command + Z] キーを取り消しに、[!UICONTROL Command + Shift + Z] キーをやり直しに使用します。
   >   * [!DNL Windows]：[!UICONTROL Ctrl + Z] キーを取り消しに、[!UICONTROL Ctrl + Y] キーをやり直しに使用します。
   >   
   >

1. 「**[!UICONTROL 保存]**」をクリックします。

## 完了率の更新

1. 変更するプロジェクトに移動します。
1. **[!UICONTROL タスク]**&#x200B;エリアで、**[!UICONTROL ガントチャート]**&#x200B;アイコンをクリックします。

   ![ガントチャートアイコンのクリック](assets/click-gantt-chart-icon.png)

   「**[!UICONTROL 自動保存]**」オプションが有効になっていると、すべての変更は自動的に保存されます。これはデフォルトで有効になっています。

1. （オプション）**[!UICONTROL 計画モード]**&#x200B;アイコンをクリックし、「手動保存」オプションの「**[!UICONTROL 標準]**」または「**[!UICONTROL タイムラインの計画]**」を選択して、変更を手動で保存します。
1. タスク内のパーセント数値をダブルクリックし、数値を入力します。

   >[!IMPORTANT]
   >
   >完了率を更新するには、[!UICONTROL オプション]ダイアログで「[!UICONTROL 完了率]」が選択されている必要があります。それには、**[!UICONTROL オプション]**&#x200B;アイコンをクリックし、「**[!UICONTROL 完了率]**」を選択します。
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)
   >

1. （オプションおよび条件付き）変更の手動保存を選択した場合、変更をキャンセルまたは再現するには、**[!UICONTROL 取り消し]**&#x200B;アイコンまたは&#x200B;**[!UICONTROL やり直し]**&#x200B;アイコンをクリックします。

   >[!TIP]
   >
   >[!UICONTROL ガントチャート]の変更の取り消しややり直しには、次のキーボードショートカットを使用できます。
   >
   >   
   >   
   >   * [!DNL Mac]：[!UICONTROL Command + Z] キーを取り消しに、[!UICONTROL Command + Shift + Z] キーをやり直しに使用します。
   >   * [!DNL Windows]：[!UICONTROL Ctrl + Z] キーを取り消しに、[!UICONTROL Ctrl + Y] キーをやり直しに使用します。
   >   
   >

1. [!UICONTROL ガントチャート]の右上隅にある「**[!UICONTROL 保存]**」をクリックします。

## プロジェクトリソースの標準化

タスクリストの[!UICONTROL ガントチャート]を使用して、リソースを標準化できます。

[!UICONTROL ガントチャート]でのリソースの標準化については、[[!UICONTROL ガントチャート]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md)でのリソースの標準化を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
