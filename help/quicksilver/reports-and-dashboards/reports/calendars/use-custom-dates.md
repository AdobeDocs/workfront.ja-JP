---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: カレンダーレポートでのカスタム日付フィールドの使用
description: カレンダーレポートは、作業内容を視覚的に表現する動的なレポートです。タスク、イシューおよびプロジェクトに関するカレンダーレポートでカスタム日付フィールドを使用できます。
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: c88c8dc7431f3bc711ae1942df12925fafa7eff0
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 86%

---

# カレンダーレポートでのカスタム日付フィールドの使用

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。プレビューサンドボックス環境でのみ使用できます。</span>

[!UICONTROL カレンダー]レポートは、作業内容を視覚的に表示する動的なレポートです。次のオブジェクトに対して、カレンダーレポートでカスタム日付フィールドを使用できます。

* タスク
* イシュー
* プロジェクト

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!UICONTROL Reports]、[!UICONTROL Dashboards]、および[!UICONTROL Calendars]に対する[!UICONTROL Edit]アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>カレンダーレポートに対する [!UICONTROL Manage] 権限</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

1. [!DNL Workfront] インスタンスで使用可能なフィールド内に、カスタム日付フィールドと値が設定されている必要があります。カスタムの日付を使用してカスタムフォームを設定していない場合は、[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) の手順に従ってください。
1. カレンダーに追加する予定のプロジェクト、タスク、またはイシューにカスタムフォームを添付し、日付を指定します。詳しくは、[オブジェクトにカスタムフォームを追加](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。

## 生産の品目グループを設定します

カレンダーに表示する項目のグループの表示方法を選択できます。

{{step1-to-calendars}}

1. 新しいアイテム グループを追加するカレンダーを選択します。
または
「**[!UICONTROL +新規カレンダ」をクリックし]** カレンダ名を入力します。

   >[!NOTE]
   >
   >カレンダーレポートを作成するには、アクセスレベルで[!UICONTROL レポート]、[!UICONTROL ダッシュボード]、[!UICONTROL カレンダー]への[!UICONTROL 編集]アクセス権が必要です。

1. 左側で「**[!UICONTROL カレンダーに追加]**」、「**[!UICONTROL 詳細項目を追加]**」の順にクリックします。

1. 以下を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>項目のグループの名前を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>項目のグループの色を選択します。カレンダーレポートには、すべての項目が選択した色で表示されます。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><strong>[!UICONTROL Custom dates]</strong> を選択します。<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>日付の表示方法を選択します。</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>：カレンダーには単一の日付のオブジェクトが表示されます。</li>
        <li><strong>[!UICONTROL Duration]（開始～終了）</strong>：カレンダーには、数日間にわたるオブジェクトが表示されます。<br><p>メモ：<strong>[!UICONTROL Duration]</strong> を選択する場合、終了日は開始日より後に指定する必要があります。開始日より前に指定すると、項目がカレンダーに表示されません。</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Custom Dates]</strong></td>
      <td><p>追跡するオブジェクトに添付するカスタム日付名を入力します。</p><p><strong>メモ：</strong>パフォーマンスの問題を避けるため、カスタム日付名の検索は 50 件の結果に制限されています。</td>
     </tr>
    </tbody>
   </table>

1. 次のセクションに進みます。

## 実稼動環境の項目グループにオブジェクトを追加

項目の表示方法を設定した後、カレンダーに表示するオブジェクトをグループに追加する必要があります。

1. 「**[!UICONTROL カレンダーに何を追加しますか？]**」セクションで、次を選択します。

   * **[!UICONTROL タスク]**
   * **[!UICONTROL プロジェクト]**
   * **[!UICONTROL イシュー]**

1. カレンダーに追加するオブジェクトタイプに応じて、「**[!UICONTROL タスクを追加]**」、「**[!UICONTROL プロジェクトを追加]**」または「**[!UICONTROL イシューを追加]**」をクリックします。
   ![カレンダーのオブジェクトを選択](assets/field-name.png)

1. ドロップダウンメニューで、フィールド名を入力し、カレンダーに表示するオブジェクトのフィールドソース（**[!UICONTROL 遅延タスク]**&#x200B;など）を選択します。
1. カレンダーのグループ化の条件文を設定します。

   ![条件文](assets/condition-statement-calendar.png)

   条件の設定について詳しくは、[フィルターおよび条件修飾子](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)を参照してください。

