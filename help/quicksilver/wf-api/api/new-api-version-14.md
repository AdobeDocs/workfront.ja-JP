---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 14 の新機能
description: Adobe Workfrontは、2021 年 9 月 10 日に API バージョン 14 をリリースしました。 API バージョン 14 では、バージョン 14 から次の変更がおこなわれました。
author: Becky
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 2%

---

# API バージョン 14 の新機能

Adobe Workfrontは、2021 年 9 月 10 日に API バージョン 14 をリリースしました。 API バージョン 14 では、バージョン 14 から次の変更がおこなわれました。

## 追加されたリソース

API バージョン 14 にはリソースが追加されませんでした。

## 削除されたリソース

API バージョン 14 ではリソースが削除されませんでした。

## 変更されたリソース

API バージョン 14 で次のリソースを変更しました。

* [請求レコード (BILL)](#billingrecord-bill)
* [カテゴリ (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [顧客 (CUST)](#customer-cust)
* [顧客の環境設定 (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [グループ (GROUP)](#group-group)
* [メモタグ (NTAG)](#notetag-ntag)
* [プロジェクト (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [リソース割り当て (RSALLO)](#resource-allocation-rsallo)
* [役割（役割）](#role-role)
* [テンプレート (TMPL)](#template-tmpl)
* [タイムシート (TSHET)](#timesheet-tshet)

### 請求レコード (BILL) {#billingrecord-bill}

BillingRecord オブジェクトは、請求可能な収益、時間、または費用を記録します。 この情報は、外部の会計システムで請求書を作成する際に使用できます。

請求レコードについて詳しくは、 [請求レコードの作成](../../manage-work/projects/project-finances/create-billing-records.md).

BillingRecord オブジェクトによってフラグが追加されました **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">ダイレクトフィールド</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>追加済み. カテゴリはカスタムフォームです。 このパラメーターは、カスタムFormsを BillingRecord オブジェクトに追加する機能をサポートするために追加されました。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">参照フィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>カテゴリ</b> </p> <p>追加済み. カテゴリはカスタムフォームです。 このパラメーターは、カスタムフォームを BillingRecord オブジェクトに追加する機能をサポートするために追加されました。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">コレクションフィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>追加済み. BillingRecord オブジェクトに関連付けられた Categories （カスタムフォーム）のコレクションを表します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>追加済み. この操作により、カスタムフォームフィールドの式が再計算されます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### カテゴリ (CTGY) {#category-ctgy}

Category オブジェクトはカスタムフォームです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>次の値が追加されました。</p> 
      <ul> 
       <li> <p> 請求（請求レコード）</p> </li> 
      </ul> <p>この値は、カスタムフォームを BillingRecord オブジェクトに追加する機能をサポートするために追加されました。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>このアクションは、パラメータ objID と objCode を取り、ブール値を返します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

CustomEnum オブジェクトは、ステータスコードを人間が読み取り可能なテキストに変換する際に役立ちます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">クエリ</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>追加済み. このクエリは、グループとサブグループのステータスを作成および管理する機能をサポートします。 </p> <p>詳しくは、 <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">グループステータスの管理</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 顧客 (CUST) {#customer-cust}

Customer オブジェクトは、Workfrontのインスタンスを使用する組織を表します。

これは内部オブジェクトです。

### 顧客の環境設定 (CUSTPR) {#customerpreferences-custpr}

CustomerPreferences オブジェクトは、Workfrontのインスタンスに対して顧客が設定した一連の環境設定を表します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>次の値が追加されました。</p> 
      <ul> 
       <li> <p>更新時の画像の追加をユーザーに許可（更新：images.toggle）</p> </li> 
      </ul> <p>このパラメータは、作業項目の更新に画像を追加する機能をサポートします。 </p> <p>詳しくは、 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業を更新</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

DocumentVersion オブジェクトは、ファイルの特定のバージョン（書き込まれた資料、画像、その他の形式の情報など）を表します。

ドキュメントのバージョンについて詳しくは、 [新しいバージョンのドキュメントをアップロード](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>追加済み. このフィールドには、バージョンが配達確認に関連付けられている場合に、Workfront Proof からの最後のコールバックの日時が記録されます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### グループ (GROUP) {#group-group}

Group オブジェクトは、一連のユーザーとチームを表します。 グループは、多くの場合、部門の構造を表します。

グループについて詳しくは、 [Adobe Workfrontのグループとチーム](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>追加済み. このアクションは、groupID の配列を取り出し、それらのグループをサブグループとして指定したグループに追加します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### メモタグ (NTAG) {#notetag-ntag}

NoteTag オブジェクトは、作業項目の更新時に、ユーザーまたはチームにタグ付けする行為を表します。

アップデートでのタグ付けについて詳しくは、 [更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">操作</td> 
   <td> <p>次の操作が NoteTag オブジェクトに追加されました。</p> 
    <ul> 
     <li> <p><b>カウント</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>レポート</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### プロジェクト (PROJ) {#project-proj}

プロジェクトはWorkfront内の作業項目で、Workfrontが作業をおこなう際に役立つ主要な構成要素です。 Project オブジェクトは、共通の特定の目標を持つタスクのグループを表します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>追加済み.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

QueueDef オブジェクトは、Queue を表します。Queue は、ユーザーが問題を送信できるようにヘルプデスク領域に公開されたプロジェクトです。

リクエストキューについて詳しくは、 [リクエストキューの作成](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>追加済み. このアクションは、リクエストキューおよびトピックグループ内のパスを使用してリクエストを検索する機能をサポートします。</p> <p>パスによるリクエストキューの検索について詳しくは、 <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Workfront Web アプリでのリクエストの作成とドラフトの生成</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Adobe Workfront要求の作成と送信</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### リソース割り当て (RSALLO) {#resource-allocation-rsallo}

Resource Allocation オブジェクトは、特定のプロジェクトに必要なリソースの見積もりを表します。 このオブジェクトは、レガシーのリソースプランナーでのみ使用されます。 新しいリソース・プランナの対応するフィールドには、予算時間 (BGHR) を使用します。

リソース割り当てオブジェクトがフラグを削除しました **レポート可能**.

### 役割（役割） {#role-role}

ロールオブジェクト（ジョブロール）は、Designer や Product Manager など、ユーザーが入力できる機能能力またはスキルセットを表します。

ジョブの役割について詳しくは、 [ジョブロールの概要](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">追加済み. オブジェクトが Active の場合は値 true を持ち、そうでない場合は false を持つブール型パラメータです。 [ アクティブ ] に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトにアタッチできます。</p> </li> 
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

### テンプレート (TMPL) {#template-tmpl}

Template オブジェクトは、プロジェクトのパターンを表します。 プロジェクトは、テンプレートから作成して時間を節約できます。 テンプレートにはチームとタスクが含まれ、テンプレートから作成されたすべてのプロジェクトにコピーされます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ダイレクトフィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">追加済み. このフィールドは、グループをテンプレートに関連付ける機能をサポートするために追加されました。</p> <p style="font-weight: normal;">詳しくは、 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">プロジェクトテンプレートの編集</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">参照フィールド</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>グループ</p> <p style="font-weight: normal;">追加済み. このフィールドは、グループをテンプレートに関連付ける機能をサポートするために追加されました。</p> <p style="font-weight: normal;">詳しくは、 <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">プロジェクトテンプレートの編集</a>.</p> </li> 
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
