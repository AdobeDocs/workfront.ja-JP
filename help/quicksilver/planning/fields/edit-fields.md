---
title: フィールド設定の編集
description: Adobe Workfront Planningでは、作成済みのフィールドのフィールド設定を編集できます。 ここでは、Workfront計画フィールドの設定を変更する方法について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 23%

---


# フィールド設定の編集

<!--leave the choice value information in yellow till January 2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Adobe Workfront Planningでは、既存のフィールドの設定を編集できます。

Adobe Workfront Planning フィールドの作成については、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

この記事では、Workfront Planning フィールドの設定を編集する方法について説明します。レコードのフィールド値の編集については、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontおよびプランニングパッケージ</p> <p>任意のワークフローとプランニングパッケージ</p>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++     

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table>
-->

## フィールド設定の編集に関する考慮事項

フィールドの設定を変更する前に、次の点を考慮する必要があります。

* フィールド設定は、レコードタイプテーブルからのみ編集できます。
* レコードページまたはテーブルビュー以外の他のビューでフィールドの設定を編集することはできません。
* フィールドを保存した後は、フィールドタイプを編集できません。
* 数値、パーセンテージ、通貨のいずれかのフィールドについて、そのフィールドが添付されているレコードに既に負の値が格納されている場合は、選択済みの「負の数を許可」設定の選択を解除することはできません。
* フィールドを保存した後、次のフィールド要素の設定を編集できます。

   * 任意のフィールドの名前または説明
   * 単一選択または複数選択フィールドのオプション。
   * 数式フィールドの式。

  >[!WARNING]
  >
  >数式の式が変更されたり、select-type フィールドからオプションが追加または削除されたりすると、設定が変更されたフィールドに既に保存されている情報を持つレコードのデータが失われます。
  >
  >フィールドの設定を変更すると、このデータ損失が発生する可能性があるという警告や兆候はありません。
  >
  >フィールド設定が変更されたことを他のユーザーに通知しません。

* 接続されたレコードから既存のルックアップフィールドを編集できます。
* この記事の「[&#x200B; フィールド設定を編集](#edit-field-settings-1)」セクションで説明されているようにフィールドを編集するだけでなく、フィールド値を更新しながら、テーブルビューでレコードを編集する際に、1つまたは複数の選択フィールドの選択肢を編集することもできます。 詳しくは、この記事の「[&#x200B; テーブルビューでレコードを編集する際に既存の選択フィールドに新しい選択肢を追加する](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view)」セクションを参照してください。

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--
this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## フィールド設定の編集

{{step1-to-planning}}

1. レコードフィールドを編集するワークスペースをクリックします。

   ワークスペースが開き、ワークスペース内のすべてのレコードタイプがカードに表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. （条件付き） **テーブルビュー**&#x200B;のタブをクリックします。

   そのレコードタイプに関連付けられている既存のすべてのレコードが、テーブルビューの行に表示されます。
1. 編集するフィールドの列ヘッダーにポインタを合わせ、フィールド名の後の下向き矢印をクリックして「**フィールドを編集**」をクリックします。

   または

   フィールドの列ヘッダーをダブルクリックします。

   ![&#x200B; テーブルヘッダーのフィールド名の後の矢印メニューが強調表示される](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. フィールドに関する情報を更新し、「**保存**」をクリックします。

   詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* フィールドを保存した後は、フィールドタイプを更新できません。
   >
   >* フィールド設定（フィールドオプションまたは数式式）を変更すると、変更されたフィールドに既に情報を含むレコードは、値をリアルタイムで更新します。 フィールド設定の変更によってトリガーされた値の変更に対する警告や監査ログはありません。 フィールドを表示するすべてのユーザーには、変更が適用された新しい値がすぐに表示されます。

   フィールド情報は、ワークスペースを表示するためのアクセス権を持つ全員が更新されます。

1. （条件付き）接続されたレコードフィールドの場合は、**参照フィールドを編集**&#x200B;をクリックし、接続されたレコードタイプからいずれかの参照フィールドを追加または削除します。

   詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。


## テーブルビューでレコードを編集するときに、既存の選択フィールドに新しい選択肢を追加する

<!--some of this information is also available in Edit records article - update both when necessary-->

テーブルビューでレコードを編集する際に、既存の単一選択フィールドまたは複数選択フィールドに新しい選択肢を追加できます。

>[!IMPORTANT]
>
>この節で説明する機能は、テーブルビューでのみ使用できます。 1つまたは複数の選択フィールドが表示される他の領域では使用できません。

**例**

「新規」および「クローズ」の選択肢を持つ「ステータス」という単一選択フィールドがあり、進行中ステータスの選択肢を追加する場合があります。 次のいずれかの操作を行って、選択肢を追加できます。

* フィールドの編集。 詳しくは、この記事の「[&#x200B; フィールド設定を編集](#edit-field-settings-1)」の節を参照してください。
* 以下の説明に従って、テーブルビューでレコードを編集する際に新しいオプションを追加します。

レコードを編集する際に、既存の選択フィールドに新しい選択肢を追加するには、次の手順に従います。

1. レコードタイプページに移動し、テーブルビューを開きます。
1. テーブルビューで選択肢を追加する1つまたは複数の選択フィールドを新しい列として追加します。 詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。
1. フィールドのセルをダブルクリックして、フィールドのインライン編集を開始します。
1. 追加する選択肢の名前を入力し、**選択肢を追加**&#x200B;をクリックします。

   ![&#x200B; テーブルビューの単一選択フィールドに選択肢を追加](assets/add-choice-in-table-view-for-single-select-field.png)

   新しい選択肢は、すぐに単一選択フィールドに追加されます。

   新しい値も各選択肢に追加されます。 API呼び出しやその他の統合では、選択肢の値を使用できます。 詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

