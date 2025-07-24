---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 時間タイプの管理
description: 時間タイプを時間エントリに関連付けることができます。時間タイプは、時間エントリの定義に使用するラベルです。 時間タイプは、一般的な時間の場合と、プロジェクト固有の時間の場合があります。
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 23%

---

# 時間タイプを管理

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

<div class="preview">

このページで強調表示されている情報は、まだ一般公開されていない機能を示しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 プレビューリリースから 1 週間後に、すべてのお客様の実稼動環境でも同じ機能が使用できるようになります。

詳しくは、[ インターフェイスの最新化 ](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md) を参照してください。

</div>

時間タイプは、時間エントリの定義に使用するラベルです。 時間タイプを時間エントリに関連付けることができます。

時間タイプには、次の 2 つのカテゴリがあります。

* **プロジェクト固有の時間タイプ**：プロジェクト、タスクおよびイシューのログ時間です。プロジェクト固有の時間タイプは、プロジェクト、タスク、イシューの時間を記録できる、[!DNL Adobe Workfront] 内の任意の場所で時間エントリに関連付けることができます。

  [!DNL Workfront]で時間を記録する場合、使用できるプロジェクト固有の時間タイプは、システムレベル、プロジェクトレベルおよびユーザーレベルで設定された設定オプションによって異なります。

  以下のデフォルトのプロジェクト固有の時間タイプは、常に使用できます。

   * プロジェクト時間
   * タスク時間
   * イシュー時間

  [!DNL Workfront] 時間タイプと空き時間の定義 [ で説明されているように、](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md) 管理者は、プロジェクト固有の時間タイプを使用可能にすることを決定します。

  >[!NOTE]
  >
  >[!DNL Workfront] システムでプロジェクト固有の時間タイプを有効にする場合は、システム内の各プロジェクトで、1 つ以上のプロジェクト固有の時間タイプを有効にする必要があります。システムレベルではプロジェクト固有の時間タイプを有効にできず、プロジェクトレベルではプロジェクト固有の時間タイプを利用できません。

* **一般的な時間タイプ**：一般的な時間は、プロジェクト、タスク、または問題に関連付けることはできず、タイムシートに直接記録されます。

時間の記録および時間タイプとの関連付けについて詳しくは、[ 時間の記録 ](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md) を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td>システム管理者</td>
  </tr> 
 </tbody> 
</table>

*このテーブルの詳細については、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## ビルトインの時間タイプ

Workfront には、一連のビルトインの時間タイプが付属しています。これらの時間タイプは、編集または非表示にできません。

[!DNL Workfront] に付属する時間タイプは以下のとおりです。

* **[!UICONTROL 病欠時間]**: プロジェクト、タスク、または問題の時間エントリに関連付けることができない一般的な時間タイプ。 病欠時間は、収益としてカウントできません。
* **[!UICONTROL 休暇]**: プロジェクト、タスク、または問題の時間エントリに関連付けることはできない一般的な時間タイプ。 休暇を収益としてカウントすることはできません。
* **[!UICONTROL 一般的なオーバーヘッド]**：プロジェクト、タスク、または問題の時間エントリに関連付けることができない一般的な時間タイプ。 プロジェクト計画プロセスでは、収益としてカウントできます。
* **[!UICONTROL プロジェクト時間]**: プロジェクトの時間エントリにのみ関連付けることができる一般的な時間タイプ。
* **[!UICONTROL タスク時間]**: タスクの時間エントリにのみ関連付けることができる一般的な時間タイプ。
* **[!UICONTROL 問題時間]**：問題の時間エントリにのみ関連付けることができる一般的な時間タイプ。

## 時間タイプを作成

[!DNL Workfront] 管理者は、組織の時間タイプをシステムレベルおよびプロジェクトレベルで作成できます。

システムレベルで時間タイプを定義した後、ユーザーは特定のプロジェクトまたは特定のユーザーが使用できる時間タイプを定義できます。

詳しくは、[ 時間タイプと可用性の定義 ](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md) を参照してください

時間タイプを作成する手順は、次のとおりです。

{{step-1-to-setup}}

1. 左側のパネルで **タイムシートと時間** をクリックし、**時間タイプ** をクリックします。

