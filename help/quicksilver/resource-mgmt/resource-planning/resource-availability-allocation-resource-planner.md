---
product-area: resource-management
navigation-topic: resource-planning
title: Adobe Workfront リソースプランナーを使用してリソースの可用性と割り当てをレビューする
description: リソースプランナーでは、リソースの空き時間と、プロジェクトの予定作業や予算計上作業の量を表示できます。これらの値は、時間、FTE（フルタイム換算）やコストの金額で表示され、列に編成されます。
author: Alina
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: ht
source-wordcount: '1270'
ht-degree: 100%

---

# Adobe Workfront リソースプランナーを使用してリソースの可用性と割り当てをレビューする

リソースプランナーでは、リソースの空き時間と、プロジェクトの予定作業や予算計上作業の量を表示できます。これらの値は、時間、FTE（フルタイム換算）やコストの金額で表示され、列に編成されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>レビュー以上 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の項目に対する表示以上のアクセス権：</p> 
    <ul> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>財務データ</p> </li> 
     <li> <p>ユーザー</p> </li> 
     <li> <p>プロジェクト</p> </li> 
    </ul> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リソースプランナーで表示するプロジェクトに対する表示権限以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

<!--note from the table about the license: Review or higher: 
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (waiting on Vazgen to confirm - working differenly in classic)
      </MadCap:conditionalText>
     -->

## 前提条件

