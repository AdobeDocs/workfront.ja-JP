---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 11 の新機能
description: Adobe Workfront API に、レポート用のリソースとして ReportableBudgedHour が追加されました。BudgetedHour にない参照フィールド、コアフィールドおよびデフォルトフィールドを特長として備えています。
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: ht
source-wordcount: '3573'
ht-degree: 100%

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
   <td>直接フィールド</td> 
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
     <li style="font-weight: bold;">accessor</li> 
     <li style="font-weight: bold;">顧客</li> 
     <li style="font-weight: bold;">user</li> 
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
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode</li> 
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
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs</li> 
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

Adobe Workfront API に、レポート用のリソースとして ReportableBudgedHour が追加されました。BudgetedHour にない参照フィールド、コアフィールドおよびデフォルトフィールドを特長として備えています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>配分日は、リソースプランナーで時間数を予算計上した週の最初の日（日曜日）です。</p> </li> 
     <li> <p style="font-weight: bold;">budgetedHours </p> <p>予算計上時間数は、プロジェクトでリソースが達成すべき作業に対して、リソースマネージャーが予算計上した時間数です</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>特定のレポート可能な予算計上時間数オブジェクトに割り当てられた、一意の Workfront ID です。</p> </li> 
     <li style="font-weight: bold;">plannedBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>特定のプロジェクトに割り当てられた一意の Workfront ID です。</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>特定の担当業務に割り当てられた一意の Workfront ID です。</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>特定のユーザーに割り当てられた一意の Workfront ID です。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">プロジェクト</p> <p>ReportableBudgetedHour が関連付けられているプロジェクトです。</p> </li> 
     <li> <p style="font-weight: bold;">役割</p> <p>ReportableBudgetedHour が関連付けられている担当業務です。</p> </li> 
     <li> <p style="font-weight: bold;">ユーザー</p> <p>ReportableBudgetedHour が関連付けられているユーザーです。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コアフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">名前</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">名前</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">COUNT</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">REPORT </li> 
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
     <li><a href="#iteration" class="MCXref xref">イテレーション</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">レイアウトテンプレート</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilestonePath</a> </li> 
     <li><a href="#note" class="MCXref xref">メモ</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
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
     <li><a href="#risk" class="MCXref xref">リスク</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">タスク</a> </li> 
     <li><a href="#team" class="MCXref xref">チーム</a> </li> 
     <li><a href="#template" class="MCXref xref">テンプレート</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">タイムシート</a> </li> 
     <li><a href="#update" class="MCXref xref">更新</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">作業 </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

 

### AccessLevelPermissions {#accesslevelpermissions}

AccessLevelPermissions オブジェクトは、一連のアクセス権限を表します。この一連の権限は、アクセスレベルに関連付けることができます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> <p>次のフィールドに可能な値 BUDGETING_INFORMATION が追加されました。これにより、権限を持つユーザーは、プランナーで優先度と予算計上時間数を編集することができます。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
    </ul> </td> 
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
     <li> <p style="font-weight: bold;">アクション</p> <p>可能な値 BUDGETING_INFORMATION を追加しました。これにより、権限を持つユーザーは、プランナーで優先度と予算計上時間数を編集することができます。 </p> </li> 
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
   <td> <p>次のフィールドに可能な値 BUDGETING_INFORMATION が追加されました。これにより、権限を持つユーザーは、プランナーで優先度と予算計上時間数を編集することができます。</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions  </li> 
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
   <td colspan="2">直接フィールド<p style="font-weight: normal;">次のフィールドには、AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR というバリデーターが追加されました。これらのバリデーターは、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないことを指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC（完成時総コスト見積り）の計算に透明性を持たせるため、パブリック API に以下のフィールドを追加しました。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP（実行された作業の予算計上コスト）は、出来高とも呼ばれ、この指標の計算時点で実際に完了したタスク量の予算計上コストを表す、プロジェクトのパフォーマンス指標です。タスクの場合、BCWP = 実績完了率 x タスク予算となります。プロジェクトの場合、BCWP = SUM(すべての親タスクと個々のタスクの BCWP 値) となります。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS（予定された作業の予算計上コスト）は、予定値とも呼ばれ、この指標の計算時点で完了しているべきタスク量の予算計上コストを表す、プロジェクトのパフォーマンス指標です。タスクの場合、BCWS = 予定完了率 x タスク予算となります。プロジェクトの場合、BCWS = SUM(すべての親タスクと個々のタスクの BCWS 値) となります。</p></li>
    </ul><p style="font-weight: normal;">次のフィールドに可能な値 ET が追加されました。この値は、週末や休日を考慮しない、経過月数の単位を表します。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">次のフィールドに、CURRENCY というフラグが追加されました。</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">次のフィールドが承認オブジェクトから削除されました。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">次のフィールドが承認オブジェクトに追加されました。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">承認オブジェクトから削除されました</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">承認オブジェクトに追加されました。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

