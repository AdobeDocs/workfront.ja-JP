---
title: Adobe Workfront Planning のメール通知の管理
description: Adobe Workfront Planning のレコードコメントで誰かがあなたをタグ付けすると、そのタグについてのメール通知を受け取ります。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: f8ad026582be5b4c89939af8f135151ffaabccfe
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 26%

---


# Adobe Workfront Planning のメール通知の管理

{{planning-important-intro}}

次の状況が発生した場合は、Workfront Planning からメール通知を受信できます。

* 誰かがレコードのコメントであなたをタグ付けします
<!--
* Someone asks for your permission to access a view or a workspace
* Someone confirms your access has been granted for a view or a workspace
* Someone has denied your access for a view or a workspace. -->


>[!IMPORTANT]
>
>Workfront Planning から通知を受け取るには、会社がAdobeの Unified Experience の顧客である必要があります。
>
>詳しくは、[WorkfrontのAdobe統合エクスペリエンス ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。

レコードコメント内の他のタグ付けについて詳しくは、[ レコードコメントの管理 ](/help/quicksilver/planning/records/manage-record-comments.md) を参照してください。

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
   <td role="rowheader"><p>Adobe Workfront計画*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容の詳細については、<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfrontの価格とパッケージ </a> を参照してください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
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


## でのメール通知 <!--when someone tags you in a comment--> 管理

1. （条件付き）誰かがレコードのコメントでタグを付けた後、タグとコメントを通知するメール通知に移動します。 メールの送信者はAdobe Experience Cloudです。

   ![](assets/email-notification-example.png)

1. 「**Workfront**」ボックスのメッセージをクリックします。

   レコードの詳細ページがWorkfrontで開きます。 レコードを更新したり、コメントに返信したりできます。

1. （条件付き）使用可能な場合は、「**すべての通知を表示**」をクリックします。 <!--check with Lilit - do non-IMS users have this button??-->
**通知** ページがAdobe Experience Cloudで開きます。 すべてのAdobe Experience Cloud アプリケーションからのすべての通知が表示されます。

<!--
## Manage email notifications when requesting, granting, or denying permissions to a view or a workspace

For information about requesting, granting, or denying permissions to a view or a workspace, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). 
-->