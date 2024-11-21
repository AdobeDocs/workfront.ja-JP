---
title: Adobe Workfront Planning のアプリ内通知の管理
description: レコードのコメントでタグが付けられると、そのタグに関するメール通知が届きます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 24%

---


# Adobe Workfront Planning のアプリ内通知の管理

{{planning-important-intro}}

次のシナリオが発生した場合は、Workfront Planning からアプリ内通知を受け取ることができます。

* 誰かがレコードのコメントであなたをタグ付けします

  レコードコメント内の他のタグ付けについて詳しくは、[ レコードコメントの管理 ](/help/quicksilver/planning/records/manage-record-comments.md) を参照してください。
* 他のユーザーから、ビューまたはワークスペースにアクセスする許可を要求されています
* ビューまたはワークスペース <!--Isk confirmed there is no notification for denying permissions - did not test--> ーバーへのアクセスが許可されたことを確認するメッセージが表示されます

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
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

+++ Expand to view access requirements for Workfront Planning. 

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
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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

+++
-->

## コメントで誰かがあなたをタグ付けしたとき、アプリ内通知を管理します

1. （条件付き）レコードのコメントで誰かがタグを付けた後、Adobe Experience Cloudのアプリ内 **通知** アイコン ![](assets/experience-cloud-notifications-icon.png) に移動します。

   ![](assets/in-app-notification-example.png)

1. 通知をクリックします。

   Workfront Planning に「レコードの詳細」ページが開きます。 レコードを更新したり、コメントに返信したりできます。

1. （任意） **すべて既読としてマーク** をクリックして、すべての通知を既読にしたことを示します。
1. （任意）「**すべて表示**」をクリックして、Adobe Experience Cloudの **通知** ページに移動します。

## 権限をリクエストおよび付与する際のアプリ内通知の管理

ビューやワークスペースに対する権限を要求または付与された場合、アプリ内通知を受け取ります。

ビューまたはワークスペースに対する権限の要求、付与、または拒否の詳細については、[ ビューまたはワークスペースに対する権限の要求 ](/help/quicksilver/planning/access/request-permissions.md) を参照してください。

Adobe Workfront Planning 通知の管理については、[Workfront Planning 通知環境設定の管理 ](/help/quicksilver/planning/notifications/manage-notification-preferences.md) を参照してください。