---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 時間タイプの管理
description: 時間タイプを時間エントリに関連付けることができます。 時間タイプは、時間エントリの定義に使用するラベルです。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# 時間タイプの管理

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

時間タイプを時間エントリに関連付けることができます。 時間タイプは、時間エントリの定義に使用するラベルです。

次の 2 つの時間タイプがあります。

* **プロジェクト固有の時間タイプ**:これは、プロジェクト、タスクおよび問題にログオンする時間です。 プロジェクト固有の時間タイプは、 [!DNL Adobe Workfront] ここで、プロジェクト、タスクおよび問題に関する時間を記録できます。

   ログイン時 [!DNL Workfront]を使用する場合、使用できるプロジェクト固有の時間タイプは、システムレベル、プロジェクトレベル、ユーザーレベルで設定された構成オプションによって異なります。

   次のデフォルトのプロジェクト固有の時間タイプは、常に使用できます。

   * プロジェクト時間
   * タスク時間
   * 問題時間

   この [!DNL Workfront] 管理者は、 [タイムシートの時間の種類と可用性を定義する](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   >[!NOTE]
   >
   >プロジェクト固有の時間タイプを [!DNL Workfront] システムでは、システム内の各プロジェクトで、少なくとも 1 つのプロジェクト固有の時間タイプを有効にする必要があります。 システムレベルでは、プロジェクト固有の時間タイプを有効にすることはできません。また、プロジェクトレベルでは、プロジェクト固有の時間タイプを使用できません。

* **一般的な時間タイプ**:一般時間は、プロジェクト、タスク、またはタスクに関連付けることはできず、タイムシートに直接記録されます。 ログ時間について詳しくは、 [ログ時間](../../../timesheets/create-and-manage-timesheets/log-time.md).

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
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 組み込みの時間タイプ

Workfrontには、組み込みの時間タイプが付属しています。 これらの時間タイプは編集できず、非表示にすることはできません。

に付属する時間タイプ [!DNL Workfront] 次の場合：

* **[!UICONTROL 病欠時間]**:プロジェクト、タスク、または問題の時間エントリに関連付けることができない一般的な時間タイプです。
* **[!UICONTROL 休暇時間]**:プロジェクト、タスク、または問題の時間エントリに関連付けることができない一般的な時間タイプです。
* **[!UICONTROL 一般的な間接費]**:プロジェクト、タスク、または問題の時間エントリに関連付けることができない一般的な時間タイプです。 ただし、プロジェクト計画プロセスでは収益としてカウントできます。
* **[!UICONTROL プロジェクト時間]**:プロジェクトの時間エントリにのみ関連付けることができる一般的な時間タイプです。
* **[!UICONTROL タスク時間]**:タスクの時間エントリにのみ関連付けることができる一般的な時間タイプです。
* **[!UICONTROL 発行時間]**：問題の時間エントリにのみ関連付けることができる一般的な時間タイプ。

## 時間タイプの作成

As a [!DNL Workfront] 管理者は、システムレベルとプロジェクトレベルの両方で、組織の新しい時間タイプを作成できます。 システムレベルとプロジェクトレベルで時間タイプを作成した後、ユーザーは、特定のプロジェクトとユーザーに対して使用可能な時間タイプを定義できます。 詳しくは、 [タイムシートの時間の種類と可用性を定義する](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

新しい時間タイプを作成するには：

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe] Workfront、 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL タイムシートと時間]** > **[!UICONTROL 時間タイプ]**.

1. クリック **[!UICONTROL 新しい時間タイプ].**
1. 次の情報を **[!UICONTROL 新しい時間タイプ]** フォーム：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名前 ]</td> 
      <td>新しい時間に、システムで簡単に認識できる名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 説明 ]</td> 
      <td>時間タイプの説明を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL スコープ ]</td> 
      <td> <p>ドロップダウンメニューで正しい範囲を選択して、時間タイプが一般的かプロジェクト固有の時間タイプかを定義します。</p> <p>一般時間タイプは、タイムシートにのみ表示され、プロジェクト、タスク、またはタスクに関連付けることはできません。</p> <p><b>重要</b>:カスタムの時間タイプ（[!UICONTROL プロジェクト固有 ]）がある場合は、それを [!UICONTROL 一般 ] に変更すると、既存のタスク、問題およびプロジェクトの時間はすべてシステムのデフォルトのタイプに設定されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 売上高としてカウント ]</td> 
      <td>この時間タイプに関連付けられた時間エントリが売上高の計算に影響を与える場合は、このオプションを選択します。</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL 売上高としてカウント]**:この時間タイプに関連付けられた時間エントリが売上高の計算に影響を与える場合は、このオプションを選択します。

1. クリック **[!UICONTROL 時間タイプを作成].**

## 時間タイプを非アクティブ化

時間タイプが廃止され、ユーザーが時間エントリを関連付ける必要がなくなった場合は、時間タイプを無効にできます。

時間タイプを非アクティブ化すると、 [!DNL Workfront] 時間タイプが表示される場所

時間を非アクティブ化するには、次のように入力します。

1. クリック **[!UICONTROL 設定]** 右上隅付近 [!DNL Adobe Workfront] グローバルナビゲーションバーの

1. 展開 **[!UICONTROL タイムシートと時間の基本設定]**&#x200B;を選択し、「 **[!UICONTROL 時間タイプ]**.

1. 非アクティブ化する時間タイプを選択します。

1. クリック **[!UICONTROL 無効化]**.
