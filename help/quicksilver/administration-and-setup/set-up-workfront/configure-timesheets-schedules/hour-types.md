---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 時間タイプを管理
description: 時間タイプを時間エントリに関連付けることができます。時間タイプは、時間エントリの定義に使用するラベルです。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: ht
source-wordcount: '759'
ht-degree: 100%

---

# 時間タイプを管理

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

時間タイプを時間エントリに関連付けることができます。時間タイプは、時間エントリの定義に使用するラベルです。

以下の 2 つの時間タイプがあります。

* **プロジェクト固有の時間タイプ**：プロジェクト、タスクおよびイシューのログ時間です。プロジェクト固有の時間タイプは、プロジェクト、タスク、イシューの時間を記録できる、[!DNL Adobe Workfront] 内の任意の場所で時間エントリに関連付けることができます。

  [!DNL Workfront]で時間を記録する場合、使用できるプロジェクト固有の時間タイプは、システムレベル、プロジェクトレベルおよびユーザーレベルで設定された設定オプションによって異なります。

  以下のデフォルトのプロジェクト固有の時間タイプは、常に使用できます。

   * プロジェクト時間
   * タスク時間
   * イシュー時間

  [!DNL Workfront] 管理者は、[タイムシートの時間タイプと空き時間を定義](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)の説明に従って、どのプロジェクト固有の時間タイプが使用できるかを決定します。

  >[!NOTE]
  >
  >[!DNL Workfront] システムでプロジェクト固有の時間タイプを有効にする場合は、システム内の各プロジェクトで、1 つ以上のプロジェクト固有の時間タイプを有効にする必要があります。システムレベルでは、プロジェクト固有の時間タイプを有効にすることはできません。また、プロジェクトレベルでは、プロジェクト固有の時間タイプを使用できません。

* **一般的な時間タイプ**：一般的な時間数はプロジェクト、タスク、やイシューに関連付けることができず、タイムシートに直接記録されます。時間の記録について詳しくは、[時間を記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!DNL Workfront] 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか、[!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront]管理者がアクセスレベルを変更する方法については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 組み込みの時間タイプ

Workfront には、一連の組み込みの時間タイプが付属しています。これらの時間タイプは編集できず、非表示にすることができません。

[!DNL Workfront] に付属する時間タイプは以下のとおりです。

* **[!UICONTROL 病欠時間]**：プロジェクト、タスクやイシューの時間エントリに関連付けることができない一般的な時間タイプです。
* **[!UICONTROL 休暇時間]**：プロジェクト、タスクやイシューの時間エントリに関連付けることができない一般的な時間タイプです。
* **[!UICONTROL 一般オーバーヘッド]**：プロジェクト、タスクやイシューの時間エントリに関連付けることができない一般的な時間タイプです。ただし、プロジェクト計画プロセスでは収益としてカウントできます。
* **[!UICONTROL プロジェクト時間]**：プロジェクトの時間エントリにのみ関連付けることができる一般的な時間タイプです。
* **[!UICONTROL タスク時間]**：タスクの時間エントリにのみ関連付けることができる一般的な時間タイプです。
* **[!UICONTROL イシュー時間]**：イシューの時間エントリにのみ関連付けることができる一般的な時間タイプです。

## 時間タイプを作成

[!DNL Workfront] 管理者は、システムレベルとプロジェクトレベルの両方で、組織の新しい時間タイプを作成できます。システムレベルとプロジェクトレベルで時間タイプを作成した後、ユーザーは、特定のプロジェクトやユーザーがどの時間タイプを使用できるかを定義できます。詳しくは、[タイムシートの時間のタイプと空き時間を定義](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)を参照

新しい時間タイプを作成するには、以下のように行います。

1. [!DNL Adobe] Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) の順にクリックします。

1. **[!UICONTROL タイムシートと時間]**／**[!UICONTROL 時間タイプ]**&#x200B;をクリックします。

1. **[!UICONTROL 新しい時間タイプ]をクリックします。**
1. **[!UICONTROL 新しい時間タイプ]**&#x200B;フォームに、以下の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>新しい時間タイプに、システムで簡単に認識できる名前を付けます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>時間タイプの説明を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>ドロップダウンメニューで正しい範囲を選択して、時間タイプが一般的かプロジェクト固有の時間タイプかを定義します。</p> <p>一般的な時間タイプは、タイムシートにのみ表示され、プロジェクト、タスクやイシューに関連付けることができません。</p> <p><b>重要</b>：カスタムの時間タイプ（[!UICONTROL Project Specific]）がある場合、この時間タイプを [!UICONTROL General] に変更すると、既存のタスク、イシューおよびプロジェクトの時間がすべてシステムのデフォルトのタイプに設定されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count As Revenue]</td> 
      <td>この時間タイプに関連付けられた時間エントリを収益の計算に反映させたい場合は、このオプションを選択します。</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL 収益とみなす]**：この時間タイプに関連付けられる時間エントリを収益の計算に反映させる場合は、このオプションを選択します。

1. 「**[!UICONTROL 時間タイプを作成]」をクリックします。**

## 時間タイプの非アクティブ化

時間タイプが廃止され、ユーザーが時間エントリを関連付ける必要がなくなった場合は、時間タイプを非アクティブ化できます。

時間タイプを非アクティブ化すると、[!DNL Workfront] の時間タイプが表示される場所で、時間タイプが非表示になります。

時間タイプを非アクティブ化するには、次の手順に従います。

1. グローバルナビゲーションバーで [!DNL Adobe Workfront] の右上隅付近にある「**[!UICONTROL 設定]**」をクリックします。

1. **[!UICONTROL タイムシートおよび時間設定]**&#x200B;を展開し、「**[!UICONTROL 時間タイプ]**」をクリックします。

1. 非アクティブ化する時間タイプを選択します。

1. 「**[!UICONTROL 非アクティブ化]**」をクリックします。
