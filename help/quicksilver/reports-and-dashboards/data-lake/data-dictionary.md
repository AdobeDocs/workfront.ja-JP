---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect データディクショナリ
description: ここでは、Workfront Data Connect のデータの構造と内容について説明します。
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 44342db0a473eac70212d08cedf9ac0f571cda0b
workflow-type: tm+mt
source-wordcount: '8129'
ht-degree: 7%

---

# Workfront Data Connect データディクショナリ

ここでは、Workfront Data Connect のデータの構造と内容について説明します。

>[!NOTE]
>
>データ接続のデータは 4 時間ごとに更新されるので、最近の変更がすぐには反映されない場合があります。

## テーブルタイプ

Data Connect で使用して、最もinsightの多い方法でWorkfront データを表示できるテーブルタイプが多数あります。

* **現在のテーブル**

  「現在のテーブル」には、Workfrontの場合と同様に、すべてのオブジェクトのデータが表示され、データの現在のステータスが表示されます。 ただし、Workfront内よりもはるかに低い待ち時間でナビゲーションできます。

* **イベントテーブル**

  イベント テーブルは、Workfront内のすべての変更レコードを追跡します。つまり、オブジェクトのステータスが変わるたびに、変更がいつ行われたか、誰が変更を加えたか、および何が変更されたかを示すレコードが作成されます。 したがって、このテーブルはポイントインタイムの比較に役立ちます。 このテーブルには、過去 3 年間のレコードのみが含まれます。

* **日別履歴テーブル**

  「毎日の履歴」 テーブルには、「イベント」 テーブルの短縮バージョンが表示されます。このテーブルでは、各オブジェクトの状態が、個々のイベントが発生した時間ではなく日単位で表示されます。 したがって、このテーブルはトレンド分析に役立ちます。

<!-- Custom table -->

## エンティティ関係図

Workfront（およびデータ接続データレイク）のオブジェクトは、個々の値だけでなく、他のオブジェクトとの関係によって定義されます。 以下のエンティティ関係図は、データ接続のオブジェクト関係の高度なマッピングを提供します。 この図は、次のリンクを使用して表示およびダウンロードできます。