リソースプランナーを使用するには、求められるすべての前提条件を満たす必要があります。詳しくは、[リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

>[!IMPORTANT]
>
>リソースプランナーの正しい機能に必要な前提条件のいずれかが不足している場合、数値の一部がゼロになるか、予算計上時間数がグレー表示されることがあります。

## リソースの空き時間と割り当て

リソースの空き時間と割り当てを表示する列は、リソースプランナーに適用するビューに応じて変わります。プロジェクト別、役割別またはユーザー別のリソースプランナーでの情報の表示について詳しくは、[リソースプランナーのナビゲーションの概要](../../resource-mgmt/resource-planning/resource-planner-navigation.md)を参照してください。

表示をリソースプランナーに変更する際は、以下の点を考慮してください。

* **プロジェクトごとに表示**&#x200B;ビュー、または&#x200B;**役割ごとに表示**&#x200B;ビューを適用すると、以下の列が表示されます。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * 利用可能時間数、FTE またはコスト
   * 予定時間数、FTE またはコスト
   * 予算計上時間数、FTE またはコスト
   * 時間数、FTE またはコスト差異
   * 正味時間数、FTE またはコスト

* **ユーザー別に表示**&#x200B;ビューを適用する場合、以下の列が表示されます。

   * 利用可能時間数または FTE
   * 計画時間数または FTE
   * 時間または FTE の差異
   * 予定時間配分率

>[!TIP]
>
>**ユーザーごとに表示**&#x200B;ビューをリソースプランナーに適用する場合、この情報はコストとして利用できません。
>
>それぞれの列の表示内容について詳しくは、数値が表示される列の名前の上にマウスを移動すると表示されます。\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>それぞれの列に表示されるデータについて詳しくは、以下の記事を参照してください。
>
>* [リソースプランナーでのプロジェクトビューと役割ビューでの時間数、FTE、コスト情報の概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [ユーザービューを使用する場合は、リソースプランナーで使用可能、予定、実際の時間数、または FTE を表示する](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>

## 時間別、FTE またはコスト別の情報の表示

1. リソースプランナーに移動します。

   デフォルトでは、情報はリソースプランナーに時間別に表示されます。

1. ドロップダウンメニューを展開します。\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. 次のオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">時間</td> 
      <td>稼働状況および割り当て情報を時間単位で表示します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>稼働状況および割り当て情報を FTE で表示します。</p> <p>リソースプランナーでの FTE の計算方法について詳しくは、<a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソースプランナーのユーザーと役割に対する時間と FTE の計算の概要</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">コスト</td> 
      <td> <p>プロジェクトビューまたは役割ビューでリソースプランナーを表示している場合、コスト別に稼働状況および割り当て情報を表示します。この情報は、システムの通貨で値を表示します。システム通貨は Workfront 管理者が定義します。Workfront でのシステム通貨の設定について詳しくは、<a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">為替レートの設定</a>を参照してください。</p> <p><b>メモ</b>

   リソースプランナーでコスト情報を表示するには、ユーザーと担当業務を 1 時間あたりのコスト率に関連付ける必要があります。<br style="font-style: italic;">時間単価の担当業務との関連付けについて詳しくは、<a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成と管理</a>を参照してください。<br style="font-style: italic;">時間単価をユーザーに関連付ける方法について詳しくは、<a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。<br style="font-style: italic;">リソースプランナーでのコストの計算方法について詳しくは、<a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">リソースプランナーでのコストの計算</a>を参照してください。</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">のカスタマイズ</td> 
      <td>リソースプランナーに表示される列のカスタムビューを作成します。次の手順に従って、リソースプランナーに表示するオプションを選択します。 </td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付き）**カスタマイズ**&#x200B;を選択した場合、**表示される指標のカスタマイズ**&#x200B;ボックスを使用してカスタムビューを設定します。

   ![](assets/planner-customize-view-box-350x114.png)

1. 左側の&#x200B;**表示タイプ**&#x200B;列で、次のビューの 1 つを選択します。

   * プロジェクト
   * 役割
   * ユーザー

1. 「**選択した項目を表示**」セクションで、選択したビューの列に表示する情報のタイプを選択します。次の表に、各ビューで使用可能なオプションを示します。

   | **オプション** | ユーザー ビュー | プロジェクト ビュー | 役割ビュー |
   |---|---|---|---|
   | 利用可能 | ✔ | ✔ | ✔ |
   | 予定 | ✔ | ✔ | ✔ |
   | 予算計上 |   | ✔ | ✔ |
   | 差異 |   | ✔ | ✔ |
   | 純価 |   | ✔ | ✔ |
   | 実際 | ✔ |   |   |
   | 差異 | ✔ |   |   |
   | パーセント | ✔ |   |   |

1. 「プロジェクト」ビューと「役割」ビューで純価を計算する際は、「予算計上」ではなく「予定」の情報を使用するために、「**純残存の計算に予定の値を使用**」を選択します。

   このオプションを選択すると、次の式を使って純価が計算されます。

   ```
   Net = Available - Planned
   ```

   >[!TIP]
   >
   >**このオプションは、「選択した項目を表示」セクションで表示をカスタマイズするための 1 つ以上のオプションを選択した場合にのみ適用されます。**

1. 「**保存**」をクリックします。

   選択した列を含むカスタマイズされたビューが表示されます。

   リソースプランナーの「時間」ドロップダウンメニューには、カスタマイズされたビューが「カスタム」としてリストされます。

   >[!NOTE]
   >
   >カスタマイズされたビューは 1 つだけ指定できます。

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## ユーザー割り当てグラフの表示

ユーザーの利用可能時間に対する予定配分をグラフに表示できます。

ユーザーの配分をグラフに表示するには：

1. リソースプランナーに移動します。

   リソースプランナーへのアクセスについて詳しくは、[リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md)にある[リソースプランナーの場所](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner)を参照してください。

1. 「**ユーザー別に表示**」を選択します。

   >[!TIP]
   >
   >ユーザー割り当てグラフは、「ユーザービュー」でのみ表示できます。

1. 次の情報を表示するには、**ユーザー割り当てグラフ**&#x200B;アイコン ![RP_user_allocation_chart.png](assets/rp-user-allocation-chart.png) をクリックします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべてのユーザーに対する配分超過なしの利用可能時間率</td> 
      <td>これは、すべてのユーザーが期間内に作業可能な時間であり、利用可能時間の合計に対する割合で表示されます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべてのユーザーに対する配分超過率 </td> 
      <td> <p>これは、期間内にユーザーが割り当て超過となっている時間であり、利用可能時間の合計に対する割合で表示されます。</p> <p><b>メモ</b>

   予定時間数が利用可能時間数よりも多い場合は、割り当て超過が発生します。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">すべてのユーザーに対する低稼働率</td> 
      <td> <p>これは、期間内にユーザーが割り当て不足となる時間であり、利用可能時間の合計に対する割合で表示されます。</p> <p><b>メモ</b>

   低稼働率は、予定時間数が利用可能時間よりも短い場合に発生します。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">この期間中に少なくとも 1 人のユーザーで配分が超過しています</td> 
      <td>これは、すべてのユーザーの合計時間は期間内で割り当て超過でないものの、少なくとも 1 人のユーザーに対して割り当て超過があることを示しています。<br>赤色でハイライト表示される割り当て超過のユーザーの時間を確認するには、ユーザーのリストをスクロールします。</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_allocation_chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. （オプション）グラフ内の「**すべてのユーザーに対する配分超過率**」エリアをクリックします。\
   割り当てが超過しているすべてのユーザーは赤でハイライト表示されます。
1. （オプション）グラフ内の「**すべてのユーザーに対する低稼働率**」エリアをクリックします。\
   十分に活用されていないすべてのユーザーは青色で強調表示されます。

1. （オプション）少なくとも 1 人のユーザーが割り当て超過になっている場所を示すインジケーターアイコン ![one_user_overallocation_marker.png](assets/one-user-overallocation-marker.png) をクリックします。\
   割り当て超過のユーザーは赤で強調表示されます。

1. （オプション）ページを更新して、グラフを折りたたみます。
