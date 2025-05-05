---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 20 の新機能
description: Adobe Workfront は、2022年4月6日（PT）に API バージョン 20 をリリースしました。API バージョン 20 では、バージョン 19 から次の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 61%

---

# API バージョン 20 の新機能

Adobe Workfront は、2025年5月4日（PT）に API バージョン 20 をリリースしました。API バージョン 20 では、バージョン 19 から次の変更が行われました。

## 追加されたリソース

API バージョン 20 にはリソースが追加されませんでした。

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## 削除されたリソース

API バージョン 20 で削除されたリソースはありません。

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
                <p><code>REMOVE_CUSTOMFORM</code> （カスタム データから削除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （サブプロジェクトの追加）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （カスタム データから削除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （サブプロジェクトの追加）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （カスタム データから削除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （サブプロジェクトの追加）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> （カスタム データから削除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （サブプロジェクトの追加）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> （カスタム データから削除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （サブプロジェクトの追加）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （カスタム データから削除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （サブプロジェクトの追加）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （カスタム データから削除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （サブプロジェクトの追加）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
              <li>
                <p><code>tiff</code> （enum.fileextension.tiff）</p>
              </li>
            </ul>
          </li>
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
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>billedRevenue</li>
              <li>予算</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRiskCost</li>
              <li>plannedvalue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>フラグ <code>DYNAMIC</code>、<code>LAZY_READ</code>、を追加しました。 <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>フラグを追加しました <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>可能な値 <code>URH</code> を追加しました（ユーザーおよび役割（毎時）） </li>
          <li><p><b>revenueType</b></p> <p><code>URH</code> （ユーザーおよびロール （毎時））、<code>URC</code> （ユーザーおよびロール （毎時、キャップ付き）、および <code>URF</code> （ユーザーおよびロール （毎時、固定））の可能な値を追加しました</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
          <p>以下のフィールドが追加されました。</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Assignment（ASSIGN）

Assignment オブジェクトは、作業項目とその作業に割り当てられたユーザー、チーム、またはグループとの関連付けを表します。

Assignment オブジェクトは、フラグ `ATTRIBUTE_ATTACHABLE` および `DOMAIN_EXTENDABLE` を追加しました。


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### アバター

アバターのオブジェクトは、ユーザー写真です。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>追加済み</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コアフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>追加済み</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b> コピー </b>
            </p>
             <p>追加済み</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

### Baseline（BLIN）

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
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>予算</li>
              <li>eac</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>actualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>フラグを追加しました <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BaselineTask（BSTSK）

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
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>actualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>フラグを追加しました <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BillingRecord（BILL）

BillingRecord オブジェクトは、請求可能な収益、時間または費用を記録します。この情報は、外部の会計システムで請求書を作成する際に使用できます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>量</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>追加済み</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

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
            <p><b> 設定 </b>
            </p>
             <p>追加済み</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Company（CMPY）

会社オブジェクトは、人物の集まりで構成される組織を表します。

Company オブジェクトがフラグ `SHARABLE` を追加しました。

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

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
             <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> （singleassignmentschedule）</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> （config.loggedtaskissuemove）</p></li>
            </ul>
          </li>
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
      <td>
           <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>率</li>
      </td>
    </tr>
  </tbody>
</table>


### FinancialData（FINDAT）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualExpenseCost</li>
              <li>actualFixedRevenue</li>
              <li>actualLaborCost</li>
              <li>actualLaborCostHours</li>
              <li>actualLaborRevenue</li>
              <li>actualNonBillableExpenseCost</li>
              <li>fixedCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedFixedRevenue</li>
              <li>plannedLaborCost</li>
              <li>plannedLaborCostHours</li>
              <li>plannedLaborRevenue</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianceExpenseCost</li>
              <li>varianceLaborCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

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
            <p><b> 通貨 </b>
            </p>
             <p>追加済み</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>追加済み</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask（OPTASK）

OpTask オブジェクトは、一般にイシューと呼ばれます。イシューは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業アイテムです。イシューは、ヘルプデスクへのリクエストである場合もあります。変更指示、リクエスト、バグもイシューです。

OpTask オブジェクトはフラグ DOMAIN_EXTENDABLE を追加しました

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>actualCost</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
              <li>actualCost</li>
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
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>INTRNL</code> （内部参照）</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> （複数選択内部検索）</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> （enum.parameterdisplaytypeenum.uiextension）</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio（PORT）

ポートフォリオオブジェクトは、同じリソース（通常はプロジェクトを完了するための資金や人材）を競い合って完了するプロジェクトのコレクションです。

Portfolio オブジェクトがフラグ `DOMAIN_EXTENDABLE` を追加しました。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>整合済み</li>
              <li>予算</li>
              <li>通貨</li>
              <li>netValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Program（PRGM）

