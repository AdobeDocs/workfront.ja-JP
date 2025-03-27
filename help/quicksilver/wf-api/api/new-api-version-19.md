---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 19 の新機能
description: Adobe Workfront は、2022年4月6日（PT）に API バージョン 19 をリリースしました。API バージョン 19 では、バージョン 18 から次の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
exl-id: 84909dea-7ce1-4ad3-90f5-9dbdb354eaa4
source-git-commit: 1c1f9f46ea25ffa7d01c1a762b0478a5edb3339e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 50%

---

# API バージョン 19 の新機能

Adobe Workfront は、2024年4月8日（PT）に API バージョン 19 をリリースしました。API バージョン 19 では、バージョン 18 から次の変更が行われました。

## 追加されたリソース

API バージョン 19 にはリソースが追加されませんでした。

## 削除されたリソース

API バージョン 19 で削除されたリソースはありません。

## 変更されたリソース

### AccessLevel（ACSLVL）

AccessLevel オブジェクトはユーザーに関連付けられていて、ユーザーのアクセス権を指定する AccessLevelPermissions のセットを表します。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>追加された可能な値は次のとおりです。
            </p>
            <ul>
              <li>
                <p>Workfront AI アシスタント（AIOFF）を無効にする
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Assignment（ASSIGN）

Assignment オブジェクトは、作業項目とその作業に割り当てられたユーザー、チーム、またはグループとの関連付けを表します。

Assignment オブジェクトによってフラグ **DATA_EXTENDIBLE** が追加されました。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次の直接フィールドを追加しました。
        <ul>
          <li>
            <p><b>categoryID</b><p>カテゴリはカスタムフォームです。このフィールドでは、割り当てにカスタムフォームを追加する機能をサポートしています。
            </p>
          </li>
          <li>
            <p><b>優先度</b><p>このフィールドでは、次の値を使用できます。
            <ul>
              <li>0 （なし）</li>
              <li>1 （低）</li>
              <li>2 （標準）</li>
              <li>3 （高）</li>
              <li>4 （緊急）</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>次の参照フィールドを追加しました。
        <ul>
          <li>
            <p><b>category</b><p>カテゴリはカスタムフォームです。このフィールドでは、割り当てにカスタムフォームを追加する機能をサポートしています。
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>次のコレクションフィールドを追加しました。
        <ul>
          <li>
            <p><b>objectCategories</b><p>カテゴリはカスタムフォームです。このフィールドでは、割り当てにカスタムフォームを追加する機能をサポートしています。
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Category（CTGY）

カテゴリオブジェクトはカスタムフォームです。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>割り当てにカスタムフォームを追加する機能をサポートするために、次のフィールドが追加されました。
        <ul>
          <li>
            <p><b>catObjCode</b><p>追加された可能な値は次のとおりです。
            </p>
            <ul>
              <li>
                <p>Assignment（ASSIGN）
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>追加された可能な値は次のとおりです。
            </p>
            <ul>
              <li>
                <p>Assignment（ASSIGN）
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 分類子（CLSF）

分類子は場所です。

<table>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>以下のアクションを追加しました。
        <ul>
          <li>
            <b>activateClassifiers</b>
          </li>
          <li>
            <b>deactivateClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### 顧客

顧客オブジェクトは、Workfront のインスタンスを使用する組織を表します。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumTypes</b><p>追加された可能な値は次のとおりです。
            </p>
            <ul>
              <li>
                <p>割り当ての優先度（PRIORITY_ASSIGNMENT）
                </p>
              </li>
             </ul>
          </li>
              <p>CustomEnum オブジェクトは、ステータスコードを人間が読み取り可能なテキストに変換する際に役立ちます。</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### CustomerPreferences（CUSTPR）

CustomerPreferences オブジェクトは、Workfront のインスタンスに対して顧客が設定した一連の環境設定を表します。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>名前</b><p>以下の可能な値を削除しました。
            </p>
            <ul>
              <li>
                <p>更新ストリームで Zoom 統合を有効にする（パスワード：zoomIntegrationEnabled）
                </p>
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
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>フィールド <code>folderID</code> を追加しました。</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>追加済み。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### ExchangeRate（EXRATE）

ExchangeRate オブジェクトは、Workfrontで設定された通貨の為替レートを表します。 ExchangeRate オブジェクトは動的ではありません。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
      <ul>
      <li>次のフィールドにバリデーター <code>REQUIRED</code> が追加されました。
        <ul>
          <li><p><b>通貨</b></li>
          <li><p><b>率</b></li></ul>
      <li>次のフィールドが追加されました。
        <ul>
          <li><p><b>enteredByID</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>
      <ul>
        <li>次のフィールドが追加されました。
        <ul>
          <li><p><b>enteredBy</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### グループ（GROUP）

グループオブジェクトは、一連のユーザーとチームを表します。グループは、多くの場合、部門の構造を表します。

