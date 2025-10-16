---
title: Adobe Workfront Planning 通知設定の管理
description: Adobe Workfront Planning の通知設定を管理できる場合があります。 この記事では、通知の環境設定を行う方法について説明します。
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 8%

---


# Adobe Workfront Planning 通知設定の管理

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Workfront Planning で次のアクションが発生した場合、アプリ内通知またはメール通知を受け取ることがあります。

* 他のユーザーによって、あなたまたはチームがレコード ページのコメントに追加されます
* ビューまたはワークスペースにアクセスする権限を要求するユーザーがいます
* 他のユーザーからビューまたはワークスペース <!--I could not test this but Isk confirmed--> へのアクセス権が付与されている
* Workfront Planning の要求を発行します。
* 送信されたWorkfront Planning 要求が誰かに承認または拒否されています。
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p><p>Standard, Light, or Contributor
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
</table> -->

Workfrontの計画通知の詳細については、次の記事も参照してください。

* レコードのコメントの詳細については、「[&#x200B; レコードのコメントの管理 &#x200B;](/help/quicksilver/planning/records/manage-record-comments.md)」を参照してください。
* Adobe Workfront Planning からのアプリ内通知について詳しくは、[Workfront Planning のアプリ内通知の管理 &#x200B;](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md) を参照してください。
* Adobe Workfront Planning からのメール通知については、[Workfront Planning のメール通知の管理 &#x200B;](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md) を参照してください。


## 通知設定の管理

1. Adobe Experience Cloudの資格情報を使用してWorkfrontにログインします。
1. 画面右上の **アカウントメニュー** アイコン ![Experience Cloudのアカウントメニューアイコン &#x200B;](assets/account-menu-icon-on-experience-cloud.png) をクリックし、**環境設定** をクリックします。
1. 「**通知**」セクションで、「**Workfront**」をクリックします。
1. 受信する通知を選択します。
または
受信停止する通知の選択を解除します。

   ![Workfront Planning のAdobe Experience Cloud通知パネル &#x200B;](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Workfrontでは、次の通知を利用できます。

   * **メンション**:Workfront Planning で誰かがあなたまたは自分のチームのコメントをタグ付けすると、通知が届きます
   * **リクエスト**：次のいずれかの操作が行われると、通知が届きます。

      * Workfront Planning オブジェクトへのアクセス権を要求または付与します
      * Workfront計画リクエストを送信しました
      * 自分が送信したWorkfront計画リクエストのステータスが変わる
      * Workfront計画リクエストに対する承認を要求、付与または却下

   通知の管理について詳しくは、[&#x200B; アカウント環境設定と通知 &#x200B;](https://experienceleague.adobe.com/ja/docs/core-services/interface/features/account-preferences) を参照してください。

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/ja/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