プログラムオブジェクトは、ポートフォリオ内のプロジェクトのサブセットで、類似のプロジェクトを 1 つにグループ化できます。

Program オブジェクトはフラグ `DOMAIN_EXTENDABLE` を追加しました。

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
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>billedRevenue</li>
              <li>予算</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>eac</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>plannedvalue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>フラグを追加しました <code>CURRENCY</code></li>
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
                <p><code>REMOVE_CUSTOMFORM</code> （カスタム データから削除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （サブプロジェクトの追加）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （カスタム データから削除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （サブプロジェクトの追加）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Rate（RATE）

Rate オブジェクトは、Workfront の請求料金を表します。

Rate オブジェクトはフラグ `ATTRIBUTE_ATTACHABLE` を追加しました。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>以下のフィールドが追加されました。
          <ul>
          <li>通貨</li>
          <li>locked</li>
          <li>タイプ</li>
          <li>value</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Role（ROLE）

Role オブジェクト（担当業務）は、デザイナーやプロダクトマネージャーなど、ユーザーが入力できる機能またはスキルセットを表します。

Role オブジェクトがフラグ `DOMAIN_EXTENDABLE` を追加しました。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
          <p>以下のフィールドが追加されました。
          <ul>
          <li>billingRates</li>
          <li>costRates</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
              <li>
                <p><code>tiff</code> （enum.fileextension.tiff）</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion（SCOREQ）

ScoreCardQuestion オブジェクトは、スコアカードに追加された質問を表します。これらの質問は通常、ポートフォリオマネージャーが決定し、その回答によって、マネージャーはプロジェクトがポートフォリオの目標にどの程度適合しているかを理解できます。

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
             <p>追加された可能な値は次のとおりです。</p>
             <ul>
              <li><p><code>INTRNL</code> （内部参照）</p></li>
              <li><p><code>MULTINTRNL</code> （複数選択内部検索）</p></li>
              <li><p><code>UIEXTNSION</code> （enum.parameterdisplaytypeenum.uiextension）</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Task（TASK）

タスクオブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

Task オブジェクトはフラグ `DOMAIN_EXTENDABLE` を追加しました。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>追加された可能な値は次のとおりです。<ul><li><code>URH</code> （ユーザーおよび役割（毎時）</li></ul></li>
          <li><p><b>revenueType</b></p> <p>追加された可能な値は次のとおりです。<ul><li><code>URH</code> （ユーザーおよび役割（毎時）</li><li><code>URC</code> （ユーザーおよび役割（毎時） （上限付き）</li><li><code>URF</code> （ユーザーおよび役割（毎時） +固定）</li></ul></li>
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
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>予算</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>workRequired</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
          <p>以下のフィールドが追加されました。</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateTask（TTSK）

TemplateTask オブジェクトは、テンプレートに含まれるタスクを表します。テンプレートタスクは、テンプレートが使用されるプロジェクト内のタスクになります。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>billingAmount</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>revenueType</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>追加された可能な値は次のとおりです。<ul><li><code>URH</code> （ユーザーおよび役割（毎時）</li></ul></li>
          <li><p><b>revenueType</b></p> <p>追加された可能な値は次のとおりです。<ul><li><code>URH</code> （ユーザーおよび役割（毎時）</li><li><code>URC</code> （ユーザーおよび役割（毎時） （上限付き）</li><li><code>URF</code> （ユーザーおよび役割（毎時） +固定）</li></ul></li>
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
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
             <p>削除されました</p>
          </li>
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
                <p><code>externalFolderMetadataError</code> （enum.updatetypeenum.externalFolderMetadataError）</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### User （USER）

ユーザーオブジェクトは、ログインしてシステムとやり取りできる Workfront アカウントを持つユーザーを表します。

ユーザーオブジェクトがフィールド `ATTRIBUTE_ATTACHABLE` と `DOMAIN_EXTENDABLE` を追加しました。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
          <p>以下のフィールドが追加されました。</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
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
            <p>次のフィールドにフラグ <code>RESTRICTABLE</code> が追加されました。
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>次のフィールドのタイプが <code>double</code> から <code>class java.math.BigDecimal</code> に変更されました。
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>フラグ <code>DYNAMIC</code>、<code>LAZY_READ</code>、を追加しました。 <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>フラグを追加しました <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>可能な値 <code>URH</code> を追加しました（ユーザーおよび役割（毎時）） </li>
          <li><p><b>revenueType</b></p> <p><code>URH</code> （ユーザーおよびロール （毎時））、<code>URC</code> （ユーザーおよびロール （毎時、キャップ付き）、および <code>URF</code> （ユーザーおよびロール （毎時、固定））の可能な値を追加しました</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



