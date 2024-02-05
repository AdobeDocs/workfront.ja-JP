---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 16 の新機能
description: Adobe Workfront では、2022年4月6日に API バージョン 16 がリリースされています。API バージョン 16 では、バージョン 15 から次の変更が行われました。
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 100%

---

# API バージョン 16 の新機能

Adobe Workfront は、2023年4月6日（PT）に API バージョン 16 をリリースしました。API バージョン 16 では、バージョン 15 から次の変更が行われました。

## 追加されたリソース

API バージョン 16 で追加されたリソースはありません。

## 削除されたリソース

API バージョン 16 で削除されたリソースはありません。

## 変更されたリソース

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Approval（APPROVAL）](#approval-approval)
* [CustomerPreferences（CUSTPR）](#customerpreferences-custpr)
* [ExternalSection（EXTSEC）](#externalsection-extsec)
* [Hour（HOUR）](#hour-hour)
* [LayoutTemplate（UITMPL）](#layouttemplate-uitmpl)
* [Note（NOTE）](#note-note)
* [OpTask / Issue（OPTASK）](#note-note)
* [Project（PROJ）](#project-proj)
* [Rate（RATE）](#rate-rate)
* [RichTextNote（RHNOTE）](#richtextnote-rhnote)
* [Role / Job Role（ROLE）](#role--job-role-role)
* [Task（TASK）](#task-task)
* [Timesheet（TSHET）](#timesheet-tshet)
* [UIFilter / Filter（UIFT）](#uifilter--filter-uift)
* [UIGroupBy / Grouping（UIGB）](#uigroupby--grouping-uigb)
* [UIView / View表示（UIVW）](#uiview--view-uivw)
* [User （USER）](#user-user)
* [UserNote（USRNOT）](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

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
            <p><b>workPerDate</b>
            </p>
            <p>このフィールドが追加され、1 日あたりの必要な作業時間数を分単位で表示します。形式は <code>YYYY-MM-DD: (number of minutes)</code> で、タイムゾーンが考慮されます。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Assignment（ASSIGN）

割り当てオブジェクトは、作業アイテムと、作業アイテムに割り当てられたユーザー、チーム、グループとの間の接続を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>このフィールドが追加され、1 日あたりの必要な作業時間数を分単位で表示します。形式は <code>YYYY-MM-DD: (number of minutes)</code> で、タイムゾーンが考慮されます。</p>
          </li>
          <li>
            <p><b>isContoured</b>
            </p>
            <p>この追加されたフィールドは、割り当てが配分されているかどうかを反映するブール値です。割り当ての 1 日あたりの分数がワークロードバランサーで編集された場合、割り当ては配分されています。</p>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
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
            <p>追加された可能な値は次のとおりです。</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
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
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>このアクションは、コントリビューターライセンスの所有者を自動アップグレードするオプションを顧客が無効にしたかどうかを示すブール値を返します。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection（EXTSEC）

ExternalSection オブジェクトは、Workfront レポートに埋め込まれる外部 web ページです。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>これが追加され、レポートに埋め込まれた iFrame の URL を計算します。</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>これが追加され、レポートに埋め込まれた iFrame の URL（複数）を計算します。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>追加済み。このパラメーターは、<code>batchSave</code> で作成された時間を識別するために使用されます。 </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### Note（NOTE）

メモオブジェクトは、Workfront オブジェクトに対するコメントまたは更新です。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
          <li>
            <p><b>attachedDocuments</b>
            </p>
            <p>このフィールドが追加され、コメントに添付されたドキュメントのリストを表します。</p>
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
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>このフィールドが追加され、1 日あたりの必要な作業時間数を分単位で表示します。形式は <code>YYYY-MM-DD: (number of minutes)</code> で、タイムゾーンを考慮します。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>このアクションにより、複数のチームをタスクまたはイシューに割り当てる機能をサポートするフィールド <code>teamIDs</code> が追加されました。</p>
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
            <p>このフィールドが追加され、プロジェクトのすべての予算計上時間数の合計を表します。</p>
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
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>これらのパラメーターは Role オブジェクトから Rate オブジェクトに移動され、（個別の日付範囲に対して）Role オブジェクトと User オブジェクトが複数の値を持つようになりました。</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>これらのパラメーターは、Rate がアタッチされるオブジェクトの ID とオブジェクトコードを表します。
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>このアクションが追加され、Rate オブジェクトが指定された Object にアタッチされます。このエンドポイントは、Rate がアタッチ可能なすべてのオブジェクトで機能します。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote（RHNOTE）

RichTextNote オブジェクトは、Workfront オブジェクトに対して行われるコメントまたは更新です。太字や斜体のテキストなどのリッチテキストが含まれます。

RichTextNote オブジェクトによって、`REPORTABLE` フラグが削除されます。

### Role / Job Role（ROLE）

Role オブジェクト（担当業務）は、デザイナーやプロダクトマネージャーなど、ユーザーが入力できる機能またはスキルセットを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
           <li>
            <p><b>料率</b>
            </p>
            <p>これが追加され、この役割にアタッチされる Rate オブジェクトを表します。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>workPerDate</b>
            </p>
            <p>このフィールドが追加され、1 日あたりの必要な作業時間数を分単位で表示します。形式は <code>YYYY-MM-DD: (number of minutes)</code> で、タイムゾーンを考慮します。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>このアクションに <code>teamIDs</code> フィールドが追加され、複数のチームをタスクまたはイシューに割り当てる機能がサポートされます。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>availableActions</b>
            </p>
            <p>このパラメーターによって、<code>READ_ONLY</code> フラグが削除されます。</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>このパラメーターによって、<code>READ_ONLY</code> フラグが削除されます。</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>このパラメーターが追加され、「一就業日と同等の時間数」の変更に関係なく、タイムシートの期間を日数で保存します。例えば、「同等の時間数」が 6 に設定されていて、1 日が記録される場合、「同等の時間数」は 8 時間に変更されます。<code>totalDays</code> の値は 1 のままです。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filter（UIFT）



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>このアクションが追加され、フィルタークエリマップを使用して null 許容フィールドに <code>allowingnull</code> 結合を追加します。</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>これらのアクションは、システム全体でフィルター、ビューおよびグループ化を共有する機能をサポートします。</p><p>詳しくは、<a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">フィルター、ビューまたはグループをすべてのユーザーに使用可能にする</a>を参照してください。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Grouping（UIGB）


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">アクション</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>これらのアクションは、システム全体でフィルター、ビューおよびグループ化を共有する機能をサポートします。</p><p>詳しくは、<a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">フィルター、ビューまたはグループ化をすべてのユーザーが使用できるようにする</a>を参照してください。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView / View表示（UIVW）

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接フィールド</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>次の値を追加しました。</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
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
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>これらのアクションは、システム全体でフィルター、ビューおよびグループ化を共有する機能をサポートします。</p><p>詳しくは、<a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">フィルター、ビューまたはグループ化をすべてのユーザーが使用できるようにする</a>を参照してください。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### User （USER）

ユーザーオブジェクトは、ログインしてシステムとやり取りできる Workfront アカウントを持つユーザーを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
           <li>
            <p><b>rates</b>
            </p>
            <p>これが追加され、このユーザーに付加されている Rate オブジェクトを表します。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote（USRNOT）

UserNote オブジェクトは通知です。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">クエリ</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>次の値を追加しました。
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>workPerDate</b>
            </p>
            <p>このフィールドが追加され、1 日あたりの必要な作業時間数を分単位で表示します。形式は <code>YYYY-MM-DD: (number of minutes)</code> で、タイムゾーンを考慮します。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
