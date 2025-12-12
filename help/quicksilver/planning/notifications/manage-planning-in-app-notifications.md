---
title: Adobe Workfront Planning のアプリ内通知の管理
description: 自分または自分のチームがレコードコメントでタグ付けされると、そのタグに関するメール通知が届きます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 9%

---


# Adobe Workfront Planning のアプリ内通知の管理

{{planning-important-intro}}

次のシナリオが発生した場合は、Workfront Planning からアプリ内通知を受け取ることができます。

* 誰かがあなたまたはチームをレコードコメントでタグ付けします

  レコードコメント内の他のタグ付けについて詳しくは、[&#x200B; レコードコメントの管理 &#x200B;](/help/quicksilver/planning/records/manage-record-comments.md) を参照してください。
* 他のユーザーから、ビューまたはワークスペース <!--<span class="preview">or record</span>--> にアクセスする許可を要求されています
* ビューまたはワークスペース <!--<span class="preview">or record</span>--> ーバーへのアクセスが許可されたことを確認するメッセージが表示されます <!--Isk confirmed there is no notification for denying permissions - did not test-->

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
<p>任意のWorkfrontと任意の Planning パッケージ</p> <p>任意のワークフローおよび任意の計画パッケージ</p>
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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

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

## コメントで誰かがあなたをタグ付けしたとき、アプリ内通知を管理します

1. （条件付き）誰かがレコードのコメントで自分またはチームをタグ付けした後、Adobe Experience Cloudのアプリ内 **通知** アイコン ![Experience Cloud 通知アイコン &#x200B;](assets/experience-cloud-notifications-icon.png) に移動します。

   ![&#x200B; アプリ内通知の例 &#x200B;](assets/in-app-notification-example.png)

1. 通知をクリックします。

   Workfront Planning に「レコードの詳細」ページが開きます。 レコードを更新したり、コメントに返信したりできます。

1. （任意） **すべて既読としてマーク** をクリックして、すべての通知を既読にしたことを示します。
1. （任意）「**すべて表示**」をクリックして、Adobe Experience Cloudの **通知** ページに移動します。

## 権限をリクエストおよび付与する際のアプリ内通知の管理

ビューやワークスペースに対する権限を要求または付与された場合、アプリ内通知を受け取ります。<!--<span class="preview">or record</span>-->

権限のリクエスト、付与または拒否について詳しくは、[&#x200B; ビューまたはワークスペースに対する権限のリクエスト &#x200B;](/help/quicksilver/planning/access/request-permissions.md) を参照してください。

Adobe Workfront Planning 通知の管理については、[Workfront Planning 通知環境設定の管理 &#x200B;](/help/quicksilver/planning/notifications/manage-notification-preferences.md) を参照してください。
