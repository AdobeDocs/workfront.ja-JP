---
title: ビューまたはWorkspaceに対する権限のリクエスト
description: 以前に共有されたことがないリンクを他のユーザーから送信されたビューまたはワークスペースに対する権限をリクエストできます。
hidefrontoc: true
hide: true
source-git-commit: 83c716dea3815ed9a2ce4c3d0598ef42b128de87
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 16%

---


<!-- update metadata when released: 

---
title: Request Permissions to a View or a Workspace
description: You can request permissions to a view or a workspace that others sent you a link to which has not been previously shared with you. 
author: Alina
feature: Workfront Planning
role: User, Admin
---
-->

<!--add this to miniTOC and TOC-->

# ビューまたはワークスペースに対する権限のリクエスト

以前に共有されたことがないリンクを他のユーザーから送信されたビューまたはワークスペースに対する権限をリクエストできます。

ビューに対する権限のリクエストは、ワークスペースに対する権限のリクエストと似ています。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

<!--at GA, check that the Workfront plans article linked below has Planning info-->

Workfront Planning にアクセスするには、次のものが必要です：

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
   <td>  <p>許可リクエストが許可されると、次の権限を取得できます。</p>
   <ul><li><p>ビューの表示または管理</p></li>
   <li><p>ワークスペースの表示、Contributeまたは管理</p></li></ul>  
   <p>ワークスペースおよびビューに対する管理権限を持つユーザーのみが、ビューを公開して共有できます。</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ビューまたはワークスペースに対する権限のリクエスト

ビューに対する権限のリクエストは、ワークスペースに対する権限のリクエストと似ています。

アクセス権のないワークスペースまたはビューへのリンクが他のユーザーによって共有された場合：

1. ビューまたはワークスペースで、共有されているリンクをクリックします。

   **アクセス権がありません** ページが表示され、ビューまたはワークスペースに対するアクセス権がないことを示すメッセージが表示されます。

   ![](assets/request-access-to-view.png)

1. （条件付き）共有リンクが、アクセス権を持つワークスペースのビュー用である場合は、「**既存のビューで開く**」をクリックします。 ワークスペースへのアクセス権を持っている場合、レコードタイプページがデフォルトのビューで開きます。

1. （オプションおよび条件付き）ワークスペースを表示する権限がない場合、使用可能なボックスにパーソナライズされたメッセージを追加し、「**アクセスをリクエスト**」をクリックします。

   ビューまたはワークスペースに対する管理権限を持つすべてのユーザーは、アクセスリクエストに関する次の通知を受け取ります。
   * アプリ内通知
     ![](assets/in-app-notification-for-access-request.png)
   * メール通知
     ![](assets/email-notification-for-access-request.png)

   ビューとワークスペースに対する権限の付与については、次の記事を参照してください。

   * [ビューの共有](/help/quicksilver/planning/access/share-views.md)
   * [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)
1. （条件付き）ビューまたはワークスペースマネージャーからビューまたはワークスペースに対する権限が付与されると、権限が付与または拒否されたことを確認するメール通知が届きます。<!--check this - I was not able to test this-->