ApprovalPath オブジェクトは、承認プロセス内の分岐です。承認パスは、承認プロセスが関連付けられているオブジェクトのステータスに基づいています。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">可能な値 ET を追加しました。この値は、週末や休日を考慮しない、経過月数の単位を表します。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

ApprovalProcess オブジェクトは、プロジェクト、タスク、イシューに関連付けることができる、複数段階の承認です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">この追加されたフィールドは、オブジェクトがアクティブの場合は値が true、そうでない場合は false の値を持つブーリアン型パラメーターです。「アクティブ」に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトに添付できます。「アクティブ」に設定されていないオブジェクトは、ドロップダウンメニューや先行入力フィールドには表示されず、他のオブジェクトにアタッチできません。 </p> </li> 
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

割り当てオブジェクトは、作業アイテムと、作業アイテムに割り当てられたユーザー、チーム、グループとの間の接続を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">可能な値 ET を追加しました。この値は、週末や休日を考慮しない、経過月数の単位を表します。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BaselineTask {#baselinetask}

ベースラインは、特定の時点でのプロジェクトのパフォーマンスを示すスナップショットです。主要な日付、進捗状況、コスト、売上高など、プロジェクトに関する主要な情報が保存されています。ベースラインを作成すると、そのベースラインのベースラインタスクに関するタスク情報も取り込まれます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">可能な値 ET を追加しました。この値は、週末や休日を考慮しない、経過月数の単位を表します。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### カテゴリ {#category}

カテゴリオブジェクトはカスタムフォームです。このオブジェクトに関するレポートを作成し、他のオブジェクトレポートにも表示できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">この追加されたフィールドは、オブジェクトがアクティブの場合は値が true、そうでない場合は false の値を持つブーリアン型パラメーターです。「アクティブ」に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトに添付できます。「アクティブ」に設定されていないオブジェクトは、ドロップダウンメニューや先行入力フィールドには表示されず、他のオブジェクトにアタッチできません。 </p> </li> 
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

会社オブジェクトは、人物の集まりで構成される組織を表します。会社は、ユーザーまたはプロジェクトに関連付けられます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">この追加されたフィールドは、オブジェクトがアクティブの場合は値が true、そうでない場合は false の値を持つブーリアン型パラメーターです。「アクティブ」に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトに添付できます。「アクティブ」に設定されていないオブジェクトは、ドロップダウンメニューや先行入力フィールドには表示されず、他のオブジェクトにアタッチできません。 </p> </li> 
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
   <td> <p>次のクエリが CustomEnum オブジェクトに追加されました</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
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
  <tr data-mc-conditions=""> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">次の値を追加しました。 </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ（プロジェクト状況）</li> 
       <li style="font-weight: normal;">CONDITION_TASK（タスク条件）</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK（イシュー条件）</li> 
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
   <td> <p style="font-weight: normal;">次のアクションが顧客オブジェクトに追加されました</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

CustomerPreferences オブジェクトは、Workfront のインスタンスに対して顧客が設定した一連の環境設定を表します。

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
     <li style="font-weight: bold;"> <p>名前</p> <p style="font-weight: normal;">次の値を追加しました。</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy（パスワードの複雑さの要件）</li> 
       <li style="font-weight: normal;"> password:password.minimumLength（最小パスワード長）</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout（モバイルセッションのタイムアウト値）</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff（ユーザーの休暇）</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.manualrole（手動制御役割）</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole（config.proofhq.defaultnonrecipientrole） </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole（config.proofhq.defaultnonrecipientguestrole）</li> 
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

Document オブジェクトは、ファイル（書かれた資料、画像、その他の形式の情報など）を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>アクション</td> 
   <td> <p>次のアクションがドキュメントオブジェクトに追加されました。</p> 
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

### イテレーション {#iteration}

イテレーションオブジェクトは、1 つのアジャイルイテレーションを表します。イテレーションとは、アジャイルストーリーの計画と完了に使用される、個別の期間です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> <p>次のフィールドがイテレーションオブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">pointsCompleted</li> 
     <li style="font-weight: bold;">totalPoints</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### レイアウトテンプレート {#layout-template}

