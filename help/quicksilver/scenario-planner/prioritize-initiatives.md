---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーでイニシアチブの優先順位を更新する
description: イニシアチブは、計画にリストされている順序で計画から担当業務と予算リソースを受け取るため、イニシアチブに優先順位を付けることが重要です。
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 88%

---

# [!DNL Scenario Planner] でイニシアチブの優先順位を更新します。

イニシアチブは、計画にリストされている順序で計画から担当業務と予算リソースを受け取るため、イニシアチブに優先順位を付けることが重要です。

自分が作成したプラン、または誰かが共有したプランに基づいて、イニシアチブに優先順位を付けることができます。

計画の作成の詳細については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) での計画の作成と編集を参照してください。

イニシアチブの作成の詳細については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) でのイニシアチブの作成と編集を参照してください。

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

     ![](assets/multi-select-initiative-number.png)

   * 計画の下部にある「**[!UICONTROL 優先順位]**」ボックスをクリックし、次のオプションから選択します。

      * **[!UICONTROL 上部]**：選択したイニシアチブをイニシアチブリストの一番上に移動します。選択されたイニシアチブは計画の最初にリストされます。
      * **[!UICONTROL 下部]**：選択したイニシアチブをイニシアチブリストの一番下に移動します。選択されたイニシアチブは計画の最後にリストされます。
      * **[!UICONTROL 数字を選択]**：選択したイニシアチブを、ここで指定したイニシアチブの後に移動します。

        ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] は、選択したイニシアチブを指定した場所に即座に配置し、それに応じてすべてのイニシアチブの数が更新されます。

1. 「**[!UICONTROL 計画を保存]**」をクリックして、変更を保存します。
