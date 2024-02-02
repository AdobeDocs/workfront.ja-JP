---
product-area: enterprise-scenario-planner-product-area
keywords: 公開,計画,プロジェクト,シナリオ,シナリオ
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーでイニシアチブを公開して、プロジェクトをアップデートまたは作成
description: 既存のイニシアチブからプロジェクトを作成したり、Adobe Workfront Scenario Planner でシナリオを公開して、イニシアチブに以前リンクされていたプロジェクトをアップデートしたりできます。
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: ht
source-wordcount: '1694'
ht-degree: 100%

---

# [!DNL Scenario Planner] でイニシアチブをアップデートまたは作成

[!DNL Adobe Workfront Scenario Planner] からシナリオを公開すると、以下のことが実現されます。

* シナリオのイニシアチブから複数のプロジェクトを作成し、それらをリンクします。
* シナリオのイニシアチブに既にリンクされているプロジェクトを、リンクされたイニシアチブからの情報でアップデートします。プロジェクトをプランに読み込む際に、プロジェクトをイニシアチブにリンクすることもできます。詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) 内のプランにプロジェクトを読み込みを参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] プラン*</p> </td> 
   <td>[!UICONTROL Business] 以降</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] ライセンス*</p> </td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td>製品 </td> 
   <td> <p>この記事で説明する機能にアクセスするには、[!DNL Adobe Workfront Scenario Planner] 用の追加ライセンスを購入する必要があります。</p> <p>[!DNL Workfront Scenario Planner] の取得について詳しくは、<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!DNL Scenario Planner]</a> を使用する場合に必要なアクセス権を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>アクセスレベル*</p> </td> 
   <td> 
    <ul> 
    <li>[!DNL Scenario Planner] およびプロジェクト用の[!UICONTROL Edit]アクセス権</li></ul>

<p><b>メモ</b>

まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルを作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>オブジェクト権限</p> </td> 
   <td> 
    <ul> 
     <li>プランに対する[!UICONTROL Manage]権限 </li> 
     <li>公開済みプロジェクトに対する[!UICONTROL Manage]権限</li> 
    </ul> <p>プロジェクトへの追加アクセス権のリクエストについて詳しくは、<a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトの利用申請</a>を参照してください。</p> <p>プランへの追加アクセス権のリクエストについて詳しくは、<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!DNL Scenario Planner]</a> でのプランへの利用申請を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Workfront Scenario Planner]への追加アクセス権について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md) を使用するために必要なアクセス権を参照してください。

## 前提条件

開始する前の確認事項。

* 計画からイニシアチブを公開する前に、計画を作成して保存する必要があります。

## プロジェクトへのイニシアチブの公開に関する考慮事項

* 1 つのプランから公開できるシナリオは 1 つだけです。
* 1 つのイニシアチブは 1 つのプロジェクトにのみリンクできます。
* 複数のイニシアチブが異なるプランに属している場合、1 つのプロジェクトを複数のイニシアチブにリンクできます。

  >[!TIP]
  >
  >プロジェクトが複数のプラン上に存在し、すべてのプランからプロジェクトに情報を公開する場合、最新の公開によって、プロジェクト上の既存の [!DNL Scenario Planner] 情報が上書きされます。

* プランにプロジェクトを読み込んでプラン上にイニシアチブが作成された場合、イニシアチブを公開すると、リンクされたプロジェクトもイニシアチブの情報でアップデートされます。

  >[!TIP]
  >
  >同じプロジェクトを複数のプランに読み込むことができます。公開すると、複数のイニシアチブにリンクされているプロジェクトのイニシアチブ情報が上書きされる場合があります。

  プロジェクトへの読み込みによるイニシアチブの作成について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) でプランにプロジェクトを読み込むを参照してください。

* プロジェクトに対して行った変更は、リンクされたイニシアチブには転送されません。



## イニシアチブを公開

>[!IMPORTANT]
>
>プラン上のイニシアチブに変更（競合の解決を含む）を加えた場合、新しい情報をプロジェクトに表示するには、イニシアチブを再公開する必要があります。この情報は、対応するイニシアチブを公開する場合にのみ、イニシアチブにリンクされたプロジェクトに表示されます。イニシアチブ間の競合の解決方法について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md) でのイニシアチブの競合の解決を参照してください。

1. Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、次に「**[!UICONTROL シナリオ]**」をクリックします。
1. （オプションおよび条件付き）既存の計画から公開する場合は、計画の右上隅にある&#x200B;**[!UICONTROL フィルター]**&#x200B;アイコン ![](assets/filter-nwepng.png) をクリックし、次のオプションのいずれかを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>自分が所有しているプランまたは自分と共有しているプランがすべて表示されます。これがデフォルトです。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL My plans]</td> 
      <td>自分で作成したプランを表示します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Shared with me]</td> 
      <td> <p>自分では作成していないが自分と共有しているプランを表示します。</p> <p>重要：プランを公開するには、共有しているプランに対する [!UICONTROL Manage] 権限が必要です。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. （オプション）**[!UICONTROL 検索]**&#x200B;アイコン ![](assets/search-icon.png) をクリックし、プランの名前を入力し始めると、リスト内でプランがすぐに見つかります。