1. 「**時間タイプ**」セクションで、「**新しい時間タイプ**」をクリックします。
1. **新しい時間タイプ** ダイアログボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>システムで簡単に認識できる時間タイプ名を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>時間タイプの説明を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p><strong> 範囲 </strong> ドロップダウンメニューで、時間タイプが一般的な時間タイプかプロジェクト固有の時間タイプかを選択します。</p> <p>一般的な時間タイプは、タイムシートにのみ表示され、プロジェクト、タスク、または問題に関連付けることはできません。</p> <p><b>重要</b></p><p> [!UICONTROL プロジェクト固有 ] のカスタム時間タイプがあり、それを [!UICONTROL 一般 ] に変更した場合、既存のタスク、問題、およびプロジェクト時間はすべて、システムの既定の時間タイプに設定されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="preview">[!UICONTROL 収益カウント ]</span></td> 
      <td><p>この時間タイプに関連付けられた時間エントリを収益の計算に反映させたい場合は、このオプションを選択します。</p>
      <p>病欠時間と休暇時間は、収益としてカウントできません。</p>
      <p><b>メモ</b></p>
      <p>一般的な時間タイプが収益としてカウントされる場合、時間を記録しているユーザーのプロファイルに関連付けられたコスト率は、時間コストに関連付けられます。  
      </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 時間タイプを作成]** <span class="preview"> または **保存** をクリックします。</span>

   時間タイプはWorkfront システムに追加され、デフォルトで有効になっています。

## 時間タイプの編集

[!DNL Workfront] 管理者は、組織の時間タイプをシステムレベルおよびプロジェクトレベルで編集できます。

>[!NOTE]
>
>* ビルトインの時間タイプは編集できません。
>* 時間タイプを一括で編集することはできません。

{{step-1-to-setup}}

1. 左側のパネルで **タイムシートと時間** をクリックし、**時間タイプ** をクリックします。

1. 時間タイプ名をクリックするか、時間タイプを選択して、リストの上部にある **編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。
1. **時間タイプを編集** ダイアログボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>システムで簡単に認識できる時間タイプ名を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>時間タイプの説明を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p><strong> 範囲 </strong> ドロップダウンメニューで、時間タイプが一般的な時間タイプかプロジェクト固有の時間タイプかを選択します。</p> <p>一般的な時間タイプは、タイムシートにのみ表示され、プロジェクト、タスク、または問題に関連付けることはできません。</p> <p><b>重要</b></p> <p>[!UICONTROL プロジェクト固有 ] のカスタム時間タイプがあり、それを [!UICONTROL 一般 ] に変更した場合、既存のタスク、問題、およびプロジェクト時間はすべて、システムの既定の時間タイプに設定されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="preview">[!UICONTROL 収益カウント ]</span></td> 
      <td><p>この時間タイプに関連付けられた時間エントリを収益の計算に反映させたい場合は、このオプションを選択します。</p>
      <p>病欠時間と休暇時間は、収益としてカウントできません。</p>
      <p><b>メモ</b></p>
      <p>一般的な時間タイプが収益としてカウントされる場合、時間を記録しているユーザーのプロファイルに関連付けられたコスト率は、時間コストに関連付けられます。  
      </td> 
     </tr> 
    </tbody> 
   </table>


1. **[!UICONTROL 変更を保存]** <span class="preview"> または **保存** をクリックします。</span>

   変更内容が保存され、時間タイプが編集されます。

## 時間タイプの非アクティブ化

ユーザーに時間を関連付けさせたくない場合、時間タイプをディアクティベートできます。 時間タイプを非アクティブ化すると、時間タイプが表示される [!DNL Workfront] のどこからでも非表示になります。

>[!NOTE]
>
>* 組み込みの時間タイプは非アクティブ化できません。
>* 時間タイプは一括で非アクティブ化できます。
>* プロジェクト固有の時間タイプを非アクティブ化すると、そのタイプでログに記録されたすべての時間は、自動的にビルトインのプロジェクト固有の時間タイプにデフォルト設定されます。 例えば、プロジェクトのログ時間はデフォルトでプロジェクト時間タイプに、タスクのログ時間はデフォルトでタスク時間タイプに設定されます。
>* 一般的な時間タイプを非アクティブ化すると、ログ時間はタイムシートに残りますが、ユーザーは、今後その時間タイプの時間をログに記録できなくなります。



時間タイプを非アクティブ化するには、次の手順に従います。

{{step-1-to-setup}}

1. 左側のパネルで **[!UICONTROL タイムシートと時間]** をクリックし、**[!UICONTROL 時間タイプ]** をクリックします。

1. 非アクティブ化する時間タイプを選択します。 複数の時間タイプを選択できます。

1. 「**詳細**」をクリックしてから「**アクティベートを解除** をクリックします。

   ![ 時間タイプのリンクのアクティブ化と非アクティブ化 ](assets/activate-and-deactivate-hour-type-links.png)

   時間タイプは非アクティブ化され、ユーザーは時間をログに記録すると見つけることができなくなります。

1. （任意）時間タイプを再アクティブ化するには、**時間タイプ** リストでその時間を選択し、**詳細**/**アクティブ化** をクリックします。

