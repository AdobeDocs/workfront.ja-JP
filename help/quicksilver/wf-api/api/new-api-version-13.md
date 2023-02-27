---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 13 の新機能
description: Adobe Workfrontは、2021 年 4 月 23 日に API バージョン 13 をリリースしました。 API バージョン 13 では、バージョン 12 から次の変更がおこなわれました。
author: Becky
feature: Workfront API
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# API バージョン 13 の新機能

Adobe Workfrontは、2021 年 4 月 23 日に API バージョン 13 をリリースしました。 API バージョン 13 では、バージョン 12 から次の変更がおこなわれました。

## 追加されたリソース

API バージョン 13 にはリソースが追加されませんでした。

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
     <li> <p><a href="#optask" class="MCXref xref">Opタスク</a> </p> </li> 
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

AccessLevel オブジェクトは、ユーザーに関連付けられ、ユーザーがアクセスできる AccessLevelPermissions のセットを表します。

アクセスレベルの詳細については、 [アクセスレベルの仕組み](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>ダイレクトフィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>説明</b> </p> <p>バリデーターMAX_LENGTH が追加されました。このバリデーターは、説明の長さが 4,000 文字以下であることを指定しています。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

BreadCrumb オブジェクトは、Workfront作業項目の親/子階層内の要素を表します。 パンくずリストは、作業項目がPortfolio、プロジェクト、プロジェクト、タスクの構造にどのように適合するかを示します。

パンくずリストについて詳しくは、 [新しいAdobe Workfrontエクスペリエンスのパンくずリストの概要](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>ダイレクトフィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>オブジェクトコードは、 <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラ</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

BurndownEvent オブジェクトは、反復の分解を変更するオブジェクトを表します。

バーンダウンについて詳しくは、 [バーンダウン](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>ダイレクトフィールド</p> </td> 
   <td> <p>以下のフィールドは、NOT_GROUPABLE フラグを削除しました </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
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
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">次の値を追加しました。</p> 
      <ul> 
       <li style="font-weight: normal;">パスワード：aemAPIKey(config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">タイムシート：default.timesheet.restrict.timesheet.edit.owners.admins (config.timesheet.restrict.timesheet.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>アクション</td> 
   <td> <p>CustomerPreferences リソースに次のアクションが追加されました。</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>引数を取ります。</p> 
      <ul> 
       <li> <p>環境設定（マップ）</p> </li> 
      </ul> </li> 
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
   <td> <p>ダイレクトフィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>次の値が追加されました。</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>NOT_FILTERABLE フラグを追加しました</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### グループ  {#group}

Group オブジェクトは、一連のユーザーとチームを表します。 グループは、多くの場合、部門の構造を表します。

グループについて詳しくは、 [Adobe Workfrontのグループとチーム](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>アクション</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>このアクションは、グループの親グループ（特定のグループがサブグループであるグループ）の配列を返します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

JournalEntry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。 フィールドを Journal Entry オブジェクトの一部としてログに記録するように設定すると、そのフィールドを変更するたびに対応する Journal Entry が作成されます。

JournalEntry リソースが REPORTABLE フラグを追加しました。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>ダイレクトフィールド</p> </td> 
   <td> <p>次のフィールドは、NOT_GROUPABLE フラグを削除しました。</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>以下のフィールドには NOT_FILTERABLE フラグが追加されました。</p> 
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

Adobe Workfrontの管理者またはグループ管理者は、テンプレートを作成して、Adobe Workfrontのレイアウト要素をカスタマイズできます。 LayoutTemplate オブジェクトは、Adobe Workfront Classic に固有です。

新しいAdobe Workfrontエクスペリエンスでレイアウトテンプレートを表すオブジェクトについては、 [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>ダイレクトフィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>説明</b> </p> <p>バリデーターMAX_LENGTH が追加されました。このバリデーターは、説明の長さが 4,000 文字以下であることを指定しています。</p> </li> 
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
     <li> <p><b>externalIntegrationType</b> </p> <p>次の値が追加されました。</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>フィールドの検索</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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
   <td> <p>ダイレクトフィールド</p> </td> 
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

ProofApproval オブジェクトは、配達確認に直接接続される承認を表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>ダイレクトフィールド</p> </td> 
   <td> <p>次のフィールドが ProofApproval リソースに追加されました。</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>決定日</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
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
     <li> <p><b>documentPosition</b> </p> <p>追加済み. 次の値を指定できます。</p> 
      <ul> 
       <li> <p>0 （カスタムフォームの後）</p> </li> 
       <li> <p>1 （カスタムフォームの前）</p> </li> 
      </ul> </li> 
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
   <td> <p>フィールドの検索</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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

### タイムシート {#timesheet}

Timesheet オブジェクトは、Tasks、Projects、および Overhead Hour Types の実績作業時間をユーザーが入力できる仮想タイムカードを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>追加済み</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>コアフィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>削除済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TimesheetProfile {#timesheetprofile}

Timesheet オブジェクトは、Tasks、Projects、および Overhead Hour Types の実績作業時間をユーザーが入力できる仮想タイムカードを表します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>ダイレクトフィールド</td> 
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

Adobe Workfrontの管理者またはグループ管理者は、テンプレートを作成して、Adobe Workfrontのレイアウト要素をカスタマイズできます。 LayoutTemplate オブジェクトは、新しいAdobe Workfrontエクスペリエンスに固有のものです。

Adobe Workfront Classic のレイアウトテンプレートを表すオブジェクトについては、 [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> <p>UITemplate リソースに以下のアクションが追加されました。</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>引数を取ります。</p> 
      <ul> 
       <li> <p>overrideIfExists(boolean)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>引数を取ります。</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists(boolean)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegation {#userdelegation}

UserDelegation オブジェクトは、特定の期間、あるユーザーから別のユーザーに作業を委任する行為を表します。

UserDelegation オブジェクトに REPORTABLE というフラグが追加されました。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> <p>以下のフィールドは、NOT_GROUPABLE フラグを削除しました</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">デフォルトのフィールド</td> 
   <td> <p>次のフィールドが追加されました。</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
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
   <td> <p>フィールドの検索</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
