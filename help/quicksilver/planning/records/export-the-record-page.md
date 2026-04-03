---
title: レコードページの書き出し
description: レコードのプレビューページまたは詳細ページをAdobe Workfront PlanningからMicrosoft Word ファイルに書き出すことができます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 8%

---

# レコードの詳細の書き出し

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>
-->


Workfront アカウントを持っていない可能性がある他のユーザーとより効率的に共同作業を行うには、レコードの詳細ページをMicrosoft Word ファイルに書き出して共有します。

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
   <td><p>明るいまたはそれ以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースおよびレコードタイプ </a>に対する表示以上の権限 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
  </tr> 
  <tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> LightまたはContributor ライセンスを持つユーザーには、Planningを含むレイアウトテンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトでプランニング領域を有効にできます。</p></div></li></ul>
</td>
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
   <td> <p>Light or higher</p>
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
   <td>   <p>View or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
 -->


## レコードの詳細の書き出しに関する考慮事項：

* レコードの詳細を次のファイル形式に書き出すことができます。

   * .docx Word
   * .pdf

* レコードのページまたはプレビュー領域の「詳細」タブのみを書き出すことができます。

* 書き出されたファイルは、サムネールとカバー画像を含むレコードページのレイアウトを保持します。

## レコードの詳細の書き出し

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードに表示されます。

1. レコードタイプカードをクリックします。
レコードタイプページが開き、そのタイプのすべてのレコードが表示されます。

1. 任意のビューから、レコードの名前をクリックします。

   レコードのプレビューボックスが開きます。

1. （オプション）「**新しいタブで開く**」アイコン「![新しいタブアイコンで詳細を開く](assets/open-details-in-a-new-tab-icon.png)」をクリックして、レコードのページを開きます。

1. 「**詳細**」タブを選択します。 「詳細」タブはデフォルトで開きます。

1. プレビューまたはレコードのページで&#x200B;**書き出し** メニュー![ レコードの詳細ページ ](assets/export-icon-in-record-details-page.png)の書き出しアイコンをクリックし、次のいずれかをクリックします。

   * **Microsoft Word**
   * **Adobe PDF**

   Word （.docx）またはPDF ファイルがダウンロードされ、コンピューターに保存されます。

   書き出されたファイルの名前は、レコードのプライマリフィールドです。

   ![書き出されたword ファイル ](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    ページに表示されず、レコードの詳細領域で「詳細を表示」をクリックした後にのみ表示される追加情報は、書き出されたPDF ファイルには表示されません。 ページに表示される情報のみが、書き出されたファイルに表示されます。


1. （オプション）ダウンロードしたファイルに移動し、開いて編集するか（Word ファイルの場合）、他のユーザーと共有します。

