---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: オブジェクトから権限を削除
description: 共有にアクセスできるオブジェクトに対する他のユーザーの権限を削除できます。オブジェクトからの権限の削除は、共有可能なすべてのオブジェクトで同一です。
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: ce7b475dbd11f9cfd7fcf9879c0f34bf993f9113
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 84%

---

# オブジェクトから権限を削除

<!--Audited: 01/2024-->

共有にアクセスできるオブジェクトに対する他のユーザーの権限を削除できます。オブジェクトからの権限の削除は、共有可能なすべてのオブジェクトで同一です。

オブジェクトを共有する場合と同様の考慮事項が、オブジェクトから権限を削除する場合にも適用されます。詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)の記事の[オブジェクトの共有に関する考慮事項](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider)の節を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。


オブジェクトを共有するには、次の条件を満たしている必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront ライセンス*</td> 
   <td> <p>新規ライセンス：コントリビューター以上</p>
   または  
   <p>現在のライセンス：リクエスト以上</p>
   <p><b>メモ</b></p>

<p>一部のオブジェクトでは、リクエスト以上のアクセス権が必要です。 </p>

<p>例えば、新規ライセンスの場合、コントリビューターはイシューを共有できますが、プロジェクトを共有できるのは標準ライセンスユーザーのみです。</p>

<p>現在のライセンスの場合、依頼者はイシューを共有できますが、プロジェクトを共有できるのは、作業者またはプランナーのみです。</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>共有するオブジェクトに対する表示以上の権限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>共有するオブジェクトに対する表示またはそれ以上の権限</p> <p>オブジェクトの継承された権限を削除する権限を管理</p>  </td> 
  </tr> 
 </tbody> 
</table>

*ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## オブジェクトの共有リストからエンティティを削除 {#remove-entities-from-the-sharing-list-of-an-object}

オブジェクトの共有リストからエンティティ（ユーザー、担当業務、チーム、グループ、会社）を削除できます。これにより、オブジェクトに対する権限が削除されます。

1. 権限を削除するオブジェクトに移動します。

   共有可能なオブジェクトについて詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

1. （条件付き）プログラム、ポートフォリオおよびドキュメントの場合は、次の操作を行います。

   1. オブジェクト名の横にある **詳細** アイコン ![ 詳細アイコン ](assets/more-icon.png) をクリックし、「**共有**」または「**共有** をクリックします。

      ![share](assets/share-a-document-350x160.png)

   1. ユーザー、チーム、グループ、会社、担当業務の横にある **x** をクリックし「オブジェクトアクセス」ボックスから削除します。

      ![ 権限を削除 ](assets/remove-permissions-on-portfolio.png)

   1. **[ユーザー名 ] のWorkfront アクセス権限が削除されます。この** ドロップダウン メニューで、ユーザーのアクセス権限を選択したオブジェクトのみから削除するか、関連付けられたすべての子オブジェクトから削除するかを選択します。

1. （条件付き）プロジェクト、タスク、イシューの場合は、次の手順を実行します。

   1. オブジェクト名の右にある「**共有**」をクリックします。

      ![share](assets/new-share-button.png)
   1. オブジェクトから削除するユーザー、役割、チーム、グループまたは会社を検索します。
   1. 「**削除**」をクリックします。
「**次から &lt;ユーザー名> を削除**」ドロップダウンメニューで、選択したオブジェクトのみからアクセス権を削除するか、それに関連付けられているすべての子オブジェクトからアクセス権を削除するかを選択します。

      ![ 削除 ](assets/remove-permissions-on-project-nwe-350x479.png)

   次のシナリオが存在します。

   * オブジェクトからのみエンティティを削除する場合、そのエンティティはオブジェクトに対する権限を失い、子オブジェクトに継承された権限を失います。以前に子項目に対して個別に権限を付与されていた場合、このオプションを選択すると、関連付けられているすべての子オブジェクトに対して同じ権限が保持されます。
   * オブジェクトとすべての子オブジェクトからエンティティを削除すると、各子オブジェクトに対して個別の権限が与えられていた場合でも、そのエンティティはオブジェクトおよびすべての子オブジェクトに対する権限を失います。

1. 「**保存**」をクリックします。

<!--
## Remove permissions from several objects in bulk

You can remove entities (users, job roles, teams, groups, companies) from several objects at a time when you bulk select them in a list.

>[!NOTE]
>
>You cannot view what access entities have for all the objects selected when you select them in bulk. You must know which entity you want to remove from the sharing of the objects selected before removing their permissions.

1. Go to the list of objects that you want to share.

   For information about which objects can be shared, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Select several objects in the list, then click the **Share** icon ![share icon](assets/share-icon.png)at the top of the list. 
1. Type the name of the user, role, team, group, or company for which you want to remove the access in the **Edit `<Object Name>` access to** field. 
1. From the access drop-down menu, select **No Access**.

   ![remove in bulk](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. In the `<User Name>`'s Workfront access will be removed from this drop-down menu, select whether you want their access to be removed just from the objects that you have selected, or from all other children objects associated with it.  
   The following scenarios exist:

   * If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they were previously granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;
   * If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they were previously given individual permission on each child object.

   **Example:** Select whether to remove permissions to just the tasks you selected in a list, or to the issues and documents attached to the tasks as well.

   ![access](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Optional) To change permissions in bulk for several objects, select another level of sharing for the selected entity.

   For example, if they have Manage permissions, select Contribute or View instead. 

1. Click **Save**.

-->

## 継承した権限を削除

継承された権限はオブジェクトから削除できます。これにより、親オブジェクトへのユーザーのアクセスに関係なく、所有者は子オブジェクトへのアクセス権を取得するユーザーを特定できます。

>[!IMPORTANT]
>
>継承された権限を削除できるのは、管理権限を持つユーザーのみです。

継承した権限を削除するには：

1. 管理権限を持つオブジェクトに移動します。例えば、タスクに移動します。
1. この記事の「[オブジェクトの共有リストからエンティティを削除する](#remove-entities-from-the-sharing-list-of-an-object)」で説明されているように、オブジェクトアクセスボックスに移動します。
1. **継承された権限** の横にある **オフ** を選択して無効にします。

   これにより、親オブジェクト（プロジェクトなど）に対する権限を付与されたユーザーが、デフォルトでこのタスクに対する権限を持つことを防ぐことができます。タスクに権限を付与するには、タスクの共有リストに個々のエンティティをリストする必要があります。

   >[!TIP]
   >
   >継承された権限リストから個々のエンティティを削除することはできません。リストされているすべてのエンティティに対して、継承された権限のみ無効にできます。

1. 「**保存**」をクリックします。

## オブジェクトを非公開にする

システム全体でオブジェクトを共有している場合や、オブジェクトを公開して外部のユーザーと共有している場合は、システム全体または公開の権限を削除して、再び非公開にすることができます。 

オブジェクトをシステム全体または公開で使用できるようにする方法について詳しくは、[オブジェクトを共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)を参照してください。

オブジェクトを非公開にするには、次の手順を実行します。

1. 非公開にするオブジェクトに移動します。\
   例えば、レポートに移動します。
1. 「**レポートのアクション**」、「**共有**」の順にクリックします。

   ![ プライベートにする ](assets/report-permissions-make-private-nwe-350x477.png)

1. 歯車アイコンをクリックし、「**これを外部ユーザーに公開** のチェックを外します。
1. **アクセス権を持つユーザー** ドロップダウンメニューで、**招待されたユーザーのみがアクセスできる** をクリックして、すべてのWorkfront ユーザーとの共有を停止します。
1. **保存**&#x200B;をクリックします。
