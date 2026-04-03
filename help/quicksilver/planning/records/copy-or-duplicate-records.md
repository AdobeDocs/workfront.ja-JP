---
title: レコードを複製
description: 既存のレコードは、テーブルビューで複製できます。 既存のレコードの同一コピーがレコードタイプページに追加されます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 20%

---

# レコードの複製

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Adobe Workfront Planning では、レコードはレコードタイプのインスタンスです。

既存のレコードは、テーブルビューで複製できます。 既存のレコードの同一コピーがレコードタイプページに追加されます。

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
   <td>   <p>ワークスペースおよびレコードタイプに対する権限の貢献度を上げます  </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr>   
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

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
   <td><p> Standard</p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table>
-->


## レコード <!--in a record type table (I don't think you can create them elsewhere right now)-->を複製します

既存のレコードを複製することで、レコードタイプページのテーブルビューでレコードを作成できます。 既存のレコードと同じレコードが作成され、元のレコードの下に追加されます。


{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトで、レコードタイプのページがテーブルビューで開きます。
選択したタイプのすべてのレコードがビューに表示されます。

1. （条件付き）テーブルビューを選択します。

1. 次のいずれかの操作を行います。

   * レコードの名前にカーソルを合わせ、レコード名のインラインにある&#x200B;**詳細** メニューをクリックし、**重複** アイコン ![重複アイコン グレー](assets/duplicate-icon-gray.png)をクリックします。

     ![ テーブルビューのレコードからのその他のメニュー](assets/more-menu-from-record-in-table-view.png)

   * レコードを選択し、ページ下部のツールバーにある「**複製**」アイコン「![複製アイコン白と青](assets/duplicate-icon-white-and-blue.png)」をクリックします。

     ![ テーブルビューのツールバーにアイコンを複製](assets/duplicate-icon-in-toolbar-in-table-view.png)

   元のレコードの下に、同じ名前の同じレコードが作成されます。 新しいレコードのすべてのフィールドには、元のレコードと同じ情報が入力されます。

1. （オプション）テーブルビューで使用可能なフィールドで新しいレコードに関する情報の更新を開始するか、レコードのプレビューまたはページでレコードと更新情報をクリックします。

   >[!NOTE]
   >
   >  * レコードに必須のフィールドはありません。ただし、レコードを相互にリンクする際にレコードを識別すると便利なので、レコードのプライマリフィールドの情報を追加することをお勧めします。 プライマリフィールドについて詳しくは、[ テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)および[プライマリフィールドの概要](/help/quicksilver/planning/fields/primary-field-overview.md)を参照してください。
   >
   >  * 他のレコードタイプまたは計算フィールドを参照するフィールドは、読み取り専用フィールドです。

   レコードの編集について詳しくは、[ レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

1. （オプション）次のキーボードショートカットを使用して、テーブルビューで新しいレコードまたはその情報を追加するときに、元に戻したり、やり直したりします。

   * CTRL + Z （⌘ + Z for Mac）で変更を元に戻す
   * CTRL + Shift + Z （⌘ + Shift + Z for Mac）を使用して、変更をやり直します。
