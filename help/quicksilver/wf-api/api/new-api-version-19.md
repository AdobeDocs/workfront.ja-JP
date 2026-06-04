---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 19 の新機能
description: Adobe Workfront は、2022年4月6日（PT）に API バージョン 19 をリリースしました。 API バージョン 19 では、バージョン 18 から次の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
exl-id: 84909dea-7ce1-4ad3-90f5-9dbdb354eaa4
TQID: https://experienceleague.adobe.com/5LLcfkvjzqNZ9tswEkV7lMgFxHS4qcVFJ9YMUI6JazY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 902
ht-degree: 51%

---

# API バージョン 19 の新機能

Adobe Workfront は、2024年4月8日（PT）に API バージョン 19 をリリースしました。 API バージョン 19 では、バージョン 18 から次の変更が行われました。

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
            <p><b>アクセス制限</b><p>追加された可能な値は次のとおりです。
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

割り当てオブジェクトは、作業項目とその作業に割り当てられたユーザー、チーム、またはグループとの間の接続を表します。

割り当てオブジェクトがフラグ **DATA_EXTENDIBLE**&#x200B;を追加しました。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のダイレクトフィールドを追加しました。
        <ul>
          <li>
            <p><b>categoryID</b><p>カテゴリはカスタムフォームです。このフィールドは、カスタムフォームを割り当てに追加する機能をサポートしています。
            </p>
          </li>
          <li>
            <p><b>優先度</b><p>このフィールドでは、次の値を使用できます。
            <ul>
              <li>0 （なし）</li>
              <li>1 （低）</li>
              <li>2 （通常）</li>
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
            <p><b>カテゴリ</b><p>カテゴリはカスタムフォームです。このフィールドは、カスタムフォームを割り当てに追加する機能をサポートしています。
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
            <p><b>objectCategories</b><p>カテゴリはカスタムフォームです。このフィールドは、カスタムフォームを割り当てに追加する機能をサポートしています。
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
      <td>次のアクションを追加しました。
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
                <p>割り当て優先度（PRIORITY_ASSIGNMENT）
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
            <p><b>名前</b><p>次の可能な値を削除しました。
            </p>
            <ul>
              <li>
                <p>更新ストリームでZoom統合を有効にする（パスワード：zoomIntegrationEnabled）
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
            <p><b>createLargeDocument</b><p>フィールド <code>folderID</code>を追加しました。</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>追加済み。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### ExchangeRate（EXRATE）

ExchangeRate オブジェクトは、Workfrontで設定された為替レートを表します。 ExchangeRate オブジェクトは動的ではありません。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
      <ul>
      <li>次のフィールドがバリデータ <code>REQUIRED</code>を追加しました：
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

グループオブジェクトは、一連のユーザーとチームを表します。 グループは、多くの場合、部門の構造を表します。

グループオブジェクトがフラグ **SHARABLE**&#x200B;を追加しました。

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
          <li><p><b>rejectionComment</b></li>
          <li><p><b>submittedByID</b></li>
          </ul>
          <p><b>時間</b> フィールドに次の変更が加えられました。</p>
          <ul> 
          <li> バリデータ <b>GREATER_THAN</b>を削除しました</li>
          <li> バリデータ <b>NOT_EQUAL</b>を追加しました</li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
      次のアクションが追加されました。
        <ul>
          <li><p><b>承認</b></li>
          <li><p><b>承認しない</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry（JRNLE）

JournalEntry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。 フィールドをジャーナルエントリオブジェクトの一部としてログに記録するように設定すると、そのフィールドが変更されるたびに、対応するジャーナルエントリが作成されます。

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
                <p>CR （コスト率）
                </p>
              </li>
              <li>
                <p>請求率（BR）
                </p>
              </li>
              <li>
                <p>ゼネラルファイナンス（GF）
                </p>
              </li>
              <li>
                <p>複合金融（CF）
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
            <p><b>displayType</b></p><p>より使いやすく柔軟なシステムを作成するために、<b> ウィジェット（WIDGET） </b> フィールドタイプは廃止され、次のフィールドタイプに分割されました。
            <ul>
            <li>Adobe XD （ADOBEXD）</li>
            <li>画像（画像）</li>
            <li>PDF（PDF）</li>
            <li>ビデオ（ビデオ）</li>
            <li>外部参照（EXTRNL）</li>
            <li>複数選択外部参照（MULTEXTRNL）</li>
            <li>ネイティブフィールド（WFNATIVE）</li>
            <li>プランニングフィールド（WFPLANNING）</li>
            <li>期間別KPI （タイムフェーズ）</li>
            <li>ロールアップ（ロールアップ）</li>
            <li>文書（文書）</li>
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

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。 これらの質問は通常、ポートフォリオマネージャーが決定し、その回答によって、マネージャーはプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
            <p><b>displayType</b></p><p>より使いやすく柔軟なシステムを作成するために、<b> ウィジェット（WIDGET） </b> フィールドタイプは廃止され、次のフィールドタイプに分割されました。
            <ul>
            <li>Adobe XD （ADOBEXD）</li>
            <li>画像（画像）</li>
            <li>PDF（PDF）</li>
            <li>ビデオ（ビデオ）</li>
            <li>外部参照（EXTRNL）</li>
            <li>複数選択外部参照（MULTEXTRNL）</li>
            <li>ネイティブフィールド（WFNATIVE）</li>
            <li>プランニングフィールド（WFPLANNING）</li>
            <li>期間別KPI （タイムフェーズ）</li>
            <li>ロールアップ（ロールアップ）</li>
            <li>文書（文書）</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment （TASSGN）

TemplateAssignment オブジェクトは、テンプレートタスクとその作業に割り当てられたユーザー、チーム、またはグループとの接続を表します。 テンプレートをプロジェクトに使用すると、そのユーザー、チーム、またはグループがタスクに割り当てられます。

TemplateAssignment オブジェクトがフラグ **DATA_EXTENDIBLE**&#x200B;を追加しました。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>次のダイレクトフィールドを追加しました。
        <ul>
          <li>
            <p><b>categoryID</b><p>カテゴリはカスタムフォームです。このフィールドは、カスタムフォームを割り当てに追加する機能をサポートしています。
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>次の参照フィールドを追加しました。
        <ul>
          <li>
            <p><b>カテゴリ</b><p>カテゴリはカスタムフォームです。このフィールドは、カスタムフォームを割り当てに追加する機能をサポートしています。
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
            <p><b>objectCategories</b><p>カテゴリはカスタムフォームです。このフィールドは、カスタムフォームを割り当てに追加する機能をサポートしています。
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
            <p><b>objCode</b></p><p>削除済み。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>
