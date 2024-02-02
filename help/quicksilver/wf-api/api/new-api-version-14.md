---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 14 の新機能
description: Adobe Workfront は、2021年9月9日（PT）に API バージョン 14 をリリースしました。API バージョン 14 では、バージョン 14 から次の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: ht
source-wordcount: '891'
ht-degree: 100%

---

# API バージョン 14 の新機能

Adobe Workfront は、2021年9月9日（PT）に API バージョン 14 をリリースしました。API バージョン 14 では、バージョン 14 から次の変更が行われました。

## 追加されたリソース

API バージョン 14 にはリソースが追加されませんでした。

## 削除されたリソース

API バージョン 14 ではリソースが削除されませんでした。

## 変更されたリソース

API バージョン 14 で次のリソースを変更しました。

* [BillingRecord（BILL）](#billingrecord-bill)
* [Category（CTGY）](#category-ctgy)
* [CustomEnum（CSTEM）](#customenum-cstem)
* [Customer（CUST）](#customer-cust)
* [CustomerPreferences（CUSTPR）](#customerpreferences-custpr)
* [DocumentVersion（DOCV）](#documentversion-docv)
* [Group（GROUP）](#group-group)
* [NoteTag（NTAG）](#notetag-ntag)
* [Project（PROJ）](#project-proj)
* [QueueDef（QUED）](#queuedef-qued)
* [Resource Allocation（RSALLO）](#resource-allocation-rsallo)
* [Role（ROLE）](#role-role)
* [Template（TMPL）](#template-tmpl)
* [Timesheet（TSHET）](#timesheet-tshet)

### BillingRecord（BILL） {#billingrecord-bill}

BillingRecord オブジェクトは、請求可能な収益、時間または費用を記録します。この情報は、外部の会計システムで請求書を作成する際に使用できます。

請求記録について詳しくは、[請求記録の作成](../../manage-work/projects/project-finances/create-billing-records.md)を参照してください。

BillingRecord オブジェクトにフラグ **DATA_EXTENDIBLE** が追加されました。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">直接フィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>追加済み。カテゴリはカスタムフォームです。このパラメーターは、カスタムフォームを BillingRecord オブジェクトに追加する機能をサポートするために追加されました。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">参照フィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>category</b> </p> <p>追加済み。カテゴリはカスタムフォームです。このパラメーターは、カスタムフォームを BillingRecord オブジェクトに追加する機能をサポートするために追加されました。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">コレクションフィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>追加済み。BillingRecord オブジェクトに関連付けられた Category（カスタムフォーム）のコレクションを表します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>追加済み。このアクションにより、カスタムフォームフィールドの式が再計算されます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Category（CTGY） {#category-ctgy}

カテゴリオブジェクトはカスタムフォームです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>次の値を追加できます。</p> 
      <ul> 
       <li> <p> BILL（BillingRecord）</p> </li> 
      </ul> <p>この値は、カスタムフォームを BillingRecord オブジェクトに追加する機能をサポートするために追加されました。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>このアクションは、パラメーター objID と objCode を取り、ブール値を返します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum（CSTEM） {#customenum-cstem}

CustomEnum オブジェクトは、ステータスコードを人間が読み取り可能なテキストに変換する際に役立ちます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">クエリ</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>追加済み。このクエリは、グループとサブグループのステータスを作成および管理する機能をサポートします。 </p> <p>詳しくは、<a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">グループステータスの管理</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Customer（CUST） {#customer-cust}

顧客オブジェクトは、Workfront のインスタンスを使用する組織を表します。

これは内部オブジェクトです。

### CustomerPreferences（CUSTPR） {#customerpreferences-custpr}

CustomerPreferences オブジェクトは、Workfront のインスタンスに対して顧客が設定した一連の環境設定を表します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>次の値を追加できます。</p> 
      <ul> 
       <li> <p>更新時の画像の追加をユーザーに許可（更新：images.toggle）</p> </li> 
      </ul> <p>このパラメーターは、作業アイテムの更新に画像を追加する機能をサポートします。 </p> <p>詳しくは、<a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業の更新</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion（DOCV） {#documentversion-docv}

DocumentVersion オブジェクトは、ファイルの特定のバージョン（書き込まれた資料、画像、その他の形式の情報など）を表します。

ドキュメントのバージョンについて詳しくは、[新しいバージョンのドキュメントのアップロード](../../documents/managing-documents/upload-new-document-version.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>追加済み。このフィールドには、バージョンがプルーフに関連付けられている場合に、Workfront Proof からの最後のコールバックの日時が記録されます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### グループ（GROUP） {#group-group}

グループオブジェクトは、一連のユーザーとチームを表します。グループは、多くの場合、部門の構造を表します。

グループについて詳しくは、[Adobe Workfront のグループとチーム](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>追加済み。このアクションは、groupID の配列を取り出し、それらのグループをサブグループとして指定したグループに追加します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag（NTAG） {#notetag-ntag}

NoteTag オブジェクトは、作業アイテムの更新時に、ユーザーまたはチームにタグ付けする行為を表します。

更新でのタグ付けについて詳しくは、[更新時のその他ユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>次の操作が NoteTag オブジェクトに追加されました。</p> 
    <ul> 
     <li> <p><b>COUNT</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>REPORT</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Project（PROJ） {#project-proj}

プロジェクトは Workfront 内の作業アイテムで、Workfront が人々の作業を支援するための主要な構築ブロックです。プロジェクトオブジェクトは、共通の特定の目標を持つタスクのグループを表します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>追加済み。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef（QUED） {#queuedef-qued}

QueueDef オブジェクトは、キューを表します。キューは、ユーザーがイシューを送信できるようにヘルプデスクエリアに公開されたプロジェクトです。

リクエストキューについて詳しくは、[リクエストキューの作成](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>追加済み。このアクションは、リクエストキューおよびトピックグループ内のパスを使用してリクエストを検索する機能をサポートします。</p> <p>パスによるリクエストキューの検索について詳しくは、<a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Adobe Workfront リクエストの作成と送信</a>の <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Workfront web アプリでのリクエストの作成とドラフトの作成</a>を参照してください。</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Resource Allocation（RSALLO） {#resource-allocation-rsallo}

Resource Allocation オブジェクトは、特定のプロジェクトに必要なリソースの見積もりを表します。このオブジェクトは、従来のリソースプランナーでのみ使用されます。新しいリソースプランナーの対応するフィールドには、予算計上時間数（BGHR）を使用します。

Resource Allocation オブジェクトでフラグ **REPORTABLE** が削除されました。

### Role（ROLE） {#role-role}

Role オブジェクト（担当業務）は、デザイナーやプロダクトマネージャーなど、ユーザーが入力できる機能またはスキルセットを表します。

担当業務について詳しくは、[担当業務の概要](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">追加済み。オブジェクトが Active の場合は値 true を持ち、そうでない場合は false を持つブーリアン型パラメーターです。「アクティブ」に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトに添付できます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">デフォルトのフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">追加済み</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Template（TMPL） {#template-tmpl}

テンプレートオブジェクトは、プロジェクトのパターンを表します。プロジェクトをテンプレートから作成することで時間を節約できます。テンプレートにはチームとタスクが含まれ、テンプレートから作成されたすべてのプロジェクトにコピーされます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">直接フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">追加済み。このフィールドは、グループをテンプレートに関連付ける機能をサポートするために追加されました。</p> <p style="font-weight: normal;">詳しくは、<a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">プロジェクトテンプレートの編集</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>グループ</p> <p style="font-weight: normal;">追加済み。このフィールドは、グループをテンプレートに関連付ける機能をサポートするために追加されました。</p> <p style="font-weight: normal;">詳しくは、<a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">プロジェクトテンプレートの編集</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
