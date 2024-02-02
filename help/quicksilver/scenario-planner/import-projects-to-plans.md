---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーのプランにプロジェクトを読み込む
description: 既存のプロジェクトをプランに読み込むことができます。読み込まれたプロジェクトはイニシアチブに変換され、新規イニシアチブの管理と同じように、プラン内で管理できます。元のプロジェクトは、新規イニシアチブにリンクされたままです。
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: ht
source-wordcount: '1699'
ht-degree: 100%

---

# [!DNL Scenario Planner] 内のプランへのプロジェクトの読み込み

既存のプロジェクトをプランに読み込むことができます。読み込まれたプロジェクトはイニシアチブに変換され、新規イニシアチブの管理と同じように、プラン内で管理できます。元のプロジェクトは、新規イニシアチブにリンクされたままです。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

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
   <td> <p>次に対する[!UICONTROL Edit]以上のアクセス権： [!DNL Scenario Planner]</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルを作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>オブジェクトの権限</strong> </p> </td> 
   <td> <p>プランに対する[!UICONTROL Manage]権限</p> <p>プランへの追加アクセス権のリクエストについて詳しくは、<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">シナリオプランナーのプランへのアクセス権をリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## プロジェクトを新規イニシアチブとしてプランへのの読み込む際の考慮事項

