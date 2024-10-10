---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 17 の新機能
description: Adobe Workfront は、2022年4月6日（PT）に API バージョン 17 をリリースしました。API バージョン 17 では、バージョン 16 から次の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 99%

---

# API バージョン 17 の新機能

Adobe Workfront は、2023年10月12日（PT）に API バージョン 17 をリリースしました。API バージョン 17 では、バージョン 16 から次の変更が行われました。

## 追加されたリソース

<!--

### Booking (BOOKNG)

-->

### ExternalDocument（EXTDOC）

ExternalDocument オブジェクトは、Workfront の外部にあるドキュメントストレージプロバイダーに置かれるドキュメントまたはその他のデジタルアセットです。これらのアセットは、Workfront との間でリンクできます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>説明</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>内線</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>名前</b></p></li>
          <li><p><b>path</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>サイズ</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>説明</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>内線</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>名前</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>path</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>サイズ</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>value</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">デフォルトのフィールド</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>名前</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">クエリ</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li><p><b>SEARCH</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>
        <ul>
          <li><p><b>customer</b></p></li>
          <li><p><b>ユーザー</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## 削除されたリソース

API バージョン 17 で削除されたリソースはありません。

## 変更されたリソース

API バージョン 17 で次のリソースを変更しました。

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Baseline（BLIN）

ベースラインは、特定の時点でのプロジェクトのパフォーマンスを示すスナップショットです。主要な日付、進捗状況、コスト、売上高など、プロジェクトに関する主要な情報が保存されています。

Baseline オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

### BillingRecord（BILL）

BillingRecord オブジェクトは、請求可能な収益、時間または費用を記録します。この情報は、外部の会計システムで請求書を作成する際に使用できます。

BillingRecord オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Company（CMPY）

会社オブジェクトは、人物の集まりで構成される組織を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>削除されました</p>
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
            <p>可能な値として「config.defaultToNewHomeDescription」(customer:config.defaultToNewHome)&gt;/p? を追加しました。<p>これにより、組織は新しいホームエクスペリエンスをユーザーのデフォルトとして使用できます。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion（DOCV）

DocumentVersion オブジェクトは、ファイルの特定のバージョン（書き込まれた資料、画像、その他の形式の情報など）を表します。

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
            <p>可能な値「Frame.io」（FRAMEIO）を追加しました。</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>可能な値「enum.filetype.site」（site）を追加しました。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### ExchangeRate（EXRATE）

ExchangeRate オブジェクトは、Workfrontで設定された通貨の為替レートを表します。 ExchangeRate オブジェクトは動的ではありません。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>以下のフィールドが追加されました。
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>追加済み。</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Expense（EXPNS）

費用は、プロジェクトの存続中に発生する可能性のある役務以外の費用を表します。

Expense オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

### グループ（GROUP）

グループオブジェクトは、一連のユーザーとチームを表します。グループは、多くの場合、部門の構造を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>削除されました</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Hour（HOUR）

Hour オブジェクトは、ユーザーがタイムシートに記録した時間を表します。

Hour オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

### Iteration（ITRN）

イテレーションオブジェクトは、1 つのアジャイルイテレーションを表します。イテレーションとは、アジャイルストーリーの計画と完了に使用される、個別の期間です。

Iteration オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。


### JournalEntry（JRNLE）

JournalEntry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。フィールドをジャーナルエントリオブジェクトの一部としてログに記録するように設定すると、そのフィールドが変更されるたびに、対応するジャーナルエントリが作成されます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>承認者追加（AAA）</li>
              <li>レビュアー追加（AAR）</li>
              <li>レビュアー削除（ARR）</li>
              <li>承認者削除（ARA）</li>
              <li>決定承認（ADA）</li>
              <li>決定の変更後承認（ADC）</li>
              <li>決定に作業が必要（AND）</li>
              <li>決定取り消し（ADR）</li>
              <li>承認者変更（AAC）</li>
              <li>レビュアー変更（ARC）</li>
              <li>レビュー完了（RDC）</li>
              <li>レビュー取り消し（RDR）</li>
              <li>公開（PUB）</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### かんばんボード（KNBNBD）

かんばんボードは、アジャイル環境でタスクを追跡するために使用されます。

Kanban Board オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。


### LinkedFolder (LNKFDR)

LinkedFolder オブジェクトは、Google Drive や Dropbox など、外部のドキュメントプロバイダからリンクされたフォルダーを表します。

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
            <p>可能な値「Frame.io」（FRAMEIO）を追加しました。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / Issue（OPTASK）

OpTask オブジェクトは、一般にイシューと呼ばれます。イシューは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業アイテムです。イシューは、ヘルプデスクへのリクエストである場合もあります。変更指示、リクエスト、バグもイシューです。

Issue オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

### Project（PROJ）

プロジェクトは Workfront 内の作業アイテムで、Workfront が人々の作業を支援するための主要な構築ブロックです。プロジェクトオブジェクトは、共通の特定の目標を持つタスクのグループを表します。

Project オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

### ProjectUser（PRTU）

ProjectUser オブジェクトは、特定のプロジェクトに関連付けられたユーザーを表します。

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
            <p>追加済み。</p>
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
            <p>追加済み。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### Rate（RATE）

