---
title: Adobe Workfront Planning の通知設定の管理
description: Adobe Workfront Planningの通知の環境設定を管理できる場合があります。 この記事では、通知設定の設定方法について説明します。
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
last-update: 2026-04-01T18:23:03Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 12%

---


# Adobe Workfront Planning の通知設定の管理

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

ここでは、一般的に、Adobe Workfront通知ではなく、Adobe Workfront計画の通知を管理する方法について説明します。

Workfront Planningで次のアクションが発生すると、アプリ内通知またはメール通知が届く場合があります。

* 誰かがあなたやチームにレコードページのコメントを追加します
* ビューまたはワークスペース <!--or <span class="preview">or a record</span>-->へのアクセス許可を求めるユーザー
* 誰かが、ビューまたはワークスペース <!--or <span class="preview">or a record</span> I could not test this but Isk confirmed-->へのアクセス権限を付与しました
* Workfront計画リクエストを送信します。
* 送信したWorkfront計画リクエストを誰かが承認または却下します。
* ステータスは、送信したWorkfront Planning リクエストに変わります。

Workfront計画アクティビティから次の種類の通知を受け取って管理できます。

* アプリ内
* メール

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
</table>
-->

Workfront計画の通知の詳細については、次の記事も参照してください。

* レコードに対するコメントについて詳しくは、[&#x200B; レコードコメントの管理](/help/quicksilver/planning/records/manage-record-comments.md)を参照してください。
* 承認通知について詳しくは、次の記事を参照してください。

   * [Adobe Workfront Planning でのリクエストの承認](/help/quicksilver/planning/requests/approve-request.md)
   * [Adobe Workfront Planning リクエストを送信して、レコードを作成](/help/quicksilver/planning/requests/submit-requests.md)
* Workfront Planningからのアプリ内通知について詳しくは、[Adobe Workfront Planningのアプリ内通知の管理](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)を参照してください。
* Workfront Planningからのメール通知について詳しくは、[Adobe Workfront Planningのメール通知の管理](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)を参照してください。


## 通知設定の管理

>[!NOTE]
>
>Workfront計画の通知は、ユーザープロファイルページのAdobeの通知領域ではなく、Workfrontの環境設定エリアを使用して管理します。

1. Adobe Experience Cloudの資格情報でWorkfrontにログインします。
1. 画面の右上にある&#x200B;**アカウントメニュー** アイコン ![Experience Cloud](assets/account-menu-icon-on-experience-cloud.png)のアカウントメニューアイコンをクリックし、**環境設定**&#x200B;をクリックします。
1. **通知** セクションで、**Workfront**&#x200B;をクリックします。
1. 受信する通知を選択します。
または
受信を停止する通知の選択を解除します。

   ![Workfront PlanningのAdobe Experience Cloud通知パネル &#x200B;](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Workfrontでは、次の通知を利用できます。

   * **承認**：誰かがプランニングの承認依頼を送信したとき、または自分からプランニング オブジェクトへのアクセスをリクエストしたいときに通知が届きます。
   * **メンション**: Workfront Planningのコメントで誰かが自分またはチームにタグ付けを行うと、通知が届きます
   * **リクエスト**：次のいずれかの操作を行うと、通知が届きます。

      * Workfront Planning オブジェクトに対する権限をリクエストまたは付与します
      * あなたはWorkfront Planning リクエストを送信しました
      * 変更を送信したWorkfront Planning リクエストのステータス
      * Workfront Planningのリクエストに対する承認のリクエスト、付与または拒否

   通知の管理について詳しくは、[&#x200B; アカウントの環境設定と通知](https://experienceleague.adobe.com/ja/docs/core-services/interface/features/account-preferences)を参照してください。

<!--
OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
