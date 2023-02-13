---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: カレンダーレポートでの推定日の使用
description: カレンダーレポートは、作業内容を視覚的に表現する動的なレポートです。 タスク、タスクおよびプロジェクトに関するカレンダーレポートで、[ 予定日 ] フィールドを使用できます。
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 1%

---

# 用途 [!UICONTROL 推定日] カレンダーレポート内

カレンダーレポートは、作業内容を視覚的に表現する動的なレポートです。 次のオブジェクトに対して、カレンダ・レポートで「予定日」フィールドを使用できます。

* タスク
* 問題
* プロジェクト

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL プラン ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL ][!UICONTROL レポート ]、[!UICONTROL ダッシュボード ] および [!UICONTROL カレンダー ] へのアクセス権の編集</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>カレンダーレポートへの [!UICONTROL 管理 ] アクセス</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 項目のグループを設定

カレンダーに表示する項目のグループの表示方法を選択できます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **[!UICONTROL カレンダー]**.

1. 新しい項目のグループを追加するカレンダーを選択します。\
   または\
   クリック **[!UICONTROL +新しいカレンダー]** カレンダー名を入力します。

   >[!NOTE]
   >
   >必ず [!UICONTROL 編集] ～へのアクセス [!UICONTROL レポート], [!UICONTROL ダッシュボード]、および [!UICONTROL カレンダー] をクリックし、カレンダーレポートを作成します。

1. 左側で、 **[!UICONTROL カレンダーに追加]**&#x200B;を選択し、「 **[!UICONTROL 詳細項目の追加]**.

1. 以下を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL この項目グループに名前を付ける ]</strong></td>
      <td>項目のグループの名前を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL カラー ]</strong></td>
      <td>項目のグループの色を選択します。 すべての項目が、選択した色でカレンダーレポートに表示されます。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 日付フィールド ]</strong></td>
      <td><p>選択 <strong>[!UICONTROL 推定日 ]</strong>. 予定日について詳しくは、 </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">プロジェクトの概要予定開始日</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">プロジェクト、タスクおよび問題に関する予定完了日の概要</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL カレンダーで表示 ]</strong></td>
      <td><p>日付の表示方法を選択します。</p>
       <ul>
        <li><strong>[!UICONTROL 開始日のみ ]</strong>:カレンダーには、1 つの日付にオブジェクトが表示されます。</li>
        <li><strong>[!UICONTROL 終了日のみ ]</strong>:カレンダーには、1 つの日付にオブジェクトが表示されます。</li>
        <li><strong>[!UICONTROL 期間 ] （開始から終了）</strong>:カレンダーには、一定期間のオブジェクトが表示されます。</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL 実際の日付に切り替え（可能な場合）]</strong></td>
      <td><p>カレンダーは、利用可能な場合は自動的に実際の日付に切り替わります。 <br>選択 <strong>[!UICONTROL はい ]</strong> または <strong>[!UICONTROL いいえ ]</strong> をクリックして、実際の日付に切り替えます。 実際の日付について詳しくは、</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">プロジェクトの概要実績開始日 </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">プロジェクトの概要実績完了日 </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. 次の節に進みます。

## オブジェクトを項目のグループに追加

アイテムの表示方法を設定した後、カレンダーに表示するオブジェクトをグループ化に追加する必要があります。

1. 内 **[!UICONTROL カレンダーに追加する項目を選択してください。]** セクション、選択

   * **[!UICONTROL タスク]**
   * **[!UICONTROL プロジェクト]**
   * **[!UICONTROL 問題]**

1. クリック **[!UICONTROL タスクを追加]**, **[!UICONTROL プロジェクトを追加]**&#x200B;または **[!UICONTROL 問題の追加]**（カレンダーに追加するオブジェクトタイプに応じて）\
   ![カレンダーのオブジェクトを選択](assets/field-name.png)

1. ドロップダウンメニューで、フィールド名を入力し、カレンダーに表示するオブジェクトのフィールドソースを選択します ( 例： **[!UICONTROL 遅延タスク]**) をクリックします。
1. カレンダーのグループ化の条件文を設定します。

   ![条件文](assets/condition-statement-calendar.png)

   条件の設定について詳しくは、 [フィルターおよび条件修飾子](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. （オプション）手順 1 ～ 4 を繰り返して、カレンダーのグループ化用の追加オブジェクトを指定します。
1. 内 **[!UICONTROL タスク/プロジェクト/問題のラベルを次の値に設定…]** [ ] フィールドで、このカレンダーグループ内のオブジェクトにカレンダー内でどのようにラベルを付けるかを選択します。

   >[!NOTE]
   >
   >特定のオブジェクトに対してデフォルトのラベルオプションが使用できない場合は、代わりにオブジェクト名が表示されます。 例えば、親タスクラベルが選択され、親タスクがオブジェクトに関連付けられていない場合、 [!DNL Adobe Workfront] カレンダーに表示されているオブジェクト名が表示されます。

1. 「**[!UICONTROL 保存]**」をクリックします。
