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
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# 設定 [!UICONTROL リソース管理] 環境設定

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

As a [!DNL Adobe Workfront] 管理者は、 [!UICONTROL リソース管理] システムの環境設定。 これらの環境設定では、 [!DNL Workfront] リソースのスケジュールおよび計画ツール。

## アクセス要件

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>システム管理者のアクセスレベル</p> <p>詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>メモ</b>:

まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## ユーザーの容量を計算する際に考慮される情報

ユーザーの容量を計算する際、Workfrontでは次の情報が考慮されます。

* ユーザーのスケジュールまたはWorkfrontシステムのスケジュールで定義された、スケジュールされた時間数 [!UICONTROL デフォルトのスケジュール]
* [!UICONTROL スケジュール] [!UICONTROL 例外] ( [!UICONTROL スケジュール] が使用されている場合、ユーザーのスケジュールの例外である場合、または [!DNL Workfront] [!UICONTROL デフォルトのスケジュール])
* ユーザーのオフタイム
* フルタイム相当 ([!UICONTROL FTE]) に含まれます。 [!DNL Workfront] システム。 この [!UICONTROL FTE] は、スケジュールで定義されているように、ユーザーがフルタイムで作業する場合は 1 に等しくなります。
* の値 [!UICONTROL 作業時間] ユーザーがプロジェクト関連の作業に費やした時間を参照するユーザーの場合。 会議やトレーニングなどのオーバーヘッド時間は含まれません。 この [!UICONTROL 作業時間] が 1 に等しいのは、ユーザーが作業に使用できる状態が [!UICONTROL FTE] スケジュールとは、会議やトレーニングなど、プロジェクトに関連しない作業に時間を費やさないということです。


でのリソースの計画とスケジュールに関する情報 [!DNL Workfront]を参照してください。 [リソース管理の概要](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## 設定 [!UICONTROL リソース管理] 環境設定

>[!NOTE]
>
>この設定はグローバル設定なので、この選択は、すべてのユーザーに対して、すべてのリソース管理ツールのシステム全体のすべての計算に影響を与えます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. クリック **[!UICONTROL リソース管理]**.
1. 次のいずれかの方法を選択して、でのユーザーの可用性を計算します。 [!DNL Workfront]:

   * **デフォルトのスケジュール**: [!DNL Workfront] は、システムのデフォルトスケジュールとユーザーの個々の FTE を使用して、リソース管理ツールのユーザーの使用可能時間を計算します。

      スケジュールについて詳しくは、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      ユーザーの [!UICONTROL FTE]を参照してください。  [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfrontは、Workfront管理者が [!UICONTROL デフォルトのスケジュール]:

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]
      ```

      >[!INFO]
      >
      >例えば、デフォルトスケジュールが週 40 時間の場合、ユーザーのプロファイルの FTE が 0.5 である場合、ユーザーは 1 日 1 時間のオフタイムを持ち、 [!UICONTROL 作業時間] ユーザーのプロファイルが 0.5 の場合、ユーザーは週に 9.5 時間、実際のプロジェクト作業に使用できます。
      >
      >ユーザーが 1 日に 1 時間のオフタイムを持っている場合、利用可能な時間は次のように計算されます。
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
      -->



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

   * **ユーザーのスケジュール**: [!DNL Workfront] は、ユーザーのスケジュールと [!UICONTROL デフォルトのスケジュール] システムが使用可能な [!UICONTROL FTE] リソース管理ツールでのユーザーの値。 利用可能な時間数は、ユーザーのスケジュールに従ってのみ計算されます。 の値 [!UICONTROL FTE] の値は無視されます。 これはデフォルト設定です。

      スケジュールについて詳しくは、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      ユーザーの [!UICONTROL スケジュール]を参照してください。  [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >ユーザーがスケジュールに関連付けられていない場合、ユーザーの使用可能時間は [!UICONTROL デフォルトのスケジュール].

      ユーザーが使用できる時間は、次の数式で計算されます。

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```

      利用可能な [!UICONTROL FTE] の値は、次の式で計算されます。

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >例えば、 [!UICONTROL デフォルトのスケジュール] が週に 40 時間、ユーザーのスケジュールが週に 30 時間、ユーザーの [!UICONTROL 作業時間] は 0.5 です。 [!UICONTROL FTE] の値は 0.35 です。
      >
      >ユーザーが 1 日に 2 時間の休暇を取っている場合、そのユーザーの週間利用可能 [!UICONTROL FTE] は次のように計算されます。
      >
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35
      >```

      <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. 「**[!UICONTROL 保存]**」をクリックします。