[データ接続エンティティ関係図](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>エンティティ関係ダイアグラムは処理中です。そのため、参照用にのみ使用され、変更される可能性があります。

## 日付タイプ

特定のイベントが発生するタイミングに関する情報を提供する日付オブジェクトが多数あります。

* `DL_LOAD_TIMESTAMP`：この日付は内部参照に使用され、データが現在、イベントまたは毎日の履歴テーブルに読み込まれた日時を反映します。 この日付は、データ分析には使用せず、Workfront Data Lake のベータ段階で削除される予定です。
* `CALENDAR_DATE`：この日付は、「日別の履歴」テーブルにのみ表示されます。 この表は、`CALENDAR_DATE` で指定された各日付に対して、UTC で 11:59 にどのようなデータが表示されたかを示しています。
* `BEGIN_EFFECTIVE_TIMESTAMP`：この日付は、イベント履歴テーブルと日別履歴テーブルの両方に存在し、現在の行にあるレコードの値が _to_ 変更されたタイミングで正確にレコードされます。
* `END_EFFECTIVE_TIMESTAMP`：この日付は、イベント履歴テーブルと日別履歴テーブルの両方に表示され、レコードが現在の行の値から別の行の値に _変更された_ ときにそのレコードが正確に表示されます。 `BEGIN_EFFECTIVE_TIMESTAMP` と `END_EFFECTIVE_TIMESTAMP` のクエリ間でを許可するには、新しい値がない場合でも、この値は null ではありません。 レコードがまだ有効な場合（つまり、値が変更されていない場合）、`END_EFFECTIVE_TIMESTAMP` の値は 2300-01-01 になります。

## 用語テーブル

次の表は、Workfrontのオブジェクト名（およびインターフェイスと API のオブジェクト名）と、Data Connect の同等の名前を関連付けています。

### アクセスレベル

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>アクセスレベル</td>
            <td>アクセスレベル</td>
            <td>ACSLVL</td>
            <td>アクセスレベル</td>
            <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LEGACYACCESSLEVELID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### アクセスルール

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>アクセスルール</td>
            <td>共有</td>
            <td>ACSRUL</td>
            <td>共有</td>
            <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSORID</td>
             <td>FK</td>
             <td>ACCESSOROBJCODE に基づく変数</td>
             <td>ACCESSOROBJCODE フィールドで識別されるオブジェクトのプライマリ・キー/ID</td>
        </tr>
        <tr>
             <td>ACCESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ANCESTORID</td>
             <td>PK</td>
             <td>変数（ANCESTOROBJCODE に基づく）</td>
             <td>ANCESTOROBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SECURITYOBJID</td>
             <td>FK</td>
             <td>SECURITYOBJECT コードに基づく変数</td>
             <td>SECURITYOBJCODE フィールドで識別されたオブジェクトのプライマリ・キー/ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 承認パス

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>承認パス</td>
            <td>承認パス</td>
            <td>ARVPTH</td>
            <td>承認</td>
            <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GLOBALPATHID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 承認プロセス

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>承認プロセス</td>
            <td>承認プロセス</td>
            <td>ARVPRC</td>
            <td>承認プロセス</td>
            <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 承認ステップ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>承認ステップ</td>
            <td>承認ステップ</td>
            <td>ARVSTP</td>
            <td>承認ステージ</td>
            <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPATHID</td>
             <td>FK</td>
             <td>APPROVALPATHS_CURRENT</td>
             <td>APPROVALPATHID</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 上書きされている

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>上書きされている</td>
            <td>上書きされている</td>
            <td>ARVSTS</td>
            <td>ApproverStatus</td>
            <td>APPROVERSTATES_CURRENT<br>APPROVERSTATES_DAILY_HISTORY<br>APPROVERSTATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>APPROVABLEOBJID</td>
             <td>FK</td>
             <td>変数（APPROVABLEOBJCODE に基づく）</td>
             <td>APPROVABLEOBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DELEGATEUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OVERRIDDENUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSYID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>WILDCARDUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### 割り当て

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>割り当て</td>
            <td>割り当て</td>
            <td>ASSGN</td>
            <td>割り当て</td>
            <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>譲渡病様</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
    </tbody>
</table>

### 承認待ち

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>承認待ち</td>
            <td>承認待ち</td>
            <td>AWAPVL</td>
            <td>承認待ち</td>
            <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSREQUESTID</td>
             <td>-</td>
             <td colspan="2">アクセス要求テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>APPROVABLEID</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>AWAITINGAPPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>FK</td>
             <td>DOCUMENTVERSIONS_CURRENT</td>
             <td>DOCUMENTVERSIONID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### ベースライン

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ベースライン</td>
            <td>ベースライン</td>
            <td>ブリン</td>
            <td>ベースライン</td>
            <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ベースライン ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ベースライン タスク

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ベースライン タスク</td>
            <td>ベースライン タスク</td>
            <td>BSTSK</td>
            <td>ベースライン タスク</td>
            <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ベースライン ID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>ベースライン ID</td>
        </tr>
        <tr>
             <td>BASELINETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
    </tbody>
</table>

### 請求レート

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>請求レート</td>
            <td>レートまたはレートの上書き</td>
            <td>率</td>
            <td>請求レート</td>
            <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### 請求記録

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>請求記録</td>
            <td>請求記録</td>
            <td>請求書</td>
            <td>請求記録</td>
            <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>INVOICEID</td>
             <td>-</td>
             <td colspan="2">現在、請求書テーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 予約

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>予約</td>
            <td>予約</td>
            <td>予約</td>
            <td>予約</td>
            <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BOOKINGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>FK</td>
             <td>NONLABORRESOURCES_CURRENT</td>
             <td>NONLABORRESOURCEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>TOPOBJCODE に基づく変数</td>
             <td>TOPOBJCODE フィールドで識別されるオブジェクトのプライマリキー/ID</td>
        </tr>
    </tbody>
</table>

### ビジネスプロファイル

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ビジネスプロファイル</td>
            <td>ビジネスプロファイル</td>
            <td>BSNPRF</td>
            <td>BusinessProfile</td>
            <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVEL_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>BUSINESSPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ビジネスルール

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ビジネスルール</td>
            <td>ビジネスルール</td>
            <td>BSNRUL</td>
            <td>ビジネスルール</td>
            <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSRULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### カテゴリ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>カテゴリ</td>
            <td>カスタムフォーム</td>
            <td>CTGY</td>
            <td>カテゴリ</td>
            <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### カテゴリパラメーター

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>カテゴリパラメーター</td>
            <td>カスタムフォームフィールド</td>
            <td>CTGYPA</td>
            <td>カテゴリパラメーター</td>
            <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORIESPARAMETERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>FK</td>
             <td>PARAMETERGROUPS_CURRENT</td>
             <td>PARAMETERGROUPID</td>
        </tr>
        <tr>
             <td>パラメーター ID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>パラメーター ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 分類子

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>分類子</td>
            <td>Location</td>
            <td>CLSF</td>
            <td>Location</td>
            <td>CLASSIFIER_CURRENT<br>CLASSIFIER_DAILY_HISTORY<br>CLASSIFIER_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 会社

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>会社</td>
            <td>会社</td>
            <td>CMPY</td>
            <td>会社</td>
            <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### カスタム四半期

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>カスタム四半期</td>
            <td>カスタム四半期</td>
            <td>CSTQRT</td>
            <td>カスタム四半期</td>
            <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMQUARTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### カスタム列挙

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>CustomEnum</td>
            <td>条件、優先度、重要度、ステータス</td>
            <td>システム</td>
            <td>カスタム列挙</td>
            <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CUSTOMENUMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>
<div>* レコードのタイプは、「enumClass」プロパティを使用して識別されます。 想定されるタイプは次のとおりです。<br>
<ul><li>CONDITION_OPTASK</li>
<li>CONDITION_PROJ</li>
<li>CONDITION_TASK</li>
<li>PRIORITY_OPTASK</li>
<li>PRIORITY_PROJ</li>
<li>PRIORITY_TASK</li>
<li>SEVERITY_OPTASK</li>
<li>STATUS_OPTASK</li>
<li>STATUS_PROJ</li>
<li>STATUS_TASK</li></ul></div>

### ドキュメント

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメント</td>
            <td>ドキュメント</td>
            <td>DOCU</td>
            <td>ドキュメント</td>
            <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CHECKEDOUTBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTREQUESTID</td>
             <td>-</td>
             <td colspan="2">ドキュメント要求テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>類ポートフォリオ</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>類ポートフォリオ</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RELEASEVERSIONID</td>
             <td>-</td>
             <td colspan="2">現在、リリースバージョンテーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>TOPOBJCODE に基づく変数</td>
             <td>TOPOBJCODE フィールドで識別されるオブジェクトのプライマリキー/ID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### ドキュメントの承認

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメントの承認</td>
            <td>ドキュメントの承認</td>
            <td>DOCAPL</td>
            <td>ドキュメントの承認</td>
            <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>DOCAPPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>REQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ドキュメントの承認（新規）

お客様の限定提供

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメントの承認</td>
            <td>承認</td>
            <td>該当なし</td>
            <td>該当なし</td>
            <td>APPROVAL_CURRENT<br>APPROVAL_DAILY_HISTORY<br>APPROVAL_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APPROVALID</td>
             <td>PK</td>
             <td>-</td>
             <td>メモ：これは、承認が関連付けられている DOCUMENTVERSION オブジェクトの ID でもあります。</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>変数（ASSETTYPE に基づく）</td>
             <td>ASSETTYPE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">EAUTHTENANTID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td class="key">PRODUCTID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td class="key">REALCREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### ドキュメント承認ステージ （新規）

お客様の限定提供

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメントの承認ステージ</td>
            <td>承認ステージ</td>
            <td>該当なし</td>
            <td>該当なし</td>
            <td>APPROVAL_STAGE_CURRENT<br>APPROVAL_STAGE_DAILY_HISTORY<br>APPROVAL_STAGE_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APPROVALID</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>APPROVALID</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">CREATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
    </tbody>
</table>

### ドキュメント承認ステージ参加者（新規）

お客様の限定提供

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメントの承認ステージ参加者</td>
            <td>承認の決定</td>
            <td>該当なし</td>
            <td>該当なし</td>
            <td>APPROVAL_STAGE_PARTICIPANT_CURRENT<br>APPROVAL_STAGE_PARTICIPANT_DAILY_HISTORY<br>APPROVAL_STAGE_PARTICIPANT_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td class="key">APPROVALID</td>
             <td>FK</td>
             <td>APPROVAL_CURRENT</td>
             <td>APPROVALID</td>
        </tr>
        <tr>
             <td class="key">APPROVALSTAGEPARTICIPANTID/td&gt;
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td class="key">ASSETID</td>
             <td>FK</td>
             <td>変数（ASSETTYPE に基づく）</td>
             <td>ASSETTYPE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td class="key">DECISIONUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">OBJID</td>
             <td class="type">FK</td>
             <td class="relatedtable">OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td class="key">PARTICIPANTID</td>
             <td>FK</td>
             <td class="relatedtable">変数（PARTICIPANTTYPE に基づく）</td>
             <td>PARTICIPANTTYPE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td class="key">REALREQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">REALUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">REQUESTORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td class="key">STAGEID</td>
             <td>FK</td>
             <td>APPROVAL_STAGE_CURRENT</td>
             <td>STAGEID</td>
        </tr>
    </tbody>
</table>

### ドキュメントフォルダー

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメントフォルダー</td>
            <td>ドキュメントフォルダー</td>
            <td>DOCFLD</td>
            <td>DocsFolder</td>
            <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>FK</td>
             <td>LINKEDFOLDERS_CURRENT</td>
             <td>LINKEDFOLDERID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>DOCFOLDERID</td>
        </tr>
        <tr>
             <td>類ポートフォリオ</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>類ポートフォリオ</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### ドキュメントプロバイダーメタデータ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメントプロバイダーメタデータ</td>
            <td>ドキュメントプロバイダーメタデータ</td>
            <td>DOCMET</td>
            <td>DocumentProviderMetadata</td>
            <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERMETAID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ドキュメント プロバイダー

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメント プロバイダー</td>
            <td>ドキュメント プロバイダー</td>
            <td>DOCPRO</td>
            <td>ドキュメント プロバイダー</td>
            <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>FK</td>
             <td>DOCPROVIDERCONFIG_CURRENT</td>
             <td>DOCPROVIDERCONFIGID</td>
        </tr>
        <tr>
             <td>DOCPROVIDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ドキュメントプロバイダー設定

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメントプロバイダー設定</td>
            <td>ドキュメントプロバイダー設定</td>
            <td>DOCCFG</td>
            <td>DocumentProviderConfig</td>
            <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCPROVIDERCONFIGID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ドキュメントのバージョン

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ドキュメントのバージョン</td>
            <td>ドキュメントのバージョン</td>
            <td>DOCV</td>
            <td>ドキュメントのバージョン</td>
            <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>DOCUMENTVERSIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">外部ストレージシステムの外部 ID</td>
        </tr>
        <tr>
             <td>PROOFAPPROVALSTATUSID</td>
             <td>-</td>
             <td colspan="2">現在、プルーフ承認ステータステーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>PROOFEDBYUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROODID</td>
             <td>-</td>
             <td colspan="2">現在、プルーフ テーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>PROOWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROOFSTAGEID</td>
             <td>FK</td>
             <td>-</td>
             <td colspan="2">現在、プルーフステージテーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 為替レート

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>為替レート</td>
            <td>為替レート</td>
            <td>EXRATE</td>
            <td>為替レート</td>
            <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### 費用

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>費用</td>
            <td>費用</td>
            <td>EXPNS</td>
            <td>費用</td>
            <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXPENSEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>FK</td>
             <td>EXPENSETYPES_CURRENT</td>
             <td>EXPENSETYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>TOPBJCODE に基づく変数</td>
             <td>TOPBJCODE フィールドで識別されるオブジェクトのプライマリキー/ ID</td>
        </tr>
    </tbody>
</table>

### 費用タイプ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>費用タイプ</td>
            <td>費用タイプ</td>
            <td>EXPTYPE</td>
            <td>費用タイプ</td>
            <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>EXPENSETYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### グループ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>グループ</td>
            <td>グループ</td>
            <td>グループ</td>
            <td>グループ</td>
            <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>BUSINESSLEADERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ROOTID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### 時間

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>時間</td>
            <td>時間</td>
            <td>時間</td>
            <td>時間</td>
            <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>DUPID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>EXTERNALTIMESHEETID</td>
             <td>-</td>
             <td colspan="2">Workfrontの関係ではありません。外部システムへの統合に使用します。
Self</td>
        </tr>
        <tr>
             <td>フーリド</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTORVERHEADID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
    </tbody>
</table>

### 時間タイプ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>時間タイプ</td>
            <td>時間タイプ</td>
            <td>時間</td>
            <td>時間タイプ</td>
            <td>HOURTYPES_CURRENT<br>HOURTYPES_DAILY_HISTORY<br>HOURTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>HOURTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### イテレーション

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>イテレーション</td>
            <td>イテレーション</td>
            <td>ITRN</td>
            <td>イテレーション</td>
            <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
    </tbody>
</table>

### ジャーナルエントリ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ジャーナルエントリ</td>
            <td>ジャーナルエントリ</td>
            <td>ジャングル</td>
            <td>ジャーナルエントリ</td>
            <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERSTATUSID</td>
             <td>FK</td>
             <td>APPROVERSTATES_CURRENT</td>
             <td>APPROVERSTATUSID</td>
        </tr>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">監査レコード テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>ベースライン ID</td>
             <td>FK</td>
             <td>BASELINES_CURRENT</td>
             <td>ベースライン ID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>DOCUMENTSHAREID</td>
             <td>-</td>
             <td colspan="2">ドキュメント共有テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>EDITEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXPENSEID</td>
             <td>FK</td>
             <td>EXPENSES_CURRENT</td>
             <td>EXPENSEID</td>
        </tr>
        <tr>
             <td>フーリド</td>
             <td>FK</td>
             <td>HOURS_CURRENT</td>
             <td>フーリド</td>
        </tr>
        <tr>
             <td>INITIATIVEID</td>
             <td>-</td>
             <td colspan="2">現在、イニシアチブ テーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>JOURNALENTRIESID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>類ポートフォリオ</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>類ポートフォリオ</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SUBOBJID</td>
             <td>FK</td>
             <td>変数（SUBOBJCODE に基づく）</td>
             <td>SUBOBJCODE フィールドで識別されるプライマリキー/ オブジェクトの ID</td>
        </tr>
        <tr>
             <td>SUBSCRIBEID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>TOPOBJCODE に基づく変数</td>
             <td>TOPOBJCODE フィールドで識別されるオブジェクトのプライマリキー/ID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### リンクされたフォルダー

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>リンクされたフォルダー</td>
            <td>リンクされたフォルダー</td>
            <td>LNKFDR</td>
            <td>LinkedFolder</td>
            <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCUMENTPROVIDERID</td>
             <td>FK</td>
             <td>DOCPROVIDERS_CURRENT</td>
             <td>DOCUMENTPROVIDERID</td>
        </tr>
        <tr>
             <td>EXTERNALSTORAGEID</td>
             <td>-</td>
             <td colspan="2">外部ストレージシステムの外部 ID</td>
        </tr>
        <tr>
             <td>FOLDERID</td>
             <td>FK</td>
             <td>DOCFOLDERS_CURRENT</td>
             <td>FOLDERID</td>
        </tr>
        <tr>
             <td>LINKEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LINKEDFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### マイルストーン

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>マイルストーン</td>
            <td>マイルストーン</td>
            <td>マイル</td>
            <td>マイルストーン</td>
            <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### マイルストーンパス

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>マイルストーンパス</td>
            <td>マイルストーンパス</td>
            <td>MPATH</td>
            <td>マイルストーンパス</td>
            <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 労力以外のリソース

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>労力以外のリソース</td>
            <td>労力以外のリソース</td>
            <td>NLBR</td>
            <td>労力以外のリソース</td>
            <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NONLABORRESOURCECATEGORYID</td>
             <td>FK</td>
             <td>NLBRCATEGORIES_CURRENT</td>
             <td>NLBRCATEGORYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 労力以外のリソースカテゴリ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>労力以外のリソースカテゴリ</td>
            <td>労力以外のリソースカテゴリ</td>
            <td>NLBRCY</td>
            <td>労力以外のリソースカテゴリ</td>
            <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>NLBRCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 非稼働日

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>非稼働日</td>
            <td>スケジュールの例外</td>
            <td>非世界貿易型の</td>
            <td>非稼働日</td>
            <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>NONWORKDAYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### メモ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>メモ</td>
            <td>メモ</td>
            <td>メモ</td>
            <td>メモ</td>
            <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ATTACHDOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>ATTACHOBJID</td>
             <td>FK</td>
             <td>変数（ATTACHOBJCODE に基づく）</td>
             <td>OBJCODE ATTACHOBJCODE で識別されるオブジェクトのプライマリ・キー/ID</td>
        </tr>
        <tr>
             <td>ATTACHOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>ATTACHWORKID</td>
             <td>FK</td>
             <td>作業項目_現在</td>
             <td>WORKITEMID</td>
        </tr>
        <tr>
             <td>ATTACHWORKUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>AUDITRECORDID</td>
             <td>-</td>
             <td colspan="2">現在、監査レコード テーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DOCUMENTID</td>
             <td>FK</td>
             <td>DOCUMENTS_CURRENT</td>
             <td>DOCUMENTID</td>
        </tr>
        <tr>
             <td>EXTERNALSERVICEID</td>
             <td>-</td>
             <td colspan="2">Workfrontの関係ではありません。外部システムへの統合に使用します。</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>NOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>変数（NOTEOBJCODE に基づく）</td>
             <td>NOTEOBJCODE フィールドで識別されるオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARENTENDORSEMENTID</td>
             <td>-</td>
             <td colspan="2">推奨テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>PARENTJOURNALENTRYID</td>
             <td>FK</td>
             <td>JOURNALENTRIES_CURRENT</td>
             <td>JOURNALENTRYID</td>
        </tr>
        <tr>
             <td>PARENTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>類ポートフォリオ</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>類ポートフォリオ</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROOFACTIONID</td>
             <td>-</td>
             <td colspan="2">プルーフアクションテーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>PROODID</td>
             <td>-</td>
             <td colspan="2">現在、プルーフ テーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>FK</td>
             <td>RESERVEDTEXTNOTES_CURRENT</td>
             <td>RICHTEXTNOTEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>THREADID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>FK</td>
             <td>TIMESHEETS_CURRENT</td>
             <td>TIMESHEETID</td>
        </tr>
        <tr>
             <td>TOPOBJID</td>
             <td>FK</td>
             <td>TOPOBJCODE に基づく変数</td>
             <td>TOPOBJCODE フィールドで識別されるオブジェクトのプライマリキー/ID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>


    &lt;/tbody>
</table>

### オブジェクトの統合

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>オブジェクトの統合</td>
            <td>オブジェクトの統合</td>
            <td>OBJECT</td>
            <td>ObjectIntegration</td>
            <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LINKEDOBJECTID</td>
             <td>FK</td>
             <td>変数（LINKEDOBJECTCODE に基づく）</td>
             <td>LINKEDOBJECTCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>OBJECTINTEGRATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>

    &lt;/tbody>
</table>

### オブジェクトカテゴリ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>オブジェクトカテゴリ</td>
            <td>オブジェクトカテゴリ</td>
            <td>OBJCAT</td>
            <td>オブジェクト カテゴリ</td>
            <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>OBJECTSCATEGORYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### Op タスク/問題

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>OpTask</td>
            <td>問題、要求</td>
            <td>OPTASK</td>
            <td>イシュー</td>
            <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>譲渡病様</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">現在、かんばんボードテーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">現在、キュー定義テーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>QUEUETOPICID</td>
             <td>-</td>
             <td colspan="2">キュートピック テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>RESOLVEOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOLVEPROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOLVETASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>RESOLVINGOBJID</td>
             <td>FK</td>
             <td>変数（RESOLVINGOBJCODE に基づく）</td>
             <td>RESOLVINGOBJCODE フィールドで識別されるオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SOURCEOBJID</td>
             <td>FK</td>
             <td>変数（SOURCEOBJCODE に基づく）</td>
             <td>SOURCEOBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>SOURCERETASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
    </tbody>
</table>

### パラメーター

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>パラメーター</td>
            <td>カスタムフィールド</td>
            <td>パラメーター</td>
            <td>パラメーター</td>
            <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERFILTERID</td>
             <td>-</td>
             <td colspan="2">パラメーターフィルターテーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>パラメーター ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### パラメーターグループ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>パラメーターグループ</td>
            <td>フォームセクション</td>
            <td>パラメーター</td>
            <td>パラメーターグループ</td>
            <td>PARAMETERGROUPS_CURRENT<br>PARAMETERGROUPS_DAILY_HISTORY<br>PARAMETERGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PARAMETERGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### パラメーターオプション

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>パラメーターオプション</td>
            <td>パラメーターオプション</td>
            <td>POPT</td>
            <td>パラメーターオプション</td>
            <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>パラメーター ID</td>
             <td>FK</td>
             <td>PARAMETERS_CURRENT</td>
             <td>パラメーター ID</td>
        </tr>
        <tr>
             <td>PARAMETEROPTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ポータルセクション/レポート

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ポータル セクション</td>
            <td>レポート</td>
            <td>PTLSEC</td>
            <td>レポート</td>
            <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>フィルター</td>
             <td>FK</td>
             <td>UIFILTERS_CURRENT</td>
             <td>フィルター</td>
        </tr>
        <tr>
             <td>GROUPBYID</td>
             <td>FK</td>
             <td>UIGROUBYS_CURRENT</td>
             <td>GROUPBYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTVIEWEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>PORTALSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>PUBLICRUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>FK</td>
             <td>REPORTFOLDERS_CURRENT</td>
             <td>REPORTFOLDERID</td>
        </tr>
        <tr>
             <td>RUNASUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SCHEDULEDREPORTID</td>
             <td>-</td>
             <td colspan="2">スケジュール済み報告書テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>VIEWID</td>
             <td>FK</td>
             <td>UI_CURRENT</td>
             <td>VIEWID</td>
        </tr>
    </tbody>
</table>

### 「ポータル」タブ/ダッシュボード

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>「ポータル」タブ</td>
            <td>ダッシュボード</td>
            <td>PTLTAB</td>
            <td>ダッシュボード</td>
            <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>DOCID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### ポータルのタブセクション

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ポータルのタブセクション</td>
            <td>ダッシュボードセクション</td>
            <td>PRTBSC</td>
            <td>ポータルのタブセクション</td>
            <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CALENDARPORTALSECTIONID</td>
             <td>-</td>
             <td colspan="2">カレンダーポータルセクションは現在サポートされていません</td>
        </tr>
        <tr>
             <td>EXTERNALSECTIONID</td>
             <td>-</td>
             <td colspan="2">外部セクション テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>INTERNALSECTIONID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>PORTALSECTIONOBJID</td>
             <td>FK</td>
             <td>変数（PORTALSECTIONOBJCODE に基づく）</td>
             <td>PORTALSECTIONOBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>PORTALTABID</td>
             <td>FK</td>
             <td>PORTALTABS_CURRENT</td>
             <td>PORTALTABID</td>
        </tr>
        <tr>
             <td>PORTALTABSECTIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ポータル セクションの最終閲覧者

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>PortalSectionLastViewer</td>
            <td>最終閲覧者のレポート</td>
            <td>PLSLSV</td>
            <td>PortalSectionLastViewer</td>
            <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>REPORTID</td>
        </tr>
        <tr>
             <td>REPORTLASTVIEWERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>VIEWERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### ポートフォリオ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ポートフォリオ</td>
            <td>ポートフォリオ</td>
            <td>PORT</td>
            <td>ポートフォリオ</td>
            <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">スコアカードテーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>類ポートフォリオ</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 設定

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>設定</td>
            <td>表示，フィルター，グループ化，レポート定義</td>
            <td>PROSET</td>
            <td>設定</td>
            <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### プログラム

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>プログラム</td>
            <td>プログラム</td>
            <td>PRGM</td>
            <td>プログラム</td>
            <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>類ポートフォリオ</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>類ポートフォリオ</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### プロジェクト

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>プロジェクト</td>
            <td>プロジェクト</td>
            <td>PROJ</td>
            <td>プロジェクト</td>
            <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>AEMNATIVEFOLDERTREESREFID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ALIGNMENTSCORECARDID</td>
             <td>-</td>
             <td colspan="2">スコアカードテーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>ATTACHEDRATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">スコアカードテーブルは現在サポートされていません</td>
        </tr>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>POPACCOUNTID</td>
             <td>-</td>
             <td colspan="2">現在、POP アカウント テーブルはサポートされていません。</td>
        </tr>
        <tr>
             <td>類ポートフォリオ</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>類ポートフォリオ</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">現在、キュー定義テーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SPONSORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### プロジェクト チーム ユーザー

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>プロジェクト チーム ユーザー</td>
            <td>プロジェクト チーム ユーザー</td>
            <td>PRTU</td>
            <td>プロジェクトユーザー</td>
            <td>PROJECTSUSERS_CURRENT<br>PROJECTSUSERS_DAILY_HISTORY<br>PROJECTSUSERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TMPUSERID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### プロジェクト チーム ユーザーの役割

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>プロジェクト チーム ユーザーの役割</td>
            <td>プロジェクト チーム ユーザーの役割</td>
            <td>PTEAM</td>
            <td>ProjectUserRole</td>
            <td>PROJECTSUSERSROLES_CURRENT<br>PROJECTSUSERSROLES_DAILY_HISTORY<br>PROJECTSUSERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>PROJECTSUSERSROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### レートカード

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>レートカード</td>
            <td>レートカード</td>
            <td>RTCRD</td>
            <td>レートカード</td>
            <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RATECARDID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SECURITYROOTID</td>
             <td>FK</td>
             <td>SECURITYOBJECT コードに基づく変数</td>
             <td>SECURITYOBJCODE フィールドで識別されたオブジェクトのプライマリ・キー/ID</td>
        </tr>
        <tr>
             <td>SOURCEID</td>
             <td>FK</td>
             <td>変数（SOURCEOBJCODE に基づく）</td>
             <td>SOURCEOBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>

    &lt;/tbody>
</table>

### 報告書フォルダー

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>報告書フォルダー</td>
            <td>報告書フォルダー</td>
            <td>RPTFDR</td>
            <td>報告書フォルダー</td>
            <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTFOLDERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### レポート表示統計数

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>レポート表示統計数</td>
            <td>レポート表示統計数</td>
            <td>PLSVST</td>
            <td>PortalSectionStatisticInfo</td>
            <td>REPORTVIEWSTATISTICCOUNTS_CURRENT<br>REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>REPORTID</td>
             <td>FK</td>
             <td>PORTALSECTIONS_CURRENT</td>
             <td>PORTALSECTIONID</td>
        </tr>
        <tr>
             <td>REPORTVIEWSTATISTICCOUNTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 報告可能な予算計上時間数

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>報告可能な予算計上時間数</td>
            <td>報告可能な予算計上時間数</td>
            <td>RPBGHR</td>
            <td>予算計上時間数</td>
            <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REPORTABLEBUDGETEDHOURID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### 予約時間/PTO

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>予約時間</td>
            <td>（個人）休暇</td>
            <td>RESVT</td>
            <td>休暇</td>
            <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### リソース管理者

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>リソース管理者</td>
            <td>リソース管理者</td>
            <td>RESMGR</td>
            <td>リソース管理者</td>
            <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RESOURCEMANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### リソースプール

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>リソースプール</td>
            <td>リソースプール</td>
            <td>RSPL</td>
            <td>リソースプール</td>
            <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### Rich Text メモ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>Rich Text メモ</td>
            <td>Rich Text メモ</td>
            <td>RHNOTE</td>
            <td>Rich Text メモ</td>
            <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RICHTEXTNOTEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### リッチテキストパラメーター値

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>リッチテキストパラメーター値</td>
            <td>リッチテキストパラメーター値</td>
            <td>CHVAL</td>
            <td>RichTextParameterValue</td>
            <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PARAMETERVALUEID</td>
             <td>-</td>
             <td colspan="2">パラメーター値テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>RICHTEXTPARAMETERVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### リスク

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>リスク</td>
            <td>リスク</td>
            <td>危険</td>
            <td>リスク</td>
            <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RISKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>RISKTYPEID</td>
             <td>FK</td>
             <td>RISKTYPES_CURRENT</td>
             <td>RISKTYPEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
    </tbody>
</table>

### リスクタイプ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>リスクタイプ</td>
            <td>リスクタイプ</td>
            <td>RSKTYPE</td>
            <td>リスクタイプ</td>
            <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>RISKTYPEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 役割

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>役割</td>
            <td>担当業務</td>
            <td>役割</td>
            <td>担当業務</td>
            <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">レイアウトテンプレートテーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### スケジュール

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>スケジュール</td>
            <td>スケジュール</td>
            <td>SCHED</td>
            <td>スケジュール</td>
            <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ステップ承認者

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ステップ承認者</td>
            <td>ステップ承認者</td>
            <td>SPAPVR</td>
            <td>ステージ承認者</td>
            <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>STEPAPPROVERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### タスク

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>タスク</td>
            <td>タスク</td>
            <td>タスク</td>
            <td>タスク</td>
            <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>譲渡病様</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>BILLINGRECORDID</td>
             <td>FK</td>
             <td>BILLINGRECORDS_CURRENT</td>
             <td>BILLINGRECORDID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>CONVERTEDOPTASKORIGINATORID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CURRENTAPPROVALSTEPID</td>
             <td>FK</td>
             <td>APPROVALSTEPS_CURRENT</td>
             <td>APPROVALSTEPID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>ITERATIONID</td>
             <td>FK</td>
             <td>ITERATIONS_CURRENT</td>
             <td>ITERATIONID</td>
        </tr>
        <tr>
             <td>KANBANBOARDID</td>
             <td>-</td>
             <td colspan="2">現在、かんばんボードテーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>LASTCONDITIONNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">繰り返しルールテーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>REJECTIONISSUEID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>RESERVEDTIMEID</td>
             <td>FK</td>
             <td>RESERVEDTIMES_CURRENT</td>
             <td>RESERVEDTIMEID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SUBMITTEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>SUBMITTEDBYID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### タスクの先行タスク

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>タスクの先行タスク</td>
            <td>先行タスク</td>
            <td>先行</td>
            <td>先行タスク</td>
            <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### チーム

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>チーム</td>
            <td>チーム</td>
            <td>TEAMOB</td>
            <td>チーム</td>
            <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">レイアウトテンプレートテーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>MYWORKVIEWID</td>
             <td>FK</td>
             <td>UI_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>REQUESTSVIEWID</td>
             <td>FK</td>
             <td>UI_CURRENT</td>
             <td>UIVIEWID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
    </tbody>
</table>

### チームメンバー

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>チームメンバー</td>
            <td>その他のチーム、チームメンバー</td>
            <td>TEAMMB</td>
            <td>チームメンバー</td>
            <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>TEAMMEMBERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### チーム メンバーの役割

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>チーム メンバーの役割</td>
            <td>チーム メンバーの役割</td>
            <td>チーム</td>
            <td>チーム メンバーの役割</td>
            <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>TEAMMEMBERROLEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### テンプレート

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>テンプレート</td>
            <td>テンプレート、プロジェクトテンプレート</td>
            <td>TMPL</td>
            <td>テンプレート</td>
            <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DELIVERABLESCORECARDID</td>
             <td>-</td>
             <td colspan="2">成果物のスコアカード テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEPATHID</td>
             <td>FK</td>
             <td>MILESTONEPATHS_CURRENT</td>
             <td>MILESTONEPATHID</td>
        </tr>
        <tr>
             <td>OWNERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>QUEUEDEFID</td>
             <td>-</td>
             <td colspan="2">現在、キュー定義テーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### テンプレート タスク割り当て

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>テンプレート タスク割り当て</td>
            <td>テンプレートの割り当て</td>
            <td>集計</td>
            <td>テンプレートの割り当て</td>
            <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>譲渡病様</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">Team Timelineable テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>TEMPLATEASSIGNMENTID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
    </tbody>
</table>

### テンプレートタスク

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>テンプレートタスク</td>
            <td>テンプレートタスク</td>
            <td>TTSK</td>
            <td>テンプレートタスク</td>
            <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVALPROCESSID</td>
             <td>FK</td>
             <td>APPROVALPROCESSES_CURRENT</td>
             <td>APPROVALPROCESSID</td>
        </tr>
        <tr>
             <td>譲渡病様</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EXCHANGERATEID</td>
             <td>FK</td>
             <td>EXCHANGERATES_CURRENT</td>
             <td>EXCHANGERATEID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>MILESTONEID</td>
             <td>FK</td>
             <td>MILESTONES_CURRENT</td>
             <td>MILESTONEID</td>
        </tr>
        <tr>
             <td>PARENTID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>RECURRENCERULEID</td>
             <td>-</td>
             <td colspan="2">繰り返しルールテーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ティーミド</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>TEAMTIMELINEABLEID</td>
             <td>-</td>
             <td colspan="2">Team Timelineable テーブルは現在サポートされていません</td>
        </tr>
        <tr>
             <td>TEMPLATEID</td>
             <td>FK</td>
             <td>TEMPLATES_CURRENT</td>
             <td>TEMPLATEID</td>
        </tr>
        <tr>
             <td>TEMPLATETASKID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### テンプレート タスクの先行タスク

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>テンプレート タスクの先行タスク</td>
            <td>テンプレートの先行タスク</td>
            <td>TPRED</td>
            <td>先行タスク</td>
            <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>PREDECESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>SUCCESSORID</td>
             <td>FK</td>
             <td>TEMPLATETASKS_CURRENT</td>
             <td>TEMPLATETASKID</td>
        </tr>
        <tr>
             <td>TEMPLATEPREDECESSORID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### 期間別 KPI 通貨

お客様の限定提供

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>期間別 KPI 通貨</td>
            <td>期間別の KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_CURRENCY_CURRENT<br>TIMEPHASED_CURRENCY_DAILY_HISTORY<br>TIMEPHASED_CURRENCY_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>類ポートフォリオ</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>類ポートフォリオ</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>まもなく追加されます</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCERETASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDCURRENCYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### 期間別 KPI 期間

お客様の限定提供

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>期間別 KPI 期間</td>
            <td>期間別の KPI</td>
            <td>TMPH</td>
            <td>TimePhasedKPI</td>
            <td>TIMEPHASED_DURATION_CURRENT<br>TIMEPHASED_DURATION_DAILY_HISTORY<br>TIMEPHASED_DURATION_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LOCATIONID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>類ポートフォリオ</td>
             <td>FK</td>
             <td>PORTFOLIOS_CURRENT</td>
             <td>類ポートフォリオ</td>
        </tr>
        <tr>
             <td>PROGRAMID</td>
             <td>FK</td>
             <td>PROGRAMS_CURRENT</td>
             <td>PROGRAMID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>REFERENCEID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEMAID</td>
             <td>FK</td>
             <td>まもなく追加されます</td>
             <td>SCHEMAID</td>
        </tr>
        <tr>
             <td>SOURCERETASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>TIMEPHASEDDURATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### タイムシート

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>タイムシート</td>
            <td>タイムシート</td>
            <td>TSHET</td>
            <td>タイムシート</td>
            <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TIMESHEETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### 定期タイムシート

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>定期タイムシート</td>
            <td>定期タイムシート</td>
            <td>TSPRO</td>
            <td>定期タイムシート</td>
            <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPROVERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI フィルター

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI フィルター</td>
            <td>フィルター</td>
            <td>UFT</td>
            <td>フィルター</td>
            <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>UIFILTERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI グループ化基準

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI グループ化基準</td>
            <td>グループ化</td>
            <td>UIGB</td>
            <td>グループ化</td>
            <td>UIGROUBYS_CURRENT<br>UIGROUBYS_DAILY_HISTORY<br>UIGROUBYS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>UIGROUPBYID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI テンプレート

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI テンプレート</td>
            <td>レイアウトテンプレート</td>
            <td>UITMPL</td>
            <td>レイアウトテンプレート</td>
            <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### UI ビュー

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UI ビュー</td>
            <td>表示</td>
            <td>UIVIEW</td>
            <td>表示</td>
            <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>APPGLOBALID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>PREFERENCEID</td>
             <td>FK</td>
             <td>PREFERENCES_CURRENT</td>
             <td>PREFERENCEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>UIVIEWID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### ユーザー

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ユーザー</td>
            <td>ユーザー</td>
            <td>ユーザー</td>
            <td>ユーザー</td>
            <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ACCESSLEVELID</td>
             <td>FK</td>
             <td>ACCESSLEVEL_CURRENT</td>
             <td>ACCESSLEVELID</td>
        </tr>
        <tr>
             <td>CATEGORYID</td>
             <td>FK</td>
             <td>CATEGORIES_CURRENT</td>
             <td>CATEGORYID</td>
        </tr>
        <tr>
             <td>COMPANYID</td>
             <td>FK</td>
             <td>COMPANIES_CURRENT</td>
             <td>COMPANYID</td>
        </tr>
        <tr>
             <td>DEFAULTHOURTYPEID</td>
             <td>FK</td>
             <td>HOURTYPES_CURRENT</td>
             <td>HOURTYPEID</td>
        </tr>
        <tr>
             <td>委任状</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>EAUTHUSERID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>ENTEREDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>HOMEGROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>HOMETEAMID</td>
             <td>FK</td>
             <td>TEAMS_CURRENT</td>
             <td>ティーミド</td>
        </tr>
        <tr>
             <td>LASTENTEREDNOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LASTUPDATEDBYID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>LATESTUPDATENOTEID</td>
             <td>FK</td>
             <td>NOTES_CURRENT</td>
             <td>NOTEID</td>
        </tr>
        <tr>
             <td>LAYOUTTEMPLATEID</td>
             <td>-</td>
             <td colspan="2">レイアウトテンプレートテーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>MANAGERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>PORTALPROFILEID</td>
             <td>-</td>
             <td colspan="2">ポータル プロファイル テーブルはサポートされていません</td>
        </tr>
        <tr>
             <td>PREFUID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>PRIVATERATECARDID</td>
             <td>FK</td>
             <td>RATECARD_CURRENT</td>
             <td>RATECARDID</td>
        </tr>
        <tr>
             <td>RESOURCEPOOLID</td>
             <td>FK</td>
             <td>RESOURCEPOOLS_CURRENT</td>
             <td>RESOURCEPOOLID</td>
        </tr>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SCHEDULEID</td>
             <td>FK</td>
             <td>SCHEDULES_CURRENT</td>
             <td>SCHEDULEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TIMESHEETPROFILEID</td>
             <td>FK</td>
             <td>TIMESHEETPROFILES_CURRENT</td>
             <td>TIMESHEETPROFILEID</td>
        </tr>
        <tr>
             <td>UITEMPLATEID</td>
             <td>FK</td>
             <td>UITEMPLATES_CURRENT</td>
             <td>UITEMPLATEID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>UUMUSERID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
    </tbody>
</table>

### ユーザーの委任

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ユーザーの委任</td>
            <td>ユーザーの委任</td>
            <td>USRDEL</td>
            <td>ユーザーの委任</td>
            <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>FROMUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TOUSERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERDELEGATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### ユーザー グループ

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ユーザー グループ</td>
            <td>その他のグループ</td>
            <td>USRGPS</td>
            <td>ユーザー グループ</td>
            <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>GROUPID</td>
             <td>FK</td>
             <td>GROUPS_CURRENT</td>
             <td>GROUPID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERSGROUPID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### ユーザーの場所

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ユーザーの場所</td>
            <td>ユーザーの場所</td>
            <td>USRLOC</td>
            <td>UserLocation</td>
            <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>CLASSIFIERID</td>
             <td>FK</td>
             <td>CLASSIFIER_CURRENT</td>
             <td>CLASSIFIERID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### ユーザーの役割

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ユーザーの役割</td>
            <td>その他の役割</td>
            <td>USRROL</td>
            <td>ユーザーの役割</td>
            <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ROLEID</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>FK</td>
             <td>USERROLESET_CURRENT</td>
             <td>USERROLESETID</td>
        </tr>
        <tr>
             <td>USERLOCATIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### ユーザー設定値

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>ユーザーの環境設定の値</td>
            <td>ユーザー設定</td>
            <td>USERPF</td>
            <td>ユーザー設定</td>
            <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERPREFVALUEID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### ユーザーの役割セット

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UserRoleSet</td>
            <td>ユーザーの役割セット</td>
            <td>URSET</td>
            <td>UserRoleSet</td>
            <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>初産婦</td>
             <td>FK</td>
             <td>ROLES_CURRENT</td>
             <td>ROLEID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>USERROLESETID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>

### ユーザーの決定

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>UsersDecisions</td>
            <td>ユーザーの決定</td>
            <td>USRDEC</td>
            <td>ユーザーの決定</td>
            <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>USERDECISIONID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
    </tbody>
</table>

### 作業アイテム

<table>
    <thead>
        <tr>
            <th>Workfront エンティティ名</th>
            <th>インターフェイス参照</th>
            <th>API リファレンス</th>
            <th>API ラベル</th>
            <th>データレイクの表示</th>
        </tr>
      </thead>
      <tbody>
        <tr>
            <td>作業項目</td>
            <td>作業アイテム</td>
            <td>WRKIM</td>
            <td>作業項目</td>
            <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        </tr>
      </tbody>
</table>
<table>
    <thead>
        <tr>
            <th>プライマリ/外部キー</th>
            <th>タイプ</th>
            <th>関連テーブル</th>
            <th>関連フィールド</th>
        </tr>
    </thead>
    <tbody>
        <tr>
             <td>ASSIGNMENTID</td>
             <td>FK</td>
             <td>ASSIGNMENTS_CURRENT</td>
             <td>ASSIGNMENTID</td>
        </tr>
        <tr>
             <td>OBJID</td>
             <td>FK</td>
             <td>OBJCODE に基づく変数</td>
             <td>OBJCODE フィールドで識別されたオブジェクトのプライマリキー/ ID</td>
        </tr>
        <tr>
             <td>OPTASKID</td>
             <td>FK</td>
             <td>OPTASKS_CURRENT</td>
             <td>OPTASKID</td>
        </tr>
        <tr>
             <td>PROJECTID</td>
             <td>FK</td>
             <td>プロジェクト_現在</td>
             <td>PROJECTID</td>
        </tr>
        <tr>
             <td>SYSID</td>
             <td>-</td>
             <td colspan="2">関係ではありません。内部適用目的で使用されます</td>
        </tr>
        <tr>
             <td>TASKID</td>
             <td>FK</td>
             <td>タスク_現在</td>
             <td>TASKID</td>
        </tr>
        <tr>
             <td>USERID</td>
             <td>FK</td>
             <td>USERS_CURRENT</td>
             <td>USERID</td>
        </tr>
        <tr>
             <td>WORKITEMID</td>
             <td>PK</td>
             <td>-</td>
             <td>-</td>
        </tr>
    </tbody>
</table>