Rate オブジェクトは、Workfront の請求料金を表します。

Rate オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>レートカード機能をサポートするために、次のアクションが追加されました。
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p><b>setRatesForRole</b> アクションが変更され、次のフィールドが追加されました。
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Risk（RISK）

リスクオブジェクトは、プロジェクトが時間通りに完了しない、または予算内で終了しない可能性のあるイベントを表します。計画段階では、すべての作業の承認前に、潜在的な障害物を特定するためのリスクがプロジェクトに追加されます。

Risk オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

### Role / Job Role（ROLE）

Role オブジェクト（担当業務）は、デザイナーやプロダクトマネージャーなど、ユーザーが入力できる機能またはスキルセットを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>削除されました</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Task（TASK）

タスクオブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

Task オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

### Team（TEAMOB）

チームオブジェクトは、作業アイテムに割り当てることができるユーザーの集まりです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>削除されました</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TeamMember（TEAMMB）

TeamMember オブジェクトは、特定のチームに関連付けられたユーザーです。

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
            <p>追加済み。</p>
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
            <p>追加済み。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TemplateUser（TMTU）

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
            <p>追加済み。</p>
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
            <p>追加済み。</p>
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
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
            <p>削除されました</p>
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
            <p><b>changeType</b>
            </p>
            <p>以下の値を追加しました。</p>
            <ul>
              <li>承認者追加（assetapprovalAddApprover）</li>
              <li>レビュアー追加（assetapprovalAddReviewer）</li>
              <li>承認者削除（assetapprovalRemoveApprover）</li>
              <li>レビュアー削除（assetapprovalRemoveReviewer）</li>
              <li>決定承認（assetapprovalDecisionApproved）</li>
              <li>決定に作業が必要（assetapprovalDecisionNeedsWork）</li>
              <li>決定の変更後承認（assetapprovalDecisionApprovedChanges）</li>
              <li>決定取り消し（assetapprovalDecisionRevoked）</li>
              <li>承認者変更（assetapprovalApproverChanged）</li>
              <li>レビュアー変更（assetapprovalReviewerChanged）</li>
              <li>レビュー完了（assetapprovalReviewerDecisionComplete）</li>
              <li>レビュー取り消し（assetapprovalReviewerDecisionRevoked）</li>
              <li>外部ドキュメント送信エラー（externalDocumentSendError）</li>
              <li>ドキュメントバージョン公開済み（documentVersionPublish）</li>
              <li>リンクされたフォルダーワークフロー（linkedFolderWorkflow）</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### User （USER）

ユーザーオブジェクトは、ログインしてシステムとやり取りできる Workfront アカウントを持つユーザーを表します。

User オブジェクトでは **INLINE_EDITABLE** フラグを削除しました。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>workTime</b>
            </p>
            <p>このフィールドが追加されました。ユーザーが 1 日にプロジェクト作業（間接作業以外の作業）に費やすことができる時間の割合を 0～1 の数値で表します。値が 1 の場合、ユーザーは時間の 100%をプロジェクトの作業に費やすことができます。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserGroups (USRGPS)

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
            <p>追加済み。</p>
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
            <p>追加済み。</p>
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
            <p><b>changeType</b>
            </p>
            <p>以下の値を追加しました。</p>
            <ul>
              <li>ドキュメントにあなたの承認が必要です（AAA）</li>
              <li>ドキュメントにあなたのレビューが必要です（AAR）</li>
              <li>ドキュメントの承認は不要になりました（ARA）</li>
              <li>ドキュメントのレビューは不要になりました（ARR）</li>
              <li>ドキュメントに（ユーザー）の承認が必要です（ATA）</li>
              <li>ドキュメントに（ユーザー）のレビューが必要です（ATR）</li>
              <li>ドキュメントに（ユーザー）の承認は不要になりました（RTA）</li>
              <li>ドキュメントに（ユーザー）のレビューは不要になりました（RTR）</li>
              <li>ドキュメントが承認されました（ADA）</li>
              <li>ドキュメントが変更の上承認されました（ADC）</li>
              <li>ドキュメントには作業が必要です（ADN）</li>
              <li>（ユーザー）が（ドキュメント）を承認済みとしてマークしました。あなたの承認は不要になりました。（AAN）</li>
              <li>（ユーザー）が（ドキュメント）を変更の上承認済みとしてマークしました。あなたの承認は不要になりました。（ACN）</li>
              <li>（ユーザー）が（ドキュメント）を作業が必要としてマークしました。あなたの承認は不要になりました。（AWN）</li>
              <li>ドキュメントには、承認ではなく、今すぐあなたのレビューが必要です（AAC）</li>
              <li>ドキュメントには、レビューではなく、今すぐあなたの承認が必要です（ADN）</li>
              <li>ドキュメントをレビューしました（RDC）</li>
              <li>ドキュメントをレビューしました（TRC）</li>
              <li>（ユーザー）が（ドキュメント）をレビューして完了としました。あなたの承認は不要になりました。（TRN）</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole（USRROL）

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
            <p>追加済み。</p>
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
            <p>追加済み。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
