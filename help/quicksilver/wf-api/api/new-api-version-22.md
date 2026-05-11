---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 22の新機能
description: Adobe Workfrontは、2026年5月11日（PT）にAPI バージョン 22をリリースしました。 API バージョン 22には、バージョン 21からの次の変更点が含まれています。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 682cf24c4c7932afeb66a2e5434fe3cec887e889
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 54%

---

# API バージョン 22の新機能

Adobe Workfrontは、2026年5月8日にAPI バージョン 22をリリースしました。 API バージョン 22には、バージョン 21からの次の変更点が含まれています。

## 追加されたリソース

API バージョン 22では、次のリソースが追加されました。

### ReportShareableFolder （RPSHFD）

共有可能なレポートフォルダーを使用してレポートを整理し、それらのフォルダーを他のユーザーと共有できます。 この機能は、大量のレポートを管理し、スケーラブルで一貫性のあるアクセス制御を必要とするチーム向けに設計されています。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>ID</li>
          <li>名前</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>ID</li>
          <li>名前</li>
          <li>objCode</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">デフォルトのフィールド</td>
      <td>
        <ul>
          <li>名前</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## 削除されたリソース

次のリソースがAPI バージョン 22から削除されました。

### UserLocation (USRLOC)

このオブジェクトは削除されました。

## 変更されたリソース

次のリソースがAPI バージョン 22用に変更されました。

### AccessLevel（ACSLVL）

AccessLevel オブジェクトはユーザーに関連付けられていて、ユーザーのアクセス権を指定する AccessLevelPermissions のセットを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが変更され、使用可能な値が変更されました。 詳しくは、開発者ドキュメントを参照してください。
        <ul>
          <li><b>fieldAccessPrivileges</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions（ALVPER）

AccessLevelPermissions オブジェクトは、Workfront オブジェクトにアクセス、作成または変更を行うための特定の権限を表します。 これらの権限は、アクセスレベルに関連付けることができます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが変更され、使用可能な値が変更されました。 詳しくは、開発者ドキュメントを参照してください。
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest（ACSREQ）

Workfront のオブジェクトに対する必要なアクセス権をユーザーが持っていない場合、そのオブジェクトへの利用申請を行うことができます。 AccessRequest オブジェクトは、このリクエストを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが変更され、使用可能な値が変更されました。 詳しくは、開発者ドキュメントを参照してください。
        <ul>
          <li><b>アクション</b></li>
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
      <td>次のフィールドが変更され、使用可能な値が変更されました。 詳しくは、開発者ドキュメントを参照してください。
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Approval（APPROVAL）

タスク、ドキュメント、タイムシートなどの所定の作業アイテムは、上司または他のユーザーが承認することが必要な場合があります。 承認オブジェクトは、作業アイテムに対する承認の操作を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>次のフィールドが追加されました。
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### Company（CMPY）

会社オブジェクトは、人物の集まりで構成される組織を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
        <ul>
          <li><b>esmProjectID</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum（CSTEM）

CustomEnum オブジェクトは、ステータスコードを人間が読み取り可能なテキストに変換する際に役立ちます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>追加済み
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">クエリ</td>
      <td>追加済み
        <ul>
          <li><p><b>assignmentStatus</b></p></li>
          <li><p><b>bookingStatus</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### Customer（CUST）

顧客オブジェクトは、Workfront のインスタンスを使用する組織を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが変更されました。
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>次の可能な値を追加しました。</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> （予約状況）</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> （譲渡状況）</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
         <ul>
         <li><b>isLegacyCustomerEsmStorageEnabled</b></li>
         <li><b>isLegacyCustomerSystemFileMigrationEnabled</b></li>
         <li><b>legacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>legacyCustomerSystemFileMigrationDate</b></li>
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
      <td>次のフィールドが変更されました。
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>エンタープライズストレージ管理をサポートするために、次の可能な値を追加しました。</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
              </li>
             </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>


### Document（DOCU）

Document オブジェクトは、ファイル（書かれた資料、画像、その他の形式の情報など）を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>次のアクションが変更されました。
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>objID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### DocumentFolder（DOCFDR）

ドキュメントをフォルダーに整理できます。 個人用ドキュメントエリアに個人用フォルダーを作成できます。 DocumentFolder オブジェクトは、これらのフォルダーのうちの 1 つを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmFolder</b></li>
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
      <td>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      次のフィールドが変更されました。
        <ul>
          <li><b>version</b><p>バリデータ「必須」を削除しました。</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>次のアクションが追加されました。
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">操作</td>
      <td>次の操作が追加されました。
        <ul>
          <li><p><b>EDIT</b></p>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### ExchangeRate（EXRATE）

