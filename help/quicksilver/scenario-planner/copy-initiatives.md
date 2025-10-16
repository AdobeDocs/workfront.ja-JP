---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーでのイニシアチブのコピー
description: 既存のイニシアチブをコピーして、イニシアチブを作成できます。自分が作成したプランや、誰かが自分と共有するプランのイニシアチブをコピーできます。
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 86%

---

# [!DNL Scenario Planner] 内のイニシアチブをコピーする

<!--Audited: 07/2024-->

既存のイニシアチブをコピーして、イニシアチブを作成できます。自分が作成したプランや、誰かが自分と共有するプランのイニシアチブをコピーできます。

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
   <td> <p>[!UICONTROL ライト &#x200B;] 以上</p> 
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

シナリオプランナーへのアクセスについて詳しくは、[&#x200B; の使用に必要なアクセス  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md) を参照してください。

Workfrontのアクセス要件について詳しくは、[Workfrontのドキュメントへのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

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
</table>-->

## イニシアチブをコピーする

イニシアチブをコピーする際は、次の点に注意してください。

* イニシアチブをコピーすると、コピーは元のイニシアチブと同じプランに配置されます。
* イニシアチブをコピーして、元のイニシアチブから次の情報を新しいイニシアチブに追加します。

   * [!UICONTROL 期間]
   * [!UICONTROL 担当業務]
   * [!UICONTROL ユーザー]および[!UICONTROL 固定コスト]
   * [!UICONTROL 予定便益]

* イニシアチブをコピーすると、元のイニシアチブに情報が存在する場合に、プランの次の情報を変更できます。

   * 必要な担当業務数
   * [!UICONTROL コスト]
   * [!UICONTROL プランの稼動率]
   * 担当業務の稼動率
   * [!UICONTROL 純価]

* プロジェクトを読み込んで作成されたイニシアチブ、または少なくとも 1 回プロジェクトに公開されたイニシアチブをコピーすると、次のような影響があります。

   * イニシアチブに関連付けられたプロジェクトは複製されません。
   * コピーしたイニシアチブはプロジェクトに接続されません。
   * 1 回以上公開されているプロジェクトの場合、プロジェクトの [!DNL Scenario Planner] セクションは変更されません。

  プロジェクトへのイニシアチブの公開について詳しくは、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でのイニシアチブの公開によるプロジェクトのアップデートまたは作成を参照してください。

  プロジェクトへの読み込みによるイニシアチブの作成について詳しくは、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) でプランにプロジェクトを読み込むを参照してください。

## イニシアチブをコピーする

{{step1-to-scenario-planner}}

計画のリストが表示されます。

1. プランの名前をクリックして開き、コピーするイニシアチブを確認します。
1. コピーするイニシアチブの左側にあるボックスを選択し、プランの下部に表示されるメニューから、「**[!UICONTROL コピー]**」をクリックします。

   ![&#x200B; イニシアチブをコピー &#x200B;](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] はイニシアチブをすぐにコピーし、最後に選択したイニシアチブの下に配置します。

   コピーされたイニシアチブの名前は、* のコピー`<Name of original initiative>`*&#x200B;です。

   >[!NOTE]
   >
   >新しいイニシアチブの挿入場所に応じて、既存のイニシアチブの数が変わる場合があります。

1. コピーしたイニシアチブの名前を更新します。

   >[!TIP]
   >
   >イニシアチブを再度コピーする場合に混乱を避けるために、必ずイニシアチブの名前を更新することをお勧めします。

1. （オプション）新しく作成したイニシアチブの優先度を更新します。

   イニシアチブの優先順位について詳しくは、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md) のイニシアチブ優先度を更新を参照してください。

1. 「**[!UICONTROL プランを保存]**」をクリックして、変更を保存します。