1. （オプション）手順 1 ～ 4 を繰り返して、カレンダーのグループ化に使用する追加のオブジェクトを指定します。
1. **[!UICONTROL タスク／プロジェクト／イシューのラベルを次の値に設定…]**&#x200B;フィールドで、このカレンダーグループ内のオブジェクトにカレンダー内でどのようにラベルを付けるかを選択します。

   >[!NOTE]
   >
   >特定のオブジェクトに対してデフォルトのラベルオプションがない場合は、代わりにオブジェクト名が表示されます。例えば、[!UICONTROL 親タスク]ラベルが選択されているのに、オブジェクトに関連付けられている親タスクがない場合、[!DNL Adobe Workfront] にはカレンダーに表示されているオブジェクト名が表示されます。

1. 「**[!UICONTROL 保存]**」をクリックします。

<div class="preview">

## プレビューで項目のグループを設定

カレンダーに表示する項目のグループの表示方法を選択できます。

{{step1-to-calendars}}

1. 新しいアイテム グループを追加するカレンダーを選択し、[ 詳細 ] メニューの [**編集**] をクリックします。
または
「**[!UICONTROL +新しいカレンダー]**」をクリックし、プロジェクト名を入力して、「**[!UICONTROL 詳細項目を追加]**」をクリックします。

   >[!NOTE]
   >
   >カレンダーレポートを作成するには、アクセスレベルで[!UICONTROL レポート]、[!UICONTROL ダッシュボード]、[!UICONTROL カレンダー]への[!UICONTROL 編集]アクセス権が必要です。

1. 以下を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>項目のグループの名前を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>項目のグループの色を選択します。カレンダーレポートには、すべての項目が選択した色で表示されます。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><strong>[!UICONTROL Custom dates]</strong> を選択します。<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>日付の表示方法を選択します。</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>：カレンダーには単一の日付のオブジェクトが表示されます。</li>
        <li><strong>[!UICONTROL Duration]（開始～終了）</strong>：カレンダーには、数日間にわたるオブジェクトが表示されます。<br><p>メモ：<strong>[!UICONTROL Duration]</strong> を選択する場合、終了日は開始日より後に指定する必要があります。開始日より前に指定すると、項目がカレンダーに表示されません。</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Custom Dates]</strong></td>
      <td><p>追跡するオブジェクトに添付するカスタム日付名を入力します。</p><p><strong>メモ：</strong>パフォーマンスの問題を避けるため、カスタム日付名の検索は 50 件の結果に制限されています。</td>
     </tr>
    </tbody>
   </table>

1. 次のセクションに進みます。

### プレビューでアイテムのグループにオブジェクトを追加

項目の表示方法を設定した後、カレンダーに表示するオブジェクトをグループに追加する必要があります。

1. 「**[!UICONTROL カレンダーに何を追加しますか？]**」セクションで、次を選択します。

   * **[!UICONTROL タスク]**
   * **[!UICONTROL プロジェクト]**
   * **[!UICONTROL イシュー]**
   * **休暇**

1. カレンダーに追加するオブジェクトタイプに応じて、「**[!UICONTROL タスクを追加]**」、「**[!UICONTROL プロジェクトを追加]**」、「**[!UICONTROL イシューを追加]**」または「**休暇**」をクリックします。

1. ドロップダウンメニューで、フィールド名を入力し、カレンダーに表示するオブジェクトのフィールドソース（**[!UICONTROL 遅延タスク]**&#x200B;など）を選択します。
1. カレンダーのグループ化の条件文を設定します。


   条件の設定について詳しくは、[フィルターおよび条件修飾子](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)を参照してください。

   ![カレンダーのオブジェクトを選択](assets/calendar-field-name.png)

1. （オプション）手順 1 ～ 4 を繰り返して、カレンダーのグループ化に使用する追加のオブジェクトを指定します。
1. **[!UICONTROL タスク／プロジェクト／イシューのラベルを次の値に設定…]**&#x200B;フィールドで、このカレンダーグループ内のオブジェクトにカレンダー内でどのようにラベルを付けるかを選択します。

   >[!NOTE]
   >
   >特定のオブジェクトに対してデフォルトのラベルオプションがない場合は、代わりにオブジェクト名が表示されます。例えば、[!UICONTROL 親タスク]ラベルが選択されているのに、オブジェクトに関連付けられている親タスクがない場合、[!DNL Adobe Workfront] にはカレンダーに表示されているオブジェクト名が表示されます。

   ![ タスク ラベルの設定 ](assets/set-task-labels.png)
1. **[!UICONTROL 保存]**&#x200B;をクリックします。

</div>