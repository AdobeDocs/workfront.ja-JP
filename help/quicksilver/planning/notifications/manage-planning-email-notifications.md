---
title: Adobe Workfront Planning のメール通知の管理
description: Adobe Workfront Planning のレコードコメントで誰かがあなたをタグ付けすると、そのタグについてのメール通知を受け取ります。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 14%

---


# Adobe Workfront Planning のメール通知の管理

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

次の状況が発生した場合は、Workfront Planning からメール通知を受信できます。

* 誰かがレコードのコメントであなたをタグ付けします

  レコードコメント内の他のタグ付けについて詳しくは、[ レコードコメントの管理 ](/help/quicksilver/planning/records/manage-record-comments.md) を参照してください。
* 他のユーザーから、ビューまたはワークスペースにアクセスする許可を要求されています
* ビューまたはワークスペース <!--Isk confirmed that there is nno email for denying access but did not test--> ーバーへのアクセスが許可されたことを確認するメッセージが表示されます
* Workfront Planning の要求を発行します。 詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください
* 送信されたWorkfront Planning 要求が誰かに承認または拒否されています。 詳しくは、[Adobe Workfront Planning でリクエストを承認 ](/help/quicksilver/planning/requests/approve-request.md) を参照してください
* ステータスが、送信したWorkfront計画リクエストに変わります。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 製品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>組織のWorkfrontのインスタンスは、Adobeの Unified Experience にオンボーディングされる必要があります。</p> 
<p>組織内のユーザーは、組織がAdobeの Unified Experience にオンボーディングされた場合にのみ、Workfront Planning から通知を受け取ります。 </p>
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準、ライト、またはコントリビューター</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する表示またはそれ以上の権限</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->


## コメントで誰かがあなたをタグ付けしたときのメール通知を管理します

1. （条件付きおよびオプション）誰かがレコードのコメントでタグを付けた後、タグとコメントを通知するメール通知に移動します。 メールの送信者はAdobe Experience Cloudです。

   ![](assets/email-notification-example.png)

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
リクエストを送信した後、または送信したリクエストが承認または却下された後。 メールの送信者はAdobeの Workfront です。

1. （任意）「**リクエストを開く**」をクリックします。 これにより、Workfront Planning でリクエストが開きます。

1. 画面の右上隅に ![](assets/notifications-area-icon-unified-shell.png) る **通知** アイコンをクリックして、**通知** ページにアクセスします。

   Adobe Workfront Planning 通知の管理については、[Workfront Planning 通知環境設定の管理 ](/help/quicksilver/planning/notifications/manage-notification-preferences.md) を参照してください。
