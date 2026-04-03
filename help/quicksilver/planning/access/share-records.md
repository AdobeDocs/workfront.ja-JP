---
title: レコードを共有
description: 「共有」ボタンを使用してレコードを共有し、Adobe Workfront Planningでの共同作業を増やすことができます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 9ffad1aa-3c96-40fa-9c62-7a3e00699f18
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1886'
ht-degree: 5%

---

<!--update metadata with real information at release-->

# レコードの共有

<!--
this will NOT be available in Preview ever - find a way to add this in this article that is prominent
-->

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Adobe Workfront Planningのレコードタイプで、個々のレコードに対するユーザーの権限を調整できます。

>[!WARNING]
>
>この記事に記載されている情報は、プレビュー環境では使用できません。 Workfront Planningのすべてのユーザーは、実稼動環境でのみ使用できます。

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
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  <p>ワークスペース、レコードタイプ、レコードに対する権限の管理</p>  
   <p><b>重要</b></p>
   <p>ワークスペースへの管理権限を持つユーザーのみがレコードを共有できます</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> LightまたはContributor ライセンスを持つユーザーには、Planningを含むレイアウトテンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトでプランニング領域を有効にできます。</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## レコードを共有する際の考慮事項

<!--
maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information
-->

<!--checking on the below with Lilit-->

* レコードは、人物、グループ、チーム、企業、担当業務などのエンティティと共有できます。
* 権限をレコードに制限すると、ユーザーはそのレコードとそのルックアップフィールドの値を、そのレコードが表示されるシステム内の任意の場所に表示しなくなります。
* Workfrontは、最大5つのレコードの詳細な接続でレコード権限をチェックし、ユーザーが自分と共有されたレコードのみを表示できるようにします。
* レコードに次のレベルの権限を付与できます。

   * 表示
   * 管理
* ワークスペースとレコードタイプをユーザーと共有すると、デフォルトでは、ワークスペース内のレコードに対しても同じ権限が付与されます。
ユーザーがワークスペースまたはレコードタイプに対するContribute権限を持っている場合、そのレコードタイプのレコードに対する管理権限を受け取ります。
* ワークスペースからエンティティを削除すると、そのワークスペース内のレコードタイプとすべてのレコードからすべての共有権限が削除されます。
* レコードへのユーザーのアクセスは、次の3つの設定の組み合わせによって決定されます。

   * その権限は、レコードタイプとワークスペースから継承されます
   * レコード共有ダイアログで個別に追加された権限
   * 次の権限：

      * **ワークスペース内の全員が表示できます**：これにより、ワークスペース <!-- is this OK to say "workspace? should it be "record"??-->内の全員がレコードを表示できます
      * **招待されたユーザーのみがアクセスできます**：これはデフォルトで選択されており、レコードへのアクセスを特定のユーザーに制限できます。

     >[!NOTE]
     >
     >ワークスペース内の全員がレコードタイプまたはレコードに対して&#x200B;**アクセス許可**&#x200B;を付与することを選択した場合、継承されたアクセス許可が無効になっている場合でも、ワークスペース権限の共有リストにリストされている全員が、レコードタイプとレコードに対して同じアクセス許可を持つことになります。

* ユーザーとレコードを共有すると、デフォルトでは、レコードタイプと同じ権限で追加されます。

  例：

   * レコードタイプに対する表示権限がある場合、レコードに対する表示権限を取得します
   * レコードタイプに対するContribute権限またはManage権限がある場合、レコードに対するManage権限を取得します

* ワークスペースマネージャーは、レコードタイプまたはワークスペースに対する権限を持たないユーザーとレコードを共有できます。 この場合、追加されたエンティティの横に、ワークスペースまたはレコードタイプへのアクセス権がないことを通知する警告が表示されます。  ユーザーをレコードに引き続き追加して、レコードタイプとワークスペースに追加したり、共有をキャンセルしたりできます。

<!--
ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too
-->

* ユーザーがワークスペースおよびレコードタイプに対する管理権限またはコントリビュート権限を持っていて、それらをレコード権限に追加すると、「表示」権限がグレー表示されます。 レコードには、レコードタイプと同じ権限が保持され、レコードに対して低い権限を与えることはできません。
<!--
Lilit is checking on this, it is not working correctly
-->

