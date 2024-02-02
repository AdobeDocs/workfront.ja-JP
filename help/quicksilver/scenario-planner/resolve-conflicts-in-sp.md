---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーにおけるイニシアチブの競合の解決
description: イニシアチブが互いに競合する場合は、同じリソースを求めて競い合っています。シナリオに使用できるリソースは、シナリオのすべてのイニシアチブで必要になるリソースをすべてカバーするには十分ではありません。
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: ht
source-wordcount: '2183'
ht-degree: 100%

---

# [!DNL Scenario Planner]におけるイニシアチブの競合の解決

イニシアチブが互いに競合する場合は、同じリソースを求めて競い合っています。シナリオに使用できるリソースは、シナリオのすべてのイニシアチブで必要になるリソースをすべてカバーするには十分ではありません。

この問題が発生する可能性があるのは、次のいずれかの場合です。

* イニシアチブに必要な担当業務の数が、計画に予算計上された役割の数より多い。
* イニシアチブのコストが、計画に使用できる予算額より大きい。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> プラン*</b> </p> </td> 
   <td>[!UICONTROL Business] 以降</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>ライセンス*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td><b>製品</b> </td> 
   <td> <p>この記事で説明する機能にアクセスするためには、[!DNL Adobe Workfront Scenario Planner] 用の追加ライセンスを購入する必要があります。</p> <p>[!DNL Workfront Scenario Planner]の取得については、<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!DNL Scenario Planner]</a>の使用に必要なアクセス権を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>次に対する[!UICONTROL Edit]アクセス権またはそれ以上 [!DNL Scenario Planner]</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルを作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクトの権限</strong> </p> </td> 
   <td> <p>プランに対する[!UICONTROL Manage]権限</p> <p>プランへの追加アクセス権のリクエストについて詳しくは、<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!DNL Scenario Planner]</a>でのプランへの利用申請を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 競合の解決の概要

* 競合は、担当業務やシナリオの予算の配分超過とも考えられます。
* [!DNL Workfront] が競合を検出すると、イニシアチブの期間中の競合している月に対応するバーが赤色で表示されます。この問題が発生する可能性があるのは、次のいずれかの場合です。

   * 以前のすべてのイニシアチブが計画に予算計上されたリソースを使用した後で、イニシアチブに毎月必要な担当業務の数が、計画に予算計上された役割の数より多い。
   * 以前のすべてのイニシアチブでそれらのコストをカバーするプランの予算を使用した後で、イニシアティブの月額コストが、プランで使用可能な予算より大きい。

>[!TIP]
>
>デフォルトでは、[!DNL Scenario Planner]は、別途指定しない限り、シナリオに対して 0 個の担当業務と 0 ドルまたはシステムの通貨で 0 ドルに相当する金額が予算計上されていると仮定します。担当業務の数は、担当業務に予算計上された FTE（フルタイム当量）の数または時間数を示します。
>
>シナリオプランナーのすべての計算で、Workfront は次の値を使用します：1 FTE = 8 時間。
>
>プランと予算に対応して使用可能な役割の更新については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)でのプランを作成と編集を参照してください。

* 次のいずれかを行うことで、競合を解決できます。

   * 必要なリソースが不足している場合、シナリオのイニシアチブから自動的に追加する。この記事では、このオプションを使用して競合を解決する方法について説明します。
   * プランを編集して、シナリオの担当業務と予算のリソースを調整する。詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)でのプランの作成と編集を参照してください。

## イニシアチブ間の競合の解決

1. 競合を解決するプランに移動します。

   プランの作成については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)でのプランの作成と編集を参照してください。

   イニシアチブの作成については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)でのイニシアチブの作成と編集を参照してください。

