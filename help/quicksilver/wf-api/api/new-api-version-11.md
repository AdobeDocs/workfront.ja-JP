---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 11 の新機能
description: Adobe Workfront API に、レポートのリソースとして ReportableBudgedHour が追加されました。 この機能は、BudgetedHour にない参照フィールド、コアフィールド、および既定のフィールドを備えています。
author: Becky
feature: Workfront API
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 2%

---

# API バージョン 11 の新機能

* [追加されたリソース](#added-resources)
* [削除されたリソース](#removed-resources)
* [変更されたリソース](#modified-resources)

## 追加されたリソース {#added-resources}

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReportableBudgetedHour](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

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
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accessorID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">アクセサ</li> 
     <li style="font-weight: bold;">顧客</li> 
     <li style="font-weight: bold;">ユーザー  </li> 
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

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

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
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">顧客  </li> 
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

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

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
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">顧客  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
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

### ReportableBudgetedHour {#reportablebudgetedhour}

Adobe Workfront API に、レポートのリソースとして ReportableBudgedHour が追加されました。 この機能は、BudgetedHour にない参照フィールド、コアフィールド、および既定のフィールドを備えています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>「配賦日」は、リソース・プランナに時間を予算設定した週の最初の日（日曜日）です。</p> </li> 
     <li> <p style="font-weight: bold;">budgetedHours </p> <p>予算時間とは、リソースがプロジェクトで完了する必要のある作業に対するリソースマネージャの予算時間です</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>特定のレポート可能な予算時間オブジェクトに割り当てられた一意のWorkfront ID。</p> </li> 
     <li style="font-weight: bold;">plannedBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>特定のプロジェクトに割り当てられた一意のWorkfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>特定のジョブの役割に割り当てられた一意のWorkfront ID。</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>特定のユーザーに割り当てられた一意のWorkfront ID。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">プロジェクト</p> <p>ReportableBudgetedHour が関連付けられているプロジェクトです。</p> </li> 
     <li> <p style="font-weight: bold;">役割</p> <p>ReportableBudgetedHour が関連付けられているジョブの役割です。</p> </li> 
     <li> <p style="font-weight: bold;">ユーザー</p> <p>ReportableBudgetedHour が関連付けられているユーザー。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コアフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">カウント</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">レポート </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 削除されたリソース {#removed-resources}

API v11 で削除されたリソースはありません。

## 変更されたリソース {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">承認</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">割り当て</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">BaselineTask</a> </li> 
     <li><a href="#category" class="MCXref xref">カテゴリ</a> </li> 
     <li><a href="#company" class="MCXref xref">会社</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">顧客</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">ドキュメント</a> </li> 
     <li><a href="#iteration" class="MCXref xref">反復</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">レイアウトテンプレート</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilestonePath</a> </li> 
     <li><a href="#note" class="MCXref xref">メモ</a> </li> 
     <li><a href="#optask" class="MCXref xref">Opタスク</a> </li> 
     <li><a href="#parameter" class="MCXref xref">パラメーター</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">ポートフォリオ</a> </li> 
     <li><a href="#program" class="MCXref xref">プログラム</a> </li> 
     <li><a href="#project" class="MCXref xref">プロジェクト</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">ReservedTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">危険</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">タスク</a> </li> 
     <li><a href="#team" class="MCXref xref">チーム</a> </li> 
     <li><a href="#template" class="MCXref xref">テンプレート</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">タイムシート</a> </li> 
     <li><a href="#update" class="MCXref xref"></a>を更新 </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">作業 </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions オブジェクトは、一連のアクセス許可を表します。 その後、この一連の権限をアクセスレベルに関連付けることができます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> <p>次のフィールドに、BUDGETING_INFORMATION という値が追加されました。 これにより、プランナーの優先度と予算時間を編集する権限を持つユーザーが許可されます。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
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
     <li> <p style="font-weight: bold;">アクション</p> <p>BUDGETING_INFORMATION の値を追加しました。 これにより、プランナーの優先度と予算時間を編集する権限を持つユーザーが許可されます。  </p> </li> 
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
   <td> <p>次のフィールドに、BUDGETING_INFORMATION という値が追加されました。 これにより、プランナーの優先度と予算時間を編集する権限を持つユーザーが許可されます。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
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
   <td colspan="2">ダイレクトフィールド<p style="font-weight: normal;">次のフィールドにはバリデータ AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR が追加されました。 これらのバリデータは、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないことを指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC（完了時の推定）の計算に透明性を持たせるため、パブリック API に以下のフィールドを追加しました。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP (Budgeted Cost of Work Performed) は、達成額とも呼ばれ、この指標の計算時に実際に完了したタスクの量の予算コストを表すプロジェクトの実績指標です。 タスクの場合、[BCWP =実績達成率 x タスク予算 ]。 プロジェクトの場合、BCWP = SUM（すべての親タスクと個々のタスクの BCWP 値）</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS (Budgeted Cost of Work Scheduled) は、計画値とも呼ばれ、この指標の計算時に完了する必要のあるタスクの量の予算コストを表すプロジェクトのパフォーマンス指標です。 タスクの場合、BCWS =計画完了率 x タスク予算。 プロジェクトの場合、BCWS = SUM（すべての親タスクと個々のタスクの BCWS 値）</p></li>
    </ul><p style="font-weight: normal;">次のフィールドに、ET の値が追加されました。 この値は、週末や休日を問わず月を指す経過時間（月）の単位を表します。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">以下のフィールドには CURRENCY というフラグが追加されています。</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">次のフィールドが Approval オブジェクトから削除されました。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">次のフィールドが Approval オブジェクトに追加されました。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Approval オブジェクトから削除されました  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Approval オブジェクトに追加されました。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

ApprovalPath オブジェクトは、承認プロセス内のブランチです。 承認パスは、承認プロセスが関連付けられているオブジェクトのステータスに基づきます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">可能な値 ET を追加しました。 この値は、週末や休日を問わず月を指す経過時間（月）の単位を表します。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

ApprovalProcess オブジェクトは、プロジェクト、タスク、またはイシューに関連付けることができる複数手順の承認です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">このフィールドは追加されました。オブジェクトがアクティブの場合は値が true、そうでない場合は false のブール型パラメーターです。 [ アクティブ ] に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトにアタッチできます。 [ アクティブ ] に設定されていないオブジェクトは、他のオブジェクトにアタッチするドロップダウンメニューや先行入力フィールドには表示されません。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 割り当て {#assignment}

割り当てオブジェクトは、作業項目と、作業項目に割り当てられているユーザー、チーム、またはグループとの間の接続を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">可能な値 ET を追加しました。 この値は、週末や休日を問わず月を指す経過時間（月）の単位を表します。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BaselineTask {#baselinetask}

ベースラインは、特定の時点でのプロジェクトのパフォーマンスがどのように表示されたかを示すスナップショットです。 主要な日付、進捗状況、コスト、売上高など、プロジェクトに関する主要な情報が格納されます。 基準計画を作成すると、その基準計画の基準計画タスクに関するタスク情報も取り込まれます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">可能な値 ET を追加しました。 この値は、週末や休日を問わず月を指す経過時間（月）の単位を表します。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### カテゴリ {#category}

Category オブジェクトはカスタムフォームです。 このオブジェクトに関するレポートを作成し、他のオブジェクトレポートにも表示できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">このフィールドは追加されました。オブジェクトがアクティブの場合は値が true、そうでない場合は false のブール型パラメーターです。 [ アクティブ ] に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトにアタッチできます。 [ アクティブ ] に設定されていないオブジェクトは、他のオブジェクトにアタッチするドロップダウンメニューや先行入力フィールドには表示されません。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 会社 {#company}

Company オブジェクトは、人々の集まりで構成される組織を表します。 会社は、ユーザーまたはプロジェクトに関連付けられます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">このフィールドは追加されました。オブジェクトがアクティブの場合は値が true、そうでない場合は false のブール型パラメーターです。 [ アクティブ ] に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトにアタッチできます。 [ アクティブ ] に設定されていないオブジェクトは、他のオブジェクトにアタッチするドロップダウンメニューや先行入力フィールドには表示されません。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>アクション</td> 
   <td> <p style="font-weight: normal;">次のアクションが CustomEnum オブジェクトに追加されました</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>クエリ</td> 
   <td> <p>CustomEnum オブジェクトに次のクエリが追加されました</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
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
  <tr data-mc-conditions=""> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">次の値を追加しました。 </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ （プロジェクト条件）</li> 
       <li style="font-weight: normal;">CONDITION_TASK （タスク条件）</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK （発行条件）  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>アクション</td> 
   <td> <p style="font-weight: normal;">次のアクションが Customer オブジェクトに追加されました</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

CustomerPreferences オブジェクトは、Workfrontのインスタンスに対して顧客が設定した一連の環境設定を表します。

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
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">次の値を追加しました。</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy （パスワードの複雑さの要件）</li> 
       <li style="font-weight: normal;"> password:password.minimumLength （最小パスワード長）</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout（モバイルセッションタイムアウト）</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (User Time Off)</li> 
       <li style="font-weight: normal;">タイムシート：default.timesheet.manualrole （手動制御ロール）</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole (config.proofhq.defaultnonrecipientguestrole)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>アクション</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">追加済み</p> </li> 
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
   <td> <p>次のアクションが Document オブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 反復 {#iteration}

Iteration オブジェクトは、1 つのアジャイルイテレーションを表します。 繰り返しとは、アジャイルストーリーの計画と完了に使用される、個別の期間です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> <p>次のフィールドが Iteration オブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">完了したポイント</li> 
     <li style="font-weight: bold;">totalPoints  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### レイアウトテンプレート {#layout-template}

Layout Template オブジェクトは、メインメニュー、ナビゲーションパネル、ホーム領域など、レイアウト要素の特定の配置を表します。 レイアウトテンプレートは、ユーザー、チーム、グループまたはジョブの役割に割り当てることができます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">このフィールドは追加され、レイアウトテンプレートが作業用リストとカレンダーに期限のタイムスタンプを表示するように設定されている場合は true、タイムスタンプを非表示にするように設定されている場合は false の値を持つブール型パラメータです。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### MilestonePath {#milestonepath}

マイルストーンは、タスクがプロジェクトの重要なポイントであることを示すマーカーです。 通常は、プロジェクトのフェーズの完了や、重要なアクティビティのセットなど、重要なイベントを示すために使用されます。 MilestonePath オブジェクトは、マイルストーンの集まりです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">このフィールドは追加されました。オブジェクトがアクティブの場合は値が true、そうでない場合は false のブール型パラメーターです。 [ アクティブ ] に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトにアタッチできます。 [ アクティブ ] に設定されていないオブジェクトは、他のオブジェクトにアタッチするドロップダウンメニューや先行入力フィールドには表示されません。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### メモ {#note}

Note オブジェクトは、Workfrontオブジェクトに対しておこなわれるコメントまたは更新です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> <p>次のフィールドが Note オブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>いいね！</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Opタスク {#optask}

OpTask オブジェクトは、一般にイシューと呼ばれます。 問題とは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業項目です。 問題は、ヘルプデスクへのリクエストでもかまいません。 変更管理、要求、バグも問題です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">ダイレクトフィールド<p style="font-weight: normal;">次のフィールドにはバリデータ AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR が追加されました。 これらの値は、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないことを指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">OpTask に次のフィールドが追加されました。</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">かんばんボードオブジェクトの一意のWorkfront ID。</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">「完了率」は、発行の完了済金額をパーセンテージで返すパラメータです。</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">作業  </li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>フィールドの検索</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>作業</p> <p style="font-weight: normal;">削除済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>アクション</td> 
   <td> <p>OpTask オブジェクトに次のアクションが追加されました</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### パラメーター {#parameter}

Parameter オブジェクトは、カスタムフィールドです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">可能な値 TYAH (Typeahead) を追加しました。</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">このフィールドが追加され、参照先のオブジェクトのオブジェクトコードを参照します。 すべてのオブジェクトのオブジェクトコードは、 <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラ</a>.  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ポートフォリオ {#portfolio}

Portfolioオブジェクトとは、同じリソース、通常は費用や担当者を競い合って完了するプロジェクトの集まりです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>説明</p> <p style="font-weight: normal;">バリデーターMAX_LENGTH が追加されました。このバリデーターは、説明の長さが 4,000 文字以下であることを指定しています。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### プログラム {#program}

Program オブジェクトは、ポートフォリオ内のサブセットで、類似したプロジェクトを 1 つにグループ化できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>説明</p> <p style="font-weight: normal;">バリデーターMAX_LENGTH が追加されました。このバリデーターは、説明の長さが 4,000 文字以下であることを指定しています。</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">このフィールドは追加されました。オブジェクトがアクティブの場合は値が true、そうでない場合は false のブール型パラメーターです。 [ アクティブ ] に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトにアタッチできます。 [ アクティブ ] に設定されていないオブジェクトは、他のオブジェクトにアタッチするドロップダウンメニューや先行入力フィールドには表示されません。  </p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">バリデーターMAX_LENGTH が追加されました。このバリデーターは名前の長さを 255 文字以下にするように指定しています。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### プロジェクト {#project}

プロジェクトはWorkfront内の作業項目で、Workfrontが作業をおこなう際に役立つ主要な構成要素です。 Project オブジェクトは、共通の特定の目標を持つタスクのグループを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">ダイレクトフィールド<p style="font-weight: normal;">次のフィールドにはバリデータ AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR が追加されました。 これらの値は、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないことを指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC（完了時の推定）の計算に透明性を持たせるため、パブリック API に以下のフィールドを追加しました。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP (Budgeted Cost of Work Performed) は、達成額とも呼ばれ、この指標の計算時に実際に完了したタスクの量の予算コストを表すプロジェクトの実績指標です。 タスクの場合、[BCWP =実績達成率 x タスク予算 ]。 プロジェクトの場合、BCWP = SUM（すべての親タスクと個々のタスクの BCWP 値）</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS (Budgeted Cost of Work Scheduled) は、計画値とも呼ばれ、この指標の計算時に完了する必要のあるタスクの量の予算コストを表すプロジェクトのパフォーマンス指標です。 タスクの場合、BCWS =計画完了率 x タスク予算。 プロジェクトの場合、BCWS = SUM（すべての親タスクと個々のタスクの BCWS 値）</p></li>
    </ul><p style="font-weight: normal;">以下のフィールドには CURRENCY というフラグが追加されています。</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">次のフィールドは、Project オブジェクトから削除されました。</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ProofApproval {#proofapproval}

ProofApproval オブジェクトは、配達確認に直接接続される承認を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isWaitingDecision</p> <p style="font-weight: normal;">このフィールドが追加され、配達確認が判定を待機している場合は値が true、待機していない場合は false のブール値パラメーターです。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef オブジェクトは、Queue を表します。Queue は、ヘルプデスク領域に公開され、ユーザーが問題を送信できるようにするプロジェクトです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> <p>次のフィールドに、BUDGETING_INFORMATION という値が追加されました。 これにより、プランナーの優先度と予算時間を編集する権限を持つユーザーが許可されます。</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

ReservedTime オブジェクトは、ユーザーの個人時間に指定された日数を表し、ユーザーが作業に使用できないことを示します。

ReservedTime リソースにより、フラグ REPORTABLE が追加されました。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> <p>以下のフィールドは、NOT_GROUPABLE フラグを削除しました。</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>次のフィールドが ReservedTime オブジェクトから削除されました。</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>タスク</p> <p style="font-weight: normal;">削除済み  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>編集</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

ResourcePlannerFilter オブジェクトは、リソースプランナーに表示する項目を決定する一連のルールです。

ResourcePlannerFilter リソースにより、SHARABLE というフラグが追加されました。 オブジェクトに対する他の変更はありませんでした。

### 危険 {#risk}

Risk オブジェクトは、プロジェクトが予定通りに完了しない、または予算内で終了しない可能性のあるイベントを表します。 計画段階では、作業の承認前に、潜在的な障害物を特定するためのリスクがプロジェクトに追加されます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> <p>次のフィールドがリスクオブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteriedByID</p> <p style="font-weight: normal;">オブジェクトを最初に作成したユーザーの ID。</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>ユーザーがWorkfrontでオブジェクトを送信した日付。</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Last Update Date パラメーターは、最終更新がオブジェクトに対して行われた日付を返します。</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Last Updated By ID は、オブジェクトを更新した最後のユーザーのユーザー ID を返すパラメーターです。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> <p style="font-weight: normal;">次の参照フィールドが RIsk オブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy  </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

ScheduledReport オブジェクトは、配信のスケジュールを設定したレポートを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">次の可能な値が追加されました。</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。 これらの質問は通常、Portfolio管理者が決定し、その回答によって、管理者はプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">可能な値 TYAH (Typeahead) を追加しました。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### タスク {#task}

Task オブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">ダイレクトフィールド<p style="font-weight: normal;">次のフィールドにはバリデータ AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR が追加されました。 これらの値は、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないことを指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC（完了時の推定）の計算に透明性を持たせるため、パブリック API に以下のフィールドを追加しました。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP (Budgeted Cost of Work Performed) は、達成額とも呼ばれ、この指標の計算時に実際に完了したタスクの量の予算コストを表すプロジェクトの実績指標です。 タスクの場合、[BCWP =実績達成率 x タスク予算 ]。 プロジェクトの場合、BCWP = SUM（すべての親タスクと個々のタスクの BCWP 値）</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS (Budgeted Cost of Work Scheduled) は、計画値とも呼ばれ、この指標の計算時に完了する必要のあるタスクの量の予算コストを表すプロジェクトのパフォーマンス指標です。 タスクの場合、BCWS =計画完了率 x タスク予算。 プロジェクトの場合、BCWS = SUM（すべての親タスクと個々のタスクの BCWS 値）</p></li>
    </ul><p style="font-weight: normal;">次のフィールドに、ET の値が追加されました。 この値は、週末や休日を問わず月を指す経過時間（月）の単位を表します。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">次のフィールドが Task オブジェクトから削除されました。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">次のフィールドが Task オブジェクトに追加されました。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">削除済み  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### チーム {#team}

Team オブジェクトは、作業項目に割り当てることができるユーザーの集まりです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">このフィールドは Team オブジェクトに追加されました。 「アジャイル推定タイプ」は、ストーリーの作業負荷の推定方法を決定します。 推定時間数が時間単位の場合は、ストーリーに追加される予定時間数です。 ポイント数が推定される場合、各ポイントでは、ポイントの設定に基づいて計画時間数がストーリーに追加されます（デフォルトは 8 時間）。 「アジャイル推定」タイプで使用できる値は次のとおりです。</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS （ストーリーポイント）</li> 
       <li style="font-weight: normal;">時間（時間）</li> 
       <li style="font-weight: normal;">LEGACY_POINTS ( 時間（ポイント）)  </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### テンプレート {#template}

Template オブジェクトは、プロジェクトのパターンを表します。 プロジェクトは、時間を節約するために、テンプレートから作成できます。 テンプレートにはチームとタスクが含まれ、テンプレートを使用するとプロジェクトにコピーされます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">このフィールドは追加されました。オブジェクトがアクティブの場合は値が true、そうでない場合は false のブール型パラメーターです。 [ アクティブ ] に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトにアタッチできます。 [ アクティブ ] に設定されていないオブジェクトは、他のオブジェクトにアタッチするドロップダウンメニューや先行入力フィールドには表示されません。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateAssignment {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">可能な値 ET を追加しました。 この値は、週末や休日を問わず月を指す経過時間（月）の単位を表します。  </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

TemplateTask オブジェクトは、Template に含まれる Task を表します。 テンプレートタスクは、テンプレートが使用されるプロジェクト内のタスクになります。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> <p style="font-weight: normal;">次のフィールドに、ET の値が追加されました。 この値は、週末や休日を問わず月を指す経過時間（月）の単位を表します。</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriority</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### タイムシート {#timesheet}

Timesheet オブジェクトは、Tasks、Projects、および Overhead Hour Types の実績作業時間をユーザーが入力できる仮想タイムカードを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>コアフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">削除済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 更新 {#update}

Workfrontの作業項目を更新して、ユーザーに現在のステータスを知らせることができます。 Update オブジェクトは、これらの更新の 1 つを表します。 更新は、ユーザーが入力するか、Workfrontシステムが作成します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">可能な値 referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata) を追加しました。  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>クエリ</td> 
   <td> <p style="font-weight: normal;">次のクエリが Update オブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>アクション</td> 
   <td> <p style="font-weight: normal;">次のアクションが User オブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>クエリ</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>アクション</td> 
   <td> <p style="font-weight: normal;">次のアクションが User オブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">acknowledgeMyNotifications</li> 
     <li style="font-weight: bold;">unacknowledAllObjectsTypeCount  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>クエリ</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">追加済み</p> </li> 
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
   <td colspan="2">ダイレクトフィールド<p style="font-weight: normal;">次のフィールドにはバリデータ AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR が追加されました。 これらの値は、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないことを指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC（完了時の推定）の計算に透明性を持たせるため、パブリック API に以下のフィールドを追加しました。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP (Budgeted Cost of Work Performed) は、達成額とも呼ばれ、この指標の計算時に実際に完了したタスクの量の予算コストを表すプロジェクトの実績指標です。 タスクの場合、[BCWP =実績達成率 x タスク予算 ]。 プロジェクトの場合、BCWP = SUM（すべての親タスクと個々のタスクの BCWP 値）</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS (Budgeted Cost of Work Scheduled) は、計画値とも呼ばれ、この指標の計算時に完了する必要のあるタスクの量の予算コストを表すプロジェクトのパフォーマンス指標です。 タスクの場合、BCWS =計画完了率 x タスク予算。 プロジェクトの場合、BCWS = SUM（すべての親タスクと個々のタスクの BCWS 値）</p></li>
    </ul><p style="font-weight: normal;">次のフィールドに、ET の値が追加されました。 この値は、週末や休日を問わず月を指す経過時間（月）の単位を表します。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">次のフィールドは Work オブジェクトから削除されました。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">次のフィールドが Work オブジェクトに追加されました。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">削除済み  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
