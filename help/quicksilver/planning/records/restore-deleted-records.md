---
title: 削除したレコードの復元
description: Adobe Workfront Planningの「最近削除された」領域から、削除されたレコードを復元できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 7%

---

# 削除されたレコードの復元

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Adobe Workfront Planningの「最近削除された」領域から、削除されたレコードを復元できます。

レコードの削除について詳しくは、[&#x200B; レコードの削除](/help/quicksilver/planning/records/delete-records.md)を参照してください。

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

## 削除されたレコードの回復に関する考慮事項

* 自分または他のユーザーが削除したレコードを復元できます。
* レコードは、最近削除されたビンに30日間保存されます。 30日後、レコードはWorkfront Planningから完全に削除されます。
* 削除されたレコードが他のレコードにリンクされている場合、リンクされたレコードは削除されませんが、削除されたレコードの情報も削除されます。 削除されたレコードを復元すると、接続されたレコードから情報が復元されます。
* レコードを一括で復元できます。
* レコードが削除されると、次の情報が「最近削除されたビン」に保存されます。
   * **名前**：これは、レコードのプライマリフィールドの情報です。 レコードプライマリフィールドについて詳しくは、[プライマリフィールドの概要](/help/quicksilver/planning/fields/primary-field-overview.md)を参照してください。
   * **削除日**: レコードが削除された日時。
   * **最近削除された時間**: レコードが削除されてからの時間。 現在の日付より30日以上前に削除されたレコードは、「最近削除されたビン」に表示されません。
   * **削除者**: レコードを削除したユーザーの名前。

## 削除されたレコードの復元

1. レコードを削除したレコードタイプページに移動します。
1. 任意のレコードタイプのページビューの右上隅にある&#x200B;**取り消し** アイコン ![取り消しアイコン &#x200B;](assets/undo-icon.png)をクリックし、**最近削除した**&#x200B;をクリックします。

   最近削除された&#x200B;**個のボックスが表示されます。**

   ![最近削除されたボックス &#x200B;](assets/recently-deleted-box.png)

1. 削除するレコードを選択し、**復元** > **復元**&#x200B;をクリックします。 複数のレコードを選択できます。

   復元が成功した場合は、画面の下部に成功通知が表示されます。
1. テーブルビューに移動し、復元されたレコードを確認します。
