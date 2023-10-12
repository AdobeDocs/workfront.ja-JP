---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 17 の新機能
description: Adobe Workfrontは、2022 年 4 月 7 日に API バージョン 17 をリリースしました。 API バージョン 17 では、バージョン 15 から次の変更がおこなわれました。
author: Becky
feature: Workfront API
source-git-commit: e0b040b062796a1d1b1e0c029ca0ef71b77ed54a
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 4%

---

# API バージョン 17 の新機能

Adobe Workfrontは、2023 年 10 月 13 日に API バージョン 17 をリリースしました。 API バージョン 17 では、バージョン 16 から次の変更がおこなわれました。

## 追加されたリソース

<!--

### Booking (BOOKNG)

-->

### ExternalDocument (EXTDOC)

ExternalDocument オブジェクトは、Workfrontの外部にあるドキュメントストレージプロバイダーに配置されるドキュメントまたはその他のデジタルアセットです。 これらのアセットは、Workfrontとの間でリンクできます。

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
          <li><p><b>name</b></p></li>
          <li><p><b>パス</b></p></li>
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
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>パス</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>サイズ</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>値</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">デフォルトのフィールド</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
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
      <td role="rowheader">オペレーション</td>
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
          <li><p><b>顧客</b></p></li>
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

API バージョン 17 で削除されたリソースはありませんでした。

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

### ベースライン (BLIN)

ベースラインは、特定の時点でのプロジェクトのパフォーマンスがどのように表示されたかを示すスナップショットです。 主要な日付、進捗状況、コスト、売上高など、プロジェクトに関する主要な情報が格納されます。

Baseline オブジェクトがフラグを削除しました **INLINE_EDITABLE**.

### 請求レコード (BILL)

BillingRecord オブジェクトは、請求可能な収益、時間、または費用を記録します。 この情報は、外部の会計システムで請求書を作成する際に使用できます。

BillingRecord オブジェクトがフラグを削除しました **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### 会社 (CMPY)

Company オブジェクトは、人々の集まりで構成される組織を表します。

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
            <p>削除済み</p>
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
            <p>可能な値「config.defaultToNewHomeDescription」(customer:config.defaultToNewHome)&gt;/p？を追加しました。<p>これにより、組織は新しいホームエクスペリエンスをユーザーのデフォルトとして使用できます。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

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
            <p>可能な値「Frame.io」を追加しました (FRAMEIO)</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>可能な値「enum.filetype.site」を追加しました (site)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### ExchangeRate (EXRATE)

ExchangeRate オブジェクトは、Workfrontで設定された為替レートを表します。 ExchangeRate オブジェクトは動的ではありません。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが追加されました。
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
          <p>追加済み.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### 費用 (EXPNS)

費用は、プロジェクトの存続中に発生する可能性のある非労務費を表します。

費用オブジェクトがフラグを削除しました **INLINE_EDITABLE**.

### グループ (GROUP)

Group オブジェクトは、一連のユーザーとチームを表します。 グループは、多くの場合、部門の構造を表します。

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
            <p>削除済み</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 時間 (HOUR)

Hour オブジェクトは、ユーザーがタイムシートに記録した時間を表します。

Hour オブジェクトがフラグを削除しました。 **INLINE_EDITABLE**.

### 反復 (ITRN)

Iteration オブジェクトは、1 つのアジャイルイテレーションを表します。 繰り返しとは、アジャイルストーリーの計画と完了に使用される、個別の期間です。

Iteration オブジェクトがフラグを削除しました **INLINE_EDITABLE**.


### ジャーナルエントリ (JRNEL)

