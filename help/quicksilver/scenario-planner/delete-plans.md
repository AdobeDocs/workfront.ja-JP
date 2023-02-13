---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーのプランの削除
description: 自分で作成したプランを削除できます。 自分と共有されているプランは削除できません。
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# のプランを削除 [!DNL Scenario Planner]

自分で作成したプランを削除できます。 自分と共有されているプランは削除できません。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 計画*</b> </p> </td> 
   <td>[!UICONTROL Business] 以降</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> ライセンス*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td><b>製品</b> </td> 
   <td> <p>の追加ライセンスを購入する必要があります。 [!DNL Adobe Workfront Scenario Planner] をクリックして、この記事で説明する機能にアクセスします。</p> <p>詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">を使用するために必要なアクセス [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>[!UICONTROL 編集 ] 以降の [!DNL Scenario Planner]</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクト権限</strong> </p> </td> 
   <td> <p>プランに対する [!UICONTROL 管理 ] 権限</p> <p>プランへの追加アクセス権のリクエストについて詳しくは、 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">内のプランへのアクセスをリクエスト [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 計画を削除

>[!IMPORTANT]
>
>削除したプランは復元できません。

プランを削除するか、プラン内の 1 つのシナリオを削除できます。

* [計画を削除](#delete-plans)
* [シナリオの削除](#delete-scenarios)

### 計画を削除

>[!IMPORTANT]
>
>プランを削除する際は、次の点を考慮してください。
>
>* プランに関連する情報もすべて削除されます。 これには、ジョブの役割やコストに関する情報を含む、プランに関連するすべてのシナリオとイニシアチブが含まれます。 この情報は復元できません。
>* プランに公開済みのシナリオが含まれる場合、削除されたイニシアチブにリンクされたプロジェクトが保持され、 [!DNL Scenario Planner] 領域が [!UICONTROL プロジェクトの詳細] 」セクションに入力します。
>
>  プロジェクトへのイニシアチブの公開については、 [プロジェクトを更新または作成するには、 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

計画を削除する手順は、次のとおりです。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png)を選択し、「 [!UICONTROL シナリオ].

   プランのリストが表示されます。

1. プランの名前をクリックして開きます。
1. 次をクリック： **[!UICONTROL その他のメニュー]** ![](assets/more-menu.png) プラン名の右に移動し、 **[!UICONTROL 削除]** > **[!UICONTROL はい、削除します]**.

   プランが削除され、プランのリストに戻ります。

### シナリオの削除 {#delete-scenarios}

>[!IMPORTANT]
>
>シナリオを削除する際は、次の点を考慮してください。
>
>* シナリオを削除すると、すべてのイニシアチブとその情報がシナリオから削除されます。 他のシナリオにコピーした場合、イニシアチブは他のシナリオに残ります。
>* シナリオを削除すると、後続のシナリオでは削除されたシナリオの数が適用され、カウント順が保持されます。 たとえば、シナリオ 4 を削除すると、シナリオ 5 はシナリオ 4 になります。
>* シナリオに関する一部のイニシアチブが公開されると、イニシアチブにリンクされたプロジェクトが保持され、「シナリオプランナー」領域はリンクされたプロジェクトに残ります
>* 公開されたイニシアチブが別のシナリオに存在する場合、プロジェクトへのリンクを含め、そのシナリオにとどまります。 これらのイニシアチブを他のシナリオから公開すると、リンクされたプロジェクトが、それらのシナリオの新しい情報で更新されます。
>
>  プロジェクトへのイニシアチブの公開については、 [プロジェクトを更新または作成するには、 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

シナリオを削除するには：

1. シナリオを削除するプランに移動します。

   デフォルトでは、初期シナリオが表示されます。

1. クリック **[!UICONTROL シナリオの比較]**.
1. シナリオカードの右上隅にある **[!UICONTROL 詳細]** メニュー ![](assets/more-menu.png)を選択し、「 **[!UICONTROL 削除]**.

   シナリオが削除されます。

1. クリック **[!UICONTROL プランを保存]** 変更を保存します。

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


