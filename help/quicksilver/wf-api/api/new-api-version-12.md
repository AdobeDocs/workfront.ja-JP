---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 12 の新機能
description: Workfrontは、2020 年 11 月 13 日に API バージョン 12 をリリースしました。 API バージョン 12 には、バージョン 11 から次の変更が含まれています。
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2516'
ht-degree: 2%

---

# API バージョン 12 の新機能

Workfrontは、2020 年 11 月 13 日に API バージョン 12 をリリースしました。 API バージョン 12 には、バージョン 11 から次の変更が含まれています。

## 追加されたリソース

次のリソースは、Workfront API バージョン 12 で追加された新しいリソースです。

* [BreadCrumb](#breadcrumb)
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

BreadCrumb オブジェクトは、Adobe Workfront作業項目の親/子階層内の要素を表します。 パンくずリストは、作業項目がPortfolio、プロジェクト、プロジェクト、タスクの構造にどのように適合するかを示します。

Workfrontのパンくずリストについて詳しくは、 [新しいAdobe Workfrontエクスペリエンスのパンくずリストの概要](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

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

より多くのオブジェクトでリッチテキストフィールドを使用できるようになりました。 この可用性をサポートするため、RichTextParameterValue オブジェクトがWorkfrontに追加されました。

詳しくは、 [Adobe Workfront API のリッチテキストフィールド](../../wf-api/general/rich-text-field-api.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
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
     <li> <p><a href="#group" class="MCXref xref">グループ </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">Opタスク</a> </p> </li> 
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

AccessLevel オブジェクトは、ユーザーに関連付けられ、ユーザーがアクセスできる AccessLevelPermissions のセットを表します。

アクセスレベルの詳細については、 [アクセスレベルの仕組み](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

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

AccessLevelPermissions オブジェクトは、Workfrontオブジェクトにアクセス、作成、または変更するための特定の権限を表します。 これらの権限は、アクセスレベルに関連付けることができます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> <p>この権限を含むアクセスレベルを持つユーザーは、ワークロードバランサーで予定時間を更新できます。</p> <p>詳しくは、 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">ユーザー割り当て管理時のタスク計画時間の更新</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>この権限を含むアクセスレベルのユーザーは、カスタムフォームにフィールドを追加できます。</p> <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>この権限を含むアクセスレベルを持つユーザーは、削除アクセス権を持つユーザーフィールドをシステム全体で共有できます。</p> <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">カスタムフィールドとウィジェットの共有を設定する</a>.</p> </li> 
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

ユーザーが必要なWorkfront内のオブジェクトへのアクセス権を持っていない場合、そのオブジェクトへのアクセス権をリクエストできます。 AccessRequest オブジェクトは、このリクエストを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">アクション</p> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> <p>この権限を含むアクセスレベルを持つユーザーは、ワークロードバランサーで予定時間を更新できます。</p> <p>詳しくは、 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">ユーザー割り当て管理時のタスク計画時間の更新</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>この権限を含むアクセスレベルのユーザーは、カスタムフォームにフィールドを追加できます。</p> <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>この権限を含むアクセスレベルを持つユーザーは、削除アクセス権を持つユーザーフィールドをシステム全体で共有できます。</p> <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">カスタムフィールドとウィジェットの共有を設定する</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

AccessRule オブジェクトは、ユーザーが作成したプロジェクトを共有する方法を決定するカスタムアクセスレベルのルールセットを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> <p>この権限を含むアクセスレベルを持つユーザーは、ワークロードバランサーで予定時間を更新できます。</p> <p>詳しくは、 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">ユーザー割り当て管理時のタスク計画時間の更新</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>この権限を含むアクセスレベルのユーザーは、カスタムフォームにフィールドを追加できます。</p> <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>この権限を含むアクセスレベルを持つユーザーは、削除アクセス権を持つユーザーフィールドをシステム全体で共有できます。</p> <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">カスタムフィールドとウィジェットの共有を設定する</a>.</p> </li> 
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

ActivityLog オブジェクトは、特定のWorkfront Proof アカウントで発生したすべてのアクティビティの完全なリストです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>オペレーション</p> </td> 
   <td> <p>次の操作が ActivityLog オブジェクトから削除されました：</p> 
    <ul> 
     <li> <p><strong>追加</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnnouncementAttachment {#announcementattachment}

AnnouncementAttachment オブジェクトは、Workfrontのお知らせに添付されたファイルを表します。

お知らせの添付ファイルについて詳しくは、 [お知らせの送信](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>ダイレクトフィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>次の可能な値を追加しました。</p> 
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

タスク、ドキュメント、タイムシートなどの特定の作業項目に対しては、管理者や他のユーザーが作業項目に対してサインオフする必要が生じる場合があります。 Approval オブジェクトは、作業項目に対するサインオフの操作を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>次のフラグを削除しました。</p> 
      <ul> 
       <li> <p>動的、</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>次のフラグを追加しました。</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>動的、</p> </li> 
       <li> <p>読み取り専用</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>このフィールドが追加され、タスクの完了に 1 日あたりの作業量が小、中、大のどれになるかを表します。 次の値を指定できます。</p> 
      <ul> 
       <li> <p>1 （小）</p> </li> 
       <li> <p>2 （中）</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>Workfrontの作業量について詳しくは、 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CalendarSection {#calendarsection}

カレンダーセクションは、カレンダーレポートです。

カレンダーレポートの詳細については、 [カレンダーレポートの概要](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> <p style="font-weight: normal;">次のフィールドが CalendarSection オブジェクトに追加され、カレンダーレポートでのユーザー設定の日付の使用に関する新しい機能がサポートされました。 </p> <p style="font-weight: normal;">詳しくは、 <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">カレンダーレポートでのカスタム日付フィールドの使用</a>.</p> 
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

Company オブジェクトは、人々の集まりで構成される組織を表します。

会社について詳しくは、 [会社の作成と編集](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">会社が関連付けられているグループの ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>グループ</p> <p style="font-weight: normal;">会社が関連付けられているグループ。 会社をグループに関連付けると、グループ管理者はグループアクセスと会社に対する権限を拡張できます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 顧客 {#customer}

Customer オブジェクトは、Workfrontのインスタンスを使用する組織を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>アクション</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">このアクションは、引数 CustomerProductTypeEnum を取り、その顧客がその製品のアカウントを持っているかどうかを示すブール値を返します。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

CustomerPreferences オブジェクトは、Workfrontのインスタンスに対して顧客が設定した一連の環境設定を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">次の可能な値を追加しました。</p> 
      <ul> 
       <li style="font-weight: normal;">password:zoomIntegrationEnabled （更新ストリームで Zoom 統合を有効にする）</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled (config.general.quip.enabled)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ドキュメント {#document}

Document オブジェクトは、ファイル（書き込まれた資料、画像、その他の形式の情報など）を表します。

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

ドキュメントのバージョンについて詳しくは、 [新しいバージョンのドキュメントをアップロード](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">削除された可能性のある値：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>アクション</td> 
   <td> <p>次のアクションが Document オブジェクトに追加されました。</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">このアクションは、 documentVersonID 引数（文字列）を受け取り、レビュー担当者の決定を示すマップを返します。</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">このアクションは、次の引数を取ります。</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (string)</p> </li> 
       <li> <p>reviewerDecision （文字列）</p> </li> 
       <li> <p>comment （文字列）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### グループ  {#group}

Group オブジェクトは、一連のユーザーとチームを表します。 グループは、多くの場合、部門の構造を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">グループに割り当てられたビジネスリーダーの ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">グループに割り当てられたビジネスリーダー。 ビジネスリーダーとは、グループのビジネス上の意思決定を行う人のことです。</p> <p style="font-weight: normal;">ビジネスリーダーの詳細については、 <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">ビジネスリーダーの概要</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>アクション</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>このアクションは、次の引数を取ります。</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID （文字列）</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>このアクションは、次の引数を取ります。</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removedMemberDs (string[])</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

LinkedFolder オブジェクトは、Google Drive やDropboxなど、外部のドキュメントプロバイダからリンクされたフォルダを表します。

リンクされたフォルダの詳細については、 [外部アプリケーションからドキュメントをリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>ダイレクトフィールド</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">削除された可能性のある値：</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Opタスク {#optask}

OpTask オブジェクトは、一般にイシューと呼ばれます。 問題とは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業項目です。 問題は、ヘルプデスクへのリクエストでもかまいません。 変更管理、要求、バグも問題です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>ダイレクトフィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>順序は、アジャイルバックログ上のタスクまたはストーリーの位置を示します。</p> <p>このフィールドは、次のフラグを削除しました。
       <ul>
        <li>動的、</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> <p>これらの操作では、引数のステータスが追加され、新しい [ 開始 ] ボタン機能をサポートするようになりました。この機能は、ユーザーがボタンをクリックして、項目の作業を開始したことを示す作業項目のステータスを変更します。</p> <p>詳しくは、 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業対象」ボタンを「開始」ボタンに置き換えます</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### パラメーター {#parameter}

Parameter オブジェクトは、カスタムフィールドです。

Parameter リソースにより、フラグ SHARABLE が追加されました。

カスタムフィールドについて詳しくは、 [カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>次の値を追加できます。</p> 
      <ul> 
       <li> <p>リッチ（リッチテキスト）</p> <p>詳しくは、 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API のリッチテキストフィールド</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>次の値を追加できます。</p> 
      <ul> 
       <li> <p>リッチ（書式付きテキストフィールド）</p> <p>詳しくは、 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API のリッチテキストフィールド</a>.</p> </li> 
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

Portfolioオブジェクトとは、同じリソース、通常は費用や担当者を競い合って完了するプロジェクトの集まりです。

ポートフォリオについて詳しくは、 [Adobe WorkfrontのPortfolioの概要](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
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

Program オブジェクトは、ポートフォリオ内のプロジェクトのサブセットで、類似のプロジェクトを 1 つにグループ化できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
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

QueueDef オブジェクトは、Queue を表します。Queue は、ヘルプデスク領域に公開され、ユーザーが問題を送信できるようにするプロジェクトです。

リクエストキューについて詳しくは、 [リクエストキューの作成](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li><strong>requestorCoreAction</strong> <p>次の possibleValues が追加されました。</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTERING </p> <p>この権限を含むアクセスレベルを持つユーザーは、ワークロードバランサーで予定時間を更新できます。</p> <p>詳しくは、 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">ユーザー割り当て管理時のタスク計画時間の更新</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>この権限を含むアクセスレベルのユーザーは、カスタムフォームにフィールドを追加できます。</p> <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>この権限を含むアクセスレベルを持つユーザーは、削除アクセス権を持つユーザーフィールドをシステム全体で共有できます。</p> <p>詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">カスタムフィールドとウィジェットの共有を設定する</a></p> </li> 
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
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>形式</strong> </p> <p>次の可能な値を追加しました。</p> 
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

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。 これらの質問は通常、Portfolio管理者が決定し、その回答によって、管理者はプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。

スコアカードに関する質問の詳細は、「 [スコアカードの作成](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">可能な値 RICH を追加しました（書式付きテキストフィールド） </p> <p style="font-weight: normal;">詳しくは、 <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Adobe Workfront API のリッチテキストフィールド</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### タスク {#task}

Task オブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>このフィールドが追加され、タスクの完了に 1 日あたりの作業量が小、中、大のどれになるかを表します。 次の値を指定できます。</p> 
      <ul> 
       <li> <p>1 （小）</p> </li> 
       <li> <p>2 （中）</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>Workfrontの作業量について詳しくは、 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> <p>これらの操作では、引数のステータスが追加され、新しい [ 開始 ] ボタン機能をサポートするようになりました。この機能は、ユーザーがボタンをクリックして、項目の作業を開始したことを示す作業項目のステータスを変更します。</p> <p>詳しくは、 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業対象」ボタンを「開始」ボタンに置き換えます</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### チーム {#team}

Team オブジェクトは、作業項目に割り当てることができるユーザーの集まりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> <p>チームリソースに次のフィールドが追加されました。</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>このフィールドは、完了したカードがかんばんボードに残る日数を表します。</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>このフィールドは、チームをグループに関連付けます。 これにより、チームがグループの一部として識別され、グループ管理者がチームを管理できるようになります。</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>チームの [ 作業 ] ボタンが [ 開始 ] ボタンとして設定されているかどうかを示すブール型パラメータです。 チームのメンバーが [ 開始 ] ボタンをクリックして作業項目の作業を開始すると、その項目のステータスが [ 新規 ] から [ チーム設定 ] に設定されたステータスに変わります。</p> </li> 
     <li> <p>次のフィールドでは、個々の作業項目の「開始」ボタンに対してカスタムステータスを指定できます。</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatus</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatus</strong> </p> <p><strong>workOnItTaskStatus</strong> </p> </li> 
      </ul> <p>「開始」ボタンについて詳しくは、 <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業対象」ボタンを「開始」ボタンに置き換えます</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">参照フィールド</td> 
   <td> <p>チームリソースに次のフィールドが追加されました：</p> 
    <ul> 
     <li> <p><strong>グループ</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

TemplateTask オブジェクトは、Template に含まれる Task を表します。 テンプレートタスクは、テンプレートが使用されるプロジェクト内のタスクになります。

テンプレートタスクの詳細については、 [テンプレートタスクの編集](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>このフィールドが追加され、タスクの完了に 1 日あたりの作業量が小、中、大のどれになるかを表します。 次の値を指定できます。</p> 
      <ul> 
       <li> <p>1 （小）</p> </li> 
       <li> <p>2 （中）</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>Workfrontの作業量について詳しくは、 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### タイムシート {#timesheet}

Timesheet オブジェクトは、Tasks、Projects、および Overhead Hour Types の実績作業時間をユーザーが入力できる仮想タイムカードを表します。

タイムシートの詳細については、 [タイムシートの概要](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">コアフィールド</td> 
   <td> <p>次のフィールドは、タイムシートリソースから削除されました：</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 更新

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>次の可能な値が追加されました。</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">イニシアチブの詳細については、 <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">シナリオプランナーのイニシアチブの概要</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ユーザー {#user}

User オブジェクトは、Workfrontにログインしてシステムとやり取りできるアカウントを持つ人物を表します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> <p>ユーザーリソースに次のフィールドが追加されました。</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>ユーザーが非アクティブ化された日時を表します。</p> <p>非アクティブなユーザーについて詳しくは、 <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーを非アクティブ化または再アクティブ化する</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>このフィールドには、Workfront目標へのユーザーのアクセス権が表示されます。 次の値を指定できます。</p> 
      <ul> 
       <li> <p>アクセスなし</p> </li> 
       <li> <p>ビュー</p> </li> 
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
       <li> <p>ids （文字列）</p> </li> 
       <li> <p>objCode （文字列）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 作業  {#work}

Work オブジェクトは、Task と OpTask の両方が継承する共通のインターフェイスで、2 つの間で共通のコードを共有します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>順序は、アジャイルバックログ上のタスクまたはストーリーの位置を示します。</p> <p>このフィールドは、次のフラグを削除しました。</p> 
      <ul> 
       <li> <p>動的、</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>このフィールドには、次のフラグが追加されました。</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>動的、</p> </li> 
       <li> <p>読み取り専用</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>このフィールドが追加され、タスクの完了に 1 日あたりの作業量が小、中、大のどれになるかを表します。 次の値を指定できます。</p> 
      <ul> 
       <li> <p>1 （小）</p> </li> 
       <li> <p>2 （中）</p> </li> 
       <li> <p>3 （大）</p> </li> 
      </ul> <p>Workfrontの作業量について詳しくは、 <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>.</p> </li> 
    </ul> <p style="font-weight: normal;">  </p> </td> 
  </tr> 
 </tbody> 
</table>
