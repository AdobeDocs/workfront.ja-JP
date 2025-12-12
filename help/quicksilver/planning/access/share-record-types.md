---
title: レコードタイプの共有
description: レコードタイプを他のユーザーと共有して、Adobe Workfront Planning を使用する際の共同作業を確保できます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '1514'
ht-degree: 6%

---


<!-- take the Remove permissions section out, at the end - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

<!--keep global record types in yellow till Jan 2026-->

# レコードタイプの共有

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードタイプを他のユーザーと共有して、Adobe Workfront Planning でレコードを操作する際に共同作業を確実に行うことができます。

>[!IMPORTANT]
>
>ワークスペースへのアクセス権を持つユーザーには、ワークスペース内のすべてのレコードタイプに対する少なくとも表示権限が自動的に付与されます。
>ビューを共有しても、ユーザーはレコードタイプに対する権限を持ちません。 共有ワークスペースのみが、レコードタイプに対する権限をユーザーに付与できます。
>
>* Adobe Workfront Planning でのオブジェクトの共有の一般的な情報については、[Workfront Planning での共有権限の概要 &#x200B;](/help/quicksilver/planning/access/sharing-permissions-overview.md) も参照してください。
>* 詳しくは、この記事の [&#x200B; レコードタイプを共有する場合の考慮事項 &#x200B;](#considerations-when-sharing-record-types) の節を参照してください。

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
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontおよび Planning パッケージ</p> 
または
<p>任意のワークフローおよび計画パッケージ</p> 
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
   <td>  <p>ワークスペースとレコードタイプに対する権限の管理</p>  
   <p><b>重要</b></p>
   <p>ワークスペースに対する管理権限を持つユーザーのみが、レコードタイプに対する管理権限を共有できます</p></td> 
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>Users must be added to the Adobe Admin Console in order to gain permissions to Workfront Planning views.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
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
   <td>  <p>Manage permissions to a record type</p>  
   <p>Only users with Manage permissions to a workspace can share Manage permissions to a record type</p></td> 
  </tr> 
 
</tbody> 
</table>-->

## レコードタイプを共有する場合の考慮事項

* ワークスペースに対する権限を付与すると、デフォルトでユーザーはワークスペースのレコードタイプに対して同じ権限を付与されます。

  さらに、個々のレコードタイプに対する権限を調整できます。

  ただし、レコード タイプに対して、ワークスペースに対する権限よりも高い権限をユーザーに付与することはできません。
* ワークスペースでのレコードタイプに対する権限よりも低い権限をユーザーに付与できます。 例えば、ワークスペースに対する投稿権限、レコードタイプに対する表示権限を持つことができます。
* ワークスペースに対する管理権限を持つユーザーは、常にワークスペース内のすべてのレコードタイプに対する管理アクセス権を保持します。 継承された権限がオフになっている場合でも、レコードタイプで権限を下げることはできません。

* 現時点では、レコードタイプを共有すると、次のことが可能です。

   * レコードタイプを初めて共有し、ワークスペースに対する権限を持たないユーザーには、ワークスペースに対する表示権限を付与します。

     これにより、ワークスペースのすべてのレコードタイプに対する表示権限も付与されます。

     レコードタイプに対する権限を付与すると、共有ボックスに、ユーザーがワークスペースにも追加されたことを示す表示が表示されます。
   * 継承された権限を無効にする場合は、ワークスペース内のすべてのユーザー（ワークスペースマネージャーを除く）のレコードタイプを表示のみに設定します。

     ワークスペースに対する管理権限を持つユーザーは、レコードタイプに対して継承された権限をオフにした場合でも、常にレコードタイプに対する管理権限を持ちます。
   * レコードタイプに対するユーザーの権限を下げます。 ワークスペース上のユーザーの権限をレコードタイプに増やすことはできません。

     例えば、ワークスペースに対する投稿権限を持っているユーザーは、その権限を特定のレコードタイプに変更して表示できます。 ただし、ワークスペースに対する表示権限を持っているユーザーは、どのレコードタイプに対しても投稿権限を付与できません。

* ワークスペース内のユーザーからレコードタイプへのアクセスを削除することはできません。 少なくともワークスペースに対する表示権限を持っている場合、すべてのユーザーに少なくともすべてのレコードタイプに対する表示権限があります。

* レコードタイプは、次のエンティティと内部で共有できます。

  Workfront ユーザー、グループ、チーム、会社、担当業務
* Workfront以外のユーザーとレコードタイプを外部で共有することはできません。
* ワークスペース権限がビュー権限よりも高くないユーザーにレコードタイプを付与するには、まずビュー権限よりも高い権限でワークスペースを共有する必要があります。 ワークスペースの上位の権限がレコードタイプに適用されます。

<div class="preview">

* グローバルレコードタイプを共有する場合は、次のようなシナリオが考えられます。

   * グローバルレコードタイプは、元のワークスペースから共有できます。
   * グローバルレコードタイプは、セカンダリワークスペースに追加した後は共有できません。

  詳しくは、[&#x200B; クロスワークスペースレコードタイプの概要 &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md) を参照してください。

</div>

## レコードタイプに対する権限の共有

ワークスペースに対する管理権限を持っている場合は、ワークスペースの個々のレコードタイプに対する権限を調整できます。

{{step1-to-planning}}

1. レコードタイプを共有するワークスペースを開きます。

1. 次のいずれかの操作を行います。

   * レコードタイプカードから、**詳細** メニュー/**共有** をクリックします。
   * レコードタイプカードをクリックしてレコードタイプのページを開き、任意のレコードタイプ表示で **共有**/**レコードタイプを共有** をクリックします。

   **共有** ボックスが開きます。

   ![&#x200B; 継承された権限を持つレコードタイプの権限 &#x200B;](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. （オプション） **アクセスできるユーザー** 領域では、「**ワークスペースのすべてのユーザーが表示** オプションがデフォルトで選択されています。  ワークスペースに対する表示以上の権限を持つすべてのユーザーは、レコードタイプを表示できます。

1. （任意）「**継承された権限**」オプションのユーザー数をクリックして、ワークスペースから権限を継承するユーザー、チーム、グループ、会社または担当業務を表示します。

   >[!TIP]
   >
   >継承された権限リストから個々のエンティティを削除することはできません。

1. （オプションおよび条件付き）レコードタイプを特定のエンティティと共有し、ワークスペースに対して既に付与されているレコードタイプとは異なるアクセス権を付与する場合は、次の操作を行います。

   1. **継承された権限** ドロップダウンメニューから **無効** を選択します。

   >[!TIP]
   >
   >Workspace管理者には、引き続きレコードタイプに対する管理権限があります。

   1. 「**このレコードタイプへのアクセスを許可**」フィールドで、ワークスペースに設定されている権限レベルとは異なる権限レベルを付与するユーザー、チーム、グループ、会社または担当業務を追加します。
   1. 権限レベルを選択します。

   >[!IMPORTANT]
   >
   >* チーム、グループ、会社、担当業務に加えて、Adobe Admin Consoleに追加されたユーザーとのみ共有できます。 Workfrontのみのユーザーを追加することはできません。 詳しくは、[Adobe Admin Consoleでのユーザーの管理 &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) を参照してください。
   >* ワークスペースでのレコードタイプに対する権限よりも大きな権限をユーザーに付与することはできません。
   >* ワークスペースに対する管理権限を持っているユーザーには、レコードタイプに対する管理権限よりも少ない権限を付与することはできません。
   >* ワークスペースに対する投稿権限があるユーザーには、レコードタイプに対する権限を小さくすることができます。
   > 詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

1. ワークスペースへのアクセス権を持たないユーザーにレコードタイプを表示する権限を付与するには、「**このビューへのアクセスを許可**」フィールドにユーザー、グループ、チーム、会社、担当業務の名前を入力し始め、リストに表示されたらクリックします。

   選択したエンティティは、レコードタイプと、**表示** 権限を持つワークスペースに追加されます。

   システム管理者は、常に共有されているレコードタイプに対する管理権限を受け取り、ユーザーがシステム管理者であることを示しています。

1. （オプション） **リンクをコピー** をクリックして、レコードタイプへのリンクをクリップボードにコピーし、他のユーザーと共有します。
1. 「**保存**」をクリックします。

   レコードタイプが他のユーザーと共有されるようになりました。
レコードタイプを共有したユーザーは、次のエンティティに権限を付与したことについてのアプリ内通知とメール通知の両方を受け取ります。

   * レコードタイプ
   * ワークスペース（レコードタイプが共有される前にワークスペースに対する権限を持っていなかった場合）。

1. コピーしたリンクを他のユーザーと共有します。リンクを受け取るユーザーは、アクティブユーザーで、レコードタイプページにアクセスして選択したビューに表示できるようにするには、Workfrontにログインする必要があります。 表示するには、そのレコードタイプに対する権限が必要です。

## レコードタイプに対する権限の削除

レコードタイプからユーザーの権限を削除できます。 ただし、少なくともワークスペースに対する表示権限は保持され、同時にレコードタイプに対する表示権限も付与されます。 ワークスペース内のレコードタイプに対する権限を付与したくない場合は、ワークスペースからアクセス権を削除する必要があります。

{{step1-to-planning}}

1. 共有を停止するレコードの種類があるワークスペースを開き、レコードの種類のカードをクリックします。 レコードタイプページが開きます。

1. 任意のビューのタブで、レコードタイプの右上隅にある「**共有**」をクリックします。
1. **レコードタイプを共有** をクリックします。

   **共有** ボックスが開きます。
1. 権限を削除するユーザー、グループ、チーム、会社、または担当業務を見つけ、名前の右側にある権限ドロップダウンメニューを展開して、「**削除**」をクリックします。<!--check the screen shot below - the UI text for View might not be accurate-->

   ![&#x200B; レコードタイプ共有ドロップダウンの「削除」オプション &#x200B;](assets/remove-option-on-record-type-sharing-drop-down.png)

1. 「**保存**」をクリックします。

   レコードタイプに対して示された権限がなくなりました。 ただし、ワークスペース権限も削除しない限り、ワークスペースに対する権限は保持されたままになります。

   レコードタイプへのアクセスから削除されたユーザーに対して、これらの権限がなくなったという通知はありません。

<!-- This is not working yet: *************************** edit this before publishing, because this was not tested with record types - this section came from sharing views *******************: 

## Grant permissions to a record type from a permission request

Users who access a link to a record type to which they do not have permissions can request permissions to the record type. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)
1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->