* プロジェクトを新規イニシアチブとしてプランに読み込む前に、プロジェクトを作成する必要があります。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* プロジェクトを新規イニシアチブとしてプランに読み込むには、プロジェクトに対して少なくとも[!UICONTROL 表示]権限が必要です。
* 同じプロジェクトを複数のプランに読み込むことができます。
* 読み込むプロジェクトには、プランの時間枠に日付が含まれている必要があります。[!UICONTROL 予定完了日]がプランの開始日より早いプロジェクトや、[!UICONTROL 予定開始日]がプランの終了日より遅いプロジェクトは読み込むことができません。
* 一度に 100 以上のプロジェクトを読み込むことはできません。
* 一部のプロジェクト情報もプランに読み込まれ、イニシアチブ情報になります。プランに読み込まれてイニシアチブ情報になるプロジェクト情報について詳しくは、この記事の[プランに読み込まれたプロジェクト情報](#project-information-imported-into-the-plan)の節を参照してください。
* リンクされたプロジェクトで行われた変更は、プランのイニシアチブには影響しません。
* プランのイニシアチブに対して行われた変更は、リンクされたプロジェクトには自動的には影響しません。イニシアチブの変更は、プランからイニシアチブを公開する場合にのみ、リンクされたプロジェクトに影響します。公開イニシアチブがリンクされたプロジェクトに与える影響について詳しくは、「[ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でイニシアチブを公開することに よるプロジェクトの更新または作成」を参照してください。
* プロジェクトの読み込みによって作成されたイニシアチブを削除しても、プロジェクトは削除されません。
* イニシアチブにリンクされたプロジェクトを削除しても、イニシアチブは削除されません。

## プランに読み込まれたプロジェクト情報 {#project-information-imported-into-the-plan}

プロジェクトをプランに読み込むと、一部のプロジェクト情報もプランに読み込まれ、イニシアチブ情報になります。次の表に、プロジェクトをプランに読み込んだ際に、どのプロジェクト情報がイニシアチブ情報になるかを示します。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>プロジェクト情報</td> 
   <td>イニシアチブ情報 </td> 
  </tr> 
  <tr> 
   <td>プロジェクト名</td> 
   <td>イニシアチブ名</td> 
  </tr> 
  <tr> 
   <td>プロジェクト予定日</td> 
   <td> <p>イニシアチブの開始月と終了月。</p> <p>プロジェクトが月の中間に開始または終了する場合、読み込まれた日付は、プランの 1 か月分をカバーするように延長されます。例えば、プロジェクト予定日が 2020年3月20日～5月5日（PT）の場合、読み込まれたイニシアチブの日付は 2020年3月～5月になります。</p> <p>予定開始日または予定完了日がプランの期間を超える場合、読み込まれたイニシアチブがプランの前または後に開始したことを視覚的に示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>タスクとイシューに割り当てられた担当業務</td> 
   <td> <p>イニシアティブの担当業務。 </p> <p>メモ：   <p>プロジェクトの期間中にユーザーが役割を変更した場合、読み込まれる役割は、プロジェクト読み込み時の割り当てのステータスによって異なります。次のシナリオが存在します。</p> 
     <ul> 
      <li> <p>タスクまたはイシューに割り当てられたユーザーが、割り当てを[!UICONTROL Done]とマークした後に役割を変更された場合、[!DNL Workfront] は、そのユーザーが割り当てを[!UICONTROL Done]としてマークする前に実行していた役割をイニシアチブに読み込みます。</p> </li> 
      <li> <p>タスクまたはイシューに割り当てられたユーザーがプロジェクトの期間中に役割を変更したが、タスクまたはイシューに対する割り当てがプロジェクトのインポート時に[!UICONTROL Done]とマークされていない場合、[!DNL Workfront] は、割り当てられたユーザーの現在の役割のみを読み込みます。 </p> </li> 
     </ul> <p>割り当てのステータスについて詳しくは、<a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe [!DNL Workfront] 用語集</a>の「割り当てステータス」を参照してください。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシューに割り当てられた担当業務に関連するプロジェクト[!UICONTROL Planned Hours]</td> 
   <td> <p><span>プランが FTE と時間のどちらを使用するように設定されているかに応じて、プロジェクトのタスクの[!UICONTROL Planned Hours]は、プランの</span> [!UICONTROL Required FTEs]<span> または[!UICONTROL Required hours]</span>になります。 </p> <p>FTE または時間を使用するプランの設定に関する情報については、「<a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">[!DNL Scenario Planner]</a> でのプランの作成および編集」を参照してください。 </p> <p>次の点に注意してください。</p> 
    <ul> 
     <li> <p>[!DNL Workfront] は、タスクとタスクに割り当てられたジョブの役割、またはタスクまたはタスクに割り当てられたユーザーが関連付けられたジョブの役割をプロジェクトで使用し、必要なジョブの役割として新しいイニシアチブに転送します。 </p> </li> 
     <li> <p>FTE を使用するようにプランを設定すると、プロジェクトのタスクおよびイシューに関するジョブの役割に関連する予定時間数がまず FTE に変換されます。次に、この FTE がイニシアチブの担当業務に割り当てられます。<span>予定時間数は [!DNL Workfront] で均等に分配されます。タスクまたはイシューが複数の月にわたる場合、イニシアチブ期間中の各月の予定時間数が月次 FEF に換算され、イニシアチブの各月に転送されます。</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><span>たとえば、タスクが 9 月に 80 時間の予定時間数で担当業務に割り当てられている場合、インポートされた担当業務には、9 月のイニシアチブに対して 0.5 FTE と表示されます。</span> </p> </li> 
     <li> <p>[!DNL Workfront] は次の式を使用して、イニシアチブに関連付けられている必須担当業務の FTE を計算します。</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>説明：[!DNL Scenario Planner] は、1 か月に 160 時間の労働時間があると仮定しています。</p> <p>例えば、プロジェクトの期間が 1200 分で、プロジェクトの担当業務が予定時間数の 600 分に関連付けられている場合、その FTE は 0.5 になります。プロジェクトをインポートする場合、新しく作成されたイニシアチブの必須担当業務 FTE は、イニシアチブの各月で 0.5 になります。 </p> </li> 
     <li>プロジェクトのタスクに予定時間数がゼロで担当業務が割り当てられた場合、イニシアチブの担当業務に対する必須 FTE はデフォルトではゼロになります。 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>[!UICONTROL Duration]が 0 のプロジェクトのタスクに担当業務が割り当てられた場合、タスクに予定時間数が設定されている場合でも、イニシアチブの担当業務の必須 FTE <span>または時間</span>はデフォルトで 0 になります。 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## プロジェクトをプランにインポート

>[!IMPORTANT]
>
>プランにインポートしたプロジェクトは、プランのイニシアティブになります。2 つの項目はリンクされていますが、独立したエンティティとして存在し、更新されても自動的に影響し合うことはありません。
>
>次のように動作します。
>
>* プロジェクトをプランにインポートした後は、プロジェクトの変更はイニシアチブに影響を与えません。これらの変更には、担当業務の割り当てに対する変更が含まれます。
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* イニシアチブへの変更は、イニシアチブを対応するプロジェクトに公開する場合にのみ、プロジェクトの [!DNL Scenario Planner] 領域の情報に影響します。それ以外の場合、プロジェクトのタスクおよびイシューの[!UICONTROL 予定時間数]には影響しません。
>
>  イニシアティブの公開がリンクされたプロジェクトにどのような影響を与えるかについては、「[シナリオプランナーでイニシアチブを公開して、プロジェクトをアップデートまたは作成](../scenario-planner/publish-scenarios-update-projects.md)」を参照してください。
>

1. [!DNL Workfront] の右上隅で&#x200B;**[!UICONTROL メインメニュー]**![](assets/main-menu-icon.png)をクリックし、[!DNL Scenarios] をクリックして [!DNL Scenario Planner] にアクセスします。

1. プロジェクトを読み込むプランの名前をクリックします。
1. 「**[!UICONTROL 新規イニシアチブ]**」をクリックしてから、「**[!UICONTROL プロジェクトをインポート]**」をクリックします。

   「[!UICONTROL プロジェクトをインポート]」ボックスが表示されます。プランの時間枠に日付が含まれるプロジェクトがリストに表示されます。

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >すべてのステータスのプロジェクトがリストに表示されます。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. （オプション）**[!UICONTROL フィルターアイコン]** ![](assets/filter-nwepng.png) をクリックし、リストから使用可能なフィルターを選択して、リストのプロジェクト数を減らします。デフォルトでは、プロジェクトのリストは、プロジェクトのリストでユーザーが現在選択しているプロジェクトフィルターでフィルタリングされます。

1. （オプション）**[!UICONTROL 検索アイコン]** ![](assets/search-icon.png) をクリックして、画面上の任意のフィールドに表示されるキーワードを追加します。 検索語を含む項目がリストに自動的に表示され、すべての項目が非表示になります。

1. （条件付き）**[!UICONTROL X アイコン]**&#x200B;をクリックして検索を削除して、すべてのプロジェクトを表示します。
1. プロジェクトを 100 個まで選択し、「**[!UICONTROL インポート]**」をクリックします。

   プロジェクトは、新しいイニシアチブとしてインポートされます。

   次の点に注意してください。

   * プロジェクトアイコン ![](assets/project-icon-sp.png) がイニシアチブ名の右側に表示されます。
   * プロジェクトのタイムラインがプランの期間を超える場合、イニシアチブのバーは、左側（プロジェクト開始日がプランの日付より前の場合）または右側（プロジェクト終了日がプランの日付より後の場合）が尖った形状になります。

     ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * 月数と担当業務が、プロジェクトの役割に合わせて更新されます。

   >[!TIP]
   >
   >担当業務に関連付けられたコストは、イニシアチブレベルで更新され、プロジェクトからはインポートされません。

1. 新しいイニシアチブを表すバーをクリックして、右側のイニシアチブの詳細パネルを開きます。

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   **[!UICONTROL イニシアチブ期間]**&#x200B;領域で、次の情報を確認します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Duration]</td> 
      <td>これは、イニシアチブの期間（月単位）です。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>イニシアチブの開始日と終了日。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Project]</td> 
      <td> <p>リンクされたプロジェクトの[!UICONTROL Planned Start]および[!UICONTROL Completion dates]。</p> <p>ヒント： [!UICONTROL Project]情報が見つからない場合、プロジェクトは削除されています。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. イニシアチブの名前を編集します。 デフォルトでは、プロジェクトの名前と一致します。
1. （オプション）次のいずれかを実行します。

   * 「**[!UICONTROL 必須担当業務]**」セクションで担当業務を更新
   * 「**[!UICONTROL コスト]**」セクションで&#x200B;**[!UICONTROL 固定コスト]**&#x200B;を更新

   * 「**[!UICONTROL 利用可能な担当業務を更新する]**」または「**[!UICONTROL 利用可能な予算を更新する]**」をクリックして、新規イニシアティブとプラン上の他のイニシアティブとの矛盾を解決します。

1. （条件付き）「**[!UICONTROL 適用]**」をクリックして、イニシアチブに対する変更を保存します。
1. 「**[!UICONTROL 計画の保存]**」をクリックして、プランの変更内容を保存します。
1. （オプション）イニシアチブに加えた変更を、読み込み元のプロジェクトで更新するには、プランからプロジェクトを公開します。プランの公開について詳しくは、「[ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でのプロジェクトの更新または作成」を参照してください。
1. （オプション）プロジェクトアイコンをクリックして、リンクされたプロジェクトにアクセスします。

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
