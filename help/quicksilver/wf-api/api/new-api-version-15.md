---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 15 の新機能
description: Adobe Workfrontは、2022 年 6 月 14 日に API バージョン 14 をリリースしました。 API バージョン 15 では、バージョン 14 から次の変更がおこなわれました。
author: Becky
feature: Workfront API
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 3%

---

# API バージョン 15 の新機能

Adobe Workfrontは、2022 年 6 月 14 日に API バージョン 15 をリリースしました。 API バージョン 15 では、バージョン 14 から次の変更がおこなわれました。

## 追加されたリソース

* [イニシアチブ (INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [タスク定義 (TSKDEF)](#TaskDef)

* [UserApproval (USRAPV)](#UserAppr)

### イニシアチブ (INITIV)

Initiative オブジェクトは、Workfrontシナリオプランナに、ジョブの役割の種類と数、固定コスト、および計画福利厚生に関する見積もりを作成します。

イニシアチブの詳細については、 [シナリオプランナーのイニシアチブの概要](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>これは内部オブジェクトです。</p>
          </li>
          <li>
            <p><b>期間</b>
            </p>
            <p>endDate と startDate の間の時間です。</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>イニシアチブの計画完了日。</p>
          </li>
          <li>
            <p><b>enteriedByID</b>
            </p>
            <p>要求を送信したユーザーに関連付けられた ID。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>アクションに関連付けられた ID。</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>イニシアチブに関連付けられている ID。</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>イニシアチブがWorkfrontシナリオプランナーで最後に公開された日付。</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>イニシアチブの名前</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>イニシアチブに関連付けられたプランの ID。</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>イニシアチブに関連付けられたプランの名前。</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>イニシアチブに関連付けられたプロジェクトの ID。</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>イニシアチブに関連付けられたWorkfrontシナリオプランナーのシナリオの ID。</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>イニシアチブの計画開始日。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td >
        <ul>
          <li>
            <p><b>顧客</b>
            </p>
          </li>
          <li>
            <p><b>enteredBy</b>
            </p>
          </li>
          <li>
            <p><b>プロジェクト</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>name</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>カウント</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>レポート </b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

IssueDef オブジェクトは、問題の形式に関する一連のデータを表します。 このオブジェクトは、プロジェクトまたはテンプレートに添付でき、そのプロジェクトまたはテンプレートに追加される問題に影響を与えます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration (OBJINT)

場合によっては、Workfrontの作業項目を外部のソフトウェア製品のオブジェクトに直接リンクさせることができます。 ObjectIntegration オブジェクトは、このリンクを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>これは内部オブジェクトです。</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>ObjectIntegration がWorkfront System に入力された日時。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>特定の ObjectIntegration オブジェクトの一意のWorkfront ID。</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>ObjectIntegration オブジェクトがリンクを作成する外部ソフトウェア。 次の値を指定できます。</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>アナプラン</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>ObjectIntegration が関連付けられているWorkfront内のオブジェクト。</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>ObjectIntegration が関連付けられているWorkfront内のオブジェクトのオブジェクトコード。</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td >
        <ul>
          <li>
            <p><b>顧客</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### タスク定義 (TSKDEF)

TaskDef オブジェクトは、タスクの形式に関する一連のデータを表します。 このオブジェクトは、プロジェクトまたはテンプレートにアタッチでき、そのプロジェクトまたはテンプレートに追加されるタスクに影響を与えます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories
</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserApproval (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド </td>
      <td>
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>ステータス</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td >
        <ul>
          <li>
            <p><b>承認者</b>
            </p>
          </li>
          <li>
            <p><b>顧客</b>
            </p>
          </li>
          <li>
            <p><b>要求者</b>
            </p>
          </li>
          <li>
            <p><b>ユーザー</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">デフォルトのフィールド</td>
      <td >
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>ステータス</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>承認</b>
            </p>
          </li>
          <li>
            <p><b>却下する</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>追加</b>
            </p>
          </li>
          <li>
            <p><b>カウント</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>レポート</b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## 削除されたリソース

API バージョン 15 ではリソースが削除されませんでした。

## 変更されたリソース

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [アクセス規則 (ACSRUL)](#AccessRu)

* [承認（承認）](#Approval)

* [カテゴリ (CTGY)](#Category)

* [CategoryParameter (CTGYPA)](#Category2)

* [顧客の環境設定 (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [グループ (GROUP)](#Group)

* [ジャーナルエントリ (JRNEL)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [オペタスク/問題 (OPTASK)](#OpTask)

* [パラメータ (PARAM)](#Paramete)

* [Portfolio（ポート）](#Portfoli)

* [プログラム (PRGM)](#Program)

* [プロジェクト (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [タスク (TASK)](#Task)

* [テンプレート (TMPL)](#Template)

* [タイムシート (TSHET)](#Timeshee)

* [表示 (UIVIEW)](#View)

* [更新（更新）](#Update)

* [ユーザー (USER)](#User)

* [UserNote (USRNOT)](#UserNote)

* [作業（作業）](#Work)

### AccessLevel (ACSLVL)

AccessLevel オブジェクトは、ユーザーに関連付けられ、ユーザーがアクセスできる AccessLevelPermissions のセットを表します。

アクセスレベルの詳細については、 [アクセスレベル](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (string[])</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>VTMAWMG （自分のグループに関連付けられたチームを表示）</p>
              </li>
              <li>
                <p>VALLTM （すべてのチームを表示）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions (ALVPER)

AccessLevelPermissions オブジェクトは、Workfrontオブジェクトにアクセス、作成、または変更するための特定の権限を表します。 これらの権限は、アクセスレベルに関連付けることができます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （自分の所属するチームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN ( 管理するグループのチームを編集する（グループ管理者のみ）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （自分の所属するチームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN ( 管理するグループのチームを編集する（グループ管理者のみ）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （自分の所属するチームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN ( 管理するグループのチームを編集する（グループ管理者のみ）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

ユーザーが必要なWorkfront内のオブジェクトへのアクセス権を持っていない場合、そのオブジェクトへのアクセス権をリクエストできます。 AccessRequest オブジェクトは、このリクエストを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>アクション</b> （文字列）</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （自分の所属するチームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN ( 管理するグループのチームを編集する（グループ管理者のみ）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> （文字列）</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>WDL</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### アクセス規則 (ACSRUL)

AccessRule オブジェクトは、ユーザーが作成したプロジェクトを共有する方法を決定するカスタムアクセスレベルのルールセットを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （自分の所属するチームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN ( 管理するグループのチームを編集する（グループ管理者のみ）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （自分の所属するチームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN ( 管理するグループのチームを編集する（グループ管理者のみ）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （自分の所属するチームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN ( 管理するグループのチームを編集する（グループ管理者のみ）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 承認（承認）

タスク、ドキュメント、タイムシートなどの特定の作業項目に対しては、管理者や他のユーザーが作業項目に対してサインオフする必要が生じる場合があります。 Approval オブジェクトは、作業項目に対するサインオフの操作を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td >
        <ul>
          <li>
            <p><b>イニシアチブ</b>
            </p>
            <p>追加済み.</p>
            <p>Initiative オブジェクトは、Workfrontシナリオプランナに、ジョブの役割の種類と数、固定コスト、および計画福利厚生に関する見積もりを作成します。 </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>追加済み.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>追加済み.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">追加済み.</p>
            <p>場合によっては、Workfrontの作業項目を外部のソフトウェア製品のオブジェクトに直接リンクさせることができます。 ObjectIntegration オブジェクトは、このリンクを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### カテゴリ (CTGY)

Category オブジェクトはカスタムフォームです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b> （文字列）</p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>グループ（グループ）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>追加済み.</p>
            <p style="font-weight: normal;">このパラメーターは、カスタムフォームを添付できるオブジェクトの配列です。 複数のタイプのオブジェクトにカスタムフォームを添付する機能をサポートするために追加されました。</p>
            <p>可能な値： </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>追加済み.</p>
            <p style="font-weight: normal;">このパラメーターは、カスタムフォームを添付できるオブジェクトの配列です。 複数のタイプのオブジェクトにカスタムフォームを添付する機能をサポートするために追加されました。</p>
            <p>可能な値： </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>追加済み.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>追加済み.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>追加済み.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 顧客の環境設定 (CUSTPR)

CustomerPreferences オブジェクトは、Workfrontのインスタンスに対して顧客が設定した一連の環境設定を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>name</b>
            </p>
            <p>次の値が追加されました。</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (SharePoint (Graph API) 統合が有効)</p>
                <p>この値は、更新された SharePoint 統合をサポートします。</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (ユーザーがテンプレートを使用せずにプロジェクトを作成することを許可)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

ドキュメントはフォルダに整理できます。 個人用ドキュメント領域に個人用フォルダを作成できます。 DocumentFolder オブジェクトは、これらのフォルダの 1 つを表します。

DocumentFolder オブジェクトにフラグが追加されました `SHARABLE`.

### DocumentVersion (DOCV)

DocumentVersion オブジェクトは、ファイルの特定のバージョン（書き込まれた資料、画像、その他の形式の情報など）を表します。

ドキュメントのバージョンについて詳しくは、 [新しいバージョンのドキュメントをアップロード](../../documents/managing-documents/upload-new-document-version.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>次の値が追加されました。 </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>この値は、更新された SharePoint 統合をサポートします。</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### グループ (GROUP)

Group オブジェクトは、一連のユーザーとチームを表します。 グループは、多くの場合、部門の構造を表します。

グループについて詳しくは、グループとチームを参照してください。

Group オブジェクトにフラグが追加されました `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <p>次のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>カテゴリはカスタムフォームです。 このパラメーターは、カスタムFormsをグループオブジェクトに追加する機能をサポートするために追加されました。 </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>オブジェクトが Active の場合は値 true を持ち、そうでない場合は false を持つブール型パラメータです。 [ アクティブ ] に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトにアタッチできます。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td >
        <p>次のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>承認者</b>
            </p>
          </li>
          <li>
            <p><b>顧客</b>
            </p>
          </li>
          <li>
            <p><b>要求者</b>
            </p>
          </li>
          <li>
            <p><b>ユーザー</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <p>次のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>場合によっては、Workfrontの作業項目を外部のソフトウェア製品のオブジェクトに直接リンクさせることができます。 ObjectIntegration オブジェクトは、このリンクを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">デフォルトのフィールド</td>
      <td >
        <p>次のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>オブジェクトが Active の場合は値 true を持ち、そうでない場合は false を持つブール型パラメータです。 [ アクティブ ] に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトにアタッチできます。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <p>次のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>この操作により、カスタムフォームフィールドの式が再計算されます。</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ジャーナルエントリ (JRNEL)

JournalEntry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。 フィールドを Journal Entry オブジェクトの一部としてログに記録するように設定すると、そのフィールドを変更するたびに対応する Journal Entry が作成されます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>次の値が追加されました。 </p>
        <ul>
          <li>
            <p>DW （ダウンロード）</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

LinkedFolder オブジェクトは、Google Drive やDropboxなど、外部のドキュメントプロバイダからリンクされたフォルダを表します。

リンクされたフォルダの詳細については、「外部アプリケーションからドキュメントをリンクする」を参照してください。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>次の値が追加されました。 </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>この値は、更新された SharePoint 統合をサポートします。</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### オペタスク/問題 (OPTASK)

OpTask オブジェクトは、一般にイシューと呼ばれます。 問題とは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業項目です。 問題は、ヘルプデスクへのリクエストでもかまいません。 変更管理、要求、バグも問題です。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <p>次のアクションが追加されました。</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>次のアクションが変更されました：</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>追加されたフィールド <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### パラメータ (PARAM)

Parameter オブジェクトは、カスタムフィールドです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <p>次のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>次のフィールドが変更されました：</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>可能な値を追加しました <code>WIDGET </code>（ウィジェット） </p>
            <p>この値は、カスタムフォームでの画像の使用をサポートします。</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>可能な値を追加しました <code>WIDGET </code>（ウィジェット）</p>
            <p>この値は、カスタムフォームでの画像の使用をサポートします。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio（ポート）

Portfolioオブジェクトとは、同じリソース、通常は費用や担当者を競い合って完了するプロジェクトの集まりです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### プログラム (PRGM)

Program オブジェクトは、ポートフォリオ内のプロジェクトのサブセットで、類似のプロジェクトを 1 つにグループ化できます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### プロジェクト (PROJ)

プロジェクトはWorkfront内の作業項目で、Workfrontが作業をおこなう際に役立つ主要な構成要素です。 Project オブジェクトは、共通の特定の目標を持つタスクのグループを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td >
        <ul>
          <li>
            <p><b>イニシアチブ</b>
            </p>
            <p>Initiative オブジェクトは、Workfrontシナリオプランナに、ジョブの役割の種類と数、固定コスト、および計画福利厚生に関する見積もりを作成します。 </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>場合によっては、Workfrontの作業項目を外部のソフトウェア製品のオブジェクトに直接リンクさせることができます。 ObjectIntegration オブジェクトは、このリンクを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

QueueDef オブジェクトは、Queue を表します。Queue は、ユーザーが問題を送信できるようにヘルプデスク領域に公開されたプロジェクトです。

リクエストキューについて詳しくは、 [リクエストキューの作成](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （自分の所属するチームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN ( 管理するグループのチームを編集する（グループ管理者のみ）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON （自分の所属するチームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN ( 管理するグループのチームを編集する（グループ管理者のみ）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。 これらの質問は通常、Portfolio管理者が決定し、その回答によって、管理者はプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。

スコアカードに関する質問の詳細は、 [スコアカードの作成](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>可能な値を追加しました <code>WIDGET </code>（ウィジェット）</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### タスク (TASK)

Task オブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>場合によっては、Workfrontの作業項目を外部のソフトウェア製品のオブジェクトに直接リンクさせることができます。 ObjectIntegration オブジェクトは、このリンクを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### テンプレート (TMPL)

Template オブジェクトは、プロジェクトのパターンを表します。 プロジェクトは、テンプレートから作成して時間を節約できます。 テンプレートにはチームとタスクが含まれ、テンプレートから作成されたすべてのプロジェクトにコピーされます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### タイムシート (TSHET)

Timesheet オブジェクトは、Tasks、Projects、および Overhead Hour Types の実績作業時間をユーザーが入力できる仮想タイムカードを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <p>次のフィールドが削除されました：</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 表示 (UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>次の可能な値が削除されました。</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (4 カラム レイアウト)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (更新)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (更新)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (作業中)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (カスタムデータ)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (カスタム データの更新)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (状態更新)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (状態更新)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (状態更新)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (状態更新)</p>
              </li>
              <li>
                <p><code>DLIST</code> (詳細リスト)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (詳細リスト セクション)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 更新（更新）

Workfrontの作業項目を更新して、ユーザーに現在のステータスを知らせることができます。 Update オブジェクトは、これらの更新の 1 つを表します。 更新は、ユーザーが入力するか、Workfrontシステムが作成します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
            <p>可能な値を追加しました <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ユーザー (USER)

User オブジェクトは、Workfrontにログインしてシステムとやり取りできるアカウントを持つ人を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserNote (USRNOT)

UserNote オブジェクトは通知です。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>eventType</b>
            </p>
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>
                <p><code>DUP </code>（ドキュメントの配達確認を要求）</p>
              </li>
              <li>
                <p><code>DUV </code>（ドキュメントを表示できます）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 作業（作業）

Work オブジェクトは、Task と OpTask の両方が継承する共通のインターフェイスで、2 つの間で共通のコードを共有します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>場合によっては、Workfrontの作業項目を外部のソフトウェア製品のオブジェクトに直接リンクさせることができます。 ObjectIntegration オブジェクトは、このリンクを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
