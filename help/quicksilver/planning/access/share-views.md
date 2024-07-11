---
title: ビューを共有
description: Adobe Workfront Planning を使用する際に、他のユーザーとビューを共有して、共同作業を確実に行えます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 60%

---

<!--update the metadata and description when we turn this article live-->

# ビューを共有

{{planning-important-intro}}

Adobe Workfront Planning でレコードを操作する際に、他のユーザーとビューを共有して、共同作業を確実に行えます。

他のユーザーにワークスペースの権限を付与しても、レコードタイプページのビューに対する権限は付与されません。他のユーザーと共有するには、レコードタイプのページ内の個々のビューに権限を付与する必要があります。

ビューを共有すると、そのビューのすべての要素にアクセスする権限が他のユーザーに与えられます。 例えば、ビューに管理権限を付与すると、グループ化、フィルター、並べ替え、バーの外観を変更できます。


次のエンティティでビューを共有できます。

* Workfront ユーザー
* Workfront グループ
<!--* Publicly, with users outside Workfront
-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 契約</p></td>
   <td>
<p>Workfront Planning の早期アクセス段階に登録されている必要があります </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
   <p>新規：標準</p>
   または
   <p>現在：プラン </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> Adobe Workfront Planning に対するアクセス制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ビューに対する権限を管理</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p> 
</td>
  </tr>
 </tbody>
</table>

*詳細については、を参照してください [Workfrontのドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



## ビューに対する権限の共有 <!--internally-->

作成したビューまたは管理権限を持つビューを共有できます <!--with users or groups in Workfront-->.

>[!NOTE]
>
>システム管理者は、自分で作成しなかったビューは表示または共有できません。自分と共有されたビューのみにアクセスしたり、ビューのみを共有したりできます。
>
>システム管理者は、ビューに対する管理権限のみを持つことができます。

{{step1-to-planning}}

1. 共有するビューのワークスペースを開き、レコードタイプカードをクリックします。

   レコードタイプページが開きます。

1. ビュータブで、共有するビューにポインタを合わせ、ビュー名の右にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックしたあと、「**共有**」をクリックします。

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   <!--The Internal sharing tab should be selected by default.-->

1. （オプション）次のオプションから選択して、ビューを共有します。

   * **招待されたユーザーのみがアクセスできます**：ビューを共有するユーザーまたはグループを指定する必要があります。 これはデフォルトのオプションです。
   * **ワークスペースの全員が表示できます**：ワークスペースに対する表示以上の権限を持つすべてのユーザーがビューにアクセスできます。

1. が含まれる **表示アクセス権の付与先** フィールドに、ユーザーまたはグループの名前の入力を開始し、リストに表示されたらクリックします。  <!--***********replace screen shot below when public sharing is released***********-->

   ![](assets/sharing-a-view-ui-with-groups.png)

1. ドロップダウンメニューから次の権限レベルの 1 つを選択します。
   * 表示
   * 管理

     権限レベルと各レベルでユーザーが実行できるアクションについて詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

     システム管理者は、共有されたビューに対する管理権限を常に受け取ります。

1. 「**リンクをコピー**」をクリックして、ビューへのリンクをクリップボードにコピーします。
1. コピーしたリンクを他のユーザーと共有します。リンクを受け取ったユーザーが、レコードタイプのページにアクセスして、選択したビューで表示するには、ユーザーがアクティブユーザーであり、Workfront にログインしている必要があります。
1. 「**保存**」をクリックします。

   >[!TIP]
   >
   >   自分と共有されているビューには、ユーザー情報インジケーターがあります ![](assets/view-shared-with-others-people-icon.png) 表示アイコンの横。 人物インジケーターのないビューは、作成したビューです。



<!--
## Share permissions to a view publicly

You can share views you created or views you have Manage permissions to with people that do not have a Workfront license and who might be external to your organization. 

Consider the following when publicly sharing a Workfront Planning view: 

* You can share a public link to a record type page that displays in the view you are sharing.
* People accessing the record type with the public link you provide have View permissions to the record page. They cannot modify the view, the records, or any of the fields that are visible in the view. 
* The shared public link must have an expiration date after which the link is no longer accessible. 

To share a view publicly in Workfront Planning: 

{{step1-to-planning}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Click **Public sharing**.

1. Enable the **Create public link** setting.

   A link becomes available. This is a public link. When shared, anyone with the link, including people from outside your organization can access the record type page, and view records and fields on the page. 

1. Click the **Copy link** icon ![](assets/copy-link-view.png) to copy the link to your clipboard. 

1. Manually enter a date, or use the calendar in the **Link expiration date** field to select an expiration date for the public link. The record page view will not be accessible after the selected date. 

1. Click **Save**.

1. Paste the link you copied to an email, chat message, document, or in a Workfront comment to share it with others. 

-->


## ビューに対する権限を削除

{{step1-to-planning}}

1. 共有を停止するビューのワークスペースを開き、レコードタイプのカードをクリックします。 レコードタイプページが開きます。
1. 共有を削除するビューのタブ名にポインタを合わせ、 **詳細** メニュー ![](assets/more-menu.png)を選択し、 **共有**.
1. 削除するユーザーまたはグループを見つけて、ユーザー名またはグループ名の右側にある権限ドロップダウンメニューで「**削除**」をクリックします。
1. 「**保存**」をクリックします。
削除されたグループに属するユーザーは、ビューにアクセスできなくなります。ビューへのアクセスから削除されたユーザーに対しては、アクセス権が失われたという通知はありません。

<!--Replace the above instructions with the following when public sharing is released: 

{{step1-to-planning}}

1. Open the workspace whose view you want to stop sharing, then click a record type card. This opens the record type page.
1. Hover over the tab name of the view you want to remove sharing from and click the **More** menu ![](assets/more-menu.png), then click **Share**.
1. To remove the internal sharing of a view, do the following: 

   1. Ensure the **Internal sharing** tab is selected.
   1. Find the user or group what you want to remove, expand the permissions drop-down menu to the right of the user's or group's name, then click **Remove**.

1. To remove the public sharing of a view, do the following: 

   1. Click the **Public sharing** tab.
   1. Deselect the **Create public link** option. 

1. Click **Save**.
   
   People no longer have access to the view. There is no notification for the users that have been removed from accessing the view that they no longer have this access.-->