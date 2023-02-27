---
content-type: api
navigation-topic: workfront-objects
title: APIModel INTERNAL がフィールド projectid (OpTask)Category をサポートしない場合
description: APIModel INTERNAL がフィールド projectid (OpTask) をサポートしない場合
author: Becky
feature: Workfront API
exl-id: 24c900ee-a8f1-458e-a18b-c098c6314e0c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 22%

---


# カテゴリ

フィールドクラス：&quot;java.lang.IllegalArgumentException&quot;,\
メッセージ：&quot;APIModel INTERNAL はフィールド projectid (OpTask) をサポートしていません&quot;

<table style="table-layout:auto"> 
 <col width="100"> 
 <col width="100"> 
 <col width="100"> 
 <col width="240"> 
 <col width="200"> 
 <col width="100"> 
 <thead> 
  <tr> 
   <th>名前</th> 
   <th>ラベル</th> 
   <th>タイプ</th> 
   <th>説明</th> 
   <th>可能な値</th> 
   <th>フラグ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}"><strong>ID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID&quot;}">ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Identifying GUID&quot;}">GUID の識別</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;accessorIDs&quot;}"><strong>accessorIDs</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;acessorIDs&quot;}">accessorIDs</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String Array&quot;}">文字列配列</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;List of People/Team IDs that can access this object&quot;}">このオブジェクトにアクセスできる人/チーム ID のリスト</td> 
   <td> </td> 
   <td> <p><span class="dtRead">読み取り専用</span> </p> <p><span class="dtLazy">遅延読み取り</span> </p> <p><span class="dtDyn">動的</span> </p> <p><span class="dtGrp">グループ化不可</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;catObjCode&quot;}"><strong>catObjCode</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">タイプ</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type of Object the Custom form is related to&quot;}">カスタムフォームが関連するオブジェクトのタイプ</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;[{\&quot;label\&quot;:\&quot;Company\&quot;,\&quot;value\&quot;:\&quot;CMPY\&quot;},{\&quot;label\&quot;:\&quot;Task\&quot;,\&quot;value\&quot;:\&quot;TASK\&quot;},{\&quot;label\&quot;:\&quot;Project\&quot;,\&quot;value\&quot;:\&quot;PROJ\&quot;},{\&quot;label\&quot;:\&quot;Portfolio\&quot;,\&quot;value\&quot;:\&quot;PORT\&quot;},{\&quot;label\&quot;:\&quot;Program\&quot;,\&quot;value\&quot;:\&quot;PRGM\&quot;},{\&quot;label\&quot;:\&quot;User\&quot;,\&quot;value\&quot;:\&quot;USER\&quot;},{\&quot;label\&quot;:\&quot;Document\&quot;,\&quot;value\&quot;:\&quot;DOCU\&quot;},{\&quot;label\&quot;:\&quot;Issue\&quot;,\&quot;value\&quot;:\&quot;OPTASK\&quot;},{\&quot;label\&quot;:\&quot;Expense\&quot;,\&quot;value\&quot;:\&quot;EXPNS\&quot;},{\&quot;label\&quot;:\&quot;Iteration\&quot;,\&quot;value\&quot;:\&quot;ITRN\&quot;}]&quot;}"><code>[{"label":"Company","value":"CMPY"},{"label":"Task","value":"TASK"},{"label":"Project","value":"PROJ"},{"label":"Portfolio","value":"PORT"},{"label":"Program","value":"PRGM"},{"label":"User","value":"USER"},{"label":"Document","value":"DOCU"},{"label":"Issue","value":"OPTASK"},{"label":"Expense","value":"EXPNS"},{"label":"Iteration","value":"ITRN"}]</code> </td> 
   <td> <p><span class="dtEdit">編集可能</span> </p> <p><span class="dtReq">必須</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;customerID&quot;}"><strong>customerID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Customer ID&quot;}">顧客 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the Customer&quot;}">顧客の ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">グループ化不可</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;description&quot;}"><strong>説明</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">説明</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Description&quot;}">説明</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">編集可能</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;enteredByID&quot;}"><strong>enteriedByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Entered By ID&quot;}">入力者 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the User that added the Custom Form&quot;}">カスタムフォームを追加したユーザーの ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">グループ化不可</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;extRefID&quot;}"><strong>extRefID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;External Reference ID&quot;}">外部参照 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;User Editable Field inteded to be used a link to an external object&quot;}">外部オブジェクトへのリンクに使用するためのユーザー編集可能フィールド</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">編集可能</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;groupID&quot;}"><strong>groupID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Group ID&quot;}">グループ ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the first group with access to the custom form&quot;}">カスタムフォームへのアクセス権を持つ最初のグループの ID</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">編集可能</span> </p> <p><span class="dtGrp">グループ化不可</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;hasCalculatedFields&quot;}"><strong>hasCalculatedFields</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Has Calculated Fields&quot;}">計算済みフィールドあり</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Boolean&quot;}">ブール値</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Does the form have calculated fields associated with it?&quot;}">フォームに関連付けられた計算フィールドがあるか。</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">グループ化不可</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdateDate&quot;}"><strong>lastUpdateDate</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Update Date&quot;}">最終更新日</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date/Time&quot;}">日付/時刻</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Date of when the object was last modified&quot;}">オブジェクトが最後に変更された日付</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;lastUpdatedByID&quot;}"><strong>lastUpdatedByID</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Last Updated By ID&quot;}">最終更新者 ID</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;ID of the last user to Update the object&quot;}">オブジェクトを更新する最後のユーザーの ID</td> 
   <td> </td> 
   <td> <p><span class="dtGrp">グループ化不可</span> </p> </td> 
  </tr> 
  <tr> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;name&quot;}"><strong>name</strong> </td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name&quot;}">名前</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;String&quot;}">String</td> 
   <td data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Name of the Object&quot;}">オブジェクトの名前</td> 
   <td> </td> 
   <td> <p><span class="dtEdit">編集可能</span> </p> <p><span class="dtReq">必須</span> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 参照

| 名前 | ラベル | タイプ | タイプオブジェクトコード | URL |
|---|---|---|---|---|
| 顧客 | 顧客 | 顧客 | CUST | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| エントリ者 | enteredBy | ユーザー | ユーザー | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| グループ | グループ | グループ | グループ | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| 最終更新者 | lastUpdatedBy | ユーザー | ユーザー | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |


## コレクション

| 名前 | ラベル | タイプ | タイプオブジェクトコード | URL |
|---|---|---|---|---|
| アクセス ルール | accessRules | アクセス ルール | ACSRUL | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| カテゴリアクセスルール | categoryAccessRules | カテゴリアクセスルール | CATACR | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| カテゴリカスケードルール | categoryCascadeRules | カテゴリカスケードルール | CTCSRL | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| カテゴリ パラメーター | categoryParameters | カテゴリ パラメーター | CTGYPA | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |
| その他のグループ | otherGroups | グループ | グループ | [https://support.workfront.com/hc/en-us/articles/226425467](https://support.workfront.com/hc/en-us/articles/226425467) |


## アクション

| ラベル | 名前 | 引数 |
|---|---|---|
| カテゴリの割り当て | assignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| カテゴリの割り当て | assignCategory | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
| カテゴリの割り当て解除 | unassignCategories | `[{name: "objID",type: "string"},{name: "objCode",type: "string"},{name: "categoryIDs",type: "string[]"}]` |
| カテゴリの割り当て解除 | unassignCategory | `[{name: "objID",type: "string"},name: "objCode",type: "string"},{name: "categoryID",type: "string"}]` |
