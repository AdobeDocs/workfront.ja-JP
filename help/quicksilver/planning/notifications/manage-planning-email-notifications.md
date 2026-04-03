---
title: Adobe Workfront計画メール通知の管理
description: 誰かがAdobe Workfront Planningの記録的なコメントで自分やチームにタグ付けすると、そのタグのメール通知が届きます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 5%

---


# Adobe Workfront Planning のメール通知の管理

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

次のシナリオが存在する場合は、Workfront Planningからメール通知を受け取ることができます。

* 誰かがレコードのコメントで自分やチームにタグを付けます

  レコードコメント内の他のユーザーのタグ付けについて詳しくは、[&#x200B; レコードコメントの管理](/help/quicksilver/planning/records/manage-record-comments.md)を参照してください。
* ビュー、ワークスペース、またはレコードタイプ <!--or <span class="preview">or a record</span>-->へのアクセス許可を求めるユーザーがいます
* 誰かが、ビュー、ワークスペース、またはレコードタイプ <!--<span class="preview">or record</span> Isk confirmed that there is nno email for denying access but did not test-->に対するアクセス権が付与されたことを確認します
* Workfront計画リクエストを送信します。 詳しくは、[Adobe Workfront Planningでのリクエストフォームの作成と管理](/help/quicksilver/planning/requests/create-request-form.md)を参照してください
* 送信したWorkfront計画リクエストを誰かが承認または却下します。 詳しくは、[Adobe Workfront Planningでのリクエストの承認](/help/quicksilver/planning/requests/approve-request.md)を参照してください
* ステータスは、送信したWorkfront Planning リクエストに変わります。

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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

<!--
OLD: 

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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
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


## 誰かがコメントであなたをタグ付けしたときに送信されるメール通知を管理します

1. （条件付き、オプション）誰かがレコードのコメントで自分またはチームにタグを付けた後、タグとコメントを通知するメール通知に移動します。 メールの送信者はAdobe Experience Cloudです。

   ![&#x200B; メール通知の例](assets/email-notification-example.png)

1. （オプション）電子メール内の&#x200B;**Workfront** ボックス内のメッセージをクリックします。

   レコードの詳細ページがWorkfrontで開きます。 レコードを更新したり、コメントに返信したりできます。

1. （条件付き）使用可能な場合は、**すべての通知を表示**&#x200B;をクリックします。 <!--check with Lilit - do non-IMS users have this button??-->
**通知** ページがAdobe Experience Cloudで開きます。 すべてのAdobe Experience Cloud アプリケーションのすべての通知が表示されます。

## 権限をリクエストおよび付与する際のメール通知を管理します

1. （条件付き、オプション）誰かがPlanning オブジェクトタイプへのアクセス権を要求または付与した後、権限リクエストを通知するメールに移動します。 メールの送信者はAdobe Experience Cloudです。

1. （オプション）電子メール内の&#x200B;**Workfront** ボックス内のメッセージをクリックします。

   Workfrontで開く権限を要求したオブジェクト。

1. （条件付き）使用可能な場合は、**すべての通知を表示**&#x200B;をクリックします。
Adobe Experience Cloudで&#x200B;**通知** ページが開きます。 すべてのAdobe Experience Cloud アプリケーションのすべての通知が表示されます。


権限の要求、付与、または拒否について詳しくは、[&#x200B; ビューまたはワークスペースへの権限の要求](/help/quicksilver/planning/access/request-permissions.md)を参照してください。

Workfront計画の通知の管理について詳しくは、[Adobe Workfront計画の通知の環境設定の管理](/help/quicksilver/planning/notifications/manage-notification-preferences.md)を参照してください。

## Workfront Planning リクエストの送信、承認、または拒否に関するメール通知を管理します

1. （オプション）Workfrontが送信するメールに移動します
リクエストを送信した後、または送信したリクエストが承認または拒否された後。 メールの送信者はAdobe Workfrontです。

1. （オプション）「**要求を開く**」をクリックします。 これにより、Workfront Planningでリクエストが開きます。

1. リクエストの右上隅にある「**レビューして承認**」ボタンをクリックし、次のいずれかをクリックします。

   * **リクエストを承認する**&#x200B;を承認します。 Planning リクエストを承認すると、レコードが作成されます。
   * **却下**&#x200B;してリクエストを却下します。 Workfront Planningでリクエストを却下すると、レコードは作成されません。 リクエストは、ステータスが&#x200B;**Rejected**&#x200B;のリクエスト領域に保存されます。

   ![計画リクエストの「レビューと承認」ボタン &#x200B;](assets/review-approval-button-with-drop-down-expanded.png)

1. 画面の右上隅にある&#x200B;**通知** アイコン ![通知領域アイコンの統合シェル &#x200B;](assets/notifications-area-icon-unified-shell.png)をクリックして、**通知** ページにアクセスします。

   Workfront計画の通知の管理について詳しくは、[Adobe Workfront計画の通知の環境設定の管理](/help/quicksilver/planning/notifications/manage-notification-preferences.md)を参照してください。
