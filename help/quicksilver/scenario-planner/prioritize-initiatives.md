---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーのイニシアチブ優先度を更新します
description: イニシアチブは、計画にリストされている順序で計画から担当業務と予算リソースを受け取るため、イニシアチブに優先順位を付けることが重要です。
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 86%

---

# [!DNL Scenario Planner] でイニシアチブの優先順位を更新します。

イニシアチブは、計画にリストされている順序で計画から担当業務と予算リソースを受け取るため、イニシアチブに優先順位を付けることが重要です。

自分が作成したプラン、または誰かが共有したプランに基づいて、イニシアチブに優先順位を付けることができます。

計画の作成の詳細については、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) での計画の作成と編集を参照してください。

イニシアチブの作成の詳細については、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) でのイニシアチブの作成と編集を参照してください。

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

<!--<table style="table-layout:auto"> 
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

## イニシアチブの優先順位を更新する

イニシアチブの優先順位を変更すると、プラン上のリストの順序が変更されます。

より緊急性の高い取り組みを計画の一番上に配置し、リソースが利用可能な場合にのみいつでも実行できる、より流動的な取り組みを計画の一番下に配置することをお勧めします。

>[!NOTE]
>
>[!DNL Workfront] は、プランにリストされている順序でプランリソースをイニシアチブに割り当てます。
>
>例えば、プランに 3 人の利用可能なエンジニアがいて、イニシアチブ 1 とイニシアチブ 2 の完了にはそれぞれ 2 人のエンジニアが必要で、両方とも同じ時間枠にスケジュールされている場合、Workfront は 2 人のエンジニアをイニシアチブ 1 に関連付け、残りの 1 人の利用可能なエンジニアをイニシアチブ 2 に関連付けます。この場合、イニシアチブ 2 にはエンジニアが 1 人欠けているため、競合があることが示されます。場合によっては、計画の競合を回避するには、イニシアチブの優先順位を変更することが唯一の方法である場合があります。

イニシアチブの優先度を更新するには、次の手順を実行します。

{{step1-to-scenario-planner}}

計画のリストが表示されます。

1. 計画の名前をクリックして開き、優先順位を付けるイニシアチブを探します。
1. 1 つ以上のイニシアチブ名の左側にあるボックスをクリックし、次のいずれかを実行します。

   * 選択したイニシアチブ名のいずれかの左側にあるハンドルをクリックし、リスト内でハンドルを上下にドラッグしイニシアチブの優先順位を変更します。

     Workfront には、選択したイニシアチブの数が表示されます。

     ![&#x200B; 複数選択イニシアチブ番号 &#x200B;](assets/multi-select-initiative-number.png)

   * 計画の下部にある「**[!UICONTROL 優先順位]**」ボックスをクリックし、次のオプションから選択します。

      * **[!UICONTROL 上部]**：選択したイニシアチブをイニシアチブリストの一番上に移動します。選択されたイニシアチブは計画の最初にリストされます。
      * **[!UICONTROL 下部]**：選択したイニシアチブをイニシアチブリストの一番下に移動します。選択されたイニシアチブは計画の最後にリストされます。
      * **[!UICONTROL 数字を選択]**：選択したイニシアチブを、ここで指定したイニシアチブの後に移動します。

        ![&#x200B; イニシアチブの優先順位付け &#x200B;](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] は、選択したイニシアチブを指定した場所に即座に配置し、それに応じてすべてのイニシアチブの数が更新されます。

1. 「**[!UICONTROL 計画を保存]**」をクリックして、変更を保存します。
