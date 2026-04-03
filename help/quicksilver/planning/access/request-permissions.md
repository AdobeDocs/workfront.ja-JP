---
title: ビューまたはWorkspaceへの権限のリクエスト
description: アクセス権のないビューまたはワークスペースへのリンクを誰かが共有した場合、アクセス権を要求して開くことができます。 この記事では、開くことができない共有リンクに遭遇した場合に、ビューまたはワークスペースへのアクセスをリクエストする手順について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 11%

---

# ビューまたはワークスペースに対する権限のリクエスト

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>この記事で説明する機能は、組織がAdobe Unified Experienceにオンボーディングされている場合にのみ使用できます。
>
>詳しくは、[Workfront の Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。


アクセス権を持たないビューまたはワークスペースへのリンクを誰かが共有すると、ビューまたはワークスペースへのアクセス権をリクエストできます。

ビューに対する権限の要求は、ワークスペースに対する権限の要求と似ています。

この記事では、共有ページにアクセスできないユーザーがリンクを共有した場合に、ビューまたはワークスペースへのアクセスをリクエストする方法について説明します。

ビューとワークスペースへの権限の付与について詳しくは、次の記事を参照してください。

* [ビューの共有](/help/quicksilver/planning/access/share-views.md)
* [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontおよびプランニングパッケージ</p> 
または
<p>任意のワークフローとプランニングパッケージ</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>任意</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  <p>権限のリクエストが付与されると、次の権限を取得できます。</p>
   <ul><li><p>ビューの表示または管理</p></li>
   <li><p>ワークスペースの表示、投稿、または管理</p></li></ul>  
   <p>ワークスペースとビューに対する管理権限を持つユーザーのみがビューを公開できます。</p></td> 
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
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
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
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
 
</tbody> 
</table>
-->


## ビューまたはワークスペースへの権限のリクエスト

ビューに対する権限の要求は、ワークスペースに対する権限の要求と似ています。

誰かがワークスペースまたはアクセス権のないビューへのリンクを共有した場合：

1. ビューまたはワークスペース用に共有されているリンクをクリックします。

   アクセス権がない&#x200B;**** ページが表示され、ビューまたはワークスペースへのアクセス権がないことを知らせます。

   ![ ビューへのアクセスを要求](assets/request-access-to-view.png)

1. （条件付き）共有されたリンクが、アクセス権を持つワークスペースのビュー用である場合は、**既存のビューで開く**&#x200B;をクリックします。 ワークスペースにアクセスする権限がある場合は、レコードタイプページがデフォルトビューで開きます。

1. （オプションおよび条件付き）ワークスペースを表示する権限がない場合は、使用可能なボックスにパーソナライズされたメッセージを追加し、**アクセスをリクエスト**&#x200B;をクリックします。

   ビューまたはワークスペースに対する管理権限を持つすべてのユーザーは、アクセスリクエストに対して次の通知を受け取ります。
   * アプリ内通知
     ![ アクセス要求](assets/in-app-notification-for-access-request.png)のアプリ内通知
   * メール通知
     ![ アクセス要求のメール通知](assets/email-notification-for-access-request.png)

1. （条件付き）ビューまたはワークスペースマネージャーがビューまたはワークスペースに権限を付与すると、権限が付与されたことを確認するメール通知とアプリ内通知が届きます。<!--check this - I was not able to test this, but Isk confirmed.-->
