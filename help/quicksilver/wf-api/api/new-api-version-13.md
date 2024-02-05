---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 13 の新機能
description: Adobe Workfront は、2021年4月22日（PT）に API バージョン 13 をリリースしました。API バージョン 13 では、バージョン 12 から次の変更がおこなわれました。
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 100%

---

# API バージョン 13 の新機能

Adobe Workfront は、2021年4月22日（PT）に API バージョン 13 をリリースしました。API バージョン 13 では、バージョン 12 から次の変更がおこなわれました。

## 追加されたリソース

API バージョン 13 で追加されたリソースはありません。

## 削除されたリソース

API バージョン 13 ではリソースが削除されませんでした。

## 変更されたリソース

API バージョン 13 で次のリソースを変更しました。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">グループ </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">プロジェクト</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">タスク</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">チーム</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">タイムシート</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">TimesheetProfile</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">UserDelegation</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">作業 </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

AccessLevel オブジェクトはユーザーに関連付けられていて、ユーザーのアクセス権を指定する AccessLevelPermissions のセットを表します。

アクセスレベルについて詳しくは、[アクセスレベルの仕組み](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接フィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>説明</b> </p> <p>バリデーター MAX_LENGTH が追加されました。このバリデーターは、説明の長さが 4,000 文字以下にするように指定しています。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

BreadCrumb オブジェクトは、Workfront 作業アイテムの親子階層内の要素を表します。パンくずリストは、作業アイテムがポートフォリオ、プロジェクトおよびタスクの大きい構造にどのように適合するかを示します。

パンくずリストについて詳しくは、[新しい Adobe Workfront エクスペリエンスのパンくずリストの概要](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接フィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>オブジェクトコードは、<a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラー</a>で確認できます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

BurndownEvent オブジェクトは、イテレーションのバーンダウンを変更するオブジェクトを表します。

バーンダウンについて詳しくは、[バーンダウン](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接フィールド</p> </td> 
   <td> <p>以下のフィールドから、NOT_GROUPABLE というフラグを削除しました。 </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
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
       <li style="font-weight: normal;">password:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.restrict.timesheet.edit.owners.admins (config.timesheet.restrict.timesheet.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>アクション</td> 
   <td> <p>CustomerPreferences リソースに以下のアクションが追加されました。</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>引数を受け取ります。</p> 
      <ul> 
       <li> <p>環境設定（マップ）</p> </li> 
      </ul> </li> 
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
   <td> <p>直接フィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>次の値を追加できます。</p> 
      <ul> 
       <li> <p>AEM（Adobe Experience Manager）</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>NOT_FILTERABLE フラグを追加</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### グループ  {#group}

グループオブジェクトは、一連のユーザーとチームを表します。グループは、多くの場合、部門の構造を表します。

グループについて詳しくは、[Adobe Workfront のグループとチーム](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md)を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>アクション</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>このアクションは、グループの親グループ（指定されたグループがサブグループであるグループ）の配列を返します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

JournalEntry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。フィールドをジャーナルエントリオブジェクトの一部としてログに記録するように設定すると、そのフィールドが変更されるたびに、対応するジャーナルエントリが作成されます。

JournalEntry リソースに REPORTABLE フラグを追加しました。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接フィールド</p> </td> 
   <td> <p>次のフィールドから NOT_GROUPABLE フラグを削除しました。</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>以下のフィールドに NOT_FILTERABLE フラグが追加されました。</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Adobe Workfront 管理者またはグループ管理者は、テンプレートを作成して、Adobe Workfront のレイアウト要素をカスタマイズできます。LayoutTemplate オブジェクトは、Adobe Workfront Classic に固有です。

新しい Adobe Workfrontエクスペリエンスでレイアウトテンプレートを表すオブジェクトについては、[UITemplate](#uitemplate) を参照してください。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>直接フィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>説明</b> </p> <p>バリデーター MAX_LENGTH が追加されました。このバリデーターは、説明の長さが 4,000 文字以下にするように指定しています。</p> </li> 
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
     <li> <p><b>externalIntegrationType</b> </p> <p>次の値を追加できます。</p> 
      <ul> 
       <li> <p>AEM（Adobe Experience Manager）</p> </li> 
      </ul> </li> 
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
   <td> <p>フィールドの検索</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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
   <td> <p>直接フィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>直接フィールド</p> </td> 
   <td> <p>次のフィールドが ProofApproval リソースに追加されました。</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>DecisionDate</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
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
     <li> <p><b>documentPosition</b> </p> <p>追加済み。次の値を指定できます。</p> 
      <ul> 
       <li> <p>0（カスタムフォームの後)</p> </li> 
       <li> <p>1（カスタムフォームの前)</p> </li> 
      </ul> </li> 
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
   <td> <p>フィールドの検索</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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

### タイムシート {#timesheet}

タイムシートオブジェクトは、タスク、プロジェクトおよびオーバーヘッド時間タイプの実際の時間数をユーザーが入力できる仮想タイムカードを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コアフィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>削除されました</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TimesheetProfile {#timesheetprofile}

タイムシートオブジェクトは、タスク、プロジェクトおよびオーバーヘッド時間タイプの実際の時間数をユーザーが入力できる仮想タイムカードを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Adobe Workfront 管理者またはグループ管理者は、テンプレートを作成して、Adobe Workfront のレイアウト要素をカスタマイズできます。UITemplate オブジェクトは、新しい Adobe Workfront エクスペリエンスに固有のものです。

Adobe Workfront Classic のレイアウトテンプレートを表すオブジェクトについては、[LayoutTemplate](#layouttemplate) を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> <p>UITemplate リソースに以下のアクションが追加されました。</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>引数を受け取ります。</p> 
      <ul> 
       <li> <p>overrideIfExists（ブーリアン）</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>引数を受け取ります。</p> 
      <ul> 
       <li> <p>layoutTemplateIDs（string[]）</p> </li> 
       <li> <p>overrideIfExists（ブーリアン）</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegation {#userdelegation}

UserDelegation オブジェクトは、特定の期間、1 人のユーザーから別のユーザーに作業をデリゲートする行為を表します。

UserDelegation オブジェクトに REPORTABLE というフラグが追加されました。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> <p>以下のフィールドから、NOT_GROUPABLE というフラグを削除しました。</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">デフォルトのフィールド</td> 
   <td> <p>以下のフィールドが追加されました。</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
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
   <td> <p>フィールドの検索</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
