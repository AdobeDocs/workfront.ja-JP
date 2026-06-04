---
title: レコードを共有
description: 「共有」ボタンを使用してレコードを共有し、Adobe Workfront Planningでの共同作業を増やすことができます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 9ffad1aa-3c96-40fa-9c62-7a3e00699f18
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/NTytTWD-zq3PVhXn4n-GHinvQxna1wfnAXjaeYBgTEY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a93c6c9faf26d5eab1c223bd4a2646af896bf97d
workflow-type: tm+mt
source-wordcount: 1690
ht-degree: 9%

---

<!--update metadata with real information at release-->

# レコードの共有

<!--
this will NOT be available in Preview ever - find a way to add this in this article that is prominent
-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>\
<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


{{planning-important-intro}}

Adobe Workfront Planningのレコードタイプで、個々のレコードに対するユーザーの権限を調整できます。

次の方法で Adobe Workfront Planning レコードを共有できます。

* レコードへのリンクを共有します。

  詳しくは、[&#x200B; リンクを使用したレコードの共有](/help/quicksilver/planning/records/share-records.md)を参照してください。

* ワークスペースとレコードタイプを共有することで、ワークスペース内のすべてのレコードを他のユーザーと共有できます。

  詳しくは、次の記事を参照してください。

   * [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)

   * [レコードタイプの共有](/help/quicksilver/planning/access/share-record-types.md)

* **共有** オプションを使用して、個々のレコードを共有するか、複数のレコードを一括共有します。

  この記事では、**共有** オプションを使用して他のユーザーとレコードを共有する方法について説明します。

>[!IMPORTANT]
>
>* ワークスペースにアクセスできるユーザーは、少なくともワークスペース内のすべてのレコードに対する表示権限を自動的に取得します。
>* ビューを共有すると、レコードに対するユーザー権限が付与されません。 レコードタイプとレコードに対するユーザー権限を付与できるのは、共有ワークスペースのみです。
>
>Workfront Planningでのオブジェクトの共有に関する一般的な情報については、[Adobe Workfront Planningでの共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)も参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

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
   <p><b>メモ</b></p>
   <p>レコードに対する管理権限を付与できるのは、標準ライセンスを持つユーザーのみです。 他のすべてのライセンスには表示権限しかなく、「管理」オプションはグレー表示されます。</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  <p>ワークスペース、レコードタイプ、レコードに対する権限の管理</p>  
   <p><b>重要</b></p>
   <p>ワークスペースへの管理権限を持つユーザーのみがレコードを共有できます</p></td> 
  </tr>
</tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レコードを共有する際の考慮事項

<!--
maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information
-->

<!--checking on the below with Lilit-->

* レコードは、人物、グループ、チーム、会社、担当業務の各エンティティと共有できます。
* 権限をレコードに制限すると、ユーザーはそのレコードとそのルックアップフィールドの値を、そのレコードが表示されるシステム内の任意の場所に表示しなくなります。
* Workfrontは、最大5つのレコードの詳細な接続でレコード権限をチェックし、ユーザーが自分と共有されたレコードのみを表示できるようにします。
* レコードに次のレベルの権限を付与できます。

   * 表示
   * 管理
* ワークスペースとレコードタイプをユーザーと共有すると、デフォルトでは、ワークスペース内のレコードに対しても同じ権限が付与されます。
ユーザーがワークスペースまたはレコードタイプに対するContribute権限を持っている場合、そのレコードタイプのレコードに対する管理権限を受け取ります。
* ワークスペースからエンティティを削除すると、そのワークスペース内のレコードタイプとすべてのレコードからすべての共有権限が削除されます。
* ワークスペースまたはレコードタイプに対する権限を持たないユーザーとレコードを共有することはできません。

  ワークスペース内にいないユーザーとレコードを共有すると、レコードは自動的にワークスペースに追加されます。
* レコードへのユーザーのアクセスは、次の3つの設定の組み合わせによって決定されます。

   * その権限は、レコードタイプとワークスペースから継承されます
   * レコード共有ボックスに個別に追加された権限
   * ワークスペース内の&#x200B;**全員が**&#x200B;設定を表示できます。

     これにより、ワークスペース内の全員がレコードを表示できるようになります

     <!--
      Cannot do this on a record: 
      * **Only invited people can access**: This is selected by default and allows restricting access to the record to specific people. 
      -->

* ユーザーとレコードを共有すると、デフォルトでは、レコードタイプと同じ権限で追加されます。

  例：

   * レコードタイプに対する表示権限がある場合、レコードに対する表示権限を取得します
   * レコードタイプに対するContribute権限またはManage権限がある場合、レコードに対するManage権限を取得します

* ユーザーがワークスペースおよびレコードタイプに対する管理権限またはコントリビュート権限を持っていて、それらをレコード権限に追加すると、「表示」権限がグレー表示されます。 レコードには、レコードタイプと同じ権限が保持され、レコードに対して低い権限を与えることはできません。

* 1つのレコードに対して継承された権限を無効にできます。その場合、個々のレコードに対してselect ユーザー権限を付与したり、ワークスペースに属しているユーザーがワークスペースに属している場合は、**ワークスペース内のすべてのユーザーが表示できる** オプションが原因で権限を取得したりできます。

* 同じユーザーに対して複数の共有権限が適用される場合、それらの権限の最高レベルが付与されます。

  例えば、レコードが表示権限を持つユーザーと共有され、管理アクセス権を持つグループに割り当てられている場合、そのレコードに対する管理権限を受け取ります。

* 接続されたレコードの数式フィールドまたはルックアップフィールドが、権限のないレコードのフィールドに基づいている場合、レコード内のどの要素にアクセスできないかを正しく計算できます。

  <!--
   Not possible: 
   * As a workspace manager, you can share a record with a user that does not have permissions to the record type or the workspace. In this case, there is a warning next to the added entity notifying you that they don't have access to the workspace or the record type.  You can continue adding the user to the record which will also add them to the record type and workspace, or cancel the sharing.
   -->

  <!--
   ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too
   -->

<!--
Lilit is checking on this, it is not working correctly
-->

<!--
   check on this: I cannot disable inherited permissions when this setting is ON and this documented in a TIP below: When they have View permissions to the workspace or the record type, they retain View permissions to the records. You can grant them Manage permissions to the record by disabling Inherited permissions and selecting the Only invited people can access setting.
   -->

<!-- 
   not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.
   -->

<!--
   Too granular??
   If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 
   If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions 
   -->

<!--
   not sure if any of the Share record types points might match here - ask Lilit??
   -->

## レコードの共有

ワークスペースマネージャーは、個々のレコードに対する権限を調整できます。

{{step1-to-planning}}

1. ワークスペースを開き、レコードを共有するレコードタイプを開きます。

1. 次のいずれかの操作を行います。

   * テーブル表示で、レコードの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**共有**&#x200B;をクリックします。
   * テーブル表示で、1つまたは複数のレコードを選択し、リストの下部にある青いツールバーの&#x200B;**共有**&#x200B;をクリックします。
   * 任意のビューで、レコードの名前をクリックし、レコードの詳細ページの右上隅にある&#x200B;**共有**&#x200B;をクリックします。

   **共有** ボックスが開きます。

   ![継承された権限を持つレコードの](assets/permissions-for-records-with-inherited-permissions-on.png)権限

   >[!WARNING]
   >
   >異なるワークスペースに追加されたレコードに対して、権限を共有することはできません。 レコードを一括共有する場合、レコードはすべて同じワークスペースで作成する必要があります。

1. （オプション） **アクセス権を持つユーザー**&#x200B;領域で、**ワークスペース内のすべてのユーザーが** オプションをデフォルトで表示できます。  ワークスペースおよびレコードタイプに対する&#x200B;**ビュー**&#x200B;以上の権限を持つユーザーはすべて、レコードに対して同じ権限を持ちます。

1. （オプション）「**から権限を継承」オプションの下にあるユーザーのアバターをクリックして、ワークスペースから権限を継承するユーザー、チーム、グループ、企業、またはジョブロールを表示します。<!--logged bug to move "Permissions" to lowercase-->**

   継承された権限を展開すると、レコードタイプに対するユーザーの権限が表示されます。

   >[!TIP]
   >
   >継承された権限リストから個々のエンティティを削除することはできません。 ワークスペースとレコードタイプが共有されたときに関連付けられたエンティティの代わりに、チーム、グループ、会社、または担当業務のユーザーが一覧表示されます。

1. （オプションおよび条件付き）特定のエンティティとレコードを共有し、そのエンティティが既にワークスペースに対して持っているレコードタイプとは異なるアクセス権を与える場合は、次の操作を行います。

   1. **継承した権限**&#x200B;から&#x200B;**オンにした** オプションの選択を解除します。 デフォルトで選択されています。

      オプションが&#x200B;**に変更され、オフになりました**。

      >[!TIP]
      >
      >Workspaceの管理者とレコード作成者は、レコードタイプとレコードに対する管理権限を引き続き持っています。

      <!-- 
      This is no longer possible for a record: 
      (Optional) Select **Only invited people can access** from the **Who has access** area. You must indicate individual users, groups, teams, or companies to share the records with. 
      >[!TIP]
      >
      >You cannot disable or enable Inherited permissions when this setting is selected.
      -->

   1. 「**このレコードへのアクセス権を付与**」フィールドに、ワークスペースまたはレコードタイプに対して付与する権限レベルとは異なる権限レベルを付与するユーザー、チーム、グループ、会社、または担当業務を追加します。

      ユーザーとレコードを共有すると、そのユーザーの主な担当業務とその電子メールもフィールドに表示されます。 ユーザーの電子メールを表示するには、アクセスレベルのUsers オブジェクトで「連絡先情報を表示」設定を有効にする必要があります。

   1. 次のいずれかの権限レベルを選択します。

      * 表示
      * 管理

      >[!IMPORTANT]
      >
      >* ユーザーがワークスペースおよびレコードタイプに対するContributeまたはManage権限を持っている場合、ユーザーにレコードに対するManage権限を付与できます。 「表示」権限がグレー表示されます。
      >* ユーザーがレコードタイプに対してContribute以上を持っている場合、そのレコードに対して少ない権限を付与することはできません。
      >詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。
      >* ワークスペース内にないユーザーに権限を付与することはできません。 ワークスペースおよびレコードタイプに対する権限を持たないユーザーは、どのレコードにもアクセスできません。

   <!--   
   Not possible:
   1. To give users who do not have permissions to the workspace access to view a record, in the **Grant access to this view** field, start typing the name of a user, a group, team, company, or job role, then click it when it displays in the list. 
      The entity you selected is added to the record and also to the record type and the workspace with **View** permissions. 
      System administrators always receive Manage permissions to records shared with them, and there is an indication that a user is a System administrator.
   -->

1. （オプション）「**リンクをコピー**」をクリックして、レコードへのリンクをクリップボードにコピーし、他のユーザーと共有します。 リンクをクリックすると、レコードの詳細ページが開きます。
1. 「**保存**」をクリックします。

   レコードは他のユーザーと共有されるようになりました。

   レコードを共有したユーザーは、レコードに対する権限の付与に関するアプリ内通知とメール通知の両方を受け取ります。

   <!--
   not possible anymore: 
   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them.
   -->

   詳しくは、[Adobe Workfront計画通知：記事インデックス &#x200B;](/help/quicksilver/planning/notifications/notifications-information.md)を参照してください。


1. （オプション）コピーしたリンクを他のユーザーと共有します。

   リンクを受け取ったユーザーが、レコードタイプのページにアクセスして、選択したビューで表示するには、ユーザーがアクティブユーザーであり、Workfront にログインしている必要があります。

   レコードタイプを表示するには、レコードタイプに対する権限が必要です。

   詳細については、「[&#x200B; リンクを使用してレコードを共有する](/help/quicksilver/planning/records/share-records.md)」も参照してください。


## レコードへの権限の削除

ユーザーの権限をレコードから削除できます。 ただし、少なくともワークスペースの表示権限を保持し、少なくともレコードタイプの表示権限も付与します。

ワークスペース内のレコードタイプまたはレコードに対する権限を付与しない場合は、ワークスペースからアクセス権を削除する必要があります。

継承された権限からユーザーを削除することはできません。

{{step1-to-planning}}

1. レコードの共有を停止するワークスペースを開き、レコードタイプカードをクリックします。 レコードタイプページが開きます。
1. 次のいずれかの操作を行います。

   * テーブル表示で、レコードの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**共有**&#x200B;をクリックします。
   * テーブル表示で、1つまたは複数のレコードを選択し、リストの下部にある青いツールバーの&#x200B;**共有**&#x200B;をクリックします。

     同じワークスペースで作成されたレコードを選択する必要があります。
   * 任意のビューで、レコードの名前をクリックし、レコードの詳細ページの右上隅にある&#x200B;**共有**&#x200B;をクリックします。

   **共有** ボックスが開きます。
1. 権限を削除するユーザー、グループ、チーム、会社、または担当業務を見つけ、権限ドロップダウンメニューを名前右側に展開し、**削除**&#x200B;をクリックします。

   ![&#x200B; レコードの権限を削除](assets/remove-option-on-record-sharing-drop-down.png)

1. 「**保存**」をクリックします。

   ユーザーには、レコードに対する指定された権限がなくなりました。 ただし、これらの権限から削除しない限り、レコードタイプとワークスペースに対する権限は引き続き保持されます。

   これらの権限を持たなくなったレコードへのアクセスから削除されたユーザーに対する通知はありません。
