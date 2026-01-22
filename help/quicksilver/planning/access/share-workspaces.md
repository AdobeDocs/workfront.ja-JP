---
title: ワークスペースの共有
description: Adobe Workfront Planning で作業する際、ワークスペースを他のユーザーと共有して共同作業を確実に行うことができます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 54a6e633e903c73a78b36e90fb27edb445dc8d47
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 34%

---

# ワークスペースを共有

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning で作業する際、ワークスペースを他のユーザーと共有して共同作業を確実に行うことができます。

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>他のユーザーにワークスペースの権限を付与しても、レコードタイプページのビューに対する権限は付与されません。他のユーザーと共有するには、レコードタイプのページ内の個々のビューに権限を付与する必要があります。詳しくは、[ビューの共有](/help/quicksilver/planning/access/share-views.md)を参照してください。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontおよび Planning パッケージ</p> 
または
<p>任意のワークフローおよび計画パッケージ</p> 
 </tr>
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr>

<td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  <p>ワークスペースに対する権限の管理</p>  </td> 
  </tr>

</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
<p>Your organization must be onboarded to the Adobe Unified Experience for users to be able to request and grant permissions to a workspace from a permission request. </p> 
<p>Users must be added to the Adobe Admin Console in order to gain permissions to Workfront Planning workspaces.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Manage permissions to a workspace</p>  </td> 
  </tr> 

</tbody> 
</table> -->

## ワークスペースの共有に関する考慮事項

* Adobe Workfront Planning でのオブジェクトの共有の一般的な情報については、[Workfront Planning での共有権限の概要 ](/help/quicksilver/planning/access/sharing-permissions-overview.md) も参照してください。
* ワークスペースは、組織内のユーザー、チーム、役割、グループまたは会社と共有できます。
* チーム、グループ、会社、担当業務に加えて、Adobe Admin Consoleに追加されたユーザーとのみ共有できます。
* 組織外のユーザーとワークスペースを共有することはできません。
* ワークスペースを共有すると、そのワークスペースに関連付けられているすべてのレコードタイプ、レコードおよびフィールドも共有されます。
* ワークスペースを共有する場合、ビューは共有されません。 ビューは別々に共有する必要があります。
* Workspaceの権限は、レコードタイプで継承された権限として表示されます。

## ワークスペースに対する権限の共有

以下のユーザーは、ワークスペースを他のユーザーと共有できます。

* システム管理者は、自分が作成していないワークスペースを含め、すべてのワークスペースを共有できます。
* 他のすべてのユーザーは、管理権限を持つワークスペースのみを共有できます。

ワークスペースを他のユーザーと共有するには：

{{step1-to-planning}}

1. 共有するワークスペースを開き、画面の右上隅の「**共有**」をクリックします。

   ![ ワークスペースの右上にある「共有」ボタン ](assets/share-button-on-workspace-top-right.png)

1. 「**このワークスペースへのアクセスを許可**」フィールドに、ユーザー、グループ、チーム、会社または担当業務の名前の入力を開始し、リストに表示されたらクリックします。

   ![UI をグループと共有 ](assets/sharing-ui-with-groups.png)

   >[!NOTE]
   >
   >* チーム、グループ、会社、担当業務に加えて、Adobe Admin Consoleに追加されたユーザーとのみ共有できます。 Workfrontのみのユーザーを追加することはできません。 詳しくは、[Adobe Admin Consoleでのユーザーの管理 ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) を参照してください。
   >
   >* あるユーザーとワークスペースを共有すると、そのユーザーのプライマリ担当業務 <span class="preview"> およびメール </span> もフィールドに表示されます。 ユーザーのメールを表示するには、アクセスレベルでユーザーオブジェクトに対して「連絡先情報を表示」設定を有効にする必要があります。


1. ドロップダウンメニューから次の権限レベルの 1 つを選択します。
   * 表示
   * 参加
   * 管理

     権限レベルと各レベルでユーザーが実行できるアクションについて詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。
1. 「**リンクをコピー**」をクリックして、ワークスペースへのリンクをクリップボードにコピーします。
1. コピーしたリンクを他のユーザーと共有します。リンクを受け取ったユーザーがそのワークスペースにアクセスするには、アクティブユーザーであり、かつ Workfront にログインする必要があります。
1. 「**保存**」をクリックします。

   ワークスペースを共有したユーザーは、権限に関するアプリ内通知とメール通知の両方を受け取ります。

## 権限リクエストからのワークスペースに対する権限の付与

権限のないワークスペースへのリンクにアクセスするユーザーは、ワークスペースに対する権限をリクエストできます。 ワークスペースに対する管理権限を持つすべてのユーザーは、権限リクエストを受け取り、権限を付与または拒否できます。

1. （条件付き）ワークスペースの管理者は、次の領域で別のユーザーからビューにアクセスするリクエストを受け取る場合があります。

   * アプリ内通知
     ![ アクセスリクエストのアプリ内通知 ](assets/in-app-notification-for-access-request.png)
   * メール通知
     ![ アクセスリクエストのメール通知 ](assets/email-notification-for-access-request.png)
1. （条件付き）Workfrontの通知領域で、アプリ内通知をクリックします
または
メール通知で「**すべての通知を表示**」をクリックし、リスト内の通知をクリックします。

   **保留中のアクセスリクエスト** ボックスが表示されます。

   ![ 通知リストの承認ボックス ](assets/notifications-list-approval-box.png)

1. （オプション）権限を承認するユーザーについて、ユーザー名の右側にあるドロップダウンメニューから次のいずれかのオプションを選択します。
   * **表示**
   * **参加**
   * **管理**
1. 権限を承認または拒否するユーザーを選択し、「**すべて承認**」または「**すべて拒否** をクリックします。
1. **保留中のアクセスリクエスト** の左側にある左向き矢印をクリックし、「**保存**」をクリックします。

   リクエストを承認すると、ユーザーはワークスペースの共有ボックスに追加されます。 権限をリクエストするユーザーに、リクエストが承認されたことを示すメールが届きます。<!--will they also get an in-app notification??-->


## ワークスペースに対する権限の削除


{{step1-to-planning}}

1. 権限を削除するワークスペースを開き、画面の右上隅の「**共有**」をクリックします。
1. ワークスペースを共有するエンティティ名の右側にあるドロップダウンメニューをクリックし、「**削除**」をクリックします。
1. 「**保存**」をクリックします。

   削除されたユーザーは、ワークスペースまたはそのオブジェクトにアクセスできなくなります。

   ワークスペースへのアクセスから削除されたユーザーには、これらの権限がなくなったという通知はありません。