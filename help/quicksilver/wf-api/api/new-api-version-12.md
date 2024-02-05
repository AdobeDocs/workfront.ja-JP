---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 12 の新機能
description: Workfront は、2020年11月12日（PT）に API バージョン 12 をリリースしました。API バージョン 12 では、バージョン 11 から次の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2475'
ht-degree: 100%

---

# API バージョン 12 の新機能

Workfront は、2020年11月12日（PT）に API バージョン 12 をリリースしました。API バージョン 12 では、バージョン 11 から次の変更が行われました。

## 追加されたリソース

Workfront API バージョン 12 で次の新しいリソースが追加されました。

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

BreadCrumb オブジェクトは、Adobe Workfront 作業アイテムの親子階層内の要素を表します。パンくずリストは、作業アイテムがポートフォリオ、プロジェクトおよびタスクの大きい構造にどのように適合するかを示します。

Workfront のパンくずリストについて詳しくは、[新しい Adobe Workfront エクスペリエンスのパンくずリストの概要](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)を参照してください。

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>アクション</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

より多くのオブジェクトでリッチテキストフィールドを使用できるようになりました。この可用性をサポートするため、RichTextParameterValue オブジェクトが Workfront に追加されました。

詳しくは、[Adobe Workfront API のリッチテキストフィールド](../../wf-api/general/rich-text-field-api.md)を参照してください。

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コアフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 削除されたリソース

API バージョン 12 ではリソースが削除されませんでした。

## 変更されたリソース

