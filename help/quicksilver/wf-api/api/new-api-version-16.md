---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 16 の新機能
description: Adobe Workfrontは、2022 年 4 月 7 日に API バージョン 16 をリリースしました。 API バージョン 16 では、バージョン 15 から次の変更がおこなわれました。
author: Becky
feature: Workfront API
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 8afbb1f45331d79bb849afb3acf3e9ff054cefc3
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# API バージョン 16 の新機能

Adobe Workfrontは、2023 年 4 月 7 日に API バージョン 16 をリリースしました。 API バージョン 16 では、バージョン 15 から次の変更がおこなわれました。

## 追加されたリソース

API バージョン 16 に関するリソースは追加されませんでした。

## 削除されたリソース

API バージョン 16 で削除されたリソースはありませんでした。

## 変更されたリソース

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [承認（承認）](#approval-approval)
* [顧客の環境設定 (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTSEC)](#externalsection-extsec)
* [時間 (HOUR)](#hour-hour)
* [LayoutTemplate (UITMPL)](#layouttemplate-uitmpl)
* [注意（注意）](#note-note)
* [オペタスク/問題 (OPTASK)](#note-note)
* [プロジェクト (PROJ)](#project-proj)
* [レート (RATE)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [役割/ジョブの役割 (ROLE)](#role--job-role-role)
* [タスク (TASK)](#task-task)
* [タイムシート (TSHET)](#timesheet-tshet)
* [UIFilter /フィルター (UIFT)](#uifilter--filter-uift)
* [UIGroupBy /グループ化 (UIGB)](#uigroupby--grouping-uigb)
* [UIView /表示 (UIVW)](#uiview--view-uivw)
* [ユーザー (USER)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

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

### 承認（承認）

タスク、ドキュメント、タイムシートなどの特定の作業項目に対しては、管理者や他のユーザーが作業項目に対してサインオフする必要が生じる場合があります。 Approval オブジェクトは、作業項目に対するサインオフの操作を表します。

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
            <p>このフィールドに追加され、実行する必要がある 1 日あたりの作業時間（分）の数が表示されます。 形式が設定されています <code>YYYY-MM-DD: (number of minutes)</code>、はタイムゾーンを考慮します。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 割り当て (ASSIGN)

割り当てオブジェクトは、作業項目と、作業項目に割り当てられているユーザー、チーム、またはグループとの間の接続を表します。

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
            <p>このフィールドに追加され、実行する必要がある 1 日あたりの作業時間（分）の数が表示されます。 形式が設定されています <code>YYYY-MM-DD: (number of minutes)</code>、はタイムゾーンを考慮します。</p>
          </li>
          <li>
            <p><b>isContoured</b>
            </p>
            <p>このフィールドは追加され、割り当てが含まれているかどうかを反映するブール値です。 割り当ての 1 日あたりの分数がワークロード・バランサで編集された場合、割り当ては変更されました。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

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
            <p>次の可能な値が追加されました。</p>
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
            <p>このアクションは、お客様がコントリビューターのライセンス所有者を自動アップグレードするオプションを無効にしたかどうかを示すブール値を返します。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

ExternalSection オブジェクトは、Workfrontレポートに埋め込まれる外部 Web ページです。

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
            <p>これが追加され、レポートに埋め込まれた iFrame の URL が計算されます。</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>これが追加され、レポートに埋め込まれた iFrame の URL が計算されました。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 時間 (HOUR)

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
            <p>追加済み. このパラメーターは、 <code>batchSave</code>. </p>
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

### 注意（注意）

Note オブジェクトは、Workfrontオブジェクトに対しておこなわれるコメントまたは更新です。

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
            <p>このフィールドは追加され、コメントに添付されたドキュメントのリストを表します。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### オペタスク/問題 (OPTASK)

OpTask オブジェクトは、一般にイシューと呼ばれます。 問題とは、通常、タスクまたはプロジェクトを完了できない問題があることを示す作業項目です。 問題は、ヘルプデスクへのリクエストでもかまいません。 変更管理、要求、バグも問題です。

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
            <p>このフィールドに追加され、実行する必要がある 1 日あたりの作業時間（分）の数が表示されます。 形式が設定されています <code>YYYY-MM-DD: (number of minutes)</code>、はタイムゾーンを考慮します。</p>
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
            <p>このアクションにより、「 」フィールドが追加されました。 <code>teamIDs</code> ：複数のチームをタスクまたはイシューに割り当てる機能をサポートします。</p>
         </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### プロジェクト (PROJ)

プロジェクトはWorkfront内の作業項目で、Workfrontが作業をおこなう際に役立つ主要な構成要素です。 Project オブジェクトは、共通の特定の目標を持つタスクのグループを表します。

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
            <p>このフィールドが追加され、プロジェクト上のすべての予算時間の合計を表します。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### レート (RATE)

Rate オブジェクトは、Workfrontの請求率を表します。

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
           <p>これらのパラメータは、 Role オブジェクトと User オブジェクトが複数の値を持つように、 Role オブジェクトから Rate オブジェクトに移動されました（日付範囲が異なる場合）。</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>これらのパラメーターは、レートが関連付けられるオブジェクトの ID とオブジェクトコードを表します。
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
           <p>このアクションが追加され、Rate オブジェクトが指定された Object にアタッチされます。 このエンドポイントは、すべてのレートアタッチ可能オブジェクトで機能します。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

RichTextNote オブジェクトは、Workfrontオブジェクトに対して行われるコメントまたは更新です。太字や斜体のテキストなどのリッチテキストが含まれます。

RichTextNote オブジェクトがフラグを削除しました `REPORTABLE`.

### 役割/ジョブの役割 (ROLE)

ロールオブジェクト（ジョブロール）は、Designer や Product Manager など、ユーザーが入力できる機能能力またはスキルセットを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
           <li>
            <p><b>料金</b>
            </p>
            <p>これが追加され、この役割にアタッチされる Rate オブジェクトを表します。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### タスク (TASK)

Task オブジェクトは、最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要がある作業項目を表します。

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
            <p>このフィールドに追加され、実行する必要がある 1 日あたりの作業時間（分）の数が表示されます。 形式が設定されています <code>YYYY-MM-DD: (number of minutes)</code>、はタイムゾーンを考慮します。</p>
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
            <p>このアクションにより、「 」フィールドが追加されました。 <code>teamIDs</code> ：複数のチームをタスクまたはイシューに割り当てる機能をサポートします。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### タイムシート (TSHET)

Timesheet オブジェクトは、Tasks、Projects、および Overhead Hour Types の実績作業時間をユーザーが入力できる仮想タイムカードを表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">ダイレクトフィールド</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>このパラメーターはフラグを削除しました <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>このパラメーターはフラグを削除しました <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>このパラメータを追加し、「フルWorkdayの同等時間」の変更に関係なく、タイムシートの期間を日数で格納しました。  例えば、「同等の時間」が 6 に設定され、1 日がログに記録される場合、「同等の時間」は 8 時間に変更されます。 <code>totalDays</code> の値は 1 のままです。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter /フィルター (UIFT)



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
            <p>このアクションが追加され、フィルタークエリマップを使用して <code>allowingnull</code> null 可能なフィールドを結合します。</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>これらのアクションは、システム全体でフィルター、ビューおよびグループを共有する機能をサポートします。</p><p>詳しくは、 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">フィルター、ビュー、またはグループをすべてのユーザーが使用できるようにする</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy /グループ化 (UIGB)


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
            <p>これらのアクションは、システム全体でフィルター、ビューおよびグループを共有する機能をサポートします。</p><p>詳しくは、 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">フィルター、ビュー、またはグループをすべてのユーザーが使用できるようにする</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView /表示 (UIVW)

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
            <p>次の可能な値が追加されました。</p>
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
            <p>これらのアクションは、システム全体でフィルター、ビューおよびグループを共有する機能をサポートします。</p><p>詳しくは、 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">フィルター、ビュー、またはグループをすべてのユーザーが使用できるようにする</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ユーザー (USER)

User オブジェクトは、Workfrontにログインしてシステムとやり取りできるアカウントを持つ人物を表します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">コレクションフィールド</td>
      <td>
        <ul>
           <li>
            <p><b>料金</b>
            </p>
            <p>これは追加され、このユーザーにアタッチされている Rate オブジェクトを表します。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

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
            <p>次の可能な値が追加されました。
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

### 作業（作業）

Work オブジェクトは、Task と OpTask の両方が継承する共通のインターフェイスで、2 つの間で共通のコードを共有します。

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
            <p>このフィールドに追加され、実行する必要がある 1 日あたりの作業時間（分）の数が表示されます。 形式が設定されています <code>YYYY-MM-DD: (number of minutes)</code>、はタイムゾーンを考慮します。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
