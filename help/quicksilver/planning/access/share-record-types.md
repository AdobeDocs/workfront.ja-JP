---
title: レコードタイプの共有
description: レコードタイプを他のユーザーと共有して、Adobe Workfront Planning を使用する際の共同作業を確保できます。
hide: true
hidefromtoc: true
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 5005493bb98b63f4c463f424be43a9d422744846
workflow-type: tm+mt
source-wordcount: '1188'
ht-degree: 14%

---

<!-- add these to metadata on release:

author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog-->

# レコードタイプの共有

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードタイプを他のユーザーと共有して、Adobe Workfront Planning でレコードを操作する際に共同作業を確実に行うことができます。

>[!IMPORTANT]
>
>* ワークスペースに対する権限を付与すると、デフォルトでユーザーはワークスペースのレコードタイプに対して同じ権限を付与されます。
>* 個々のレコードタイプに対する権限を調整できます。
>* ワークスペースに対するアクセス権と比較して、レコードタイプに対する高いアクセス権をユーザーに付与することはできません。
> 詳しくは、この記事の [ レコードタイプを共有する場合の考慮事項 ](#considerations-when-sharing-record-types) の節を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>ユーザーが権限リクエストに基づいてビューに対する権限をリクエストおよび付与できるようにするには、組織がAdobe統合エクスペリエンスにオンボーディングされている必要があります。 </p>
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準</p>
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
   <td>  <p>レコードタイプに対する権限の管理</p>  
   <p>ワークスペースに対する管理権限を持つユーザーのみが、レコードタイプに対する管理権限を共有できます</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レコードタイプを共有する場合の考慮事項

* Adobe Workfront Planning でのオブジェクトの共有の一般的な情報については、[Workfront Planning での共有権限の概要 ](/help/quicksilver/planning/access/sharing-permissions-overview.md) も参照してください。
* レコードタイプは、次のエンティティと内部で共有できます。

   * Workfront ユーザー、グループ、チーム、会社、担当業務
* Workfront以外のユーザーとレコードタイプを外部で共有することはできません。
* 自動的に、ユーザーはワークスペースからレコードタイプ権限を継承します。
* 手動で、レコードタイプに表示権限をユーザーに付与したり、継承された権限をワークスペースから削除したりできます。

* レコードタイプ共有ボックスに追加されたユーザーのうち、ワークスペース権限を持たないユーザーは、表示権限を持つワークスペース共有に自動的に追加されます。

  ワークスペース権限を持たないユーザーにレコードの種類に対する表示権限よりも高い権限を付与するには、まずワークスペースを共有する必要があります。 レコードタイプのみを共有する場合、そのレコードタイプに対する表示権限のみを受け取ることができ、表示権限を持つワークスペースにも追加されます。 レコードタイプに対する権限を付与すると、共有ボックスに、ユーザーがワークスペースにも追加されたことを示す表示が表示されます。

* ワークスペースでのレコードタイプに対する権限よりも高い権限を他のユーザーに付与することはできません。

  例えば、ワークスペースに対する表示権限とレコードタイプに対する管理権限を誰かに付与することはできません。


## レコードタイプに対する権限の共有

ワークスペースに対する管理権限を持っている場合は、ワークスペースの個々のレコードタイプに対する権限を調整できます。

{{step1-to-planning}}

1. 共有するレコードタイプのワークスペースを開き、レコードタイプのカードをクリックします。

   レコードタイプページが開きます。

1. 任意のビューのタブで、レコードタイプの右上隅にある「**共有**」をクリックします。

   **共有** ボックスが開きます。

   ![ 継承された権限を持つレコードタイプの権限 ](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. （オプション） **アクセスできるユーザー** 領域で、次のオプションから選択します。<!--the Only invited people is supposed to be removed - rewrite this - according to Vahan-->

   * **招待されたユーザーのみがアクセスできます**：ビューを共有するユーザー、グループ、チーム、会社または担当業務を指定する必要があります。
   * **ワークスペース内の全員が表示できます**：ワークスペースに対する表示以上の権限を持つすべてのユーザーが、ビューにアクセスできます。 これはデフォルトのオプションです。<!--rewrite this based on what Lilit says in the proof: At this point, once the inherited permissions are disabled, everyone in the workspace except workspace managers will have View permission to the record type because the "Everyone in the workspace can view"  setting cannot be changed. -->

1. （オプション） **継承された権限** オプションを展開して、ワークスペースから権限を継承するユーザー、チーム、グループ、会社または担当業務を表示します。

   >[!TIP]
   >
   >継承された権限リストから個々のエンティティを削除することはできません。

1. （オプションおよび条件付き）レコードタイプを特定のエンティティと共有し、ワークスペースに対して既に付与されているレコードタイプとは異なるアクセス権を付与する場合は、次の操作を行います。

   1. 継承された権限をオフにします。
   1. 「**このレコードタイプへのアクセスを許可**」フィールドで、別の権限レベルを付与するユーザー、チーム、グループ、会社または担当業務を追加します。
   1. 権限レベルを選択します。

   >[!IMPORTANT]
   >
   >* ワークスペースでのレコードタイプに対する権限よりも大きな権限をユーザーに付与することはできません。
   >* ワークスペースに対する管理権限を持っているユーザーには、レコードタイプに対する管理権限よりも小さい権限を付与することはできません。
   >* ワークスペースに対する投稿権限があるユーザーには、レコードタイプに対する権限を小さくすることができます。
   > 詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

1. ワークスペースへのアクセス権を持たないユーザーにレコードタイプを表示するには、「**このビューへのアクセスを許可**」フィールドにユーザー、グループ、チーム、会社、担当業務の名前の入力を開始し、リストに表示されたらクリックします。

   選択したエンティティは、レコードタイプと、**表示** 権限を持つワークスペースに追加されます。

   システム管理者は、常に共有されているレコードタイプに対する管理権限を受け取り、ユーザーがシステム管理者であることを示しています。

1. **リンクをコピー** をクリックして、レコードタイプへのリンクをクリップボードにコピーします。
1. **保存**&#x200B;をクリックします。

   レコードタイプが他のユーザーと共有されるようになりました。

1. コピーしたリンクを他のユーザーと共有します。リンクを受け取ったユーザーが、レコードタイプのページにアクセスして、選択したビューで表示するには、ユーザーがアクティブユーザーであり、Workfront にログインしている必要があります。

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

## レコードタイプに対する権限の削除

<!-- take this section out - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

{{step1-to-planning}}

1. 共有を停止するレコードの種類があるワークスペースを開き、レコードの種類のカードをクリックします。 レコードタイプページが開きます。

1. 任意のビューのタブで、レコードタイプの右上隅にある「**共有**」をクリックします。

   **共有** ボックスが開きます。
1. 権限を削除するユーザー、グループ、チーム、会社、または担当業務を見つけ、名前の右側にある権限ドロップダウンメニューを展開して、「**削除**」をクリックします。<!--check the screen shot below - the UI text for View might not be accurate-->

   ![ レコードタイプ共有ドロップダウンの「削除」オプション ](assets/remove-option-on-record-type-sharing-drop-down.png)

1. **保存**&#x200B;をクリックします。

   レコードタイプにアクセスする権限がなくなりました。 Workspace 権限からも削除しない限り、ワークスペースに対する権限を持つことができます。

   ビューへのアクセスを削除されたユーザーに対しては、アクセス権がなくなったことを示す通知はありません。