Workfront API バージョン 12 で次のリソースを変更しました。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnnouncementAttachment</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">承認</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">CalendarSection</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">会社</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">顧客</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">ドキュメント</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">グループ</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">パラメーター</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">ポートフォリオ</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">プログラム</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">タスク</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">チーム</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TemplateTask</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">タイムシート</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">ユーザー</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">作業 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevel {#accesslevel}

AccessLevel オブジェクトはユーザーに関連付けられていて、ユーザーのアクセス権を指定する AccessLevelPermissions のセットを表します。

アクセスレベルについて詳しくは、[アクセスレベルの仕組み](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md)を参照してください。

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions オブジェクトは、Workfront オブジェクトにアクセス、作成または変更を行うための特定の権限を表します。これらの権限は、アクセスレベルに関連付けることができます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> <p>この権限を含むアクセスレベルを持つユーザーは、ワークロードバランサーで予定時間を更新できます。</p> <p>詳しくは、<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>の<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">ユーザー割り当て管理時にタスク予定時間数を更新</a>を参照してください。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>この権限を含むアクセスレベルのユーザーは、カスタムフォームにフィールドを追加できます。</p> <p>詳しくは、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>の<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a>を参照してください。</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>この権限を含むアクセスレベルを持つユーザーは、ユーザーフィールドをシステム全体で削除アクセス権と共有できます。</p> <p>詳しくは、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">カスタムフィールドとウィジェットの共有の設定</a>を参照してください。</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

Workfront のオブジェクトに対する必要なアクセス権をユーザーが持っていない場合、そのオブジェクトへの利用申請を行うことができます。AccessRequest オブジェクトは、このリクエストを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">アクション</p> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> <p>この権限を含むアクセスレベルを持つユーザーは、ワークロードバランサーで予定時間を更新できます。</p> <p>詳しくは、<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>の<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">ユーザー割り当て管理時にタスク予定時間数を更新</a>を参照してください。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>この権限を含むアクセスレベルのユーザーは、カスタムフォームにフィールドを追加できます。</p> <p>詳しくは、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>の<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a>を参照してください。</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>この権限を含むアクセスレベルを持つユーザーは、ユーザーフィールドをシステム全体で削除アクセス権と共有できます。</p> <p>詳しくは、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">カスタムフィールドとウィジェットの共有の設定</a>を参照してください。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

AccessRule オブジェクトは、作成したプロジェクトをユーザーが共有する方法を決定する、カスタムアクセスレベルのルールセットを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> <p>この権限を含むアクセスレベルを持つユーザーは、ワークロードバランサーで予定時間を更新できます。</p> <p>詳しくは、<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>の<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">ユーザー割り当て管理時にタスク予定時間数を更新</a>を参照してください。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>この権限を含むアクセスレベルのユーザーは、カスタムフォームにフィールドを追加できます。</p> <p>詳しくは、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>の<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a>を参照してください。</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>この権限を含むアクセスレベルを持つユーザーは、ユーザーフィールドをシステム全体で削除アクセス権と共有できます。</p> <p>詳しくは、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">カスタムフィールドとウィジェットの共有の設定</a>を参照してください。</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

ActivityLog オブジェクトは、特定の Workfront Proof アカウントで発生したすべてのアクティビティの完全なリストです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>操作</p> </td> 
   <td> <p>次の操作が ActivityLog オブジェクトから削除されました。</p> 
    <ul> 
     <li> <p><strong>ADD</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnnouncementAttachment {#announcementattachment}

AnnouncementAttachment オブジェクトは、Workfront のお知らせに添付されたファイルを表します。

お知らせの添付ファイルについて詳しくは、[お知らせの送信](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接フィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>次の値を追加しました。</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 承認 {#approval}

タスク、ドキュメント、タイムシートなどの所定の作業アイテムは、上司または他のユーザーが承認することが必要な場合があります。承認オブジェクトは、作業アイテムに対する承認の操作を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>次のフラグを削除しました。</p> 
      <ul> 
       <li> <p>DYNAMIC</p> </li> 
       <li> <p>LAZY_READ</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>次のフラグを追加しました。</p> 
      <ul> 
       <li> <p>AUTO_LOAD</p> </li> 
       <li> <p>DYNAMIC</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>このフィールドは、タスクを完了するためにユーザーが 1 日にあたりに必要とする作業量が小、中、大のどれになるかを表します。次の値を指定できます。</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>Workfront の作業量について詳しくは、<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CalendarSection {#calendarsection}

カレンダーセクションは、カレンダーレポートです。

カレンダーレポートの詳細については、[カレンダーレポートの概要](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> <p style="font-weight: normal;">カレンダーレポートでカスタム日付を使用する新機能をサポートするために、次のフィールドが CalendarSection オブジェクトに追加されました。 </p> <p style="font-weight: normal;">詳しくは、<a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">カレンダーレポートでのカスタム日付フィールドの使用</a>を参照してください。</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 会社 {#company}

会社オブジェクトは、人物の集まりで構成される組織を表します。

会社について詳しくは、[会社の作成と編集](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">会社が関連付けられているグループの ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>グループ</p> <p style="font-weight: normal;">会社が関連付けられているグループ。会社をグループに関連付けると、グループ管理者はグループアクセスと会社に対する権限を拡張できます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 顧客 {#customer}

顧客オブジェクトは、Workfront のインスタンスを使用する組織を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>アクション</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">このアクションは、引数 CustomerProductTypeEnum を受け取り、その顧客がその製品のアカウントを持っているかどうかを示すブール値を返します。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

CustomerPreferences オブジェクトは、Workfront のインスタンスに対して顧客が設定した一連の環境設定を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>名前</p> <p style="font-weight: normal;">次の値を追加しました。</p> 
      <ul> 
       <li style="font-weight: normal;">password:zoomIntegrationEnabled（更新ストリームで Zoom 統合を有効にする）</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled（config.general.quip.enabled）</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ドキュメント {#document}

Document オブジェクトは、ファイル（書かれた資料、画像、その他の形式の情報など）を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>アクション</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

DocumentVersion オブジェクトは、ファイルの特定のバージョン（書き込まれた資料、画像、その他の形式の情報など）を表します。

ドキュメントのバージョンについて詳しくは、[新しいバージョンのドキュメントのアップロード](../../documents/managing-documents/upload-new-document-version.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">可能性のある値を削除しました：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP（Quip）</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>アクション</td> 
   <td> <p>次のアクションがドキュメントオブジェクトに追加されました。</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">このアクションは、documentVersonID 引数（文字列）を受け取り、レビュアーの決定を示すマップを返します。</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">このアクションは、次の引数を受け取ります。</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID（文字列）</p> </li> 
       <li> <p>reviewerDecision（文字列）</p> </li> 
       <li> <p>comment (string)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### グループ  {#group}

グループオブジェクトは、一連のユーザーとチームを表します。グループは、多くの場合、部門の構造を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">グループに割り当てられたビジネスリーダーの ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">グループに割り当てられたビジネスリーダー。ビジネスリーダーとは、グループのビジネス上の決定を行う人物のことです。</p> <p style="font-weight: normal;">ビジネスリーダーについて詳しくは、<a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">ビジネスリーダーの概要</a>を参照してください。<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>アクション</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>このアクションは、次の引数を受け取ります。</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID (string)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>このアクションは、次の引数を受け取ります。</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removedMemberDs (string[])</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

LinkedFolder オブジェクトは、Google Drive や Dropbox など、外部のドキュメントプロバイダからリンクされたフォルダーを表します。

リンクされたフォルダーの詳細情報については、[外部アプリケーションからドキュメントをリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接フィールド</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">可能性のある値を削除しました：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP（Quip）</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

OpTask オブジェクトは、一般にイシューと呼ばれます。イシューは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業アイテムです。イシューは、ヘルプデスクへのリクエストである場合もあります。変更指示、リクエスト、バグもイシューです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>直接フィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>順序は、アジャイルバックログ上のタスクまたはストーリーの位置を示します。</p> <p>このフィールドは、次のフラグを削除しました。
       <ul>
        <li>DYNAMIC</li>
        <li>LAZY_READ</li>
        <li>NOT_GROUPABLE</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> <p>これらのアクションでは、引数のステータスが追加され、新しい「開始」ボタン機能をサポートするようになりました。この機能は、ユーザーがボタンをクリックして、アイテムの作業を開始したことを示す作業アイテムのステータスを変更します。</p> <p>詳しくは、<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業をする」ボタンを「開始」ボタンに置き換え</a>を参照してください。</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### パラメーター {#parameter}

パラメーターオブジェクトは、カスタムフィールドです。

パラメーターリソースにより、フラグ SHARABLE が追加されました。

カスタムフィールドについて詳しくは、[カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)で[カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>次の値を追加できます。</p> 
      <ul> 
       <li> <p>RICH（リッチテキスト）</p> <p>詳しくは、<a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API のリッチテキストフィールド</a>を参照してください。</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>次の値を追加できます。</p> 
      <ul> 
       <li> <p>RICH（書式付きテキストフィールド)</p> <p>詳しくは、<a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API のリッチテキストフィールド</a>を参照してください。</p> </li> 
      </ul> </li> 
     <li> <p><strong>ラベル</strong> </p> <p>追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">コレクションフィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>ラベル</strong> </p> <p>追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ポートフォリオ {#portfolio}

ポートフォリオオブジェクトは、同じリソース（通常はプロジェクトを完了するための資金や人材）を競い合って完了するプロジェクトのコレクションです。

ポートフォリオについて詳しくは、[Adobe Workfront の Portfolio の概要](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">ポートフォリオが関連付けられているグループの ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>グループ</p> <p style="font-weight: normal;">ポートフォリオが関連付けられているグループ。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### プログラム {#program}

プログラムオブジェクトは、ポートフォリオ内のプロジェクトのサブセットで、類似のプロジェクトを 1 つにグループ化できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">プログラムが関連付けられているグループの ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>グループ</p> <p style="font-weight: normal;">プログラムが関連付けられているグループ。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef オブジェクトは、キューを表します。キューは、ユーザーがイシューを送信できるようにヘルプデスクエリアに公開されたプロジェクトです。

リクエストキューについて詳しくは、[リクエストキューの作成](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li><strong>requestorCoreAction</strong> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> <p>この権限を含むアクセスレベルを持つユーザーは、ワークロードバランサーで予定時間を更新できます。</p> <p>詳しくは、<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>の<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">ユーザー割り当て管理時にタスク予定時間数を更新</a>を参照してください。</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>この権限を含むアクセスレベルのユーザーは、カスタムフォームにフィールドを追加できます。</p> <p>詳しくは、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>の<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a>を参照してください。</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>この権限を含むアクセスレベルを持つユーザーは、ユーザーフィールドをシステム全体で削除アクセス権と共有できます。</p> <p>詳しくは、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">カスタムフィールドとウィジェットの共有を設定</a>を参照してください。</p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>次の possibleValues が追加されました。</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTERING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

ScheduledReport オブジェクトは、配信のスケジュールを設定したレポートを表します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>形式</strong> </p> <p>次の値を追加しました。</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。これらの質問は通常、ポートフォリオマネージャーが決定し、その回答によって、マネージャーはプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。

スコアカードに関する質問について詳しくは、[スコアカードを作成](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">可能な値 RICH（書式付きテキストフィールド）を追加しました </p> <p style="font-weight: normal;">詳しくは、<a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API のリッチテキストフィールド</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### タスク {#task}

タスクオブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>このフィールドは、タスクを完了するためにユーザーが 1 日にあたりに必要とする作業量が小、中、大のどれになるかを表します。次の値を指定できます。</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>Workfront の作業量について詳しくは、<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> <p>これらのアクションでは、引数のステータスが追加され、新しい「開始」ボタン機能をサポートするようになりました。この機能は、ユーザーがボタンをクリックして、アイテムの作業を開始したことを示す作業アイテムのステータスを変更します。</p> <p>詳しくは、<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業をする」ボタンを「開始」ボタンに置き換え</a>を参照してください。</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### チーム {#team}

チームオブジェクトは、作業アイテムに割り当てることができるユーザーの集まりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> <p>チームリソースに次のフィールドが追加されました。</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>このフィールドは、完了したカードがかんばんボードに残る日数を表します。</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>このフィールドは、チームをグループに関連付けます。これにより、チームがグループの一部として識別され、グループ管理者がチームを管理できるようになります。</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>チームの「作業」ボタンが「開始」ボタンとして設定されているかどうかを示すブール値パラメーターです。チームのメンバーが「開始」ボタンをクリックして作業アイテムの作業を開始すると、その項目のステータスが「新規」からチーム設定に設定されたステータスに変わります。</p> </li> 
     <li> <p>次のフィールドでは、個々の作業アイテムの「開始」ボタンにカスタムステータスを指定できます。</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>「開始」ボタンについて詳しくは、<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業」ボタンを「開始」ボタンに置き換え</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">参照フィールド</td> 
   <td> <p>チームリソースに次のフィールドが追加されました。</p> 
    <ul> 
     <li> <p><strong>グループ</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

TemplateTask オブジェクトは、テンプレートに含まれるタスクを表します。テンプレートタスクは、テンプレートが使用されるプロジェクト内のタスクになります。

テンプレートタスクについて詳しくは、[テンプレートタスクの編集](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)を参照ください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>このフィールドは、タスクを完了するためにユーザーが 1 日にあたりに必要とする作業量が小、中、大のどれになるかを表します。次の値を指定できます。</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>Workfront の作業量について詳しくは、<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### タイムシート {#timesheet}

タイムシートオブジェクトは、タスク、プロジェクトおよびオーバーヘッド時間タイプの実際の時間数をユーザーが入力できる仮想タイムカードを表します。

タイムシートについて詳しくは、[タイムシートの概要](../../timesheets/timesheets/timesheets-overview.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">コアフィールド</td> 
   <td> <p>次のフィールドは、タイムシートリソースから削除されました。</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### アップデート

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>追加された可能な値は次のとおりです。</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">イニシアチブについて詳しくは、<a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">シナリオプランナーのイニシアチブの概要</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ユーザー {#user}

ユーザーオブジェクトは、ログインしてシステムとやり取りできる Workfront アカウントを持つユーザーを表します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> <p>ユーザーリソースに次のフィールドが追加されました。</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>ユーザーが非アクティブ化された日時を表します。</p> <p>非アクティブ化されたユーザーについて詳しくは、<a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーの非アクティブ化または再アクティブ化</a>を参照してください。</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>このフィールドには、Workfront Goals へのユーザーのアクセス権が表示されます。次の値を指定できます。</p> 
      <ul> 
       <li> <p>アクセスなし</p> </li> 
       <li> <p>表示</p> </li> 
       <li> <p>編集</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> <p>ユーザーリソースに次のアクションが追加されました。</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>このアクションは、次の引数を取ります。</p> 
      <ul> 
       <li> <p>ids（文字列）</p> </li> 
       <li> <p>objCode（文字列）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ワーク  {#work}

作業オブジェクトは、Task と OpTask の両方が継承する共通のインターフェイスで、2 つの間で共通のコードを共有します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>順序は、アジャイルバックログ上のタスクまたはストーリーの位置を示します。</p> <p>このフィールドは、次のフラグを削除しました。</p> 
      <ul> 
       <li> <p>DYNAMIC</p> </li> 
       <li> <p>LAZY_READ</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>このフィールドには、次のフラグが追加されました。</p> 
      <ul> 
       <li> <p>AUTO_LOAD</p> </li> 
       <li> <p>DYNAMIC</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>このフィールドは、タスクを完了するためにユーザーが 1 日にあたりに必要とする作業量が小、中、大のどれになるかを表します。次の値を指定できます。</p> 
      <ul> 
       <li> <p>1（小）</p> </li> 
       <li> <p>2（中）</p> </li> 
       <li> <p>3（大）</p> </li> 
      </ul> <p>Workfront の作業量について詳しくは、<a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>を参照してください。</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
