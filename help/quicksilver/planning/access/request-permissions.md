---
title: ビューまたはWorkspaceに対する権限のリクエスト
description: アクセス権のないビューまたはワークスペースへのリンクが他のユーザーと共有されている場合、そのビューまたはワークスペースを開くためのアクセス許可を要求できます。 この記事では、開くことができない共有リンクが発生した場合に、ビューまたはワークスペースへのアクセスをリクエストする手順について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: c879d06cfe7ba76df3e974c160a7349f1503f17f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 7%

---

# ビューまたはワークスペースに対する権限のリクエスト

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>この記事で説明されている機能は、組織がAdobe統合エクスペリエンスにオンボーディングされた場合にのみ使用できます。
>
>詳しくは、[Workfront の Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。


アクセス権がないビューまたはワークスペースへのリンクが他のユーザーによって共有されている場合、そのビューまたはワークスペースに対する権限をリクエストできます。

ビューに対する権限のリクエストは、ワークスペースに対する権限のリクエストと似ています。

この記事では、他のユーザーがリンクを共有していて、共有ページにアクセスできない場合に、ビューまたはワークスペースへのアクセスをリクエストする方法について説明します。

ビューとワークスペースに対する権限の付与については、次の記事を参照してください。

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
<p>任意のWorkfrontおよび Planning パッケージ</p> 
または
<p>任意のワークフローおよび計画パッケージ</p> 
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
   <td>  <p>許可リクエストが許可されると、次の権限を取得できます。</p>
   <ul><li><p>ビューの表示または管理</p></li>
   <li><p>ワークスペースの表示、投稿または管理</p></li></ul>  
   <p>ワークスペースおよびビューに対する管理権限を持つユーザーのみが、ビューを公開して共有できます。</p></td> 
  </tr> 
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、Planning を含むレイアウト テンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

<!--Old:
 
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
</table> -->


## ビューまたはワークスペースに対する権限のリクエスト

ビューに対する権限のリクエストは、ワークスペースに対する権限のリクエストと似ています。

アクセス権のないワークスペースまたはビューへのリンクが他のユーザーによって共有された場合：

1. ビューまたはワークスペースで、共有されているリンクをクリックします。

   **アクセス権がありません** ページが表示され、ビューまたはワークスペースに対するアクセス権がないことを示すメッセージが表示されます。

   ![&#x200B; 表示へのアクセスをリクエスト &#x200B;](assets/request-access-to-view.png)

1. （条件付き）共有リンクが、アクセス権を持つワークスペースのビュー用である場合は、「**既存のビューで開く**」をクリックします。 ワークスペースへのアクセス権を持っている場合、レコードタイプページがデフォルトのビューで開きます。

1. （オプションおよび条件付き）ワークスペースを表示する権限がない場合、使用可能なボックスにパーソナライズされたメッセージを追加し、「**アクセスをリクエスト**」をクリックします。

   ビューまたはワークスペースに対する管理権限を持つすべてのユーザーは、アクセスリクエストに関する次の通知を受け取ります。
   * アプリ内通知
     ![&#x200B; アクセスリクエストのアプリ内通知 &#x200B;](assets/in-app-notification-for-access-request.png)
   * メール通知
     ![&#x200B; アクセスリクエストのメール通知 &#x200B;](assets/email-notification-for-access-request.png)

1. （条件付き）ビューまたはワークスペースマネージャーからビューまたはワークスペースに対する権限を付与されると、権限が付与されたことを確認するメール通知とアプリ内通知が届きます。<!--check this - I was not able to test this, but Isk confirmed.-->
