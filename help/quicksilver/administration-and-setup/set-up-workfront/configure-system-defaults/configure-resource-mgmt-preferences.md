---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: リソース管理環境設定の指定
description: As a [!DNL Adobe Workfront] 管理者は、システムのリソース管理環境設定を構成できます。 これらのリソース管理環境設定により、 [!DNL Workfront] リソースのスケジュールおよび計画ツール。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---

# 設定 [!UICONTROL リソース管理] 環境設定

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

As a [!DNL Adobe Workfront] 管理者は、 [!UICONTROL リソース管理] システムの環境設定。 これらの環境設定では、 [!DNL Workfront] リソースのスケジュールおよび計画ツール。

でのリソースの計画とスケジュールに関する情報 [!DNL Workfront]を参照してください。 [リソース管理の概要](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者のアクセスレベル</p> <p>詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定 [!UICONTROL リソース管理] 環境設定

>[!NOTE]
>
>この選択はグローバル設定なので、システム全体、すべてのユーザー、すべてのリソース管理ツール、およびすべてのリソースプールのすべての計算に影響を与えます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. クリック **[!UICONTROL リソース管理]**.
1. 次のいずれかの方法を選択して、でのユーザーの可用性を計算します。 [!DNL Workfront]:

   * **デフォルトのスケジュール**: [!DNL Workfront] は、システムのデフォルトスケジュールとユーザーの個々の FTE を使用して、リソース管理ツールでユーザーの使用可能時間を計算します。\

      スケジュールについて詳しくは、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      ユーザー FTE の値について詳しくは、  [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfrontは、Workfront管理者が「デフォルトのスケジュール」を選択した場合に、次の式を使用してユーザーの使用可能時間を計算します。

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **例:**\
      例えば、デフォルトスケジュールが週 40 時間で、ユーザーのプロファイルの FTE が 0.5 の場合、ユーザーは週 20 時間の作業を行うことができます。

      ユーザーが 1 日に 1 時間のオフタイムを持っている場合、利用可能な時間は次のように計算されます。

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

      <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
        <div class="example" data-mc-autonum="<b>Example: </b>">      
        <span class="autonumber"><span><b>Example: </b></span></span>      
        <div>      
        <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
        <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
        <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
        </div>      
        </div></li>      
        -->

   * **ユーザーのスケジュール**: [!DNL Workfront] ユーザーのスケジュールとシステムのデフォルトスケジュールを使用して、リソース管理ツールでユーザーの使用可能な FTE 値を計算します。 利用可能な時間数は、ユーザーのスケジュールに従ってのみ計算されます。 ユーザーの FTE の値は無視されます。 これはデフォルト設定です。

      >[!NOTE]
      >
      >ユーザーがスケジュールに関連付けられていない場合、ユーザーの「使用可能な時間」は「デフォルトのスケジュール」を使用して計算されます。

      ユーザーが使用できる FTE は、次の式で計算されます。

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **例：** 例えば、「デフォルトのスケジュール」が週に 40 時間で、ユーザーのスケジュールが週に 30 時間の場合、ユーザーの FTE は 0.75 になります。

      ユーザーが 1 日に 2 時間のオフタイムを持っている場合、週別利用可能時間は次のように計算されます。

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. 「**[!UICONTROL 保存]**」をクリックします。
