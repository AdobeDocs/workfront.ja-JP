---
title: ワークスペースの削除
description: 関係がなくなったワークスペースは削除できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 31aff197d6af521df2258f3f99fea6fb5785b9e3
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 38%

---


# ワークスペースの削除

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。詳しくは、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

不要になったワークスペースは削除できます。

ワークスペースを削除する前に、そのワークスペースに関連付けられているレコードタイプ、レコード、フィールド、ビューの一部またはすべてを、別のワークスペースで再作成することをお勧めします。

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
<ul> 
<li><p>任意のWorkfrontおよびプランニングパッケージ</p></li>
または
<li><p>任意のワークフローとプランニングパッケージ</p></li></ul>
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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table>
-->

## ワークスペースの削除に関する考慮事項

* ワークスペースを削除すると、すべてのレコードタイプ、レコード、そのフィールドおよびビューも削除されます。
* 削除したワークスペースとそれらに含まれる情報は復元できません。

## ワークスペースの削除

{{step1-to-planning}}

1. （条件付き）Workfront管理者の場合は、次のいずれかをクリックします。

   * **作成したワークスペースにアクセスするための**&#x200B;のワークスペース
   * **自分または自分が作成したワークスペースで共有されているワークスペースにアクセスするためのワークスペース**&#x200B;すべて

1. （オプション）「**すべてを表示**」をクリックして、追加のワークスペースを表示します。 **すべてを表示** リンクは、2行以上のワークスペースカードがある場合にのみ表示されます。
1. （オプション）「**表示回数**」をクリックして、画面に表示されるワークスペースの数を制限します。
1. ワークスペースを削除するには、次のいずれかの操作を行います。

   * ワークスペースカードにカーソルを合わせ、カードの右上隅にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックします
または
   * ワークスペースページの右上隅にある&#x200B;**検索** アイコン ![検索アイコン ](assets/search-icon.png)をクリックして、ワークスペースを名前で検索し、ワークスペースカードをクリックしてワークスペースを開き、ワークスペース名の右側にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックします。

   >[!TIP]
   >
   >次のキーボードの組み合わせを使用して、任意のWorkfront計画ページからグローバル検索ボックスを開き、ワークスペースを検索できます。
   >
   >* Windowsの場合はCTRL+K
   >* Macの⌘+K

1. 「**削除**」をクリックします。

   ![ ワークスペースを完全に削除の確認](assets/permanently-delete-workspace-confirmation.png)

1. 指定されたスペースに「**delete**」と入力し、**完全に削除**&#x200B;をクリックします。 大文字と小文字を区別しません。

   ワークスペースは削除され、復元できません。レコードタイプ、レコード、フィールドおよびそれらに関連付けられているビューも削除されます。<!--ensure this is right at or before GA-->


