---
title: Adobe Workfront Planningのアプリ内通知の管理
description: 誰かがレコードコメントで自分やチームにタグを付けると、そのタグのメール通知が届きます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 9%

---


# Adobe Workfront Planning のアプリ内通知の管理

{{planning-important-intro}}

次のシナリオが存在する場合、Workfront Planningからアプリ内通知を受け取ることができます。

* 誰かがレコードのコメントで自分やチームにタグを付けます

  レコードコメント内の他のユーザーのタグ付けについて詳しくは、[ レコードコメントの管理](/help/quicksilver/planning/records/manage-record-comments.md)を参照してください。
* ビューまたはワークスペース <!--<span class="preview">or record</span>-->へのアクセス許可を求めるユーザーがいます
* 誰かが、ビューまたはワークスペース <!--<span class="preview">or record</span> Isk confirmed there is no notification for denying permissions - did not test-->に対するアクセス権が付与されたことを確認します

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
   <td>   <p>ワークスペースに対する表示またはそれ以上の権限</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
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
OLD:

+++ Expand to view access requirements. 

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
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
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> 

+++
-->

## 誰かがコメントであなたをタグ付けしたときに、アプリ内通知を管理します

1. （条件付き）誰かがレコードのコメントで自分やチームにタグを付けた後、Adobe Experience Cloudのアプリ内&#x200B;**通知** アイコン ![Experience cloud通知アイコン ](assets/experience-cloud-notifications-icon.png)に移動します。

   ![ アプリ内通知の例](assets/in-app-notification-example.png)

1. 通知をクリックします。

   Workfront Planningでレコードの詳細ページが開きます。 レコードを更新したり、コメントに返信したりできます。

1. （オプション）「**すべてを既読としてマーク**」をクリックして、すべての通知を読み取ったことを示します。
1. （オプション）「**すべて表示**」をクリックして、Adobe Experience Cloudの&#x200B;**通知** ページに移動します。

## 権限をリクエストおよび付与する際のアプリ内通知を管理します

誰かがビュー、ワークスペース、またはレコードタイプに対して権限をリクエストまたは付与すると、アプリ内通知が届きます。<!--<span class="preview">or record</span>-->

権限の要求、付与、または拒否について詳しくは、[ ビューまたはワークスペースへの権限の要求](/help/quicksilver/planning/access/request-permissions.md)を参照してください。

Workfront計画の通知の管理について詳しくは、[Adobe Workfront計画の通知の環境設定の管理](/help/quicksilver/planning/notifications/manage-notification-preferences.md)を参照してください。

## Planning リクエストの承認または却下の際のアプリ内通知の管理

誰かが承認リクエストを送信したとき、または誰かが送信したリクエストを承認したときに、アプリ内通知が届きます。

リクエストの送信について詳しくは、[ レコードを作成するためのAdobe Workfront Planning リクエストの送信](/help/quicksilver/planning/requests/submit-requests.md)を参照してください。

リクエストの承認について詳しくは、[Adobe Workfront Planningでのリクエストの承認](/help/quicksilver/planning/requests/approve-request.md)を参照してください。