<!--
   check on this: I cannot disable inherited permissions when this setting is ON and this documented in a TIP below: When they have View permissions to the workspace or the record type, they retain View permissions to the records. You can grant them Manage permissions to the record by disabling Inherited permissions and selecting the Only invited people can access setting.
   -->

<!-- 
   not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.
   -->

* 1つのレコードに対して継承された権限を無効にできます。この場合、個々のレコードに対して権限を付与できます。また、ワークスペース内の全員が&#x200B;**表示できるオプション**&#x200B;に属している場合は、権限を取得できます。

* 同じユーザーに複数の共有権限が適用される場合、それらの権限の中で最も高い権限が付与されます。

  例えば、レコードが表示権限を持つユーザーと共有され、管理アクセス権を持つグループの場合、レコードに対する管理権限を取得します。

  <!--
   Too granular??
   If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 
   If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions 
   -->

* 接続されたレコードの数式フィールドまたはルックアップフィールドが、権限のないレコードのフィールドに基づいている場合、レコード内のどの要素にアクセスできないかを正しく計算できます。

  <!--
   not sure if any of the Share record types points might match here - ask Lilit??
   -->

## レコード権限の共有

ワークスペースマネージャーは、個々のレコードに対する権限を調整できます。

{{step1-to-planning}}

1. レコードを共有するワークスペースを開きます。
1. レコードを共有するレコードタイプをクリックします。

1. 次のいずれかの操作を行います。

   * テーブル表示で、レコードの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**共有**&#x200B;をクリックします。
   * テーブル表示でレコードを選択し、リストの下部にある青いツールバーの&#x200B;**共有**&#x200B;をクリックします。
   * 任意のビューで、レコードの名前をクリックし、レコードの詳細ページの右上隅にある&#x200B;**共有**&#x200B;をクリックします。

   **共有** ボックスが開きます。

   ![継承された権限を持つレコードの](assets/permissions-for-records-with-inherited-permissions-on.png)権限

1. （オプション） **アクセス権を持つユーザー**&#x200B;領域で、**ワークスペース内のすべてのユーザーが** オプションをデフォルトで表示できます。  ワークスペースおよびレコードタイプに対する&#x200B;**ビュー**&#x200B;以上の権限を持つユーザーはすべて、レコードに対して同じ権限を持ちます。

1. （オプション）「**継承された権限**」オプションの下にあるユーザー数をクリックして、ワークスペースから権限を継承するユーザー、チーム、グループ、企業、またはジョブロールを表示します。

   >[!TIP]
   >
   >継承された権限リストから個々のエンティティを削除することはできません。<!--test this!-->

1. （オプションおよび条件付き）特定のエンティティとレコードを共有し、そのエンティティが既にワークスペースに対して持っているレコードタイプとは異なるアクセス権を与える場合は、次の操作を行います。

   1. 「**継承された権限**」ドロップダウンメニューから「**無効化**」を選択します。

   >[!TIP]
   >
   >Workspace マネージャーは、レコードタイプとレコードに対する管理権限を引き続き持っています。

   1. （オプション）「**招待されたユーザーのみが**&#x200B;に&#x200B;**アクセス可能なユーザー**&#x200B;領域からアクセスできます」を選択します。 レコードを共有する個々のユーザー、グループ、チーム、会社を指定する必要があります。

      >[!TIP]
      >
      >この設定が選択されている場合、継承された権限を無効または有効にすることはできません。


   1. **このレコードタイプへのアクセス権を付与** フィールドに、ワークスペースまたはレコードタイプに対して付与する権限レベルとは異なる権限レベルを付与するユーザー、チーム、グループ、会社、または担当業務を追加します。
   1. 次のいずれかの権限レベルを選択します。

      * 表示
      * 管理

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* グループ、グループ、企業、担当業務に加えて、Adobe Admin Consoleに追加されたユーザーとのみ共有できます。 Workfrontのみのユーザーを追加することはできません。 詳しくは、[Adobe Admin Consoleでのユーザーの管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)を参照してください。
   >* ユーザーがワークスペースおよびレコードタイプに対するContributeまたはManage権限を持っている場合、ユーザーはレコードに対するManage権限を保持します。 「表示」権限がグレー表示されます。<!--this is not dimmed at this time, Lilit to check-->
   >* ユーザーがレコードタイプに対してContribute以上を持っている場合、そのレコードに対して少ない権限を付与することはできません。
   > 詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。
   >* ユーザーとレコードを共有すると、そのユーザーの主要な担当業務<span class="preview">とその電子メール </span>もフィールドに表示されます。 ユーザーの電子メールを表示するには、アクセスレベルのUsers オブジェクトで「連絡先情報を表示」設定を有効にする必要があります。