1. （オプション）**[!DNL Initial scenario]**&#x200B;ドロップダウンメニューから、レビューするシナリオを選択します。

   >[!TIP]
   >
   >プランには、複数のシナリオが含まれる場合があります。プランの競合を確認する場合、[!DNL Workfront] では、選択されたシナリオで現在利用可能なリソースと、そのシナリオのイニシアチブで必要なリソースに注目します。シナリオについては、[ [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md)でのプランシナリオの作成と比較を参照してください。

1. 「**[!UICONTROL 競合を表示]**」が有効になっていることを確認します。これはデフォルトで有効になっています。

   ![](assets/show-scenarios-toggle-on.png)

   競合する最初のイニシアチブでは、競合する月が赤で表示され、イニシアチブ名の横に警告アイコンが表示されます。

   競合する最初のイニシアチブ以降のすべてのイニシアチブでは、プランのチャートの背景が赤で表示されます。

   イニシアチブに競合が表示された場合、少なくとも 1 つの特定の役割の担当業務の数、発生したコスト、またはその両方が、特定の月のプランに定義された担当業務の数または予算を超えていることを意味します。

   ![](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. 次のいずれかの操作を行って、存在する可能性のある競合についての詳細を把握します。

   * イニシアチブ名の横にある警告アイコンの上にマウスポインターを置くと、担当業務と予算のどちらに競合が存在するかわかります。

     ![](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

     イニシアチブで担当業務を超過して割り当てたか、コストを多く見積りすぎたかに応じて、警告アイコンの上にマウスポインターを置くと、次のオプションのいずれかが表示されます。

      * 担当業務の競合の詳細を表示
      * 予算の競合の詳細を表示
      * 担当業務と予算の詳細を表示

   * 月別にプランを表示する場合、プランのタイムラインで月の上にマウスポインターを置くと、その月に必要なリソースと、その月の競合が人物かコスト関連なのかがを表示されます。

     ![](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

     次の月次情報を、プランレベルで確認します。

      * その月に予定されているイニシアチブに対する、その月に利用可能、必須、割り当て超過の担当業務の数
      * その月に予定されているすべてのイニシアチブに対する、その月に利用可能、必須、割り当て超過のコスト

        >[!TIP]
        >
        >[!UICONTROL 利用可能]なコストとは、その月のシナリオの予算です。

   * イニシアチブの赤いバーの上にマウスポインターを置くと、その月に発生した競合に関する追加情報のボックスが表示されます。

     ![](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

     イニシアチブのレベルで、追加情報ボックスの次のフィールドを確認します。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">競合が発生する月</td> 
        <td>追加情報ボックスのタイトルに表示されます。</td> 
       </tr> 
       <tr> 
        <td role="rowheader">イニシアチブ名</td> 
        <td>追加情報ボックスのタイトルに表示されます。</td> 
       </tr> 
       <tr> 
        <td role="rowheader">[!UICONTROL Job Roles]</td> 
        <td> <p>選択した月に対して割り当て超過の、このイニシアチブに関連付けられている担当業務。次の列には、選択した月に必要な担当業務や、その月に利用可能な担当業務の数と矛盾する担当業務の情報が表示されます。</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>：選択した月のシナリオで利用可能な担当業務の数。</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong>：選択した月のイニシアティブに必要な各担当業務の数。</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]：</strong>イニシアチブで必要な数とシナリオから利用可能な数との差。 </p> </li> 
         </ul> <p>ヒント：[!UICONTROL Available] 担当業務の数が [!UICONTROL Required] 担当業務の数よりも多い場合や一致する場合でも、[!DNL Scenario Planner] が割り当て超過を示す場合があります。これは、同じ月にプランで利用できる担当業務を既に利用している上位のイニシアチブが存在するということです。 </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">コスト</td> 
        <td> <p>選択した月のイニシアチブのコスト。次の列には、選択した月に必要なコストと利用可能な予算に関する情報が表示されます。</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>：選択した月のプランから利用可能な予算です。</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong>：選択した月の、このイニシアティブに関連するコスト。</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]：</strong>イニシアチブのコストと、プランから利用可能な予算の差。 </p> </li> 
         </ul> <p>ヒント：[!UICONTROL Available] コストが、選択した月のイニシアチブの [!UICONTROL Required] コストよりも多い場合や一致する場合でも、[!DNL Scenario Planner] がコストの割当超過を示す場合があります。これは、同じ月のプランに、既に予算を使用している上位のイニシアチブが存在するということです。 </p> </td> 
       </tr> 
      </tbody> 
     </table>

1. イニシアチブの詳細パネルを開き、競合が発生した場所と解決方法に関する詳細情報を表示するには、次のいずれかの操作を実行します。

   * イニシアチブの名前の横にある警告アイコンをクリックします。
   * イニシアチブのバーをクリックします。
   * イニシアチブの名前の右にある&#x200B;**[!UICONTROL その他]**&#x200B;アイコン ![](assets/more-icon.png) をクリックし、**[!UICONTROL 編集]**&#x200B;をクリックします。

     イニシアチブの詳細パネルが右側に表示されます。

     イニシアチブに十分な人材や予算がない場合は、次のセクションの横に赤い警告アイコンが表示されます。

   * [!UICONTROL 必須担当業務]
   * [!UICONTROL コスト]

1. （条件付き）担当業務の競合があるイニシアチブの場合は、「**[!UICONTROL 必須担当業務]**」セクションを開いて、イニシアチブに必要なすべての担当業務を表示します。割り当て超過の可能性がある担当業務を特定します。イニシアチブの各月の各担当業務に必要な FTE または時間数を確認します。割り当て超過の月の FTE または時間数を示すボックスは、赤い枠で表示されます。

   ![](assets/details-panel-overallocated-roles-350x275.png)

1. （オプション）イニシアチブのタイムラインの月の横にある右向き矢印をクリックすると、担当業務の競合がある月がさらに表示されます。

   ![](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. （オプション）競合がある担当業務の下の&#x200B;**[!UICONTROL 詳細を表示]**&#x200B;をクリックすると、競合が発生している場所を確認し、プランのグラフ領域で競合する月をハイライト表示することができます。各担当業務に関する追加情報が表示されます。

   担当業務ごとに、次のフィールドが表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>各月のプランで使用可能な担当業務の数。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>プランの予算から特定の月の上位イニシアティブに割り当て済みの担当業務の数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>イニシアチブで必要な担当業務の数と、上位イニシアチブが一部の担当業務を使用した後にプランで利用できる担当業務の数の違い。Workfront では、次の式を使用して [!UICONTROL Overallocated]担当業務の数を計算します。</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >プランのグラフでは、担当業務が割り当てられている月に、各イニシアチブに必要な役割の名前と数が表示されます。担当業務の名前を確認するには、[!UICONTROL 月]ビューを選択する必要があります。

   ![](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. 担当業務の競合を解決するには、次のいずれかを行います。

   * イニシアチブの各月の担当業務の数を手動で少ない数に調整します。
   * 担当業務の名前にポインタを合わせ、**[!UICONTROL 削除]アイコン** ![](assets/delete.png) をクリックして、その担当業務をイニシアチブから削除します。
   * 「**[!UICONTROL 計画の利用可能リソースに担当業務を追加する]**」を選択し、「**[!UICONTROL 適用]**」をクリックします。

     これにより、担当業務の FTE または時間数の不足数がシナリオの「[!UICONTROL 利用可能]」フィールドに追加されます。

     >[!NOTE]
     >
     >競合を解決するために役割を追加したことにより、プラン内のすべてのシナリオではなく、選択したシナリオの[!UICONTROL 利用可能な]担当業務が変更されます。

     プランのタイムラインで月ごとに表示される上向きの緑色の矢印 ![](assets/upward-green-arrow.png) は、その月のプランにさらにリソースが追加されたことを示しています。このインジケーターを表示するには、[!UICONTROL 月]ビューを選択する必要があります。

   * （条件付き）可能な場合は、詳細パネルを閉じ、最初にプランから予算リソースが割り当てられるようにイニシアチブに高い優先度を設定します。イニシアチブの優先度の更新については、[シナリオプランナでのイニシアチブ優先度の更新](../scenario-planner/prioritize-initiatives.md)を参照してください。

1. （オプション）「**[!UICONTROL 詳細を表示しない]**」をクリックして追加の詳細ボックスを閉じ、「**[!UICONTROL 適用]**」をクリックして、担当業務に加えた変更を保存します。

1. （条件付き）コストの競合があるイニシアチブの場合は、イニシアチブの詳細パネルの「**[!UICONTROL コスト]**」セクションに移動して、イニシアチブの期間中の毎月のコストをレビューします。選択したイニシアチブのコストをカバーするための十分な資金がプランの予算に含まれていない月を特定します。使用可能な予算が不十分なボックスは赤い枠線で表示されます。
1. （オプション）イニシアチブのタイムラインの月の横にある右矢印をクリックすると、コストをカバーするための十分な予算がない月をさらに表示できます。

   ![](assets/details-panel-insufficient-costs-350x239.png)

1. （オプション）コスト情報の下にある「**[!UICONTROL 詳細を表示]**」をクリックして、競合が発生している箇所を確認し、プランのグラフで競合している月をハイライト表示します。コストタイプごとに、次の追加フィールドが表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>各月のプランの予算から賄えるコスト。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>プランの予算から上位のイニシアチブに既に割り当てられている金額。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>イニシアチブに必要なコストと、上位のイニシアチブで利用可能な予算の一部を使用した後でプランの予算から賄える金額の月ごとの差額。[!DNL Workfront] では、次の式を使用して割り当て超過コストの数値を計算します。</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] では、次の式を使用して、現在のイニシアチブに必要なコストを月ごとに計算します。</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >プランのグラフでは、コストが不十分な月には、イニシアチブに必要な役割の名前と数が表示されます。コストの金額を表示するには、月ビューを選択する必要があります。

   ![](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >プランの作成時にプランの[!UICONTROL 予算]ボックスの「[!UICONTROL 人件費を含める]」設定を無効にした場合、[!UICONTROL 人件費]行は、どのシナリオのどのイニシアチブに対しても表示されません。この場合、Workfront では、コストの競合を判断するための計算に人件費を組み込みません。プランの作成については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)でのプランの作成と編集を参照してください。

1. コストの競合を解決するには、次のいずれかを行います。

   * イニシアチブの各月の[!UICONTROL 固定費]の数値を手動で少ない数値に調整します。
   * 「**[!UICONTROL 必須担当業務]**」セクションで、可能であれば、人件費予算のある月の担当業務数を手動で調整します。これで人件費の数値が減ります。

     >[!TIP]
     >
     >人件費を手動で調整することはできません。

   * 「**[!UICONTROL 計画の予算を増額]**」を選択し、「**[!UICONTROL 適用]**」をクリックします。

     これで不足していた月のシナリオの予算に不足分の金額が追加され、シナリオ全体の予算も更新されます。

     >[!NOTE]
     >
     >コストの競合を解決するために金額を追加したことにより、プラン内のすべてのシナリオではなく、選択したシナリオの予算が変更されます。

   * （条件付き）可能な場合は、詳細パネルを閉じ、最初にプランから予算リソースが割り当てられるようにイニシアチブに高い優先度を設定します。イニシアチブの優先順位の更新について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md) のイニシアチブ優先度の更新を参照してください。

1. 「コスト」セクションに変更を加える場合は、「**[!UICONTROL 適用]**」をクリックします。
1. 「**[!UICONTROL プランを保存]**」をクリックして変更を保存します。