レイアウトテンプレートオブジェクトは、メインメニュー、ナビゲーションパネル、ホームエリアなど、レイアウト要素の特定の配置を表します。レイアウトテンプレートは、ユーザー、チーム、グループ、担当業務に割り当てることができます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">この追加されたフィールドは、レイアウトテンプレートが作業用リストとカレンダーに期限のタイムスタンプを表示するように設定されている場合は true、タイムスタンプを非表示にするように設定されている場合は false の値を持つブーリアン型パラメーターです。 </p> </li> 
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

マイルストーンは、タスクがプロジェクトの重要なポイントであることを示すマーカーです。通常は、プロジェクトのフェーズの完了や、一連の重要なアクティビティなど、重要なイベントを示すために使用されます。MilestonePath オブジェクトは、マイルストーンの集まりです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">この追加されたフィールドは、オブジェクトがアクティブの場合は値が true、そうでない場合は false の値を持つブーリアン型パラメーターです。「アクティブ」に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトに添付できます。「アクティブ」に設定されていないオブジェクトは、ドロップダウンメニューや先行入力フィールドには表示されず、他のオブジェクトにアタッチできません。 </p> </li> 
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

メモオブジェクトは、Workfront オブジェクトに対するコメントまたは更新です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> <p>次のフィールドがメモオブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">proofID  </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>いいね</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

OpTask オブジェクトは、一般にイシューと呼ばれます。イシューは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業アイテムです。イシューは、ヘルプデスクへのリクエストである場合もあります。変更指示、リクエスト、バグもイシューです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接フィールド<p style="font-weight: normal;">次のフィールドには、AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR というバリデーターが追加されました。これらのバリデーターは、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないように指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">OpTask に次のフィールドが追加されました。</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">かんばんボードオブジェクトの一意の Workfront ID です。</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">完了率は、完了したイシューの量をパーセンテージで返すパラメーターです。</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">ワーク  </li>
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
     <li style="font-weight: bold;"> <p>ワーク</p> <p style="font-weight: normal;">削除されました</p> </li> 
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
   <td> <p>次のアクションが OpTask オブジェクトに追加されました</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### パラメーター {#parameter}

