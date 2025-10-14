---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Scenario Planner でのプランの削除
description: 自分で作成した計画を削除できます。自分と共有されている計画は削除できません。
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 81%

---

# [!DNL Scenario Planner] で計画を削除

自分で作成した計画を削除できます。自分と共有されている計画は削除できません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] プラン*</p> </td> 
   <td> <ul></li>
   <li><p>新規：Ultimate </p></li>
   <p>シナリオプランナーは、新しいWorkfront Select プランまたはWorkfront Prime プランでは使用できません。 </p>
   <li><p>現在：[!UICONTROL Business] 以上</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] ライセンス*</p> </td> 
   <td> <p>新規：ライト以上</p> 
   <p>現在：[!UICONTROL Review] 以上</p> </td> 
  </tr> 
  <tr> 
   <td>製品* </td> 
   <td> <ul><li><p>新しいWorkfrontプランの場合：</p><p> Adobe Workfront</li></p>
   <li><p>現在のWorkfront プランの場合： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront シナリオプランナー</p></li></ul>

<p>詳しくは、<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!DNL Scenario Planner]</a> ールの使用に必要なアクセス権」を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>アクセスレベル </td> 
   <td> <p>[!UICONTROL Edit]アクセス権 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>オブジェクト権限 </p> </td> 
   <td> <p>プランに対する[!UICONTROL Manage]権限</p> <p>プランへの追加アクセス権のリクエストについて詳しくは、<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!DNL Scenario Planner]</a> でのプランへの利用申請を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfrontへのアクセス要件ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 計画を削除

>[!IMPORTANT]
>
>削除した計画は復元できません。

計画を削除するか、計画内の 1 つのシナリオを削除できます。

* [計画を削除](#delete-plans)
* [シナリオの削除](#delete-scenarios)

### 計画を削除

>[!IMPORTANT]
>
>計画を削除する際は、次の点を考慮してください。
>
>* 計画に関連する情報もすべて削除されます。これには、担当業務やコストに関する情報を含む、計画に関連するすべてのシナリオとイニシアチブが含まれます。この情報は復元できません。
>* 公開済みのシナリオが計画に含まれる場合、削除されたイニシアチブにリンクされたプロジェクトが保持され、[!DNL Scenario Planner] エリアは「[!UICONTROL プロジェクトの詳細]」セクションに残ります。
>
>  プロジェクトへのイニシアチブの公開について詳しくは、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でのイニシアチブの公開によるプロジェクトのアップデートまたは作成を参照してください。

計画の削除方法は、次のとおりです。

{{step1-to-scenario-planner}}

計画のリストが表示されます。

1. 計画の名前をクリックして開きます。
1. 計画名の右側にある **[!UICONTROL 詳細メニュー]**![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックし、**[!UICONTROL 削除]**/**[!UICONTROL はい、削除します]** をクリックします。

   計画が削除され、計画のリストに戻ります。

### シナリオの削除 {#delete-scenarios}

>[!IMPORTANT]
>
>シナリオを削除する際は、次の点を考慮してください。
>
>* シナリオを削除すると、すべてのイニシアチブとその情報がシナリオから削除されます。他のシナリオにコピーした場合、イニシアチブは他のシナリオに残ります。
>* シナリオを削除すると、後続のシナリオでは削除されたシナリオの数が適用され、カウント順が保持されます。例えば、シナリオ 4 を削除すると、シナリオ 5 はシナリオ 4 になります。
>* シナリオに関する一部のイニシアチブが公開されると、イニシアチブにリンクされたプロジェクトが保持され、シナリオプランナーのエリアはリンクされたプロジェクトに残ります
>* 公開されたイニシアチブが別のシナリオに存在する場合、そのイニシアチブ（プロジェクトへのリンクを含む）は、そのシナリオに残ります。これらのイニシアチブを他のシナリオから公開すると、リンクされたプロジェクトがそれらのシナリオからの新しい情報で更新されます。
>
>  プロジェクトへのイニシアチブの公開について詳しくは、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でのイニシアチブの公開によるプロジェクトのアップデートまたは作成を参照してください。

シナリオの削除方法は、次のとおりです。

1. シナリオを削除する計画に移動します。

   デフォルトでは、最初のシナリオが表示されます。

1. 「**[!UICONTROL シナリオを比較]**」をクリックします。
1. シナリオカードの右上隅にある **[!UICONTROL その他]** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックしてから、**[!UICONTROL 削除]** をクリックします。

   シナリオが削除されます。

1. 「**[!UICONTROL 計画を保存]**」をクリックして、変更を保存します。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


