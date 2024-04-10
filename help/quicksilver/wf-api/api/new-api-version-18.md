---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 18 の新機能
description: Adobe Workfront は、2022年4月6日（PT）に API バージョン 18 をリリースしました。API バージョン 18 では、バージョン 15 から次の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 69%

---

# API バージョン 18 の新機能

Adobe Workfront は、2024年4月8日（PT）に API バージョン 18 をリリースしました。API バージョン 18 では、バージョン 15 から次の変更が行われました。

## 追加されたリソース

API バージョン 18 にはリソースが追加されませんでした。

## 削除されたリソース

API バージョン 18 で削除されたリソースはありません。

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
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （原価率の表示）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （請求料金の表示）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （一般財務の表示）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （コスト率の編集）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （請求レートの編集）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （財務全般の編集）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （原価率の表示）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （請求料金の表示）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （一般財務の表示）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （コスト率の編集）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （請求レートの編集）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （財務全般の編集）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （原価率の表示）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （請求料金の表示）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （一般財務の表示）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （コスト率の編集）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （請求レートの編集）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （財務全般の編集）</p>
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
            <p><b>アクション</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （原価率の表示）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （請求料金の表示）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （一般財務の表示）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （コスト率の編集）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （請求レートの編集）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （財務全般の編集）</p>
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
            <p><b>coreAction</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （原価率の表示）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （請求料金の表示）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （一般財務の表示）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （コスト率の編集）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （請求レートの編集）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （財務全般の編集）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （原価率の表示）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （請求料金の表示）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （一般財務の表示）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （コスト率の編集）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （請求レートの編集）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （財務全般の編集）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （原価率の表示）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （請求料金の表示）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （一般財務の表示）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （コスト率の編集）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （請求レートの編集）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （財務全般の編集）</p>
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
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 承認待ち（AWAPVL）

<table>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p>次の操作を追加しました。
            </p>
            <ul>
              <li>
                <p><b>追加</b>
                </p>
              </li>
              <li>
                <p><b>削除</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ベースライン （BLIN）

ベースラインは、特定の時点でのプロジェクトのパフォーマンスを示すスナップショットです。主要な日付、進捗状況、コスト、売上高など、プロジェクトに関する主要な情報が保存されています。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ベースライン タスク （BSTSK）

ベースラインは、特定の時点でのプロジェクトのパフォーマンスを示すスナップショットです。主要な日付、進捗状況、コスト、売上高など、プロジェクトに関する主要な情報が保存されています。ベースラインを作成すると、そのベースラインのベースラインタスクに関するタスク情報も取り込まれます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
            <p><b>catObjCode</b>:
            </p>
            <p>追加された可能な値は次のとおりです。
            <ul>
              <li>
                <p><code>NLBRCY</code> （非労務資源の区分）
                </p>
              </li>
              <li>
                <p><code>HOUR</code> （時間）
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> （評価カード）
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>追加された可能な値は次のとおりです。
            <ul>
              <li>
                <p><code>NLBRCY</code> （非労務資源の区分）
                </p>
              </li>
              <li>
                <p><code>HOUR</code> （時間）
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> （評価カード）
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ドキュメント （DOCU）

Document オブジェクトは、ファイル（書かれた資料、画像、その他の形式の情報など）を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>次のパラメーターを追加しました。
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>:
            </p>
            <p>追加済み。この新しいアクションでは、次のパラメーターを使用します。
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### FinancialData （FINDAT）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p><code>AAO</code> （enum.actiontypeenum.assetapproval.opened）</p>
              </li>
              <li>
                <p><code>ADM</code> （enum.actiontypeenum.assetapproval.locked.all.decisions.made）</p>
              </li>
              <li>
                <p><code>AUL</code> （enum.actiontypeenum.assetapproval.unlocked.manual）</p>
              </li>
              <li>
                <p><code>ALM</code> （enum.actiontypeenum.assetapproval.locked.manual）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask （OPTASK）

OpTask オブジェクトは、一般にイシューと呼ばれます。イシューは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業アイテムです。イシューは、ヘルプデスクへのリクエストである場合もあります。変更指示、リクエスト、バグもイシューです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>:
            </p>
            <p>以下のフィールドを追加しました。
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>:
            </p>
            <p>以下のフィールドを追加しました。
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
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
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>createProjectWithOverride</b>
            </p>
             <p>追加済み。
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ProjectUserRole （PTEAM）

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
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
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （原価率の表示）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （請求料金の表示）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （一般財務の表示）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （コスト率の編集）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （請求レートの編集）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （財務全般の編集）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （原価率の表示）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （請求料金の表示）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （一般財務の表示）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （コスト率の編集）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （請求レートの編集）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （財務全般の編集）</p>
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
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>次のフラグを追加しました。
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>動的
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>displayName</b></p><p>追加済み。</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>displayName</b>
            </p><p>追加済み。</p>
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
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>convertToProject</b>
            </p>
             <p>次のフィールドを追加しました。
             <ul><li><code>copyCategories</code></li></ul>
            </p>
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
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### TemplateTask （TTSK）

TemplateTask オブジェクトは、テンプレートに含まれるタスクを表します。テンプレートタスクは、テンプレートが使用されるプロジェクト内のタスクになります。<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole （TTEAM）

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
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
            <p>次のフィールドを削除しました。
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
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
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
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
            <p><b>recentUpdatesObjIDs</b>
            </p>
            <p>追加済み。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue （USERPF）

UserPrefValue オブジェクトは、ユーザーの環境設定を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>value</b>
            </p>
            <p>バリデーターを追加しました。 <code>MAX_LENGTH</code></p>
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
            <p>以下のフィールドを追加しました。
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

