---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 時間タイプを管理
description: 時間タイプを時間エントリに関連付けることができます。時間タイプは、時間エントリの定義に使用するラベルです。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: ed179058cfec1332384ef76cb04598278109291b
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 93%

---

# 時間タイプを管理

<!--Audited: 07/2024-->

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

  [ 時間タイプと空き時間の定義 ](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md) で説明されているように、[!DNL Workfront] 管理者は、プロジェクト固有の時間タイプを使用可能にすることを決定します。

  >[!NOTE]
  >
  >[!DNL Workfront] システムでプロジェクト固有の時間タイプを有効にする場合は、システム内の各プロジェクトで、1 つ以上のプロジェクト固有の時間タイプを有効にする必要があります。システムレベルでは、プロジェクト固有の時間タイプを有効にすることはできません。また、プロジェクトレベルでは、プロジェクト固有の時間タイプを使用できません。

* **一般的な時間タイプ**：一般的な時間数はプロジェクト、タスク、やイシューに関連付けることができず、タイムシートに直接記録されます。時間の記録について詳しくは、[時間を記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>新規：[!UICONTROL Standard]</p>
   <p>現在：[!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td> <p>[!DNL Workfront] 管理者であることが必要です。</p> <p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 組み込みの時間タイプ

Workfront には、一連の組み込みの時間タイプが付属しています。これらの時間タイプは編集できず、非表示にすることができません。

[!DNL Workfront] に付属する時間タイプは以下のとおりです。

* **[!UICONTROL 病欠時間]**：プロジェクト、タスクやイシューの時間エントリに関連付けることができない一般的な時間タイプです。病欠時間は収益としてカウントできません。
* **[!UICONTROL 休暇時間]**：プロジェクト、タスクやイシューの時間エントリに関連付けることができない一般的な時間タイプです。休暇時間は収益としてカウントできません。
* **[!UICONTROL 一般オーバーヘッド]**：プロジェクト、タスクやイシューの時間エントリに関連付けることができない一般的な時間タイプです。ただし、プロジェクト計画プロセスでは収益としてカウントできます。
* **[!UICONTROL プロジェクト時間]**：プロジェクトの時間エントリにのみ関連付けることができる一般的な時間タイプです。
* **[!UICONTROL タスク時間]**：タスクの時間エントリにのみ関連付けることができる一般的な時間タイプです。
* **[!UICONTROL イシュー時間]**：イシューの時間エントリにのみ関連付けることができる一般的な時間タイプです。

## 時間タイプを作成

[!DNL Workfront] 管理者は、システムレベルとプロジェクトレベルの両方で、組織の新しい時間タイプを作成できます。システムレベルとプロジェクトレベルで時間タイプを作成した後、ユーザーは、特定のプロジェクトやユーザーがどの時間タイプを使用できるかを定義できます。詳しくは、[ 時間タイプと可用性の定義 ](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md) を参照してください

新しい時間タイプを作成するには、以下のように行います。

{{step-1-to-setup}}

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
      <td><p>この時間タイプに関連付けられた時間エントリを収益の計算に反映させたい場合は、このオプションを選択します。</p>
      <p>病欠時間と休暇時間は、収益としてカウントできません。</p>
      <p><b>メモ</b></p>
      <p>一般的な時間タイプが収益としてカウントされる場合、時間を記録しているユーザーのプロファイルに関連付けられたコスト率は、時間コストに関連付けられます。  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL 収益とみなす]**：この時間タイプに関連付けられる時間エントリを収益の計算に反映させる場合は、このオプションを選択します。

1. 「**[!UICONTROL 時間タイプを作成]」をクリックします。**

## 時間タイプの非アクティブ化

時間タイプが廃止され、ユーザーが時間エントリを関連付ける必要がなくなった場合は、時間タイプを非アクティブ化できます。

時間タイプを非アクティブ化すると、[!DNL Workfront] の時間タイプが表示される場所で、時間タイプが非表示になります。

時間タイプを非アクティブ化するには、次の手順に従います。

{{step-1-to-setup}}

1. **[!UICONTROL タイムシートおよび時間設定]**&#x200B;を展開し、「**[!UICONTROL 時間タイプ]**」をクリックします。

1. 非アクティブ化する時間タイプを選択します。

1. 「**[!UICONTROL 非アクティブ化]**」をクリックします。