Group オブジェクトはフラグ **共有可能** を追加しました。

### Hour（HOUR）

Hour オブジェクトは、ユーザーがタイムシートに記録した時間を表します。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
      次のフィールドが追加されました。
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilled</b></li>
          <li><p><b>rejectedByID</b></li>
          <li><p><b>rejectedOnDate</b></li>
          <li><p><b>rejectComment</b></li>
          <li><p><b>submittedByID</b></li>
          </ul>
          <p>「<b> 時間 </b> フィールドに次の変更が加えられました。</p>
          <ul> 
          <li> 削除されたバリデーター <b>GREATER_THAN</b></li>
          <li> 追加されたバリデーター <b>NOT_EQUAL</b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
      次のアクションが追加されました。
        <ul>
          <li><p><b>承認</b></li>
          <li><p><b>承認取消</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry（JRNLE）

JournalEntry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。フィールドをジャーナルエントリオブジェクトの一部としてログに記録するように設定すると、そのフィールドが変更されるたびに、対応するジャーナルエントリが作成されます。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>フラグ</b><p>追加された可能な値は次のとおりです。
            </p>
            <ul>
              <li>
                <p>コスト率（CR）
                </p>
              </li>
              <li>
                <p>請求料金（BR）
                </p>
              </li>
              <li>
                <p>一般財務（GF）
                </p>
              </li>
              <li>
                <p>コンバインド・ファイナンス（CF）
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Parameter（PARAM）

パラメーターオブジェクトは、カスタムフィールドです。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>次の値を追加しました。
            <ul>
            <li>期間（DRTN）</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>より使いやすい柔軟なシステムを作成するために、<b>Widget （WIDGET） </b> フィールドタイプは非推奨（廃止予定）になり、次のフィールドタイプに分割されました。
            <ul>
            <li>Adobe XD （ADOBEXD）</li>
            <li>画像（IMAGE）</li>
            <li>PDF（PDF）</li>
            <li>ビデオ（ビデオ）</li>
            <li>外部検索（EXTRNL）</li>
            <li>複数選択外部検索（MULTEXTRNL）</li>
            <li>ネイティブフィールド （WFNATIVE）</li>
            <li>計画フィールド （WFPLANNING）</li>
            <li>時間配分 KPI （時間配分）</li>
            <li>ロールアップ （ロールアップ）</li>
            <li>ドキュメント（ドキュメント）</li>
           </ul>
          </li>
          <li>
            <p><b>設定</b><p>追加済み。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Role（ROLE）

Role オブジェクト（担当業務）は、デザイナーやプロダクトマネージャーなど、ユーザーが入力できる機能またはスキルセットを表します。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
    次のフィールドが追加されました。
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>
        次のフィールドが追加されました。
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion {#scorecardquestion}

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。これらの質問は通常、ポートフォリオマネージャーが決定し、その回答によって、マネージャーはプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
            <p><b>displayType</b></p><p>より使いやすい柔軟なシステムを作成するために、<b>Widget （WIDGET） </b> フィールドタイプは非推奨（廃止予定）になり、次のフィールドタイプに分割されました。
            <ul>
            <li>Adobe XD （ADOBEXD）</li>
            <li>画像（IMAGE）</li>
            <li>PDF（PDF）</li>
            <li>ビデオ（ビデオ）</li>
            <li>外部検索（EXTRNL）</li>
            <li>複数選択外部検索（MULTEXTRNL）</li>
            <li>ネイティブフィールド （WFNATIVE）</li>
            <li>計画フィールド （WFPLANNING）</li>
            <li>時間配分 KPI （時間配分）</li>
            <li>ロールアップ （ロールアップ）</li>
            <li>ドキュメント（ドキュメント）</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment （ASSGN）

TemplateAssignment オブジェクトは、テンプレート タスクと、そのタスクの作業に割り当てられたユーザー、チーム、またはグループとの関係を表します。 テンプレートがプロジェクトに使用されると、そのユーザー、チームまたはグループがタスクに割り当てられます。

TemplateAssignment オブジェクトによってフラグ **DATA_EXTENDIBLE** が追加されました。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次の直接フィールドを追加しました。
        <ul>
          <li>
            <p><b>categoryID</b><p>カテゴリはカスタムフォームです。このフィールドでは、割り当てにカスタムフォームを追加する機能をサポートしています。
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>次の参照フィールドを追加しました。
        <ul>
          <li>
            <p><b>category</b><p>カテゴリはカスタムフォームです。このフィールドでは、割り当てにカスタムフォームを追加する機能をサポートしています。
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>次のコレクションフィールドを追加しました。
        <ul>
          <li>
            <p><b>objectCategories</b><p>カテゴリはカスタムフォームです。このフィールドでは、割り当てにカスタムフォームを追加する機能をサポートしています。
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
  <tbody>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>を削除しました。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>
