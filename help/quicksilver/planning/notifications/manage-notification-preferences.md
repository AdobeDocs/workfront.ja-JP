---
title: Adobe Workfront Planning 通知設定の管理
description: Adobe Workfront Planning の通知設定を管理できる場合があります。 この記事では、通知の環境設定を行う方法について説明します。
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 14%

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

+++ 展開すると、アクセス要件が表示されます。

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
<p>組織のWorkfront インスタンスは、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
<p>組織内のユーザーは、組織がWorkfront Unified Experience にオンボーディングされた場合にのみ、Adobe Planning から通知を受け取ります。 </p>
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p><p>標準、ライト、またはコントリビューター
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
   <td> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、Planning を含むレイアウト テンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

Workfrontの計画通知の詳細については、次の記事も参照してください。

* レコードのコメントの詳細については、「[ レコードのコメントの管理 ](/help/quicksilver/planning/records/manage-record-comments.md)」を参照してください。
* Adobe Workfront Planning からのアプリ内通知について詳しくは、[Workfront Planning のアプリ内通知の管理 ](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md) を参照してください。
* Adobe Workfront Planning からのメール通知については、[Workfront Planning のメール通知の管理 ](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md) を参照してください。


## 通知設定の管理

1. Adobe Experience Cloudの資格情報を使用してWorkfrontにログインします。
1. 画面右上の **アカウントメニュー** アイコン ![Experience Cloudのアカウントメニューアイコン ](assets/account-menu-icon-on-experience-cloud.png) をクリックし、**環境設定** をクリックします。
1. 「**通知**」セクションで、「**Workfront**」をクリックします。
1. 受信する通知を選択します。
または
受信停止する通知の選択を解除します。

   ![Workfront Planning のAdobe Experience Cloud通知パネル ](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Workfrontでは、次の通知を利用できます。

   * **メンション**:Workfront Planning で誰かがあなたまたは自分のチームのコメントをタグ付けすると、通知が届きます
   * **リクエスト**：次のいずれかの操作が行われると、通知が届きます。

      * Workfront Planning オブジェクトへのアクセス権を要求または付与します
      * Workfront計画リクエストを送信しました
      * 自分が送信したWorkfront計画リクエストのステータスが変わる
      * Workfront計画リクエストに対する承認を要求、付与または却下

   通知の管理について詳しくは、[ アカウント環境設定と通知 ](https://experienceleague.adobe.com/ja/docs/core-services/interface/features/account-preferences) を参照してください。

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/ja/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