パラメーターオブジェクトは、カスタムフィールドです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">可能性のある値 TYAH（先行入力）を追加しました。</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">このフィールドが追加され、参照されるオブジェクトのオブジェクトコードを参照します。すべてのオブジェクトのオブジェクトコードは、<a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラー</a>で確認できます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ポートフォリオ {#portfolio}

ポートフォリオオブジェクトは、同じリソース（通常はプロジェクトを完了するための資金や人材）を競い合って完了するプロジェクトのコレクションです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>説明</p> <p style="font-weight: normal;">バリデーター MAX_LENGTH が追加されました。このバリデーターは、説明の長さが 4,000 文字以下にするように指定しています。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### プログラム {#program}

プログラムオブジェクトは、ポートフォリオ内のサブセットで、類似したプロジェクトを 1 つにグループ化できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>説明</p> <p style="font-weight: normal;">バリデーター MAX_LENGTH が追加されました。このバリデーターは、説明の長さが 4,000 文字以下にするように指定しています。</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">この追加されたフィールドは、オブジェクトがアクティブの場合は値が true、そうでない場合は false の値を持つブーリアン型パラメーターです。「アクティブ」に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトに添付できます。「アクティブ」に設定されていないオブジェクトは、ドロップダウンメニューや先行入力フィールドには表示されず、他のオブジェクトにアタッチできません。 </p> </li> 
     <li style="font-weight: bold;"> <p>名前 </p> <p style="font-weight: normal;">バリデーター MAX_LENGTH が追加されました。このバリデーターは名前の長さを 255 文字以下にするように指定します。 </p> </li> 
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

プロジェクトは Workfront 内の作業アイテムで、Workfront が人々の作業を支援するための主要な構築ブロックです。プロジェクトオブジェクトは、共通の特定の目標を持つタスクのグループを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接フィールド<p style="font-weight: normal;">次のフィールドには、AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR というバリデーターが追加されました。これらのバリデーターは、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないように指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC（完成時総コスト見積り）の計算に透明性を持たせるため、パブリック API に以下のフィールドを追加しました。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP（実行された作業の予算計上コスト）は、出来高とも呼ばれ、この指標の計算時点で実際に完了したタスク量の予算計上コストを表す、プロジェクトのパフォーマンス指標です。タスクの場合、BCWP = 実績完了率 x タスク予算となります。プロジェクトの場合、BCWP = SUM(すべての親タスクと個々のタスクの BCWP 値) となります。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS（予定された作業の予算計上コスト）は、予定値とも呼ばれ、この指標の計算時点で完了しているべきタスク量の予算計上コストを表す、プロジェクトのパフォーマンス指標です。タスクの場合、BCWS = 予定完了率 x タスク予算となります。プロジェクトの場合、BCWS = SUM(すべての親タスクと個々のタスクの BCWS 値) となります。</p></li>
    </ul><p style="font-weight: normal;">次のフィールドに、CURRENCY というフラグが追加されました。</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">次のフィールドは、プロジェクトオブジェクトから削除されました。</p>
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

ProofApproval オブジェクトは、プルーフに直接接続される承認を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isWaitingDecision</p> <p style="font-weight: normal;">この追加されたフィールドは、プルーフが判定を待機している場合は true、待機していない場合は false の値を持つブーリアン型パラメーターです。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

QueueDef オブジェクトは、キューを表します。キューは、ユーザーがイシューを送信できるようにヘルプデスクエリアに公開されたプロジェクトです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> <p>次のフィールドに可能な値 BUDGETING_INFORMATION が追加されました。これにより、権限を持つユーザーは、プランナーで優先度と予算計上時間数を編集することができます。</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul>  </td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

ReservedTime オブジェクトは、ユーザーの個人時間に指定された日数を表し、ユーザーが作業に使用できないことを示します。

ReservedTime リソースにより、REPORTABLE というフラグが追加されました。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> <p>以下のフィールドから、NOT_GROUPABLE というフラグを削除しました。</p> 
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
     <li style="font-weight: bold;"> <p>タスク</p> <p style="font-weight: normal;">削除されました。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>操作</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>EDIT</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

ResourcePlannerFilter オブジェクトは、リソースプランナーに表示する項目を決定する一連のルールです。

ResourcePlannerFilter リソースにより、SHARABLE というフラグが追加されました。オブジェクトに対する他の変更はありませんでした。

### リスク {#risk}

リスクオブジェクトは、プロジェクトが時間通りに完了しない、または予算内で終了しない可能性のあるイベントを表します。計画段階では、すべての作業の承認前に、潜在的な障害物を特定するためのリスクがプロジェクトに追加されます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> <p>次のフィールドがリスクオブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">オブジェクトを最初に作成したユーザーの ID。</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>ユーザーが Workfront でオブジェクトを送信した日付。</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>Last Update Date パラメーターは、最終更新がオブジェクトに対して行われた日付を返します。</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Last Updated By ID は、オブジェクトを更新した最後のユーザーのユーザー ID を返すパラメーターです。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> <p style="font-weight: normal;">次の参照フィールドがリスクオブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy </li> 
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
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">追加された可能な値は次のとおりです。</p> 
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

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。これらの質問は通常、ポートフォリオマネージャーが決定し、その回答によって、マネージャーはプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">可能な値 TYAH（Typeahead）を追加しました。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### タスク {#task}

タスクオブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接フィールド<p style="font-weight: normal;">次のフィールドには、AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR というバリデーターが追加されました。これらのバリデーターは、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないように指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC（完成時総コスト見積り）の計算に透明性を持たせるため、パブリック API に以下のフィールドを追加しました。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP（実行された作業の予算計上コスト）は、出来高とも呼ばれ、この指標の計算時点で実際に完了したタスク量の予算計上コストを表す、プロジェクトのパフォーマンス指標です。タスクの場合、BCWP = 実績完了率 x タスク予算となります。プロジェクトの場合、BCWP = SUM(すべての親タスクと個々のタスクの BCWP 値) となります。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS（予定された作業の予算計上コスト）は、予定値とも呼ばれ、この指標の計算時点で完了しているべきタスク量の予算計上コストを表す、プロジェクトのパフォーマンス指標です。タスクの場合、BCWS = 予定完了率 x タスク予算となります。プロジェクトの場合、BCWS = SUM(すべての親タスクと個々のタスクの BCWS 値) となります。</p></li>
    </ul><p style="font-weight: normal;">次のフィールドに可能な値 ET が追加されました。この値は、週末や休日を考慮しない、経過月数の単位を表します。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">次のフィールドがタスクオブジェクトから削除されました。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">次のフィールドがタスクオブジェクトに追加されました。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">削除されました。</p> </li> 
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

チームオブジェクトは、作業アイテムに割り当てることができるユーザーの集まりです。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">このフィールドはチームオブジェクトに追加されました。Agile Estimate Type は、ストーリーの作業負荷の推定方法を決定します。時間単位での推定の場合は、ストーリーに追加される予定時間数です。ポイント数での推定の場合は、各ポイントはポイントの設定に基づいて予定時間数がストーリーに追加されます（デフォルトは 8 時間）。Agile Estimate Type で使用できる値は次のとおりです。</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS（ストーリーポイント）</li> 
       <li style="font-weight: normal;">HOURS（時間）</li> 
       <li style="font-weight: normal;">LEGACY_POINTS（ポイントの時間）</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### テンプレート {#template}

テンプレートオブジェクトは、プロジェクトのパターンを表します。プロジェクトをテンプレートから作成することで時間を節約できます。テンプレートにはチームとタスクが含まれ、テンプレートを使用するとプロジェクトにコピーされます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">この追加されたフィールドは、オブジェクトがアクティブの場合は値が true、そうでない場合は false の値を持つブーリアン型パラメーターです。「アクティブ」に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトに添付できます。「アクティブ」に設定されていないオブジェクトは、ドロップダウンメニューや先行入力フィールドには表示されず、他のオブジェクトにアタッチできません。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">追加済み</p> </li> 
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
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">可能な値 ET を追加しました。この値は、週末や休日を考慮しない、経過月数の単位を表します。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

TemplateTask オブジェクトは、テンプレートに含まれるタスクを表します。テンプレートタスクは、テンプレートが使用されるプロジェクト内のタスクになります。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> <p style="font-weight: normal;">次のフィールドに可能な値 ET が追加されました。この値は、週末や休日を考慮しない、経過月数の単位を表します。</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コレクションフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### タイムシート {#timesheet}

タイムシートオブジェクトは、タスク、プロジェクトおよびオーバーヘッド時間タイプの実際の時間数をユーザーが入力できる仮想タイムカードを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>コアフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">削除されました</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### アップデート {#update}

Workfront の作業アイテムを更新して、ユーザーに現在のステータスを知らせることができます。更新オブジェクトは、これらの更新の 1 つを表します。更新は、ユーザーが入力するか、Workfront システムが作成することができます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">使用可能な値 referenceObjectCustomData（enum.updatetypeenum.referenceobjectcustomdata）を追加しました。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>クエリ</td> 
   <td> <p style="font-weight: normal;">次のクエリがアップデートオブジェクトに追加されました。</p> 
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
   <td> <p style="font-weight: normal;">次のアクションがユーザーオブジェクトに追加されました。</p> 
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
   <td> <p style="font-weight: normal;">次のアクションがユーザーオブジェクトに追加されました。</p> 
    <ul> 
     <li style="font-weight: bold;">acknowledgeMyNotifications</li> 
     <li style="font-weight: bold;">unacknowledAllObjectsTypeCount</li> 
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

### ワーク  {#work}

作業オブジェクトは、Task と OpTask の両方が継承する共通のインターフェイスで、2 つの間で共通のコードを共有します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">直接フィールド<p style="font-weight: normal;">次のフィールドには、AT_DATE_BEFORE_YEAR と AT_DATE_AFTER_YEAR というバリデーターが追加されました。これらのバリデーターは、関連付けられたオブジェクトの日付を 1900 年より前や 2200 年より後に設定できないように指定します。</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">EAC（完成時総コスト見積り）の計算に透明性を持たせるため、パブリック API に以下のフィールドを追加しました。</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">BCWP（実行された作業の予算計上コスト）は、出来高とも呼ばれ、この指標の計算時点で実際に完了したタスク量の予算計上コストを表す、プロジェクトのパフォーマンス指標です。タスクの場合、BCWP = 実績完了率 x タスク予算となります。プロジェクトの場合、BCWP = SUM(すべての親タスクと個々のタスクの BCWP 値) となります。</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">BCWS（予定された作業の予算計上コスト）は、予定値とも呼ばれ、この指標の計算時点で完了しているべきタスク量の予算計上コストを表す、プロジェクトのパフォーマンス指標です。タスクの場合、BCWS = 予定完了率 x タスク予算となります。プロジェクトの場合、BCWS = SUM(すべての親タスクと個々のタスクの BCWS 値) となります。</p></li>
    </ul><p style="font-weight: normal;">次のフィールドに可能な値 ET が追加されました。この値は、週末や休日を考慮しない、経過月数の単位を表します。</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">次のフィールドは作業オブジェクトから削除されました。</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">次のフィールドが作業オブジェクトに追加されました。</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">削除されました。</p> </li> 
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
