---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 21 の新機能
description: Adobe Workfront は、2025年10月23日（PT）に API バージョン 21 をリリースしました。API バージョン 21 では、バージョン 20 から次の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 1c3272c7830bf0a6feddea0281b0e2879b87eacf
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 85%

---

# API バージョン 21 の新機能

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。プレビューサンドボックス環境でのみ使用できます。</span>

Adobe Workfront は、2025年10月23日（PT）に API バージョン 21 をリリースしました。API バージョン 21 では、バージョン 20 から次の変更が行われました。

## 追加されたリソース

### OriginalRequest （ORGREQ）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>entryDate</li>
          <li>ID</li>
          <li>requestID</li>
          <li>requestName</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>ID</li>
          <li>objCode</li>
        </ul>
      </td>
 </tbody>
</table>

<!--

### StaffingPlanTemplate (SPTMPL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
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

-->

## 削除されたリソース

### AssignmentBillingRole （ASBLRL）

AssignmentBillingRole オブジェクトとそのすべてのフィールドが削除されました。

## 変更されたリソース

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
            <p><b>coreAction</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （連絡先情報の編集）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （連絡先情報の編集）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （連絡先情報の編集）</p>
              </li>
            </ul>
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
            <p><b>アクション</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （連絡先情報の編集）</p>
              </li>
            </ul>
         </li>
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
            <p><b>coreAction</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （連絡先情報の編集）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （連絡先情報の編集）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （連絡先情報の編集）</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### アナウンス添付ファイル （ANMATT）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>fileExtension</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>追加済み</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>追加済み</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Assignment（ASSIGN）

Assignment オブジェクトは、作業項目とその作業に割り当てられたユーザー、チーム、またはグループとの関連付けを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>削除されました</p>
              </li>
            </ul>
         </li>
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
            <p><b>catObjCode</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> （enum.categorytypeenum.staffingplantemplate）</p>
              </li>
              <li>
                <p><code>TEAMOB</code> （チーム）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> （enum.categorytypeenum.staffingplantemplate）</p>
              </li>
              <li>
                <p><code>TEAMOB</code> （チーム）</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Customer（CUST）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> （タイムライン計算のための Java アプレットの使用を無効にする）
            </p>
            <p>追加済み</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Document（DOCU）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>追加済み</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder

DocumentFolder オブジェクトにフラグ `RESTORABLE` が追加されました。

### Hour（HOUR）

Hour オブジェクトは、ユーザーがタイムシートに記録した時間を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>getTerjectionCommentporaryCloudURL</b>
            </p>
            <p>バリデーターを追加済み <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### OpTask（OPTASK）

OpTask オブジェクトは、一般にイシューと呼ばれます。イシューは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業アイテムです。イシューは、ヘルプデスクへのリクエストである場合もあります。変更指示、リクエスト、バグもイシューです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>追加済み</p>
              </li>
            </ul>
         </li>
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
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>RICHLX</code> （字句リッチテキスト）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> （単一行ロールアップ）</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>追加済み</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">デフォルトのフィールド</td>
      <td>
        <ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>追加済み</p>
           </li>
           </ul>
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
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>追加済み</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b> 通貨 </b>
            </p>
            <p>追加済み</p>
              </li>
            </ul>
         </li>
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
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>追加済み</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef（QUED）

QueueDef オブジェクトは、キューを表します。キューは、ユーザーがイシューを送信できるようにヘルプデスクエリアに公開されたプロジェクトです。

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
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （連絡先情報の編集）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> （連絡先情報の編集）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>helpDeskProjects</b>
            </p>
            <p>追加済み</p>
            </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Rate（RATE）

Rate オブジェクトは、Workfront の請求料金を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>localBillingPerHour</b>
            </p>
            <p>削除されました</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>削除されました</p>
              </li>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Role（ROLE）

Role オブジェクト（担当業務）は、デザイナーやプロダクトマネージャーなど、ユーザーが入力できる機能またはスキルセットを表します。

<div class="preview">

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b> 通貨を上書き </b>
            </p>
            <p>削除されました</p>
              </li>
          <li>
            <p><b> コスト率を上書き </b>
            </p>
            <p>削除されました</p>
              </li>
          <li>
            <p><b> 請求レートの上書き </b>
            </p>
            <p>削除されました</p>
              </li>
      </td>
    </tr>
  </tbody>
</table>

</div>

### スケジュール済みレポート （SCHREP）

ScheduledReport オブジェクトは、配信のスケジュールを設定したレポートを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>形式</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion（SCOREQ）

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。これらの質問は通常、ポートフォリオマネージャーが決定し、その回答によって、マネージャーはプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。<table>
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
            <p>次の値を追加しました。</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> （単一行ロールアップ）</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### StaffingPlan

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

<!--

### StaffingPlanResource

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

### Task（TASK）

タスクオブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>追加済み</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>追加済み</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### チーム

チーム オブジェクトは、フラグ `DATA_EXTENDIBLE` および `SHARABLE` を追加しました。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>追加済み</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">参照フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>category</b>
            </p>
            <p>追加済み</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
            <p>追加済み</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### TemplateAssignment

TemplateAssignment オブジェクトによってフラグ `ATTRIBUTE_ATTACHABLE` が追加されました。

### Timesheet（TSHET）

Timesheet オブジェクトは、タスク、プロジェクトおよびオーバーヘッド時間タイプに対して行った実際の時間数をユーザーが入力できる仮想タイムカードを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コアフィールド</td>
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

### Work（WORK）

作業オブジェクトは、Task と OpTask の両方が継承する共通のインターフェイスで、2 つの間で共通のコードを共有します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>追加済み</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>teamAssignments</b>
            </p>
            <p>追加済み</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


