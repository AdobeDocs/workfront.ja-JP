---
title: ビューまたはWorkspaceへの権限のリクエスト
description: アクセス権のないビューまたはワークスペースへのリンクを誰かが共有した場合、アクセス権を要求して開くことができます。 この記事では、開くことができない共有リンクに遭遇した場合に、ビューまたはワークスペースへのアクセスをリクエストする手順について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/FvXVCMMz-PfaT-QAaMq0c5qUruR1MJoMv6etcrAstXA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a93c6c9faf26d5eab1c223bd4a2646af896bf97d
workflow-type: tm+mt
source-wordcount: 567
ht-degree: 13%

---

# ビューまたはワークスペースに対する権限のリクエスト


<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。 すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


<!-- 
no longer needed: 
>[!IMPORTANT]
>
>The functionality described in this article is available only when your organization has been onboarded to the Adobe Unified Experience. 
>
>For more information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md). 
-->

アクセス権を持たないビューまたはワークスペースへのリンクを誰かが共有すると、ビューまたはワークスペースへのアクセス権をリクエストできます。

ビューに対する権限の要求は、ワークスペースに対する権限の要求と似ています。

この記事では、共有ページにアクセスできないユーザーがリンクを共有した場合に、ビューまたはワークスペースへのアクセスをリクエストする方法について説明します。

ビューとワークスペースへの権限の付与について詳しくは、次の記事を参照してください。

* [ビューの共有](/help/quicksilver/planning/access/share-views.md)
* [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontおよびプランニングパッケージ</p> 
または
<p>任意のワークフローとプランニングパッケージ</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>任意</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  <p>権限のリクエストが付与されると、次の権限を取得できます。</p>
   <ul><li><p>ビューの表示または管理</p></li>
   <li><p>ワークスペースの表示、投稿、または管理</p></li>
   <li><p>レコードタイプの表示、送信、管理</p></li>
   <li><p><span class="preview">レコードの表示または管理</span></p></li>
   </ul>  
   <p>ワークスペースとビューに対する管理権限を持つユーザーのみがビューを公開できます。</p></td> 
  </tr> 
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
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
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
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


## 権限をリクエスト

ビューに対する権限の要求は、ワークスペース、レコードタイプ、または<span class="preview"> レコード </span>に対する権限の要求に似ています。

誰かがワークスペース、レコードタイプ、<span class="preview"> レコード </span>、またはアクセス権のないビューへのリンクを共有した場合：

1. ビューまたはワークスペース用に共有されているリンクをクリックします。

   アクセス権がない&#x200B;**** ページが表示され、ビューまたはワークスペースへのアクセス権がないことを知らせます。

   ![ ビューへのアクセスを要求](assets/request-access-to-view.png)

   >[!NOTE]
   >
   >レコードタイプまたは<span class="preview"> レコード </span>へのアクセス権がない場合、「アクセス権がありません」ページには、ワークスペースへのアクセス権が必要であることが表示されます。


1. （条件付き）共有されたリンクが、アクセス権を持つワークスペースのビュー用である場合は、**既存のビューで開く**&#x200B;をクリックします。 ワークスペースにアクセスする権限がある場合は、レコードタイプページがデフォルトビューで開きます。

1. （オプションおよび条件付き）ワークスペースを表示する権限がない場合は、使用可能なボックスにパーソナライズされたメッセージを追加し、**アクセスをリクエスト**&#x200B;をクリックします。

   ビューまたはワークスペースに対する管理権限を持つすべてのユーザーは、アクセスリクエストに対して次の通知を受け取ります。
   * アプリ内通知
     ![ アクセス要求](assets/in-app-notification-for-access-request.png)のアプリ内通知
   * メール通知
     ![ アクセス要求のメール通知](assets/email-notification-for-access-request.png)

1. （条件付き）ビューまたはワークスペースマネージャーがビューまたはワークスペースに権限を付与すると、権限が付与されたことを確認するメール通知とアプリ内通知が届きます。<!--check this - I was not able to test this, but Isk confirmed.-->
