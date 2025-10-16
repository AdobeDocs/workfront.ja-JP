---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: リソース管理環境設定の指定
description: 管理者は、ご使用  [!DNL Adobe Workfront]  システムのリソース管理の環境設定を指定できます。 これらのリソース管理環境設定は、ユーザーの空き時間またはキャパシティおよび FTE が [!DNL Workfront] リソースのスケジュールおよび計画ツールでどのように計算されるかを決定します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 55%

---

# [!UICONTROL リソース管理]環境設定の指定

<!-- Audited: 5/2025 -->

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

[!DNL Adobe Workfront] 管理者は、ご利用のシステムで [!UICONTROL  リソース管理 ] 環境設定を指定できます。 これらの環境設定は、ユーザーの時間数、FTE 使用可能時間またはキャパシティが [!DNL Workfront] リソーススケジュールおよび計画ツールでどのように計算されるかを決定します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーのキャパシティを計算する際に考慮される情報

ユーザーのキャパシティを計算する際に、Workfront では次の情報を考慮に入れます。

* ユーザーのスケジュールまたはWorkfront システムのデフォルトのスケジュールで定義された、スケジュールされた時間数。
* スケジュールの例外（使用されるスケジュールに応じて、ユーザーのスケジュールの例外またはWorkfrontのデフォルトスケジュールに関連付けられた例外が発生する可能性があります）。
* ユーザーの休暇。
* ユーザーまたは [!DNL Workfront] システムのフルタイム当量（[!UICONTROL FTE]）の値。ユーザーがスケジュールで定義されているとおりにフルタイムで作業する場合、[!UICONTROL FTE] は 1 に等しくなります。
* ユーザーの [!UICONTROL  作業時間 ] の値。ユーザーがプロジェクト関連の作業に費やす時間を指します。 会議やトレーニングなどのオーバーヘッド時間は含まれません。[!UICONTROL 作業時間]が 1 と等しくなるのは、[!UICONTROL FTE] またはスケジュールに示される全時間にわたってユーザーが作業可能な場合で、会議やトレーニングなど、プロジェクトに関係しない作業に時間を費やさないことを意味します。


[!DNL Workfront] でのリソースの計画とスケジュールについては、[リソース管理の基本を学ぶ](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)を参照してください。


## [!UICONTROL リソース管理]環境設定の指定

>[!NOTE]
>
>これはグローバル設定なので、この選択は、すべてのリソース管理ツールで、すべてのユーザーに対して、システム全体のすべての計算に影響を及ぼします。

{{step-1-to-setup}}

1. 「**[!UICONTROL リソース管理]**」をクリックします。
1. 次のいずれかの方法を選択して、[!DNL Workfront] でのユーザーの空き時間を計算します。

   * **デフォルトスケジュール**:[!DNL Workfront] は、システムのデフォルトスケジュールとユーザーの個々の FTE を使用して、リソース管理ツールでユーザーの利用可能時間を計算します。

     詳しくは、[ スケジュールの作成 ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) および [ ユーザープロファイルの編集 ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) を参照してください。

     このオプションを選択すると、Workfrontは次の式を使用してユーザーの利用可能時間を計算します。


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >例えば、デフォルトスケジュールが週 40 時間で、ユーザーのプロファイルの FTE が 0.5 で、ユーザーのプロファイルの休暇は 1 時間で、ユーザーのプロファイルの [!UICONTROL  作業時間 ] は 0.5 で、ユーザーは週に 9.5 時間、実際のプロジェクトの作業に使用できます。
     >
     >ユーザーに 1 日に 1 時間の休暇がある場合、利用可能時間数は次のように計算されます。
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

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

   * **ユーザーのスケジュール**：[!DNL Workfront] では、ユーザーのスケジュールとシステムの[!UICONTROL デフォルトのスケジュール]を使用して、リソース管理ツールでユーザーの利用可能な [!UICONTROL FTE] 値を計算します。「利用可能時間」はユーザーのスケジュールに従ってのみ計算され、ユーザーの [!UICONTROL FTE] の値は無視されます。 これはデフォルトの設定です。

     詳しくは、[ スケジュールの作成 ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) および [ ユーザープロファイルの編集 ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) を参照してください。

     >[!NOTE]
     >
     >ユーザーがスケジュールに関連付けられていない場合、ユーザーの利用可能時間数は[!UICONTROL デフォルトのスケジュール]のみを使用して計算されます。

     ユーザーの利用可能時間数は、次の式で計算されます。


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     ユーザーの利用可能な [!UICONTROL FTE] の値は、次の式で計算されます。


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >例えば、[!UICONTROL  デフォルトのスケジュール ] が週 40 時間の場合、ユーザーのスケジュールは週 30 時間、ユーザーの [!UICONTROL  作業時間 ] は 0.5、[!UICONTROL FTE] は 0.35 です。
     >
     >ユーザーが 1 日に 2 時間の休暇を取っている場合、そのユーザーの週間利用可能 [!UICONTROL FTE] は次のように計算されます。
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

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