1. （条件付き）新しいプランから公開するには、プランを作成します。

   プランの作成については、[プランの作成と編集： [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)を参照してください。

1. （オプション）既存のプランの名前をクリックし、そのプランの新しいシナリオを作成します。

   プランのシナリオの作成については、[プランシナリオの作成と比較： [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md)を参照してください。

1. （オプション）既存のプランまたは新しいプランのイニシアチブを更新するか、新しいイニシアチブを作成します。

   イニシアチブの作成については、[イニシアチブの作成と編集： [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)を参照してください。

1. 「**[!UICONTROL 計画の保存]**」をクリックします。
1. 公開するシナリオを&#x200B;**[!UICONTROL 最初のシナリオ]**&#x200B;ドロップダウンメニューから選択して、右上隅にある&#x200B;**[!UICONTROL 公開に移動]**&#x200B;アイコン ![](assets/go-to-publish-button-icon.png) をクリックします。

   または

   「**[!UICONTROL シナリオを比較する]**」をクリックし、公開元となるシナリオカードにポインタを合わせ、**[!UICONTROL 公開に移動]**&#x200B;アイコン ![](assets/go-to-publish-button-icon.png) をクリックします。

   [!UICONTROL イニシアティブを公開]ページが表示され、シナリオ内のすべてのイニシアチブが一覧表示されます。いずれかのイニシアチブが以前に公開されている場合は、その名前の後にプロジェクトアイコン ![](assets/project-icon-sp.png) が表示され、**[!UICONTROL 最終公開日]**&#x200B;がリストに入力されます。

   >[!TIP]
   >
   >プロジェクトを読み込んで作成されたイニシアチブには、名前の右側にプロジェクトアイコン ![](assets/project-icon-sp.png) も表示されます。

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. （オプションおよび条件付き）既存のプランから公開する場合は、プランの右上隅にある&#x200B;**[!UICONTROL フィルター]**&#x200B;アイコン ![](assets/filter-nwepng.png) をクリックし、次のオプションのいずれかを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>選択したシナリオのすべてのイニシアチブを表示します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Published]</td> 
      <td>自分自身または別のユーザーが以前に公開したイニシアチブを表示します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unpublished]</td> 
      <td> <p>未公開のイニシアチブを表示します。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. （オプション）**[!UICONTROL 検索]**&#x200B;アイコン ![](assets/search-icon.png) をクリックし、プランの名前を入力し始めると、リスト内でイニシアチブがすぐに見つかります。
1. 公開する 1 つまたは複数のイニシアチブを選択し、そこからプロジェクトを作成または更新したあと、「**[!UICONTROL イニシアチブを公開]**」をクリックします。

   これにより、選択した各イニシアチブから新しいプロジェクトが作成され、公開されたイニシアチブが既にプロジェクトにリンクされている場合は、関連付けられている既存のプロジェクトが更新されます。

   >[!TIP]
   >
   >新しいプロジェクトには、公開されたイニシアチブと同じ名前が付けられます。

1. （条件付き）次のいずれかを行います。

   * 1 つのイニシアチブを公開した場合は、「**[!UICONTROL 関連プロジェクトを表示]**」をクリックして、そのイニシアチブから作成または更新されたプロジェクトを開きます。
   * 複数のイニシアチブを公開した場合は、「**[!UICONTROL 関連プロジェクトを表示]**」をクリックして、イニシアチブから公開されたプロジェクトのリストを開きます。[!DNL Workfront] では、デフォルトで[!DNL Scenario Planner]プロジェクトフィルターをプロジェクトのリストに適用します。直近に公開されたプロジェクトがリストの一番上に表示されます。

     ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. プロジェクトに関するイニシアチブ情報を表示するには、次の領域に移動します。

   * **「[!UICONTROL 更新]」セクション**：プロジェクトがイニシアチブから作成または更新されたことを示すために更新が公開されます。更新には、プロジェクトを作成または更新したイニシアチブの名前と、そのイニシアチブを含んだプランのリンクされた名前が含まれます。更新内のプランの名前をクリックすると、[!DNL Scenario Planner]でプランを開くことができます。

     ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **「[!UICONTROL プロジェクト詳細]」セクションの[!UICONTROL 概要]領域**：この領域には、リンクされたイニシアチブからの情報を含んだ新しい「[!DNL Scenario Planner]」セクションが作成されます。

     ![](assets/scenario-planner-on-project-details-350x135.png)

     次のイニシアチブ情報は、「[!UICONTROL プロジェクト詳細]」セクションの[!DNL Scenario Planner]領域に公開されています。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Duration]</span> </td> 
        <td><span>プロジェクトがイニシアチブにリンクされている場合、対応するイニシアチブの期間。このフィールドは編集できません。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Last Published Date]</span> </td> 
        <td><span>対応するイニシアチブからプロジェクトが最後に公開された日付。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Start Date]</span> </td> 
        <td><span>プロジェクトがイニシアチブにリンクされる、イニシアチブの開始月の初日。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative End Date]</span> </td> 
        <td><span>プロジェクトがイニシアチブにリンクされる、イニシアチブの終了月の最終日。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Job Roles in FTEs and Hours]</span> </td> 
        <td> <p>関連付けられている担当業務とそのイニシアチブへの時間割り当てに関する情報。これには以下が含まれます。</p> 
         <ul> 
          <li>担当業務名</li> 
          <li>FTE の数</li> 
          <li> <p>すべての FTE の時間数</p> <p>時間数または FTE 数を使用して、プランまたはイニシアチブに必要な担当業務の量を見積もることができます。</p> <p>詳しくは、<a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">シナリオプランナでのプランの作成と編集</a>を参照してください。 </p> </li> 
         </ul> 
      <p><b>ヒント</b>

     イニシアチブ内の月ごとに担当業務の数が異なる場合、このフィールドには、イニシアチブに必要な担当業務の最大数が表示されます。例えば、1 月には 1 名のコンサルタントが、2 月には 2 名のコンサルタントが必要な場合、この列にはすべての月に対して、2 FTE と、2 FE に対応する時間数が表示されます。</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >プロジェクトへの[!UICONTROL 表示]アクセス権を持つすべてのユーザーには、[!UICONTROL 概要]領域に「[!DNL Scenario Planner]」セクションが表示されます。この領域を「[!UICONTROL 詳細]」セクションに表示するかどうかを、レイアウトテンプレートを使用して制御できます。ユーザーにレイアウトテンプレートが関連付けられていない場合、この領域はデフォルトで表示されます。
     >
     >   
     >   
     >   * レイアウトテンプレートを使用した「[!UICONTROL 詳細]」セクションへの領域の追加または削除については、[レイアウトテンプレートを使用した[!UICONTROL 詳細]表示のカスタマイズ](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。
     >   * [!UICONTROL プロジェクト詳細]の[!UICONTROL 概要]領域での情報表示について詳しくは、[[!UICONTROL プロジェクト][!UICONTROL 概要]領域での情報の管理](../manage-work/projects/manage-projects/understand-project-overview-area.md)を参照してください。
     >   
     >

   * **[!UICONTROL ワークロードバランサー]にある[!UICONTROL 役割割り当て]パネルまたはプロジェクトのタスクリスト**：プロジェクトの役割割り当てに加えて、イニシアティブの役割割り当てに関する情報もこの領域に入力されます。

     詳しくは、[プロジェクトとイニシアチブ間でのリソース割り当て調整の概要](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)を参照してください。

     ![](assets/role-allocation-panel-350x174.png)

     プロジェクトの日付やリソースを変更しても、対応するイニシアチブや、イニシアチブ情報を含んだプロジェクト上の領域には影響しません。

   * **プロジェクトの[!UICONTROL ビジネスケース]の[!UICONTROL リソース予算計上]領域**：[!DNL Scenario Planner]情報を使用してプロジェクトリソースを管理するための新しいオプションが、プロジェクトの[!UICONTROL ビジネスケース]の[!UICONTROL リソース予算計上]領域に追加されました。

     詳しくは、[[!UICONTROL ビジネスケース]でのリソースの計上： [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)を参照してください。

     ![](assets/sp-in-business-case-selected-350x110.png)

1. （オプション）シナリオの公開後、次の情報を[!DNL Scenario Planner]でレビューします。

   * 公開したシナリオは、イニシアチブを公開した後の最初のシナリオになります。
   * シナリオを少なくとも 1 回公開した後は、他のシナリオからは公開できません。
   * 「[!UICONTROL 公開に移動]」オプションは、1 つ以上のイニシアチブがシナリオから公開された後に、他のすべてのシナリオから削除されます。
   * プラン内で、公開したイニシアチブのプロジェクトアイコンの横に緑色のインジケータが表示されます。

     ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * 緑色の「公開済み」インジケーターがシナリオの上部とシナリオカードに表示され、シナリオカードの「公開済み」フィールドに、公開されたシナリオ内のイニシアチブの数が表示されます。

     ![](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >シナリオのイニシアチブから公開されたすべてのプロジェクトが削除された場合、シナリオが公開されたことを示す表示は削除されます。詳しくは、[プロジェクトを削除](../manage-work/projects/manage-projects/delete-projects.md)を参照してください。

1. （オプション）イニシアチブに関する情報を更新し、前述の手順を繰り返して、イニシアチブを再公開し、リンクされたプロジェクトに関するイニシアチブ情報を更新します。

   イニシアチブの編集については、[イニシアチブの作成と編集： [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)を参照してください。


