---
title: レコードの共有
description: 「共有」ボタンを使用してレコードを共有すると、Adobe Workfront Planning でのコラボレーションを強化できます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 66dd7354f3723e266b77cb2f367b09c022e8c95e
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 5%

---


<!--update metadata with real information at release-->

# レコードの共有

<!--this will NOT be available in Preview ever - find a way to add this in this article that is prominent-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

レコードタイプ内の個々のレコードに対するユーザーの権限を調整できます。

次の方法で Adobe Workfront Planning レコードを共有できます。

* レコードへのリンクの共有。

  詳しくは、「[&#x200B; リンクを使用してレコードを共有する &#x200B;](/help/quicksilver/planning/records/share-records.md)」を参照してください。

* ワークスペースとレコードタイプを共有することで、ワークスペース内のすべてのレコードを他のユーザーと共有します。

  詳しくは、次の記事を参照してください。

   * [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)

   * [レコードタイプの共有](/help/quicksilver/planning/access/share-record-types.md)

* 「**共有** オプションを使用してレコードを共有します。

  この記事では、「**共有** オプションを使用して他のユーザーとレコードを共有する方法について説明します。

>[!IMPORTANT]
>
>ワークスペースへのアクセス権を持つユーザーには、ワークスペース内のすべてのレコードに対する少なくとも表示権限が自動的に付与されます。
>ビューを共有しても、レコードに対する権限はユーザーに付与されません。 共有ワークスペースのみが、レコードタイプとレコードに対する権限をユーザーに付与できます。
>
>Adobe Workfront Planning でのオブジェクトの共有の一般的な情報については、[Workfront Planning での共有権限の概要 &#x200B;](/help/quicksilver/planning/access/sharing-permissions-overview.md) も参照してください。


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
   <p><b>メモ</b></p>
   <p>標準ライセンスを持つユーザーのみが、レコードに対する管理権限を付与できます。 その他のライセンスは、表示権限のみを持つことができ、管理オプションは淡色表示されます。</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  <p>ワークスペース、レコードタイプおよびレコードに対する権限の管理</p>  
   <p><b>重要</b></p>
   <p>ワークスペースに対する管理権限を持つユーザーのみがレコードを共有できます</p></td> 
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

## レコードを共有する際の考慮事項

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* 人物、グループ、チーム、会社、担当業務のエンティティとレコードを共有できます。
* レコードを共有すると、そのレコードがシステム内に表示されるすべての場所でユーザーは同じアクセス権を持ちます。
* レコードに対する権限を制限すると、そのレコードが追加されているシステム内のどこにも、そのレコードとその参照フィールドの値が表示されなくなります。
* Workfrontは、最大 5 件のレコードの深い接続でレコードの権限を確認し、共有されているレコードのみを表示できるようにします。
* レコードに付与できる権限レベルは次のとおりです。

   * 表示
   * 管理
* ワークスペースとレコードタイプをユーザーと共有すると、デフォルトでは、ユーザーはワークスペースのレコードに対しても同じ権限を受け取ります。
ユーザーがワークスペースまたはレコードタイプに対する投稿権限を持っている場合、そのレコードタイプのレコードに対する管理権限を受け取ります。
* ワークスペースからエンティティを削除すると、すべての共有権限がレコードタイプとその中のすべてのレコードから削除されます。
* レコードに対するユーザーのアクセスは、次の 3 つの設定を組み合わせて決定されます。

   * レコードタイプおよびワークスペースから継承された権限
   * レコード共有ダイアログで個別に追加された権限
   * 次の権限：

      * **ワークスペース内の全員が表示できます**：これにより、ワークスペース内の全員がレコードを表示できるように <!-- is this OK to say "workspace? should it be "record"??--> ります
      * **招待されたユーザーのみがアクセスできます**：これはデフォルトで選択されており、レコードへのアクセスを特定のユーザーに制限できます。

     >[!NOTE]
     >
     >レコード タイプまたはレコードに対する **ワークスペース内の全員に表示権限** を付与すると、継承された権限が無効になっている場合でも、ワークスペース権限の共有リストに表示されるすべてのユーザーは、レコード タイプとレコードに対して同じ権限を持ちます。


* ユーザーとレコードを共有すると、デフォルトでは、レコードタイプに対する権限と同じ権限で追加されます。

  例：

   * レコードタイプに対する表示権限を持っている場合、レコードに対する表示権限を取得します
   * レコードタイプに対する投稿権限または管理権限を持っている場合、レコードに対する管理権限を取得します

* ワークスペースマネージャーは、レコードタイプまたはワークスペースに対する権限を持たないユーザーとレコードを共有できます。 この場合、追加されたエンティティの横に、ワークスペースまたはレコードタイプへのアクセス権がないことを知らせる警告が表示されます。 <!--ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too--> ユーザーをレコードに追加してレコードタイプとワークスペースにも追加するか、共有をキャンセルできます。

* ユーザーがワークスペースおよびレコードタイプに対する管理権限または投稿権限を持ち、それらをレコード権限に追加すると、表示権限がグレー表示されます。 レコードタイプに対する権限と同じ権限がレコードに保持され、レコードに対する下位の権限を付与することはできません。<!--Lilit is checking on this, it is not working correctly-->

  ワークスペースまたはレコードタイプに対する表示権限がある場合、レコードに対する表示権限を保持します。 継承された権限を無効にし、「招待されたユーザーのみがアクセスできる」設定を選択することで、レコードに管理権限を付与できます。<!-- I think this is right, but because of the above not working, I can't test-->

<!-- not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.-->

* 1 つのレコードに対して継承された権限を無効にすることができます。この場合、個々のレコードに権限を付与したり、「**ワークスペース内の全員が表示可能**」オプションに属している場合は権限を取得したりできます。

* 同じユーザーに対して複数の共有権限が適用される場合、それらの権限のうち最も高い権限を受け取ります。

  例えば、レコードが表示権限を持つユーザーと共有され、そのレコードのグループが管理アクセス権を持つ場合、そのレコードに対する管理権限を取得します。

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* 連結レコードの数式フィールドまたはルックアップ フィールドが、アクセス権のないレコードのフィールドに基づいている場合、そのレコードがアクセスできない要因となっている正しい計算が表示されます。

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## レコードの共有権限

ワークスペースマネージャーは、個々のレコードに対する権限を調整できます。

{{step1-to-planning}}

1. レコードを共有するワークスペースを開きます。
1. 共有するレコードの種類をクリックします。

1. 次のいずれかの操作を行います。

   * テーブル表示で、レコード名の上にマウスポインターを置き、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから **共有** をクリックします。
   * テーブル表示でレコードを選択し、リスト下部の青いツールバー上の **共有** をクリックします。
   * 任意の表示で、レコードの名前をクリックし、レコードの詳細ページの右上隅にある **共有** をクリックします。

   **共有** ボックスが開きます。

   ![&#x200B; 権限が継承されたレコードの権限 &#x200B;](assets/permissions-for-records-with-inherited-permissions-on.png)

1. （オプション） **アクセスできるユーザー** 領域では、「**ワークスペースのすべてのユーザーが表示** オプションがデフォルトで選択されています。  ワークスペースおよびレコードタイプに対する **表示** 以上の権限を持つすべてのユーザーは、レコードに対する同じ権限を持ちます。

1. （任意）「**継承された権限**」オプションのユーザー数をクリックして、ワークスペースから権限を継承するユーザー、チーム、グループ、会社または担当業務を表示します。

   >[!TIP]
   >
   >継承された権限リストから個々のエンティティを削除することはできません。

1. （オプションおよび条件付き）レコードを特定のエンティティと共有し、ワークスペースに対して既に付与されているレコードタイプとは異なるアクセス権を付与する場合は、次の操作を行います。

   1. **継承された権限** ドロップダウンメニューから **無効** を選択します。

   >[!TIP]
   >
   >Workspace管理者には、引き続きレコードタイプとレコードに対する管理権限があります。

   1. （オプション） **アクセス権限を持つユーザー** エリアから **招待されたユーザーのみがアクセス** を選択します。

   1. 「**このレコードタイプへのアクセスを許可**」フィールドで、ワークスペースまたはレコードタイプに付与される権限レベルとは異なる権限レベルを付与するユーザー、チーム、グループ、会社または担当業務を追加します。
   1. 次のいずれかのアクセス許可レベルを選択します。

      * 表示
      * 管理

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* チーム、グループ、会社、担当業務に加えて、Adobe Admin Consoleに追加されたユーザーとのみ共有できます。 Workfrontのみのユーザーを追加することはできません。 詳しくは、[Adobe Admin Consoleでのユーザーの管理 &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) を参照してください。
   >* ワークスペースおよびレコードタイプに対する投稿権限または管理権限を持つユーザーは、レコードに対する管理権限を保持します。 表示権限は淡色表示されます。<!--this is not dimmed at this time, Lilit to check-->
   >* ユーザーがレコードタイプに対して投稿以上を持っている場合、ユーザーにそのレコードに対するより小さな権限を付与することはできません。
   > 詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

1. ワークスペースへのアクセス権を持たないユーザーにレコードを表示するには、「**このビューへのアクセスを許可**」フィールドにユーザー、グループ、チーム、会社、担当業務の名前の入力を開始し、リストに表示されたらクリックします。

   選択したエンティティがレコードに追加され、さらにレコードタイプとワークスペースに **表示** 権限も追加されます。

   システム管理者は、常に共有レコードに対する管理権限を受け取り、ユーザーがシステム管理者であることを示しています。

1. （オプション） **リンクをコピー** をクリックして、レコードへのリンクをクリップボードにコピーし、他のユーザーと共有します。 リンクをクリックすると、レコードの詳細ページが開きます。
1. 「**保存**」をクリックします。

   これで、レコードが他のユーザーと共有されます。

   レコードを共有したユーザーは、次のエンティティに権限が付与されたというアプリ内通知とメール通知の両方を受け取ります。

   * レコード
   * 以前に権限を持ったことがない場合は、レコードタイプ
   * ワークスペース（レコードが共有される前にワークスペースに対する権限を持っていなかった場合）。

   詳しくは、[Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md) を参照してください。

1. コピーしたリンクを他のユーザーと共有します。リンクを受け取るユーザーは、アクティブユーザーで、レコードタイプページにアクセスして選択したビューに表示できるようにするには、Workfrontにログインする必要があります。 表示するには、そのレコードタイプに対する権限が必要です。 詳しくは、「[&#x200B; リンクを使用してレコードを共有する &#x200B;](/help/quicksilver/planning/records/share-records.md)」も参照してください。

## レコードに対する権限の削除

ユーザーの権限をレコードから削除できます。 ただし、少なくともワークスペースに対する表示権限は保持され、同時にレコードタイプに対する表示権限も付与されます。 ワークスペース内のレコードタイプやレコードに対する権限を持たせない場合は、ワークスペースからアクセス権を削除する必要があります。

{{step1-to-planning}}

1. レコードの共有を停止するワークスペースを開き、レコードの種類のカードをクリックします。 レコードタイプページが開きます。
1. 次のいずれかの操作を行います。

   * テーブル表示で、レコード名の上にマウスポインターを置き、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから **共有** をクリックします。
   * テーブル表示でレコードを選択し、リスト下部の青いツールバー上の **共有** をクリックします。
   * 任意の表示で、レコードの名前をクリックし、レコードの詳細ページの右上隅にある **共有** をクリックします。

   **共有** ボックスが開きます。
1. 権限を削除するユーザー、グループ、チーム、会社、または担当業務を見つけ、名前の右側にある権限ドロップダウンメニューを展開して、「**削除**」をクリックします。<!--check the screen shot below - the UI text for View might not be accurate-->

   ![&#x200B; レコードに対する権限の削除 &#x200B;](assets/remove-option-on-record-sharing-drop-down.png)

1. 「**保存**」をクリックします。

   レコードに対して示された権限を持っていないユーザー。 ただし、これらの権限からも削除しない限り、レコードタイプとワークスペースに対する権限は保持されます。

   レコードへのアクセスから削除されたユーザーに対して、これらの権限がなくなったという通知はありません。