ExchangeRate オブジェクトは、Workfrontで設定された為替レートを表します。 ExchangeRate オブジェクトは動的ではありません。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが追加されました。
        <ul>
          <li><b>portfolioID</b></li>
          <li><b>programID
          </b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### JournalEntry（JRNLE）

JournalEntry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。 フィールドをジャーナルエントリオブジェクトの一部としてログに記録するように設定すると、そのフィールドが変更されるたびに、対応するジャーナルエントリが作成されます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが変更されました。
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>次の可能な値を追加しました。</p>
             <ul>
              <li>
                <p><code>PFM</code>（フォルダーの移動）</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b> フラグ </b>
            </p>
            <p>次の可能な値を追加しました。</p>
             <ul>
              <li>
                <p><code>CI</code>（enum.journalentryflagenum.iscontactinfoentry）</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalField （JRNLF）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが変更されました。
        <ul>
          <li>
            <p><b>アクション</b>
            </p>
            <p>次の可能な値を追加しました。</p>
             <ul>
              <li>
                <p><code>PFM</code>（フォルダーの移動）</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask（OPTASK）

OpTask オブジェクトは、一般にイシューと呼ばれます。 イシューは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業アイテムです。 イシューは、ヘルプデスクへのリクエストである場合もあります。 変更指示、リクエスト、バグもイシューです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li><b>actualWorkRequired</b><p>追加されたフラグは次のとおりです。
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">フィールドを検索</td>
      <td>
        <ul>
          <li><b>actualWork</b><p>型が<code>null</code>から<code>double</code>に変更されました。</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest （ORGREQ）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>次の操作が追加されました。
        <ul>
          <li><p><b>COUNT</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>REPORT</b></p>
          <li><p><b>SEARCH</b></p>
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
      <td>次のフィールドが追加されました。
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### ParameterGroup （PGRP）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが追加されました。
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### PortalSection （PTLSEC）

PortalSection オブジェクトはReportです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが追加されました。
        <ul>
          <li><b>reportShareableFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>次のフィールドが追加されました。
        <ul>
          <li><b>reportShareableFolder</b></li>
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
      <td role="rowheader">直接フィールド</td>
      <td>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
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
      <td role="rowheader">直接フィールド</td>
      <td>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      次のフィールドが変更されました。
        <ul>
          <li><b>portfolioID</b><p>バリデーター「必須」を追加しました。</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Project（PROJ）

プロジェクトは Workfront 内の作業アイテムで、Workfront が人々の作業を支援するための主要な構築ブロックです。 プロジェクトオブジェクトは、共通の特定の目標を持つタスクのグループを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### QueueDef（QUED）

QueueDef オブジェクトは、Workfrontのリクエストキュー定義を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが変更され、使用可能な値が変更されました。 詳しくは、開発者ドキュメントを参照してください。
        <ul>
          <li><b>requestorCoreAction</b></li>
          <li><b>requestorForbiddenActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScheduledReport （SCHREP）

ScheduledReport オブジェクトは、配信のスケジュールを設定したレポートを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが変更され、使用可能な値が大幅に変更されました。 詳しくは、開発者ドキュメントを参照してください。
        <ul>
          <li><b>format</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Task（TASK）

タスクオブジェクトは、最終目標の達成（プロジェクトの完了）の一環として完了する必要がある作業項目を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>追加済み</p></li>
          <li><p><b>actualWorkRequired</b></p><p>フラグ <code>AUTO_LOAD</code>および<code>DYNAMIC</code>を追加しました。</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>convertedOpTask</b>
            </p>
            <p>追加済み</p>
          </li>
        </ul> 
      </td>
    </tr>
  </tbody>
</table>

### Template（TMPL）

テンプレートオブジェクトは、プロジェクトのパターンを表します。 プロジェクトをテンプレートから作成することで時間を節約できます。 テンプレートにはチームとタスクが含まれ、テンプレートから作成されたすべてのプロジェクトにコピーされます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>エンタープライズストレージ管理をサポートするために、次のフィールドが追加されました。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Update（UPDATE）

Workfront の作業アイテムを更新して、ユーザーに現在のステータスを知らせることができます。 更新オブジェクトは、これらの更新の 1 つを表します。 更新は、ユーザーが入力するか、Workfront システムが作成することができます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが変更されました。
        <ul>
          <li>
            <p><b>アクション</b>
            </p>
            <p>次の可能な値を追加しました。</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
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
      <td role="rowheader">直接フィールド</td>
      <td>次のフィールドが追加されました。
        <ul>
          <li><b>eauthUserID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>次のフィールドは削除されました。
        <ul>
          <li><b>userLocations</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





