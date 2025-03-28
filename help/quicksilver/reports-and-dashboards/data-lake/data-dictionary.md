---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect データディクショナリ
description: ここでは、Workfront Data Connect のデータの構造と内容について説明します。
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: eccc878f4b6fdeeffbcd5635b80ac3e26f7fb8c6
workflow-type: tm+mt
source-wordcount: '4719'
ht-degree: 4%

---

# Workfront Data Connect データディクショナリ

ここでは、Workfront Data Connect のデータの構造と内容について説明します。

>[!NOTE]
>
>データ接続のデータは 4 時間ごとに更新されるので、最近の変更がすぐには反映されない場合があります。

## テーブルタイプ

データ接続で使用して、最もインサイトを得られる方法でWorkfront データを表示できるテーブルタイプは多数あります。

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

<table>
  <thead>
    <tr>
        <th>Workfront エンティティ名</th>
        <th>インターフェイス参照</th>
        <th>API リファレンス | ラベル</th>
        <th>Data Lake テーブル</th>
        <th>関係フィールド</th>
        <th>関係テーブルとフィールド</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>アクセスレベル</td>
        <td>アクセスレベル</td>
        <td>ACSLVL | アクセス レベル</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELID （self） <br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Self<br>Not 関係。内部アプリケーションの目的で使用されます <br>USER_CURRENT | USERID<br> 関係ではありません。内部アプリケーション目的で使用されます。<br>OBJCODE フィールドで識別されるオブジェクトの ID<br> 関係ではありません。内部アプリケーション目的で使用されます。</td>
    </tr>
    <tr>
        <td>アクセスルール</td>
        <td>共有</td>
        <td>ACSRUL |共有</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br>ACCESSRULEID （self） <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>ACCESSOROBJCODE フィールドで識別されるオブジェクトの ID<br>Self<br>ANCESTOROBJCODE フィールドで識別されるオブジェクトの ID<br>USERS_CURRENT | USERID<br>SECURITYOBJCODE フィールドで識別されるオブジェクトの ID<br> リレーションシップではありません。内部アプリケーションの目的で使用されます</td>
    </tr>
    <tr>
        <td>承認パス</td>
        <td>承認パス</td>
        <td>ARVPTH |承認</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td>APPROVALPATHID （セルフ） <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションに使用されます</td>
    </tr>
    <tr>
        <td>承認プロセス</td>
        <td>承認プロセス</td>
        <td>ARVPRC |承認プロセス</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td>APPROVALPROCESSID （self） <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションに使用されます</td>
    </tr>
    <tr>
        <td>承認ステップ</td>
        <td>承認ステップ</td>
        <td>ARVSTP |承認ステージ</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td>APPROVALPATHID <br>APPROVALSTEPID （self） <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br> 関係ではありません。内部適用のために使用されます</td>
    </tr>
    <tr>
        <td>ApproverStatus</td>
        <td>上書きされている</td>
        <td>ARVSTS |承認者の状態</td>
        <td>APPROVERSTATES_CURRENT<br>APPROVERSTATES_DAILY_HISTORY<br>APPROVERSTATES_EVENT</td>
        <td>APPROVERSTATUSID （self） <br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>APPROVABLEOBJCODE フィールドで識別されるオブジェクト ID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | ユーザー ID <br>USERS_CURRENT | USERID<br>USERS_CURRENT | ユーザー ID <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>割り当て</td>
        <td>割り当て</td>
        <td>割り当て |割り当て</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID （self） <br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>Classifier テーブルは現在サポートされていません <br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>承認待ち</td>
        <td>承認待ち</td>
        <td>AWAPVL |承認待ち</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID （self） <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>アクセス要求テーブルは現在サポートされていません <br> リレーションシップではありません。内部アプリケーションの目的で使用されます <br>USERS_CURRENT | USERID<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJECTS_CURRENT | PROJECTID<br>ROLES_CURRENT | ROLEID<br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>TASKS_CURRENT | TASKID<br>TEAMS_CURRENT | TEAMID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>ベースライン</td>
        <td>ベースライン</td>
        <td>ブリン | ベースライン</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td>BASELINEID （self） <br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br> 関係ではありません。内部適用のために使用されます</td>
    </tr>
    <tr>
        <td>ベースライン タスク</td>
        <td>ベースライン タスク</td>
        <td>BSTSK | ベースライン タスク</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td>BASELINEID<br>BASELINETASKID （self） <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br> リレーションシップではありません。内部アプリケーションの目的で使用されます <br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>請求レート</td>
        <td>レートまたはレートの上書き</td>
        <td>率 |請求料率</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>RATECARDID<br>RATEID （自己） <br>ROLEID<br>SOURCERATECARDID<br>SYSID<br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>Classifier テーブルは現在サポートされていません <br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br> 労力以外のリソース カテゴリ テーブルは現在サポートされていません <br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>OBJCODE フィールドで識別されるオブジェクトの ID<br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>ROLES_CURRENT | ROLEID <br>RATECARD_CURRENT | RATECARDID <br> 関係ではありません。内部アプリケーション用に使用されます <br>TEMPLATES_CURRNT | TEMPLATEID<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>請求記録</td>
        <td>請求記録</td>
        <td>請求書 |請求記録</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID （self） <br>CATEGORYID<br>EXCHANGERATEID <br>INVOICEID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br> 請求書テーブルは現在サポートされていません <br>USERS_CURRENT | ユーザー ID <br>PROJECTS_CURRENT | PROJECTID   <br> 関係ではありません。内部適用目的で使用されます</td>
    </tr>
    <tr>
        <td>予約</td>
        <td>予約</td>
        <td>予約 |予約</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td>BOOKINGID （self） <br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br> 労力以外のリソース カテゴリ テーブルは現在サポートされていません <br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>OBJOBJCODE フィールドで識別されるオブジェクトの ID<br>PROJECTS_CURRENT | PROJECTID <br> リレーションシップではありません。内部アプリケーションの目的で使用されます <br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>TOPOBJCODE フィールドで識別されるオブジェクトの ID</td>
    </tr>
    <tr>
        <td>ビジネスプロファイル</td>
        <td>ビジネスプロファイル</td>
        <td>BSNPRF | ビジネスプロファイル</td>
        <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        <td>ACCESSLEVELID<br>BUSINESSPROFILEID （self） <br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>ACCESSLEVEL_CURRENT | ACCESSLEVELID<br>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションに使用されます</td>
    </tr>
    <tr>
        <td>ビジネスルール</td>
        <td>ビジネスルール</td>
        <td>BSNRUL | ビジネス ルール</td>
        <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        <td>BUSINESSRULEID （self） <br>ENTEREDBYID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションに使用されます</td>
    </tr>
    <tr>
        <td>カテゴリ</td>
        <td>カスタムフォーム</td>
        <td>CTGY | カテゴリ</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td>CATEGORYID （self） <br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションに使用されます</td>
    </tr>
    <tr>
        <td>カテゴリパラメーター</td>
        <td>カスタムフォームフィールド</td>
        <td>CTGYPA | カテゴリパラメーター</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID （self） <br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID<br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br> パラメーターグループ テーブルは現在サポートされていません <br>PARAMETERS_CURRENT | パラメーター ID    <br> 関係ではありません。内部適用目的で使用されます</td>
    </tr>
    <tr>
        <td>分類子</td>
        <td>Location</td>
        <td>CLSF |場所</td>
        <td>CLASSIFIER_CURRENT<br>CLASSIFIER_DAILY_HISTORY<br>CLASSIFIER_EVENT</td>
        <td>CLASSIFIERID （self） <br>ENTEREDBYID<br>LASTUPDATEDBYID<br>PARENTID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | ユーザー ID<br> 分類子_現在 | CLASSIFIERID<br> 関係ではありません。内部適用のために使用されます</td>
    </tr>
    <tr>
        <td>会社</td>
        <td>会社</td>
        <td>CMPY |会社</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td>CATEGORYID<br>COMPANYID （self） <br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | ユーザー ID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | ユーザー ID <br>RATECARD_CURRENT | RATECARDID<br> 関係ではありません。内部適用目的で使用されます</td>
    </tr>
    <tr>
        <td>カスタム四半期</td>
        <td>カスタム四半期</td>
        <td>CSTQRT |カスタム四半期</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td>CUSTOMQUARTERID （self） <br>SYSID</td>
        <td>自己 <br> 関係ではありません。内部申請のために使用されます</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>条件、優先度、重要度、ステータス</td>
        <td>システム | カスタム列挙</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT<br>* レコードのタイプは、「enumClass」プロパティを使用して識別されます。 必要なタイプは次のとおりです。<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>ドキュメント</td>
        <td>ドキュメント</td>
        <td>DOCU | ドキュメント</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASEVERSIONID<br>TASKID TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID<br>USERID<br></td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Self<br>Document Request テーブルは現在サポートされていません <br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | DOCOBJCODE 値 <br>OPTASK_CURRENT に応じた NOTEID<br>Varibale | OPTASKID<br>USER_CURRENT | ユーザー ID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Release バージョン テーブルは現在サポートされていません <br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>TOPOBJCODE value<br>USER_CURRENT に応じた変数 | ユーザー ID</td>
    </tr>
    <tr>
        <td>ドキュメントの承認</td>
        <td>ドキュメントの承認</td>
        <td>DOCAPL | ドキュメントの承認</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td>APPROVERID<br>DOCAPPROVALID （self） <br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | USERID <br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID <br> 関係ではありません。内部アプリケーションに使用されます</td>
    </tr>
    <tr>
        <td>ドキュメントフォルダー</td>
        <td>ドキュメントフォルダー</td>
        <td>DOCFLD | DocsFolder</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td>DOCFOLDERID （self） <br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIIOID <br>PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CURRENT | ポートフォリオ ID <br>PROGRAM_CURRENT | PROGRAMID    <br>PROJECTS_CURRENT | PROJECTID <br> リレーションシップではありません。内部アプリケーションの目的で使用されます <br>TASKS_CURRENT | TASKID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>DocumentProvideMetadata</td>
        <td>ドキュメント提供メタデータ</td>
        <td>DOCMET | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID （self） <br>SYSID</td>
        <td>自己 <br> 関係ではありません。内部申請のために使用されます</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>ドキュメント プロバイダー</td>
        <td>DOCPRO | ドキュメント プロバイダー</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID （self） <br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | ユーザー ID    <br> 関係ではありません。内部適用目的で使用されます</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>ドキュメントプロバイダー設定</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td>DOCPROVIDERCONFIGID （self） <br>SYSID</td>
        <td>自己 <br> 関係ではありません。内部申請のために使用されます</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>ドキュメントのバージョン</td>
        <td>DOCV | ドキュメント バージョン</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURRENT | USERID<br>External ID<br>Proof Approval Status テーブルは現在サポートされていません <br>USER_CURRENT | USERID<br>Proof テーブルは現在サポートされていません <br>USER_CURRENT | USERID<br>Proof ステージ テーブルは現在サポートされていません</td>
    </tr>
    <tr>
        <td>為替レート</td>
        <td>為替レート</td>
        <td>EXRATE |為替相場</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID （self） <br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>Self<br>PROJECTS_CURRENT | PROJECTID <br> リレーションシップではありません。内部アプリケーション用に使用されます <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>費用</td>
        <td>費用</td>
        <td>有効期限 |費用</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>EXPENSEID （セルフ） <br>EXPENSETYPEID<br>LASTUPDATEDBYID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATETASKID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Self <br>EXPENSETYPES_CURRENT | EXPENSETTYPEID <br>USERS_CURRENT | USERID <br>OBJCODE フィールドで識別されるオブジェクトの ID <br>PROJECTS_CURRENT | PROJECTID <br> リレーションシップではありません。内部アプリケーションの目的で使用されます <br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>TOPOBJCODE フィールドで識別されるオブジェクトの ID</td>
    </tr>
    <tr>
        <td>費用タイプ</td>
        <td>費用タイプ</td>
        <td>EXPTYPE |費用タイプ</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID<br>EXPENSETYPEID （self） <br>OBJID <br>SYSID  </td>
        <td>関係ではありません。内部アプリケーション目的で使用されます <br>Self<br>OBJCODE フィールドで識別されるオブジェクトの ID<br> 関係ではありません。内部アプリケーション目的で使用されます  </td>
    </tr>
    <tr>
        <td>グループ</td>
        <td>グループ</td>
        <td>GROUP | グループ</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Self<br>Layout テンプレート テーブルはサポートされません <br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>時間</td>
        <td>時間</td>
        <td>時間 |時間</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURRID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br>TASKID<br>ID timesheetid</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>Classifier テーブルは現在サポートされていません <br> リレーションシップではありません。内部アプリケーションの目的で使用されます <br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Workfrontのリレーションシップではありません。外部システムへの統合に使用されます <br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br> リレーションシップではありません。内部アプリケーション用に使用されます <br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TIMESHEET_CURRENT | TIMESHEETID</td>
    </tr>
    <tr>
        <td>時間タイプ</td>
        <td>時間タイプ</td>
        <td>時間 |時間タイプ</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>関係ではない。内部アプリケーション目的で使用 <br>Self<br> 関係ではない。内部アプリケーション目的で使用</td>
    </tr>
    <tr>
        <td>イテレーション</td>
        <td>イテレーション</td>
        <td>ITRN |反復</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID （self） <br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID <br>Self<br>USERS_CURRENT | ユーザー ID <br>USERS_CURRENT | USERID <br> 関係ではありません。内部アプリケーション目的で使用されます <br>TEAMS_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>ジャーナルエントリ</td>
        <td>ジャーナルエントリ</td>
        <td>ジャングル |仕訳</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID<br>BILLINGRECORDID<br>COMPANYID<br>DOCUMENTSHAREID<br><br> EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIALIVEID<br>JOURNALENTRIEID （セルフ） <br>OBJID<br>OPTASKID<br>PORTFOLIIOID<br>PROGRAMID PROJECTID<br>SUBOBJID<br>SUBSCRIBEID<br>SYSID<br><br> <br> <br> <br> <br> TASKID で TEMPLATEID を取得する</td>
        <td>APPROVERSTATES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br> 監査レコードテーブルは現在サポートされていません <br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTS_CURRENT | DOCUMENTID <br> ドキュメント共有テーブルは現在サポートされていません <br>USERS_CURRENT | USERID<br>EXPENSES_CURRENT | EXPENSEID<br>HOURS_CURRENT | HOURID<br>Initiative テーブルは現在サポートされていません <br>Self<br>OBJCODE フィールドで識別されるオブジェクトの ID<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>SUBOBJCODE フィールドで識別されるオブジェクトの ID<br>Subscribe テーブルは現在サポートされていません <br> リレーションシップではありません。内部アプリケーションの目的で使用されます <br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>TOPOBJCODE フィールドで識別されるオブジェクトの ID<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID （self） <br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>External ID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>Not a relationship；内部アプリケーション目的で使用されます  </td>
    </tr>
    <tr>
        <td>マイルストーン</td>
        <td>マイルストーン</td>
        <td>マイル | マイルストーン</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | MILESTONEID</td>
    </tr>
    <tr>
        <td>MilestonePath</td>
        <td>マイルストーンパス</td>
        <td>MPATH | マイルストーン パス</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>NonLaborResource</td>
        <td>労力以外のリソース</td>
        <td>NLBR |労力以外のリソース</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID<br>NONLABORRESOURCEID （self） <br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID<br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID<br> 労力以外のリソース カテゴリ テーブルは現在サポートされていません <br> リレーションシップではありません。内部アプリケーション目的で使用されます</td>
    </tr>
    <tr>
        <td>労力以外のリソースカテゴリ</td>
        <td>労力以外のリソースカテゴリ</td>
        <td>NLBRCY |労力以外のリソースカテゴリ</td>
        <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID （self） <br>PRIVATERATECARDID<br>SCHEDULEID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Self<br>RATECARD_CURRENT | RATECARDID<br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションに使用されます</td>
    </tr>
    <tr>
        <td>非稼働日</td>
        <td>スケジュールの例外</td>
        <td>非世界貿易型の |非稼働日</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID （self） <br>OBJID <br>SCHEDULEID <br>SYSID <br>USERID  </td>
        <td>Self<br>OBJCODE フィールドで識別されるオブジェクトの ID<br>SCHEDULES_CURRENT | SCHEDULEID <br> 関係ではありません。内部アプリケーション用に使用されます <br>USERS_CURRENT | ユーザー ID  </td>
    </tr>
    <tr>
        <td>メモ</td>
        <td>メモ</td>
        <td>メモ |注意</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID<br>PARENTJOURNALENTRYID PARENTNOTEID<br>PORTFOLIIOID<br>PROGRAMID<br>PROJECTID<br><br> <br> <br> <br> <br> <br> <br> <br> <br> PROOFACTIONID の PROOFID の PROOFIDid は TEMPLATETASKID の TEMPLATETASKID が TEMPLATETASKID の TEMPLATETASKID を TIMESHEID に変更した場合の USERID<br></td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>ATTACHOBJCODE<br>OPTASK_CURRENT に応じた変数 | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | USERID<br> 監査レコードテーブルは現在サポートされていません <br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENT_CURRENT | DOCUMENTID<br>Workfrontの関係ではありません。外部システムへの統合に使用されます <br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>NOTEOBJCODE<br>OPTASK_CURRENT に応じた変数 | OPTASKID<br>USER_CURRENT | USERID<br>Endorsement テーブルは現在サポートされていません <br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Proof Action テーブルは現在サポートされていません <br>Proof テーブルは現在サポートされていません <br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTE_CURRENT | NOTEID<br>TIMESHEET_CURRENT | TOPOBJCODE<br>USER<br>CURRENT に応じた TIMESHEETID_Variable | ユーザー ID</td>
    </tr>
    <tr>
        <td>オブジェクトの統合</td>
        <td>オブジェクトの統合</td>
        <td>OBJECT | ObjectIntegration</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   （self） <br>OBJID <br>SYSID  </td>
        <td>LINKEDOBJECTCODE フィールドで特定されたオブジェクトの ID <br>Self<br>OBJCODE フィールドで特定されたオブジェクトの ID <br> 関係ではなく、内部アプリケーション目的で使用されます  </td>
    </tr>
    <tr>
        <td>オブジェクトカテゴリ</td>
        <td>オブジェクトカテゴリ</td>
        <td>OBJCAT | オブジェクト カテゴリ</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID （self） <br>OBJID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>OBJCODE フィールドで識別されるオブジェクトの ID<br> 関係ではありません。内部アプリケーション目的で使用されます  </td>
    </tr>
    <tr>
        <td>OpTask</td>
        <td>問題、要求</td>
        <td>OPTASK |問題</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUEDEFID<br>ID queuetopicid<br>RESOLVEOPTASKID<br>RESOLVEPROJECTID<br>RESOLVETASKID<br>RESOLVINGOBJID<br><br> <br> <br> <br> ROLEID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br> かんばんボード テーブルは現在サポートされていません <br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Queue 定義テーブルはサポートされていません現在 <br> キュートピック テーブルはサポートされていません <br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | RESOLVINGOBJCODE<br>ROLE<br>CURRENT に応じた TASKID_Variable | ROLEID<br>SOURCEOBJCODE_TASK<br>CURRENT に応じた変数 | TASKID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>パラメーター</td>
        <td>カスタムフィールド</td>
        <td>パラメーター | パラメーター</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID （自己） <br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br> パラメーターフィルターテーブルは現在サポートされていません <br>Self<br> リレーションシップではありません。内部アプリケーション目的で使用されます  </td>
    </tr>
    <tr>
        <td>パラメーターオプション</td>
        <td>パラメーターオプション</td>
        <td>POPT | パラメーターオプション</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID<br>PARAMETEROPTIONID （self） <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>Self <br> リレーションシップではありません。内部アプリケーションに使用されます  </td>
    </tr>
    <tr>
        <td>ポータル セクション</td>
        <td>レポート</td>
        <td>PTLSEC | レポート</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID （自己） <br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VIEWID</td>
        <td>関係ではありません。内部アプリケーション用に使用されます <br>USERS_CURRENT | ユーザー ID <br>UIFILTERS_CURRENT | FILTERID<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | ユーザー ID <br>USERS_CURRENT | USERID <br>OBJOBJCODE フィールドで識別されるオブジェクトの ID<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | ユーザー ID <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID <br> スケジュール済みレポート テーブルは現在サポートされていません <br> リレーションシップではありません。内部アプリケーションの目的で使用されます <br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>「ポータル」タブ</td>
        <td>ダッシュボード</td>
        <td>PTLTAB | ダッシュボード</td>
        <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID （self） <br>SYSID<br>USERID</td>
        <td>関係ではありません。内部アプリケーション用に使用されます <br>USERS_CURRENT | USERID <br> ポータル プロファイル テーブルはサポートされません <br>Self<br>Not a relationship; used for internal application purposes <br>USERS_CURRENT | ユーザー ID  </td>
    </tr>
    <tr>
        <td>ポータルのタブセクション</td>
        <td>ダッシュボードセクション</td>
        <td>PRTBSC | [ ポータル ] タブ セクション</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID<br>PORTALSECTIONOBJID<br>PORTALTABID<br>PORTALTABSECTIONID （self） <br>SYSID</td>
        <td>カレンダーポータルセクションがサポートされていません現在 <br> 外部セクションテーブルはサポートされていません現在 <br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>PORTALSECTIONOBJCODE フィールドで識別されるオブジェクトの ID<br>PORTALTABS_CURRENT | PORTALTABID<br>Self<br> 関係ではありません。内部アプリケーション目的で使用されます</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>最終閲覧者のレポート</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td>REPORTID<br>REPORTLASTVIEWERID （self） <br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID （self） <br> 関係ではありません。内部アプリケーションの目的で使用されます <br>USERS_CURRENT | ユーザー ID  </td>
    </tr>
    <tr>
        <td>ポートフォリオ</td>
        <td>ポートフォリオ</td>
        <td>ポート |Portfolio</td>
        <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT<br>PORTFOLIOS_CUSTOM_VALUE_CURRENT<br>PORTFOLIOS_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIOS_CUSTOM_VALUE_EVENT</td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>スコアカードテーブルは現在サポートされていません <br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>設定</td>
        <td>表示，フィルター，グループ化，レポート定義</td>
        <td>PROSET |環境設定</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td>APPGLOBALID<br>PREFERENCEID （self） <br>SYSID  </td>
        <td>関係ではない。内部アプリケーション目的で使用 <br>Self <br> 関係ではない。内部アプリケーション目的で使用  </td>
    </tr>
    <tr>
        <td>プログラム</td>
        <td>プログラム</td>
        <td>PRGM | プログラム</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | ユーザー ID<br>PORTFOLIO_現在 | PORTFOLIOID<br>Self</td>
    </tr>
    <tr>
        <td>プロジェクト</td>
        <td>プロジェクト</td>
        <td>見込み | プロジェクト</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDARTECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTCONDITIONNOTEID<br>ID lastnoteid<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br>POPACCOUNTID<br>PORTFOLIIOID<br>PRIVATERATECARDID<br><br> <br> <br> <br> <br> <br> <br> <br> <br> PROGRAMID の PROGRAMID の QUEUEDEFID の ID で RESOURCEPOLID の QUEUEDEFID が SUBMITTEDBYID の ID を TEMPLATID</td>
        <td>Workfrontの関係ではありません。外部のシステム <br> スコアカードテーブルへの統合に使用されます。現在、サポートされていません <br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>Scorecard テーブルは現在サポートされていません <br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>USER_CURRENT | USERID<br>Pop アカウント テーブルは現在サポートされていません <br>PORTFOLIO_CURRENT | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Self<br>Queue 定義テーブルは現在サポートされていません <br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>プロジェクト チーム ユーザー</td>
        <td>プロジェクト チーム ユーザー</td>
        <td>PRTU | プロジェクト ユーザー</td>
        <td>PROJECTSUSERS_CURRENT<br>PROJECTSUSERS_DAILY_HISTORY<br>PROJECTSUSERS_EVENT</td>
        <td>PROJECTID<br>PROJECTSUSERID （self） <br>SYSID<br>TMPUSERID<br>USERID</td>
        <td>プロジェクト_現在 | PROJECTID<br>Self<br>Not a relationship；内部アプリケーションの目的で使用されます <br>TEMPLATES_CURRENT | TEMPLATEID<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>プロジェクト チーム ユーザーの役割</td>
        <td>プロジェクト チーム ユーザーの役割</td>
        <td>PTEAM | ProjectUserRole</td>
        <td>PROJECTSUSERSROLES_CURRENT<br>PROJECTSUSERSROLES_DAILY_HISTORY<br>PROJECTSUSERSROLES_EVENT</td>
        <td>PROJECTID<br>PROJECTSUSERSROLEID （self） <br>ROLEID<br>SYSID<br>USERID</td>
        <td>プロジェクト_現在 | PROJECTID<br>Self<br>ROLES_CURRENT | ROLEID<br> 関係ではありません。内部アプリケーション目的で使用されます <br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>RateCard</td>
        <td>レートカード</td>
        <td>RTCRD |評価カード</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>RATECARDID （self） <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | ユーザー ID <br>USERS_CURRENT | ユーザー ID    <br>Self<br>SECURITYOBJCODE フィールドで識別されるオブジェクトの ID<br>SOURCEOBJCODE フィールドで識別されるオブジェクトの ID<br> リレーションシップではありません。内部アプリケーション目的で使用されます  </td>
    </tr>
    <tr>
        <td>報告書フォルダー</td>
        <td>報告書フォルダー</td>
        <td>RPTFDR |報告書フォルダー</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td>REPORTFOLDERID （self） <br>SYSID</td>
        <td>自己 <br> 関係ではありません。内部申請のために使用されます</td>
    </tr>
    <tr>
        <td>レポート表示統計数</td>
        <td>レポート表示統計数</td>
        <td>PLSVST | PortalSectionStatisticInfo</td>
        <td>REPORTVIEWSTATISTICCOUNTS_CURRENT<br>REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        <td>REPORTID<br>REPORTVIEWSTATISTICCOUNTID （self） <br>SYSID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID<br>Self<br> 関係ではありません。内部アプリケーション目的で使用されます</td>
    </tr>
    <tr>
        <td>報告可能な予算計上時間数</td>
        <td>報告可能な予算計上時間数</td>
        <td>RPBGHR |予算計上時間数</td>
        <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        <td>PROJECTID<br>REPORTABLEBUDGETEDHOURID （self） <br>ROLEID<br>SYSID<br>USERID</td>
        <td>プロジェクト_現在 | PROJECTID<br>Self<br>ROLES_CURRENT | ROLEID<br> 関係ではありません。内部アプリケーション目的で使用されます <br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>予約時間</td>
        <td>（個人）休暇</td>
        <td>RESVT |休暇</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID （self） <br>SYSID<br>TASKID<br>USERID</td>
        <td>Self<br>Not 関係。内部アプリケーションの目的で使用されます <br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>リソース管理者</td>
        <td>リソース管理者</td>
        <td>RESMGR | リソース管理者</td>
        <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        <td>ID （self） <br>PROJECTID<br>RESOURCEMANAGERID<br>SYSID<br>TEMPLATEID</td>
        <td>Self<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>リソースプール</td>
        <td>リソースプール</td>
        <td>RSPL | リソース プール</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID （self） <br>SYSID  </td>
        <td>USERS_CURRENT | ユーザー ID <br>USERS_CURRENT | USERID <br>Self<br>Not a relationship；内部アプリケーション目的で使用されます  </td>
    </tr>
    <tr>
        <td>Rich Text メモ</td>
        <td>Rich Text メモ</td>
        <td>RHNOTE | Rich Text メモ</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID （self） <br>SYSID</td>
        <td>自己 <br> 関係ではありません。内部申請のために使用されます</td>
    </tr>
    <tr>
        <td>リッチテキストパラメーター値</td>
        <td>リッチテキストパラメーター値</td>
        <td>CHVAL | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID （self） <br>SYSID  </td>
        <td>パラメーター値テーブルは現在サポートされていません <br>Self <br> リレーションシップではありません。内部アプリケーション目的で使用されます  </td>
    </tr>
    <tr>
        <td>リスク</td>
        <td>リスク</td>
        <td>危険 |危険</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID<br>PROJECTID<br>RISKID （セルフ） <br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | ユーザー ID <br>PROJECTS_CURRENT | PROJECTID   <br>Self<br>RISKTYPES_CURRENT | RISKTYPEID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>リスクタイプ</td>
        <td>リスクタイプ</td>
        <td>RSKTYPE |危険タイプ</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>自己 <br> 関係ではありません。内部申請のために使用されます</td>
    </tr>
    <tr>
        <td>役割</td>
        <td>担当業務</td>
        <td>役割 |担当業務</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br> レイアウト テンプレート テーブルはサポートされません <br>RATECARD_CURRENT | RATECARDID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>スケジュール</td>
        <td>スケジュール</td>
        <td>SCHED | スケジュール</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>ステップ承認者</td>
        <td>ステップ承認者</td>
        <td>SPAPVR |ステージ承認者</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID （self） <br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>ROLES_CURRENT | ROLEID<br>Self<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>タスク</td>
        <td>タスク</td>
        <td>タスク | タスク</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY_TASKS<br>CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTUPDATEDBYID<br><br> LASTUPDATEDBYID MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENCERULEID<br>REJECTIONISSUEID<br><br> <br> <br> <br> <br> RESERVEDTIMEIDID の ROLEID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | ITERATIONID<br> かんばんボード テーブルは現在サポートされていません <br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | PROJECTID<br>Recurrence Rule テーブルは現在サポートされていません <br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | USERID<br>Self<br>TEAM_CURRENT | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>タスクの先行タスク</td>
        <td>先行タスク</td>
        <td>先行 |先行タスク</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td>ID （self） <br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>Self<br>TASKS_カレント | TASKID<br>TASKS_CURRENT | TASKID <br> リレーションシップではありません。内部アプリケーションに使用されます</td>
    </tr>
    <tr>
        <td>チーム</td>
        <td>チーム</td>
        <td>TEAMOB | チーム</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>Layout テンプレート テーブルはサポートされません <br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | USERID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>チームメンバー</td>
        <td>その他のチーム、チームメンバー</td>
        <td>TEAMMB | チームメンバー</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID （self） <br>USERID</td>
        <td>関係ではありません。内部アプリケーション目的で使用されます <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>TeamMemberRole</td>
        <td>チーム メンバーの役割</td>
        <td>チーム | チーム メンバーの役割</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID （self） <br>USERID</td>
        <td>ROLES_CURRENT | ROLEID <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>テンプレート</td>
        <td>テンプレート</td>
        <td>テンプレ | テンプレート</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID<br>TEAMID<br>TEAMID<br>TEMPLATEID （セルフ）</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>USERS_CURRENT | ユーザー ID <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Queue 定義テーブルは現在サポートされていません <br>SCHEDULES_CURRENT | SCHEDULEID <br> 関係ではありません。内部アプリケーション用に使用されます <br>TEAMS_CURRENT | TEAMID<br>Self</td>
    </tr>
    <tr>
        <td>テンプレートの割り当て</td>
        <td>テンプレートの割り当て</td>
        <td>集計 | テンプレートの割り当て</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID （self） <br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>OBJCODE フィールドで識別されるオブジェクトの ID<br>ROLES_CURRENT | ROLEID<br> 関係ではありません。内部アプリケーション目的で使用されます <br>TEAMS_CURRENT | TEAMID<br>Team Timelineable テーブルは現在サポートされていません <br>Self<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>テンプレートタスク</td>
        <td>テンプレートタスク</td>
        <td>TTSK | テンプレート タスク</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMELINEABLEID<br>TEMPLATEID<br>TEMPLATETTASKID （self）</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br> 繰り返しルール テーブルは現在サポートされていません <br>ROLES_CURRENT | ROLEID<br> 関係ではありません。内部アプリケーション目的で使用されます <br>TEAMS_CURRENT | TEAMID<br>Team Timelineable テーブルは現在サポートされていません <br>TEMPLATES_CURRENT | TEMPLATEID<br>Self</td>
    </tr>
    <tr>
        <td>テンプレート タスクの先行タスク</td>
        <td>テンプレートの先行タスク</td>
        <td>TPRED |先行タスク</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID<br>SUCCESSORID<br>TEMPLATEPREDECESSORID （self） <br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>Self<br> リレーションシップではありません。内部アプリケーションに使用されます</td>
    </tr>
       <tr>
        <td>期間別 KPI 通貨（顧客の利用制限）</td>
        <td>期間別の KPI</td>
        <td>TMPH | TimePhasedKPI</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | ユーザー ID</td>
    </tr>
        <tr>
        <td>期間別 KPI 期間（顧客の利用制限あり）</td>
        <td>期間別の KPI</td>
        <td>TMPH | TimePhasedKPI</td>
        <td>TIMEPHASED_DURATION_CURRENT<br>TIMEPHASED_DURATION_DAILY_HISTORY<br>TIMEPHASED_DURATION_EVENT</td>
        <td>ASSIGNMENTID<br>GROUPID<br>LOCATIONID<br>OPTASKID<br>PORTFOLIIOID<br>PROGRAMID<br>PROJECTID<br>REFERENCEID<br>ROLEID<br>SOURCERETASKID<br>TASKID<br>TIMEPHASEDDURATIONID （SELF） <br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>GROUPS_CURRENT | GROUPID<br>CLASSIFIER_CURRENT | CLASSIFIERID<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIOS_CURRENT | PORTFOLIOID<br>PROGRAMS_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID<br>KPI レコードの件名を識別します <br>ROLES_CURRENT | ROLEID<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID<br>Self<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>タイムシート</td>
        <td>タイムシート</td>
        <td>TMPH | TimePhasedKPI</td>
        <td>TIMEPHASED_CURRENCY_CURRENT<br>TIMEPHASED_CURRENCY_DAILY_HISTORY<br>TIMEPHASED_CURRENCY_EVENT</td>
        <td>ASSIGNMENTID<br>GROUPID<br>LOCATIONID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>REFERENCEID<br>ROLEID<br>SOURCERETASKID<br>TASKID<br>TIMEPHASEDCURRENCYID （SELF） <br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>定期タイムシート</td>
        <td>定期タイムシート</td>
        <td>TSPRO |定期タイムシート</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID （自分自身）</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>GROUPS_CURRENT | GROUPID<br>CLASSIFIER_CURRENT | CLASSIFIERID<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIOS_CURRENT | PORTFOLIOID<br>PROGRAMS_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID<br>KPI レコードの件名を識別します <br>ROLES_CURRENT | ROLEID<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID<br>Self<br>USERS_CURRENT | ユーザー ID</td>
    </tr>
    <tr>
        <td>UI フィルター</td>
        <td>フィルター</td>
        <td>UFT | フィルター</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID （セルフ）</td>
        <td>関係ではありません。内部アプリケーション目的で使用されます <br>USERS_CURRENT | ユーザー ID <br>USERS_CURRENT | USERID <br>OBJCODE フィールドで識別されるオブジェクトの ID<br>PREFERENCES_CURRENT | PREFERENCEID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>Self</td>
    </tr>
    <tr>
        <td>UI グループ化基準</td>
        <td>グループ化</td>
        <td>UIGB | グループ化</td>
        <td>UIGROUBYS_CURRENT<br>UIGROUBYS_DAILY_HISTORY<br>UIGROUBYS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID （self）</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br> 関係ではありません。内部アプリケーション目的で使用されます <br> 自己</td>
    </tr>
    <tr>
        <td>UI テンプレート</td>
        <td>レイアウトテンプレート</td>
        <td>UITMPL | レイアウトテンプレート</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID （self）</td>
        <td>関係ではありません。内部アプリケーション目的で使用されます <br>USERS_CURRENT | ユーザー ID <br>USERS_CURRENT | USERID <br>OBJCODE フィールドで識別されるオブジェクトの ID<br>PREFERENCES_CURRENT | PREFERENCEID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>Self</td>
    </tr>
    <tr>
        <td>UI ビュー</td>
        <td>表示</td>
        <td>UIVIEW |表示</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID （self）</td>
        <td>関係ではありません。内部アプリケーション目的で使用されます <br>USERS_CURRENT | ユーザー ID <br>USERS_CURRENT | USERID <br>OBJCODE フィールドで識別されるオブジェクトの ID<br>PREFERENCES_CURRENT | PREFERENCEID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>Self</td>
    </tr>
    <tr>
        <td>ユーザー</td>
        <td>ユーザー</td>
        <td>ユーザー | ユーザー</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID<br>PORTALPROFILEID<br><br> PREFUIID PRIVATERATECARDID<br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br><br> <br> <br> TIMESHEETPROFILEID は UITEMPLATEID の UUMUSERID</td>
        <td>ACCESSLEVEL_CURRENT |ACCESSLEVELID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br> レイアウト テンプレート テーブルはサポートされません <br>USER_CURRENT | USERID<br> ポータル プロファイル テーブルはサポートされません <br> リレーションシップではありません。内部アプリケーション用に使用されます <br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br> リレーションシップではありません。内部アプリケーションに使用されます</td>
    </tr>
    <tr>
        <td>ユーザーの委任</td>
        <td>ユーザーの委任</td>
        <td>USRDEL | ユーザーの委任</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID （self）</td>
        <td>USERS_CURRENT | USERID<br> 関係ではありません。内部アプリケーション用に使用されます <br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>ユーザー グループ</td>
        <td>その他のグループ</td>
        <td>USRGPS | ユーザーグループ</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td>GROUPID <br>SYSID<br>USERID <br>USERSGROUPID （自分自身）</td>
        <td>GROUPS_CURRENT | GROUPID <br> 関係ではありません。内部アプリケーション目的で使用されます <br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>ユーザーの場所</td>
        <td>ユーザーの場所</td>
        <td>USRLOC | UserLocation</td>
        <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        <td>CLASSIFIERID<br>SYSID<br>USERID<br>USERLOCATIONID （self）</td>
        <td>CLASSIFIER_CURRENT | CLASSIFIERID<br> 関係ではありません。内部アプリケーションの目的で使用されます <br>USERS_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>ユーザーの役割</td>
        <td>その他の役割</td>
        <td>USRROL | ユーザーの役割</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td>ROLEID <br>SYSID<br>USERID    <br>USERROLESETID<br>USERSROLEID （self）</td>
        <td>ROLES_CURRENT | ROLEID <br> 関係ではありません。内部アプリケーション目的で使用されます <br>USERS_CURRENT | ユーザー ID    <br>USERROLESET_CURRENT | USERROLESETID<br>Self</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | ユーザー設定</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID （self）</td>
        <td>関係ではありません。内部アプリケーション目的で使用されます <br>USERS_CURRENT | ユーザー ID    <br> セルフ</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>URSET | UserRoleSet</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID （self）</td>
        <td>ROLES_CURRENT | ROLEID <br> 関係ではありません。内部アプリケーション目的で使用されます <br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>UsersDecisions</td>
        <td>ユーザーの決定</td>
        <td>USRDEC | ユーザーの決定</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td>USERDECISIONID （self） <br>SYSID <br>USERID  </td>
        <td>自己 <br> 関係ではありません。内部アプリケーションの目的で使用されます <br>USERS_CURRENT | ユーザー ID </td>
    </tr>
    <tr>
        <td>作業項目</td>
        <td>作業アイテム</td>
        <td>WRKIM |作業項目</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>PROJECTID <br>SYSID<br>TASKID    <br>USERID <br>WORKITEMID （self）</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br>OBJOBJCODE フィールドで識別されるオブジェクトの ID<br>OPTASK_CURRENT | OPTASKID    <br>PROJECTS_CURRENT | PROJECTID <br> リレーションシップではありません。内部アプリケーションの目的で使用されます <br>TASKS_CURRENT | TASKID    <br>USERS_CURRENT | ユーザー ID    <br> セルフ </td>
    </tr>
  </tbody>
</table>
