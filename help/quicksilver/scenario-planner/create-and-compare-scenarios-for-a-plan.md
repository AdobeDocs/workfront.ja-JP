---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーでプランシナリオを作成および比較
description: 企業の長期戦略を計画する際、初期段階には持っていない、または考えてもみない情報は多くあります。関係者が受け入れられる最終的な戦略に到達するには、時間と実験が必要です。「what if」分析を実施して計画の複数のシナリオを作成すると、潜在的な状況を正確に予測および評価し、最終的に可能な限り最適な計画を策定するのに役立ちます。
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 88%

---

# [!DNL Scenario Planner] でプランシナリオを作成および比較

<!--Audited: 07/2024-->

企業の長期戦略を計画する際、初期段階には持っていない、または考えてもみない情報は多くあります。関係者が受け入れられる最終的な戦略に到達するには、時間と実験が必要です。「what if」分析を実施して計画の複数のシナリオを作成すると、潜在的な状況を正確に予測および評価し、最終的に可能な限り最適な計画を策定するのに役立ちます。

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

## シナリオの作成

シナリオは計画のコピーです。シナリオは必要な数だけ作成できます。ただし、簡単に比較できるように、シナリオの数を最小限に抑えることをお勧めします。

{{step1-to-scenario-planner}}

1. プランを作成するか、既存のプランの名前をクリックします。

   計画の作成について詳しくは、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) で計画を作成および編集を参照してください。

   最初に作成したプランは、「[!UICONTROL 初期シナリオ]」として自動的に保存されます。

1. 既存のシナリオの横にある下向き矢印をクリックし、**[!UICONTROL コピー]**&#x200B;アイコンを選択します。

   ![&#x200B; シナリオをコピー &#x200B;](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   これにより、コピーされたシナリオと同じ情報を持つ新しいシナリオが作成されます。計画の 2 番目のシナリオの場合は「[!UICONTROL シナリオ 2]」、3 番目のシナリオの場合は「[!UICONTROL シナリオ 3]」という名前が自動的に付けられます。シナリオ名は変更できません。 作成できるコピーの数に制限はありません。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. 次のいずれかの方法で、新しいシナリオを更新します。

   * イニシアチブを作成、更新、または削除

     >[!TIP]
     >
     >シナリオのイニシアチブを削除すると、すべてのシナリオからではなく、選択したシナリオからのみ削除されます。

     イニシアチブの作成について詳しくは、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) のイニシアチブを作成および編集を参照してください。

   * イニシアチブの優先順位を更新
   * 人材や予算の情報を調整
   * シナリオのイニシアチブの競合を確認して調整

     競合の解決について詳しくは、[イニシアチブの競合を解決 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)を参照してください。

1. 「**[!UICONTROL 計画の保存]**」をクリックして、変更を保存します。

## シナリオを比較する

シナリオを作成した後、それらを比較して組織に最適なシナリオを見つけることができます。

1. シナリオを比較する計画に移動します。
1. 「**[!UICONTROL シナリオを比較]**」をクリックします。シナリオ比較ページが表示されます。

   計画の既存のシナリオはすべて、横に並べたカード形式で表示されます。初期シナリオは常に最初にリストされ、静的です。

   ![&#x200B; セナリオカード &#x200B;](assets/scenario-cards-overlapping-350x166.png)

1. （オプション）右にスクロールして、すべてのシナリオカードを表示します。

   次の情報がシナリオカードに表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>シナリオの名前</td> 
      <td> <p>Workfront によって自動的に生成される名前であり、編集することはできません。例えば、「[!UICONTROL Initial scenario]」、「[!UICONTROL Scenario 2]」などです。 </p> </td> 
     </tr> 
     <tr> 
      <td>シナリオの説明</td> 
      <td>シナリオの詳細を説明できる手動入力。 </td> 
     </tr> 
     <tr> 
      <td>利用可能な担当業務</td> 
      <td>計画の期間中に計画の予算から利用可能な職務の数。 </td> 
     </tr> 
     <tr> 
      <td>必須担当業務</td> 
      <td>イニシアチブに基づく、必要な担当業務の数。 </td> 
     </tr> 
     <tr> 
      <td>予算</td> 
      <td>このシナリオでプランに定義された総予算。プランに関する予算情報については、<a href="../scenario-planner/plans-overview.md" class="MCXref xref">[!DNL Scenario Planner]</a> のプランの概要を参照してください。 </td> 
     </tr> 
     <tr> 
      <td>コスト</td> 
      <td>シナリオのイニシアチブに関連するコスト。コストについて詳しくは、<a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">[!DNL Scenario Planner]</a> のイニシアチブの概要を参照してください。 </td> 
     </tr> 
     <tr> 
      <td>稼働率</td> 
      <td>このシナリオのプランの [!UICONTROL Budget Utilization] の割合。[!UICONTROL Budget Utilization] の割合について詳しくは、<a href="../scenario-planner/plans-overview.md" class="MCXref xref">[!DNL Scenario Planner]</a> のプランの概要を参照してください。 </td> 
     </tr> 
     <tr> 
      <td>純価</td> 
      <td>このシナリオのプランの [!UICONTROL Net Value]。プランの [!UICONTROL Net Value] について詳しくは、<a href="../scenario-planner/plans-overview.md" class="MCXref xref">[!DNL Scenario Planner]</a> のプランの概要を参照してください。 </td> 
     </tr> 
     <tr> 
      <td>イニシアチブ</td> 
      <td>このシナリオのプランのイニシアチブ数。</td> 
     </tr> 
     <tr> 
      <td>競合</td> 
      <td>このシナリオのプラン内の競合の種類を示すイニシアチブの数。イニシアチブの競合について詳しくは、<a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">[!DNL Scenario Planner]</a> でのイニシアチブの競合を解決を参照してください。 </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >初期シナリオと追加のシナリオで情報が異なる場合は、変更された値の横に上向き矢印または下向き矢印が表示され、初期シナリオと比較して、その値の増減を示します。
   >
   >
   >![&#x200B; シナリオカードの矢印 &#x200B;](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >例えば、予算、担当業務の数、イニシアチブの数がシナリオごとに変わる場合があります。

1. シナリオの名前をクリックしてアクセスし、変更を加えます。

   詳しくは、この記事の[シナリオを作成](#create-scenarios)の節を参照してください。

1. 「**[!UICONTROL 説明を追加]**」をクリックしてシナリオの説明を追加します。

   または

   説明フィールドをクリックして更新し、画面の任意の場所をクリックして変更を保存します。

1. （任意） **[!UICONTROL 詳細]** メニュー ![&#x200B; 詳細アイコン &#x200B;](assets/more-icon.png) をクリックして、シナリオを **[!UICONTROL コピー]** または **[!UICONTROL 削除]** します。

   ![&#x200B; シナリオをコピーまたは削除 &#x200B;](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   シナリオをコピーすると、自動的にカードページに表示され、「[!UICONTROL シナリオ] `<next number in order>`」のパターンに従って名前が変更されます。

1. （条件付き）「**[!UICONTROL 削除]**」をクリックした場合は、「**[!UICONTROL はい、削除します]**」をクリックして確定します。

   削除したシナリオは復元できません。

   シナリオの削除について詳しくは、[&#x200B; [!DNL Scenario Planner]](../scenario-planner/delete-plans.md) のプランを削除を参照してください。

1. 「**[!UICONTROL プランを保存]**」をクリックして、シナリオとプランを保存します。
