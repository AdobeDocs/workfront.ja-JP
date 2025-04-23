---
title: ビューまたはWorkspaceに対する権限のリクエスト
description: アクセス権のないビューまたはワークスペースへのリンクが他のユーザーと共有されている場合、そのビューまたはワークスペースを開くためのアクセス許可を要求できます。 この記事では、開くことができない共有リンクが発生した場合に、ビューまたはワークスペースへのアクセスをリクエストする手順について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 16%

---

# ビューまたはワークスペースに対する権限のリクエスト

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>この記事で説明されている機能は、組織がAdobe統合エクスペリエンスにオンボーディングされた場合にのみ使用できます。
>
>詳しくは、[Workfront の Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。


アクセス権がないビューまたはワークスペースへのリンクが他のユーザーによって共有されている場合、そのビューまたはワークスペースに対する権限をリクエストできます。

ビューに対する権限のリクエストは、ワークスペースに対する権限のリクエストと似ています。

この記事では、他のユーザーがリンクを共有していて、共有ページにアクセスできない場合に、ビューまたはワークスペースへのアクセスをリクエストする方法について説明します。

ビューとワークスペースに対する権限の付与については、次の記事を参照してください。

* [ビューの共有](/help/quicksilver/planning/access/share-views.md)
* [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)


## アクセス要件

+++ 展開してアクセス要件を表示します…

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
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
<p><b>重要</b></p>
<p>組織内のユーザーは、組織がAdobe Unified Experience にオンボーディングされている場合にのみ、ビューとワークスペースに対する権限をリクエストできます。 </p>
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
   <li><p>ワークスペースの表示、投稿、または管理</p></li></ul>  
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

<!--replace the layout template info in the table with this at release: 

<div class="preview">
<p> Users with a Light or Contributor license must be assigned a layout template that includes the Planning option  in the following areas:</p>
   <ul><li>Main Menu</li>
   <li>Left panel of projects, portfolios, and programs</li>
   <li>Landing page</li>
   <li>Pins</li></ul>
   <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Create and manage layout templates</a>.</p>
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div>
   <p><b>NOTE</b></p>
   <p>In the Production environment, all users including the System administrators must be assigned to a layout template that includes the Planning areas.</p>

-->

## ビューまたはワークスペースに対する権限のリクエスト

ビューに対する権限のリクエストは、ワークスペースに対する権限のリクエストと似ています。

アクセス権のないワークスペースまたはビューへのリンクが他のユーザーによって共有された場合：

1. ビューまたはワークスペースで、共有されているリンクをクリックします。

   **アクセス権がありません** ページが表示され、ビューまたはワークスペースに対するアクセス権がないことを示すメッセージが表示されます。

   ![ 表示へのアクセスをリクエスト ](assets/request-access-to-view.png)

1. （条件付き）共有リンクが、アクセス権を持つワークスペースのビュー用である場合は、「**既存のビューで開く**」をクリックします。 ワークスペースへのアクセス権を持っている場合、レコードタイプページがデフォルトのビューで開きます。

1. （オプションおよび条件付き）ワークスペースを表示する権限がない場合、使用可能なボックスにパーソナライズされたメッセージを追加し、「**アクセスをリクエスト**」をクリックします。

   ビューまたはワークスペースに対する管理権限を持つすべてのユーザーは、アクセスリクエストに関する次の通知を受け取ります。
   * アプリ内通知
     ![ アクセスリクエストのアプリ内通知 ](assets/in-app-notification-for-access-request.png)
   * メール通知
     ![ アクセスリクエストのメール通知 ](assets/email-notification-for-access-request.png)

1. （条件付き）ビューまたはワークスペースマネージャーからビューまたはワークスペースに対する権限を付与されると、権限が付与されたことを確認するメール通知とアプリ内通知が届きます。<!--check this - I was not able to test this, but Isk confirmed.-->