1. ワークスペースへのアクセス権を持たないユーザーにレコードを表示するアクセス権を付与するには、「**このビューへのアクセス権を付与**」フィールドで、ユーザー、グループ、チーム、会社、またはジョブロールの名前を入力し始め、リストに表示されたらクリックします。

   選択したエンティティは、レコードに追加され、**表示**&#x200B;権限を持つレコードタイプおよびワークスペースにも追加されます。

   システム管理者は常に、共有されたレコードに対する管理権限を受け取り、ユーザーがシステム管理者であることを示します。

1. （オプション）「**リンクをコピー**」をクリックして、レコードへのリンクをクリップボードにコピーし、他のユーザーと共有します。 リンクをクリックすると、レコードの詳細ページが開きます。
1. 「**保存**」をクリックします。

   レコードは他のユーザーと共有されるようになりました。

   レコードを共有したユーザーは、次のエンティティに対する権限が付与されたことに関するアプリ内通知とメール通知の両方を受け取ります。

   * レコード
   * 以前に権限を持ったことがない場合のレコードタイプ
   * レコードが共有される前にワークスペースに対する権限を持っていない場合、ワークスペース。

   詳しくは、[Adobe Workfront計画通知：記事インデックス &#x200B;](/help/quicksilver/planning/notifications/notifications-information.md)を参照してください。

1. コピーしたリンクを他のユーザーと共有します。リンクを受け取るユーザーは、レコードタイプページにアクセスして選択したビューに表示するには、アクティブなユーザーでWorkfrontにログインする必要があります。 レコードタイプを表示するには、レコードタイプに対する権限が必要です。 詳細については、「[&#x200B; リンクを使用してレコードを共有する](/help/quicksilver/planning/records/share-records.md)」も参照してください。

## レコードへの権限の削除

ユーザーの権限をレコードから削除できます。 ただし、少なくともワークスペースの表示権限を保持し、少なくともレコードタイプの表示権限も付与します。 ワークスペース内のレコードタイプまたはレコードに対する権限を付与しない場合は、ワークスペースからアクセス権を削除する必要があります。

{{step1-to-planning}}

1. レコードの共有を停止するワークスペースを開き、レコードタイプカードをクリックします。 レコードタイプページが開きます。
1. 次のいずれかの操作を行います。

   * テーブル表示で、レコードの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**共有**&#x200B;をクリックします。
   * テーブル表示でレコードを選択し、リストの下部にある青いツールバーの&#x200B;**共有**&#x200B;をクリックします。
   * 任意のビューで、レコードの名前をクリックし、レコードの詳細ページの右上隅にある&#x200B;**共有**&#x200B;をクリックします。

   **共有** ボックスが開きます。
1. 権限を削除するユーザー、グループ、チーム、会社、または担当業務を見つけ、権限ドロップダウンメニューを名前右側に展開し、**削除**&#x200B;をクリックします。<!--check the screen shot below - the UI text for View might not be accurate-->

   ![&#x200B; レコードの権限を削除](assets/remove-option-on-record-sharing-drop-down.png)

1. 「**保存**」をクリックします。

   ユーザーには、レコードに対する指定された権限がなくなりました。 ただし、これらの権限から削除しない限り、レコードタイプとワークスペースに対する権限は引き続き保持されます。

   これらの権限を持たなくなったレコードへのアクセスから削除されたユーザーに対する通知はありません。
