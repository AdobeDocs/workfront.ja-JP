---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 15 の新機能
description: Adobe Workfront は、2022年6月14日（PT）に API バージョン 14 をリリースしました。API バージョン 15 では、バージョン 14 から以下の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2286'
ht-degree: 100%

---

# API バージョン 15 の新機能

Adobe Workfront は、2022年6月14日（PT）に API バージョン 15 をリリースしました。API バージョン 15 では、バージョン 14 から以下の変更が行われました。

## 追加されたリソース

* [イニシアチブ（INITIV）](#Initiati)

* [IssueDef（ISSDEF）](#IssueDef)

* [ObjectIntegration（OBJINT）](#ObjectIn)

* [RichTextGroupParameterValue（GRCVAL）](#RichText)

* [TaskDef（TSKDEF）](#TaskDef)

* [UserApproval（USRAPV）](#UserAppr)

### イニシアチブ（INITIV）

イニシアチブオブジェクトは、担当業務の種類と数、固定コスト、予定利益の見積もりを Workfront シナリオプランナーに作成します。

イニシアチブについて詳しくは、[シナリオプランナーのイニシアチブの概要](../../scenario-planner/initiatives-overview.md)を参照してください。

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
            <p>endDate と startDate の間の時間数。</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>イニシアチブの予定完了日。</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>リクエストを送信したユーザーに関連付けられた ID。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>アクションに関連付けられた ID。</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>イニシアチブに関連付けられた ID。</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>イニシアチブが Workfront シナリオプランナーで最後に公開された日付。</p>
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
            <p>イニシアチブに関連付けられた Workfront シナリオプランナーのシナリオの ID。</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>イニシアチブの予定開始日。</p>
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
            <p><b>取得</b>
            </p>
          </li>
          <li>
            <p><b>レポート</b>
            </p>
          </li>
          <li>
            <p><b>検索</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef（ISSDEF）

IssueDef オブジェクトは、イシューの形式に関する一連のデータを表します。このオブジェクトは、プロジェクトやテンプレートに添付でき、そのプロジェクトやテンプレートに追加されるイシューに影響を与えます。

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

### ObjectIntegration（OBJINT）

場合によっては、Workfront の作業アイテムを、外部ソフトウェア製品のオブジェクトに直接リンクすることができます。ObjectIntegration オブジェクトは、このリンクを表します。

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
            <p>ObjectIntegration がWorkfront システムに入力された日時。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>特定の ObjectIntegration オブジェクトの一意の Workfront ID。</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>ObjectIntegration オブジェクトがリンクを作成する外部ソフトウェア。次の値を指定できます。</p>
            <ul>
              <li>
                <p>Jira</p>
              </li>
              <li>
                <p>Salesforce</p>
              </li>
              <li>
                <p>Anaplan</p>
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
            <p>ObjectIntegration が関連付けられた Workfront 内のオブジェクト。</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>ObjectIntegration が関連付けられた Workfront 内のオブジェクトのオブジェクトコード。</p>
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

### TaskDef（TSKDEF）

TaskDef オブジェクトは、タスクの形式に関する一連のデータを表します。このオブジェクトは、プロジェクトやテンプレートに添付でき、そのプロジェクトやテンプレートに追加されるタスクに影響を与えます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours</b>
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
            <p><b>defaultApprovalProcess</b>
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

### UserApproval（USRAPV）

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
            <p><b>approver</b>
            </p>
          </li>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
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
            <p><b>却下</b>
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
            <p><b>削除</b>
            </p>
          </li>
          <li>
            <p><b>取得</b>
            </p>
          </li>
          <li>
            <p><b>REPORT</b>
            </p>
          </li>
          <li>
            <p><b>検索</b>
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

* [AccessLevel（ACSLVL）](#AccessLe)

* [AccessLevelPermissions（ALVPER）](#AccessLe2)

* [AccessRequest（ACSREQ）](#AccessRe)

* [AccessRule（ACSRUL）](#AccessRu)

* [Approval（APPROVAL）](#Approval)

* [Category（CTGY）](#Category)

* [CategoryParameter（CTGYPA）](#Category2)

* [CustomerPreferences（CUSTPR）](#Customer)

* [DocumentFolder（DOCFDR）](#Document)

* [DocumentVersion（DOCV）](#Document2)

* [グループ（GROUP）](#Group)

* [JournalEntry（JRNLE）](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [OpTask / Issue（OPTASK）](#OpTask)

* [Parameter（PARAM）](#Paramete)

* [Portfolio（PORT）](#Portfoli)

* [Program（PRGM）](#Program)

* [Project（PROJ）](#Project)

* [QueueDef（QUED）](#QueueDef)

* [ScoreCardQuestion（SCOREQ）](#ScoreCar)

* [Task（TASK）](#Task)

* [Template（TMPL）](#Template)

* [Timesheet（TSHET）](#Timeshee)

* [View（UIVIEW）](#View)

* [Update（UPDATE）](#Update)

* [User （USER）](#User)

* [UserNote（USRNOT）](#UserNote)

* [Work（WORK）](#Work)

### AccessLevel（ACSLVL）

AccessLevel オブジェクトはユーザーに関連付けられていて、ユーザーのアクセス権を指定する AccessLevelPermissions のセットを表します。

アクセスレベルについて詳しくは、[アクセスレベル](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md)を参照してください。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b>（string[]）</p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>VTMAWMG（自分のグループと関連付けられたチームを表示）</p>
              </li>
              <li>
                <p>VALLTM（すべてのチームを表示）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions（ALVPER）

AccessLevelPermissions オブジェクトは、Workfront オブジェクトにアクセス、作成または変更を行うための特定の権限を表します。これらの権限は、アクセスレベルに関連付けることができます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>（string[]）</p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（所属チームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN（自分が管理するグループのチームを編集する（グループ管理者のみ））</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>（string[]）</p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（所属チームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN（自分が管理するグループのチームを編集する（グループ管理者のみ））</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>（string[]）</p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（所属チームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN（自分が管理するグループのチームを編集する（グループ管理者のみ））</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest（ACSREQ）

Workfront のオブジェクトに対する必要なアクセス権をユーザーが持っていない場合、そのオブジェクトへの利用申請を行うことができます。AccessRequest オブジェクトは、このリクエストを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>action</b>（string）</p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（所属チームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN（自分が管理するグループのチームを編集する（グループ管理者のみ））</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b>（文字列）</p>
            <p>次の値を追加しました。</p>
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

### AccessRule（ACSRUL）

AccessRule オブジェクトは、作成したプロジェクトをユーザーが共有する方法を決定する、カスタムアクセスレベルのルールセットを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>（string[]）</p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（所属チームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN（自分が管理するグループのチームを編集する（グループ管理者のみ））</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>（string[]）</p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（所属チームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN（自分が管理するグループのチームを編集する（グループ管理者のみ））</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>（string[]）</p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（所属チームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN（自分が管理するグループのチームを編集する（グループ管理者のみ））</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Approval（APPROVAL）

タスク、ドキュメント、タイムシートなどの所定の作業アイテムは、上司または他のユーザーが承認することが必要な場合があります。承認オブジェクトは、作業アイテムに対する承認の操作を表します。

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
            <p>追加済み。</p>
            <p>イニシアチブオブジェクトは、担当業務の種類と数、固定コスト、予定利益の見積もりを Workfront シナリオプランナーに作成します。 </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>追加済み。</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>追加済み。</p>
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
            <p style="font-weight: normal;">追加済み。</p>
            <p>場合によっては、Workfront の作業アイテムを、外部ソフトウェア製品のオブジェクトに直接リンクすることができます。ObjectIntegration オブジェクトは、このリンクを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Category（CTGY）

カテゴリオブジェクトはカスタムフォームです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>（文字列）</p>
            <p>次の値を追加しました。</p>
            <ul>
              <li>
                <p>GROUP（グループ）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>（文字列 []）</p>
            <p>追加済み。</p>
            <p style="font-weight: normal;">このパラメーターは、カスタムフォームを添付できるオブジェクトの配列です。カスタムフォームを複数のタイプのオブジェクトに添付する機能をサポートするために追加されました。</p>
            <p>使用可能な値を以下に示します。 </p>
            <p>CMPY、PORT、PRGM、PROJ、TASK、OPTASK、USER、DOCU、EXPNS、ITRN、BILL、GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b>（string[]）</p>
            <p>追加済み。</p>
            <p style="font-weight: normal;">このパラメーターは、カスタムフォームを添付できるオブジェクトの配列です。カスタムフォームを複数のタイプのオブジェクトに添付する機能をサポートするために追加されました。</p>
            <p>使用可能な値を以下に示します。 </p>
            <p>CMPY、PORT、PRGM、PROJ、TASK、OPTASK、USER、DOCU、EXPNS、ITRN、BILL、GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter（CTGYPA）

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
            <p>追加済み。</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>追加済み。</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>追加済み。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CustomerPreferences（CUSTPR）

CustomerPreferences オブジェクトは、Workfront のインスタンスに対して顧客が設定した一連の環境設定を表します。

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
            <p>以下の値を追加しました。</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> （SharePoint（Graph API）統合が有効）</p>
                <p>この値は、アップデートされた SharePoint 統合をサポートします。</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> （ユーザーがテンプレートを使用せずにプロジェクトを作成することを許可）</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> （config.taskissue.delegate）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder（DOCFDR）

ドキュメントをフォルダーに整理できます。個人用ドキュメントエリアに個人用フォルダーを作成できます。DocumentFolder オブジェクトは、これらのフォルダーのうちの 1 つを表します。

DocumentFolder オブジェクトにフラグ `SHARABLE` が追加されました。

### DocumentVersion（DOCV）

DocumentVersion オブジェクトは、ファイルの特定のバージョン（書き込まれた資料、画像、その他の形式の情報など）を表します。

ドキュメントのバージョンについて詳しくは、[新しいバージョンのドキュメントをアップロード](../../documents/managing-documents/upload-new-document-version.md)を参照してください。

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
                <p><code>SHAREPOINT_V2</code> （SharePoint（Graph API））</p>
                <p>この値は、アップデートされた SharePoint 統合をサポートします。</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### グループ（GROUP）

グループオブジェクトは、一連のユーザーとチームを表します。グループは、多くの場合、部門の構造を表します。

グループについて詳しくは、グループとチームを参照してください。

Group オブジェクトにフラグ `DATA_EXTENDIBLE` が追加されました

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <p>以下のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>カテゴリはカスタムフォームです。このパラメーターは、カスタムフォームを Group オブジェクトに追加する機能をサポートするために追加されました。 </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>オブジェクトが Active の場合は値 true を持ち、そうでない場合は false を持つブーリアン型パラメーターです。「アクティブ」に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトに添付できます。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td >
        <p>以下のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>approver</b>
            </p>
          </li>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <p>以下のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>場合によっては、Workfront の作業アイテムを、外部ソフトウェア製品のオブジェクトに直接リンクすることができます。ObjectIntegration オブジェクトは、このリンクを表します。</p>
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
            <p>オブジェクトが Active の場合は値 true を持ち、そうでない場合は false を持つブーリアン型パラメーターです。「アクティブ」に設定されたオブジェクトは、ドロップダウンメニューと先行入力フィールドに表示され、他のオブジェクトに添付できます。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <p>以下のフィールドが追加されました。</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>このアクションにより、カスタムフォームフィールドの式が再計算されます。</p>
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

### JournalEntry（JRNLE）

JournalEntry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。フィールドをジャーナルエントリオブジェクトの一部としてログに記録するように設定すると、そのフィールドが変更されるたびに、対応するジャーナルエントリが作成されます。

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
            <p>DW（Download）</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

LinkedFolder オブジェクトは、Google Drive や Dropbox など、外部のドキュメントプロバイダからリンクされたフォルダーを表します。

リンクされたフォルダについて詳しくは、外部アプリケーションからドキュメントをリンクを参照してください。

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
                <p><code>SHAREPOINT_V2</code> （SharePoint（Graph API））</p>
                <p>この値は、アップデートされた SharePoint 統合をサポートします。</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask / Issue（OPTASK）

OpTask オブジェクトは、一般にイシューと呼ばれます。イシューは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業アイテムです。イシューは、ヘルプデスクへのリクエストである場合もあります。変更指示、リクエスト、バグもイシューです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <p>以下のアクションが追加されました。</p>
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
        <p>次のアクションが変更されました。</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>フィールドが追加されました <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Parameter（PARAM）

パラメーターオブジェクトは、カスタムフィールドです。

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
        <p>次のフィールドが変更されました。</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>使用可能な値 <code>WIDGET </code>（ウィジェット）を追加しました </p>
            <p>この値は、カスタムフォームでの画像の使用をサポートします。</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>使用可能な値 <code>WIDGET </code>（ウィジェット）を追加しました</p>
            <p>この値は、カスタムフォームでの画像の使用をサポートします。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio（PORT）

ポートフォリオオブジェクトは、同じリソース（通常はプロジェクトを完了するための資金や人材）を競い合って完了するプロジェクトのコレクションです。

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

### Program（PRGM）

プログラムオブジェクトは、ポートフォリオ内のプロジェクトのサブセットで、類似のプロジェクトを 1 つにグループ化できます。

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

### Project（PROJ）

プロジェクトは Workfront 内の作業アイテムで、Workfront が人々の作業を支援するための主要な構築ブロックです。プロジェクトオブジェクトは、共通の特定の目標を持つタスクのグループを表します。

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
            <p><b>initiative</b>
            </p>
            <p>イニシアチブオブジェクトは、担当業務の種類と数、固定コスト、予定利益の見積もりを Workfront シナリオプランナーに作成します。 </p>
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
            <p>場合によっては、Workfront の作業アイテムを、外部ソフトウェア製品のオブジェクトに直接リンクすることができます。ObjectIntegration オブジェクトは、このリンクを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef（QUED）

QueueDef オブジェクトは、キューを表します。キューは、ユーザーがイシューを送信できるようにヘルプデスクエリアに公開されたプロジェクトです。

リクエストキューについて詳しくは、[リクエストキューの作成](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

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
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（所属チームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN（自分が管理するグループのチームを編集する（グループ管理者のみ））</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（所属チームを編集）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN（自分が管理するグループのチームを編集する（グループ管理者のみ））</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion（SCOREQ）

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。これらの質問は通常、ポートフォリオマネージャーが決定し、その回答によって、マネージャーはプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。

スコアカードに関する質問について詳しくは、[スコアカードを作成](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)を参照してください。

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
            <p>可能な値 <code>WIDGET </code>（ウィジェット）を追加しました。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Task（TASK）

タスクオブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

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
            <p>場合によっては、Workfront の作業アイテムを、外部ソフトウェア製品のオブジェクトに直接リンクすることができます。ObjectIntegration オブジェクトは、このリンクを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Template（TMPL）

テンプレートオブジェクトは、プロジェクトのパターンを表します。プロジェクトをテンプレートから作成することで時間を節約できます。テンプレートにはチームとタスクが含まれ、テンプレートから作成されたすべてのプロジェクトにコピーされます。

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

### Timesheet（TSHET）

Timesheet オブジェクトは、タスク、プロジェクトおよびオーバーヘッド時間タイプに対して行った実際の時間数をユーザーが入力できる仮想タイムカードを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <p>次のフィールドが削除されました。</p>
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

### View（UIVIEW）

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
                <p><code>FOUR_COL</code> （4 カラム レイアウト）</p>
              </li>
              <li>
                <p><code>UPDATES</code> （更新）</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> （更新）</p>
              </li>
              <li>
                <p><code>WORKINGON</code> （作業中）</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> （カスタムデータ）</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> （カスタムデータの更新）</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> （ステータスの更新）</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> （ステータスの更新）</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> （ステータスの更新）</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> （ステータスの更新）</p>
              </li>
              <li>
                <p><code>DLIST</code> （詳細リスト）</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> （詳細リストセクション）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Update（UPDATE）

Workfront の作業アイテムを更新して、ユーザーに現在のステータスを知らせることができます。更新オブジェクトは、これらの更新の 1 つを表します。更新は、ユーザーが入力するか、Workfront システムが作成することができます。

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
            <p>可能な値 <code>documentVersionDownload </code>（enum.updatetypeenum.documentversiondownload）を追加しました。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### User （USER）

ユーザーオブジェクトは、ログインしてシステムとやり取りできる Workfront アカウントを持つユーザーを表します。

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

### UserNote（USRNOT）

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
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p><code>DUP </code>（このドキュメントをプルーフするようにリクエストしました）</p>
              </li>
              <li>
                <p><code>DUV </code>（ドキュメントの表示を許可します）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Work（WORK）

作業オブジェクトは、Task と OpTask の両方が継承する共通のインターフェイスで、2 つの間で共通のコードを共有します。

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
            <p>場合によっては、Workfront の作業アイテムを、外部ソフトウェア製品のオブジェクトに直接リンクすることができます。ObjectIntegration オブジェクトは、このリンクを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
