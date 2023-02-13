---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオ・プランナでの計画シナリオの作成と比較
description: 企業の長期的な戦略を計画する際には、最初に考えてもいない情報が多数存在します。 関係者が受け入れられる最終的な戦略に到達するには、時間と実験が必要です。 計画に対して複数のシナリオを作成するために「どのような場合」の分析を実行すると、潜在的な状況を正確に予測および評価し、最終的に最適な計画を作成するのに役立ちます。
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 1%

---

# でのプランシナリオの作成と比較 [!DNL Scenario Planner]

企業の長期的な戦略を計画する際には、最初に考えてもいない情報が多数存在します。 関係者が受け入れられる最終的な戦略に到達するには、時間と実験が必要です。 計画に対して複数のシナリオを作成するために「どのような場合」の分析を実行すると、潜在的な状況を正確に予測および評価し、最終的に最適な計画を作成するのに役立ちます。

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
   <td> <p>アクセス権を [!DNL Scenario Planner]</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクト権限</strong> </p> </td> 
   <td> <p>プランに対する [!UICONTROL 管理 ] 権限</p> <p>プランへの追加アクセス権のリクエストについて詳しくは、 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">内のプランへのアクセスをリクエスト [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## シナリオの作成

シナリオは、プランのコピーです。 シナリオは必要な数だけ作成できます。 ただし、シナリオを簡単に比較できるよう、シナリオの数を最小限に抑えることをお勧めします。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png)を選択し、「 [!UICONTROL シナリオ].

1. プランを作成します。

   プランの作成について詳しくは、 [でプランを作成および編集 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   最初に作成したプランは、自動的に[!UICONTROL 初期シナリオ].&quot;

1. 既存のシナリオの横にある下向き矢印をクリックし、 **[!UICONTROL コピー]** アイコン

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   これにより、コピーされたシナリオと同じ情報を持つ新しいシナリオが作成されます。 自動的に「[!UICONTROL シナリオ 2]もし君の計画の二番目のシナリオなら」[!UICONTROL シナリオ 3]「もし三番目なら、そうです。 シナリオの名前は変更できません。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. 次のいずれかの方法で、新しいシナリオを更新します。

   * イニシアチブの作成、更新、削除

      >[!TIP]
      >
      >シナリオでイニシアチブを削除すると、そのイニシアチブは選択したシナリオからのみ削除され、すべてのシナリオからは削除されません。

      イニシアチブの作成については、 [のイニシアチブを作成および編集します [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * イニシアチブの優先度を更新する
   * 担当者または予算情報の調整
   * シナリオでのイニシアチブの競合を確認および調整します

      競合の解決について詳しくは、 [次の場所でのイニシアチブの競合を解決 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. クリック **[!UICONTROL プランを保存]** 変更を保存します。

## シナリオを比較する

シナリオを作成した後、シナリオを比較して、組織に最適なシナリオを見つけることができます。

1. シナリオを比較するプランに移動します。
1. クリック **[!UICONTROL シナリオの比較]**. シナリオの比較ページが表示されます。

   プランの既存のシナリオはすべて、カード形式で並べて表示されます。 最初のシナリオは常に最初に表示され、静的です。

   ![](assets/scenario-cards-overlapping-350x166.png)

1. （オプション）右にスクロールして、すべてのシナリオカードを表示します。

   シナリオカードには、次の情報が表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>シナリオの名前</td> 
      <td> <p>Workfrontによって自動生成された名前。編集できません。 例えば、「[!UICONTROL 最初のシナリオ ]」、「[!UICONTROL シナリオ 2]」などです。 </p> </td> 
     </tr> 
     <tr> 
      <td>シナリオの説明</td> 
      <td>シナリオの詳細を説明できる手動のエントリ。 </td> 
     </tr> 
     <tr> 
      <td>使用可能なジョブの役割</td> 
      <td>プランの期間中にプランの予算から使用可能なジョブの役割の数。 </td> 
     </tr> 
     <tr> 
      <td>必須担当業務</td> 
      <td>イニシアチブに基づいて必要なジョブの役割の数。 </td> 
     </tr> 
     <tr> 
      <td>予算</td> 
      <td>このシナリオのプランに定義された合計予算です。 プランの予算情報については、 <a href="../scenario-planner/plans-overview.md" class="MCXref xref">「プランの概要」( [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>コスト</td> 
      <td>シナリオのイニシアチブに関連するコスト。 コストの詳細については、 <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">以下のイニシアティブの概要 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>稼働率</td> 
      <td>このシナリオのプランの [!UICONTROL Budget Utilization] の割合。 [!UICONTROL 予算使用率 ] の割合について詳しくは、 <a href="../scenario-planner/plans-overview.md" class="MCXref xref">「プランの概要」( [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>純価</td> 
      <td>このシナリオのプランの [!UICONTROL Net Value]。 プランの [!UICONTROL Net Value] について詳しくは、 <a href="../scenario-planner/plans-overview.md" class="MCXref xref">「プランの概要」( [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>イニシアチブ</td> 
      <td>このシナリオのプランのイニシアチブ数。</td> 
     </tr> 
     <tr> 
      <td>競合</td> 
      <td>このシナリオのプラン内の競合の種類を示すイニシアチブの数。 イニシアチブの競合について詳しくは、 <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">次の場所でのイニシアチブの競合を解決 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >最初のシナリオと追加のシナリオで情報が異なる場合は、変更された値の横に上向き矢印または下向き矢印が表示され、最初のシナリオと比較して、その値の増減を示します。
   >
   >
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >例えば、予算、役割の数、イニシアチブの数がシナリオごとに変わる場合があります。

1. シナリオの名前をクリックしてアクセスし、変更を加えます。

   詳しくは、 [シナリオの作成](#create-scenarios) 」の節を参照してください。

1. クリック **[!UICONTROL 説明を追加]** シナリオの説明を追加するには

   または

   説明フィールドをクリックして更新し、画面の任意の場所をクリックして変更を保存します。

1. （オプション） **[!UICONTROL 詳細]** メニュー ![](assets/more-icon.png) から **[!UICONTROL コピー]** または **[!UICONTROL 削除]** シナリオ。

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   シナリオをコピーすると、自動的にカードページに表示され、次のパターンに従って名前が変更されます。&quot;[!UICONTROL シナリオ] `<next number in order>`.&quot;

1. （条件付き）クリックした場合 **[!UICONTROL 削除]**&#x200B;をクリックし、 **[!UICONTROL はい、削除します]** をクリックして確定します。

   削除したシナリオは復元できません。

   シナリオの削除について詳しくは、 [のプランを削除 [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. クリック **[!UICONTROL プランを保存]** をクリックして、シナリオとプランを保存します。
