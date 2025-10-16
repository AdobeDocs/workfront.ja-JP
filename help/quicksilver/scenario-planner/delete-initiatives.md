---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーでのイニシアチブの削除
description: 自分が作成した計画や、誰かが自分と共有した計画のイニシアチブを削除できます。削除したイニシアチブを復元することはできません。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 82%

---

# [!DNL Scenario Planner]内のイニシアチブを削除

自分が作成した計画や、誰かが自分と共有した計画のイニシアチブを削除できます。削除したイニシアチブを復元することはできません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] package</p> </td> 
   <td> 
   <p>WorkfrontUltimate</p>
<p><b>メモ</b></p>
<p>別のWorkfront パッケージをお持ちの場合は、Workfront担当者にお問い合わせください。</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] ライセンス</p> </td> 
   <td> <p>[!UICONTROL ライト ] 以上</p> 
   <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
    <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>[!UICONTROL Edit]アクセス権 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>オブジェクト権限 </p> </td> 
   <td> <p>プランに対する[!UICONTROL Manage]権限</p> </td> 
  </tr> 
 </tbody> 
</table>

シナリオプランナーへのアクセスについて詳しくは、[ の使用に必要なアクセス  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md) を参照してください。

Workfrontのアクセス要件について詳しくは、[Workfrontのドキュメントへのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## イニシアチブを削除

イニシアチブを削除する際は、以下の点を考慮してください。

* イニシアチブを削除すると、そのイニシアチブに関連付けられている必要な担当業務数とコスト情報がプランから削除されます。
* プロジェクトを読み込んで作成したイニシアチブを削除しても、イニシアチブに関連付けられたプロジェクトは削除されません。
* 1 回以上プロジェクトに公開されたイニシアチブを削除すると、結果として以下のようになります。

   * イニシアチブはシナリオから削除されますが、[!DNL Scenario Planner]エリアは「[!UICONTROL プロジェクトの詳細]」セクションに残ります。
   * 削除したイニシアチブがシナリオで唯一の公開イニシアチブである場合は、プランが公開されたことを示す指標も削除されます。

     プロジェクトへのイニシアチブの公開について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でのイニシアチブの公開によるプロジェクトのアップデートまたは作成を参照してください。

     プロジェクトの読み込みによるイニシアチブの作成について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) のプランにプロジェクトを読み込むを参照してください。

1 度に 1 つのイニシアチブを削除することも、複数のイニシアチブを一括で削除することもできます。

* [イニシアチブを 1 つ削除](#delete-one-initiative)
* [イニシアチブを一括削除](#delete-initiatives-in-bulk)

### イニシアチブを 1 つ削除 {#delete-one-initiative}

{{step1-to-scenario-planner}}

計画のリストが表示されます。

1. 計画の名前をクリックして開き、削除するイニシアチブを確認します。
1. 次のいずれかの操作を行います。

   * イニシアチブ名の右側にある **[!UICONTROL その他メニュー]**![ その他メニュー ](assets/more-menu.png) をクリックし、**[!UICONTROL 削除]**/**[!UICONTROL はい、削除します]** をクリックします。

   * イニシアチブの左側にあるボックスを選択し、計画の下部に表示されるフローティングメニューで「**[!UICONTROL 削除]**」、「**[!UICONTROL はい、削除します]**」の順にクリックします。

   イニシアチブとその担当業務およびコスト情報は、プランから削除されます。

1. 「**[!UICONTROL 計画を保存]**」をクリックして、変更を保存します。

### イニシアチブを一括削除 {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

計画のリストが表示されます。

1. 計画の名前をクリックして開き、削除するイニシアチブを確認します。
1. 削除するイニシアチブの左側にあるボックスを選択し、計画の下部に表示されるメニューから、「**[!UICONTROL 削除]**」、「**[!UICONTROL はい、削除します]**」の順にクリックします。

   ![ イニシアチブの管理メニュー ](assets/bottom-manage-initiative-menu-350x45.png)

   イニシアチブとその担当業務およびコスト情報は、プランから削除されます。

1. 「**[!UICONTROL 計画を保存]**」をクリックして、変更を保存します。