JournalEntry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。 フィールドを Journal Entry オブジェクトの一部としてログに記録するように設定すると、そのフィールドを変更するたびに対応する Journal Entry が作成されます。

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
            <p>次の可能な値が追加されました。</p>
            <ul>
              <li>承認者の追加 (AAA)</li>
              <li>レビュー担当者 (AAR) を追加しました</li>
              <li>レビュー担当者 (ARR) が削除されました</li>
              <li>削除された承認者 (ARA)</li>
              <li>承認された決定 (ADA)</li>
              <li>決定が変更で承認されました (ADC)</li>
              <li>判定には作業が必要 (AND)</li>
              <li>決定が取り消されました (ADR)</li>
              <li>承認者が変更されました (AAC)</li>
              <li>レビュー担当者が変更されました (ARC)</li>
              <li>レビュー完了 (RDC)</li>
              <li>レビュー失効 (RDR)</li>
              <li>公開 (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### かんばんボード (KNBNBD)

かんばんボードは、アジャイル環境でタスクを追跡するために使用されます。

かんばんボードオブジェクトがフラグを削除しました **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

LinkedFolder オブジェクトは、Google Drive やDropboxなど、外部のドキュメントプロバイダからリンクされたフォルダを表します。

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
            <p>可能な値「Frame.io (FRAMEIO)」を追加しました。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### オペタスク/問題 (OPTASK)

OpTask オブジェクトは、一般にイシューと呼ばれます。 問題とは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業項目です。 問題は、ヘルプデスクへのリクエストでもかまいません。 変更管理、要求、バグも問題です。

Issue オブジェクトがフラグを削除しました。 **INLINE_EDITABLE**.

### プロジェクト (PROJ)

プロジェクトはWorkfront内の作業項目で、Workfrontが作業をおこなう際に役立つ主要な構成要素です。 Project オブジェクトは、共通の特定の目標を持つタスクのグループを表します。

Project オブジェクトがフラグを削除しました **INLINE_EDITABLE**.

### ProjectUser (PRTU)

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
            <p>追加済み.</p>
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
            <p>追加済み.</p>
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

### レート (RATE)

Rate オブジェクトは、Workfrontの請求率を表します。

Rate オブジェクトがフラグを削除しました **INLINE_EDITABLE**.

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
        <p>The <b>setRatesForRole</b> 次のフィールドを追加するようにアクションが変更されました。
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### リスク (RISK)

Risk オブジェクトは、プロジェクトが予定通りに完了しない、または予算内で終了しない可能性のあるイベントを表します。 計画段階では、作業の承認前に、潜在的な障害物を特定するためのリスクがプロジェクトに追加されます。

リスクオブジェクトがフラグを削除しました **INLINE_EDITABLE**.

### 役割/ジョブの役割 (ROLE)

ロールオブジェクト（ジョブロール）は、Designer や Product Manager など、ユーザーが入力できる機能能力またはスキルセットを表します。

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
            <p>削除済み</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### タスク (TASK)

Task オブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

Task オブジェクトがフラグを削除しました **INLINE_EDITABLE**.

### チーム (TEAMOB)

Team オブジェクトは、作業項目に割り当てることができるユーザーの集まりです。

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
            <p>削除済み</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TeamMember (TEAMMB)

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
            <p>追加済み.</p>
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
            <p>追加済み.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TemplateUser (TMTU)

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
            <p>追加済み.</p>
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
            <p>追加済み.</p>
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
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
            <p>削除済み</p>
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
            <p><b>changeType</b>
            </p>
            <p>次の値が追加されました。</p>
            <ul>
              <li>承認者を追加しました (assetapprovalAddApprover)</li>
              <li>レビュー担当者 (assetapprovalAddReviewer) を追加しました</li>
              <li>承認者を削除しました (assetapprovalRemoveApprover)</li>
              <li>レビュー担当者を削除しました (assetapprovalRemoveReviewer)</li>
              <li>承認された決定 (assetapprovalDecisionApproved)</li>
              <li>決定には作業が必要です (assetapprovalDecisionNeedsWork)</li>
              <li>決定は変更を伴って承認されました (assetapprovalDecisionApprovedChanges)</li>
              <li>決定が取り消されました (assetapprovalDecisionRevoked)</li>
              <li>承認者が変更されました (assetapprovalApproverChanged)</li>
              <li>レビュー担当者が変更されました (assetapprovalReviewerChanged)</li>
              <li>レビューが完了しました (assetapprovalReviewerDecisionComplete)</li>
              <li>レビュー取り消されました (assetapprovalReviewerDecisionRevoked)</li>
              <li>外部ドキュメント送信エラー (externalDocumentSendError)</li>
              <li>ドキュメントのバージョンが公開されました (documentVersionPublish)</li>
              <li>リンクされたフォルダーワークフロー (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### ユーザー (USER)

User オブジェクトは、Workfrontにログインしてシステムとやり取りできるアカウントを持つ人物を表します。

User オブジェクトがフラグを削除しました **INLINE_EDITABLE**.

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
            <p>このフィールドが追加され、0 ～ 1 の数値です。これは、ユーザーが 1 日にプロジェクト作業（間接作業以外の作業）に費やすことができる時間の割合を表します。 値が 1 の場合、ユーザーは時間の 100%をプロジェクトの作業に費やすことができます。</p>
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
            <p>追加済み.</p>
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
            <p>追加済み.</p>
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
            <p><b>changeType</b>
            </p>
            <p>次の値が追加されました。</p>
            <ul>
              <li>ドキュメントには承認が必要です (AAA)</li>
              <li>文書にはレビュー (AAR) が必要です</li>
              <li>ドキュメントが承認を必要としなくなりました (ARA)</li>
              <li>レビュー (ARR) が不要になったドキュメント</li>
              <li>ドキュメントには（ユーザー）の承認 (ATA) が必要です</li>
              <li>文書ニーズ（ユーザ）のレビュー (ATR)</li>
              <li>ドキュメントが不要になった（ユーザー）の承認 (RTA)</li>
              <li>ドキュメントは不要（ユーザー）のレビュー (RTR)</li>
              <li>承認済みドキュメント (ADA)</li>
              <li>変更により承認されたドキュメント (ADC)</li>
              <li>ドキュメントには作業が必要です (AND)</li>
              <li>（ユーザー）が（ドキュメント）を承認済みとしてマークしました。 あなたの承認は不要になりました。(AAN)</li>
              <li>（ユーザー）が（ドキュメント）を変更で承認済みとしてマークしました。 あなたの承認は不要になりました。(ACN)</li>
              <li>（ユーザー）は、（ドキュメント）を必要に応じてマークしました。 あなたの承認は不要になりました。(AWN)</li>
              <li>ドキュメントには、承認 (AAC) ではなく、今すぐレビューが必要です</li>
              <li>ドキュメントには、レビュー (AND) ではなく、今すぐの承認が必要です</li>
              <li>ドキュメントの確認 (RDC)</li>
              <li>ドキュメントのレビュー (TRC)</li>
              <li>（ユーザー）がレビュー（ドキュメント）を完了したと見なしています。 レビューは不要になりました。(TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole (USRROL)

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
            <p>追加済み.</p>
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
            <p>追加済み.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
