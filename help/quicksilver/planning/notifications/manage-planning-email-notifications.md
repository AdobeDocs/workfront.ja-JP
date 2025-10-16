---
title: Adobe Workfront Planning のメール通知の管理
description: Adobe Workfront Planning 内のレコードコメントで誰かがあなたまたは自分のチームをタグ付けすると、そのタグに関するメール通知が届きます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 5%

---


# Adobe Workfront Planning のメール通知の管理

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

次の状況が発生した場合は、Workfront Planning からメール通知を受信できます。

* 誰かがあなたまたはチームをレコードコメントでタグ付けします

  レコードコメント内の他のタグ付けについて詳しくは、[ レコードコメントの管理 ](/help/quicksilver/planning/records/manage-record-comments.md) を参照してください。
* 他のユーザーから、ビューまたはワークスペースにアクセスする許可を要求されています
* ビューまたはワークスペース <!--Isk confirmed that there is nno email for denying access but did not test--> ーバーへのアクセスが許可されたことを確認するメッセージが表示されます
* Workfront Planning の要求を発行します。 詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください
* 送信されたWorkfront Planning 要求が誰かに承認または拒否されています。 詳しくは、[Adobe Workfront Planning でリクエストを承認 ](/help/quicksilver/planning/requests/approve-request.md) を参照してください
* ステータスが、送信したWorkfront計画リクエストに変わります。

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
<li><p>任意のWorkfrontと任意の Planning パッケージ</p></li>
または
<li><p>任意のワークフローおよび任意の計画パッケージ</p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>ライト以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する表示またはそれ以上の権限</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、Planning を含むレイアウト テンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

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


## コメントで誰かがあなたをタグ付けしたときのメール通知を管理します

1. （条件付きおよびオプション）誰かがレコードのコメントで自分または自分のチームにタグを付けた後、タグとコメントを通知するメール通知に移動します。 メールの送信者はAdobe Experience Cloudです。

   ![ メール通知の例 ](assets/email-notification-example.png)

1. （任意）メール内の **Workfront** ボックスのメッセージをクリックします。

   レコードの詳細ページがWorkfrontで開きます。 レコードを更新したり、コメントに返信したりできます。

1. （条件付き）使用可能な場合は、「**すべての通知を表示**」をクリックします。 <!--check with Lilit - do non-IMS users have this button??-->
**通知** ページがAdobe Experience Cloudで開きます。 すべてのAdobe Experience Cloud アプリケーションからのすべての通知が表示されます。

## 権限をリクエストおよび付与する際のメール通知の管理

1. （条件付きおよびオプション）ビューやワークスペースへのアクセス権限がリクエストまたは許可された後は、権限リクエストを通知するメールに移動します。 メールの送信者はAdobe Experience Cloudです。

1. （任意）メール内の **Workfront** ボックスのメッセージをクリックします。

   レコードの詳細ページがWorkfrontで開きます。 レコードを更新したり、コメントに返信したりできます。

1. （条件付き）使用可能な場合は、「**すべての通知を表示**」をクリックします。
**通知** ページがAdobe Experience Cloudで開きます。 すべてのAdobe Experience Cloud アプリケーションからのすべての通知が表示されます。


ビューまたはワークスペースに対する権限の要求、付与、または拒否の詳細については、[ ビューまたはワークスペースに対する権限の要求 ](/help/quicksilver/planning/access/request-permissions.md) を参照してください。

Adobe Workfront Planning 通知の管理については、[Workfront Planning 通知環境設定の管理 ](/help/quicksilver/planning/notifications/manage-notification-preferences.md) を参照してください。

## Workfront Planning 要求の送信、承認または拒否に関する電子メール通知の管理

1. （任意） Workfrontから送信されるメールに移動します
リクエストを送信した後、または送信したリクエストが承認または却下された後。 メールの送信者はAdobe Workfront です。

1. （任意）「**リクエストを開く**」をクリックします。 これにより、Workfront Planning でリクエストが開きます。

1. 画面の右上隅にある「**通知**」アイコン ![ 通知領域アイコン Unified Shell](assets/notifications-area-icon-unified-shell.png) をクリックして、**通知** ページにアクセスします。

   Adobe Workfront Planning 通知の管理については、[Workfront Planning 通知環境設定の管理 ](/help/quicksilver/planning/notifications/manage-notification-preferences.md) を参照してください。
