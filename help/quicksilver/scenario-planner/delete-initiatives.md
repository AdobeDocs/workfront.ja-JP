---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーのイニシアチブを削除
description: 自分が作成した計画や、誰かが自分と共有した計画のイニシアチブを削除できます。削除したイニシアチブを復元することはできません。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 84%

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

*詳しくは、[Workfrontへのアクセス要件ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

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
