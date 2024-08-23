---
title: レコードを接続
description: レコードタイプ間の接続を作成した後、個々のレコードを相互に接続できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 61cad7dc76ba04ea84ff0bd5052182f040f7b4d9
workflow-type: tm+mt
source-wordcount: '2710'
ht-degree: 54%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting records to one another, you can also connect records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->


# レコードの接続

{{planning-important-intro}}

Adobe Workfront Planning レコードを相互に接続したり、他のアプリケーションのオブジェクトに接続したりできます。

この記事では、レコードを接続する方法について説明します。 レコードの接続に関する一般的な情報については、[ 接続されたレコードの概要 ](/help/quicksilver/planning/records/connected-records-overview.md) を参照してください。

まず、2 つのレコードタイプを相互に接続するか、レコードタイプを別のアプリケーションのオブジェクトタイプに接続する必要があります。これにより、リンクされたレコードフィールドが作成されます。その後、リンクされたレコードフィールドを使用して、レコードを相互に接続したり、他のアプリケーションの他のオブジェクトに接続したりできます。

レコードの接続は、レコードを別のアプリケーションのオブジェクトに接続することと似ています。

レコードタイプの相互の接続や、レコードタイプの他のアプリケーションのオブジェクトタイプへの接続について詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

レコードタイプを連結する例については、[レコードタイプとレコードの連結例](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md)を参照してください。

以下を連結することができます。

* Adobe Workfront Planning レコード
* 他のアプリケーションからのオブジェクトを含む Adobe Workfront Planning レコード。

  次のアプリケーションから、レコードを以下にリストされているタイプのオブジェクトに接続できます。

   * Adobe Workfront

      * プロジェクト
      * ポートフォリオ
      * プログラム
      * 会社
      * グループ

   * Adobe Experience Manager Assets

      * 画像ファイル
      * フォルダー

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

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
   <td> 標準
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
   <td>   <p>レコードを接続するワークスペースへの権限を管理 </p>  
   <p>ワークスペースに対する表示以上の権限。他のアプリケーションでのアクセス権に関係なく、他のアプリケーションからのオブジェクトおよびフィールドに対するすべての接続を表示します。 </p>
   <p>WorkfrontまたはExperience Manager Assetsからリンクするオブジェクトに対する表示以上の権限。 </p>
   <p>システム管理者は、自分が作成したものでないものも含めて、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューに計画エリアを含むレイアウトテンプレートを割り当てる必要があります </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

<!--OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>To connect Adobe Workfront Planning records with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace to connect records </p>  
   <p>View or higher permissions to a workspace to view all connections to objects and fields from other applications, regardless of your access in the other application. </p>
   <p>View or higher permissions to the objects you want to link from Workfront or Experience Manager Assets. </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++

## レコードを接続するための前提条件

レコードを他のレコードまたはオブジェクトと接続するには、次の条件を満たす必要があります。

* 少なくとも 1 つのワークスペース、レコードタイプおよびレコード。

  詳しくは、次の記事を参照してください。

   * [ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)
   * [レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)
   * [レコードの作成](/help/quicksilver/planning/records/create-records.md)

* レコードタイプ間の接続や、レコードタイプと他のアプリケーションからのオブジェクト間の接続。詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

## Workfront Planning からレコードを接続

計画レコードの次の領域で、Workfront Planning のレコードを関連付けることができます。

* テーブル表示の接続されたレコードフィールド
* 「詳細」タブの、接続されたレコードフィールドでのレコードのプレビューまたはページ。
* [ 接続 ] タブのレコードのプレビューまたはページ。

### テーブルビューまたはレコードページの「詳細」タブから、Adobe Workfront Planning レコードを接続します

{{step1-to-planning}}

1. レコードを接続するワークスペースをクリックします

   ワークスペースが開き、レコードタイプがカードとして表示されます。
1. レコードタイプのカードをクリックして、レコードタイプのページを開きます。
1. **テーブル** ビューの名前をクリックして開きます。
1. （オプション）テーブルに新しい行を追加して、選択したレコードタイプにレコードを追加します。詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
1. （条件付き）選択したレコードタイプを別のレコードタイプに接続した後、リンクされたレコード列に移動し、他のレコードとリンクするレコードに対応するセルをダブルクリックします。

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. 次のいずれかの操作を行います。

   * リストから接続されているレコードの名前をクリックして、選択したレコードに追加します。レコードは自動的に追加されます。
   * レコードの名前の入力を開始し、リストに名前が表示されたら選択します。レコードは自動的に追加されます。

1. （オプション）接続するレコードまたはオブジェクトが見つからず、追加する場合は、「**+追加**」をクリックして新しいレコードを追加します。 詳細については、「レコードの作成 [ の「接続時にレコードを作成する」を参照してくだ ](/help/quicksilver/planning/records/create-records.md) い。

   >[!TIP]
   >
   >    テーブル ビューで次の操作を行って、レコードのページを開くことができます。
   >1. ビューでレコードの名前をクリックします。
   >1. リンクされたレコードフィールドを見つけ、フィールドをダブルクリックします（既に接続されているレコードがある場合）
   >または
   >**レコードを接続** （フィールドが空の場合）をクリックして、接続されたレコードまたはオブジェクトタイプからレコードを追加します。
   >
   >![](assets/connect-records-from-record-page-field.png)

1. （任意）すべてのレコードを表示するには、「**すべて表示**」をクリックします。

1. （条件付き）前の手順で「**すべて表示**」をクリックした場合、「**オブジェクトを接続**」ボックスが表示されます。

   ![](assets/connected-objects-table-for-records.png)

1. 検索ボックスにレコード名を入力していき、リストに表示されたら選択します

   または

   ボックス内の 1 つまたは複数のレコードの名前を選択し、[**オブジェクトを接続**] をクリックします。

   以下が追加されます。

   * リンクされたレコードは、前の手順で選択したレコードの「リンクされたレコード」フィールドに表示されます。
   * レコードタイプを接続したときにリンクされたルックアップフィールドを追加した場合、リンクされたフィールドには、リンクされたレコードからの情報が入力されます。

   リンクされたレコードを更新すると、リンク元のレコードのリンクされたフィールドも自動的に更新されます。リンクされたフィールドは手動で編集できません。

   >[!TIP]
   >
   >* 「リンクされたフィールド」と「ルックアップフィールド」は同じ意味で使用されます。
   >
   >* レコードタイプを接続したときに複数のレコードを接続するように選択した場合、複数のオブジェクトからのフィールド値は、コンマで区切って表示されるか、レコードタイプの接続時に選択した集計に従って集計されます。

1. （オプション）レコードタイプページを閉じて、選択したワークスペースに移動します。
1. リンク先のレコードタイプのカードをクリックします。

   例えば、**キャンペーン**&#x200B;レコードを製品レコードに接続した場合は、**製品**&#x200B;カードをクリックします。

   レコードタイプカードがテーブル表示で開きます。 そうでない場合は、テーブルビューを選択します。

   **キャンペーン**&#x200B;にリンクされたレコードフィールドには、製品レコードタイプのページで製品にリンクしたキャンペーンの名前が表示されます。キャンペーン情報を更新すると、製品レコードタイプのキャンペーンにリンクされたレコードフィールドが自動的に更新されます。

### テーブル表示またはレコードページの「詳細」タブから、Adobe Workfrontの計画レコードをWorkfront オブジェクトに接続します

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

レコードタイプと Workfront オブジェクトタイプの間の接続を作成した後、個別のレコードを Workfront オブジェクトに接続できます。接続した Workfront フィールドは、オブジェクトのリンク元のレコードに自動的に入力されます。

>[!NOTE]
>
>Workfront オブジェクトタイプをWorkfrontのWorkfront Planning レコードタイプに関連付けることはできません。


{{step1-to-planning}}

1. レコードを接続するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。
1. レコードタイプのカードをクリックして、レコードタイプページを開きます。
1. **ビュー**&#x200B;ドロップダウンメニューから&#x200B;**テーブル**&#x200B;ビューを選択します。

1. 「**新規レコード**」をクリックして、選択したレコードタイプに個別のレコードを追加します。詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

1. （条件付き）選択したレコードタイプを Workfront オブジェクトタイプに接続した後、リンクされたオブジェクト列に移動し、Workfront のオブジェクトにリンクするレコードに対応するセルをダブルクリックします。

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. 次のいずれかの操作を行います。

   * リストからオブジェクトをクリックして、選択したレコードに追加します。オブジェクトはアルファベット順にリストされます。オブジェクトは自動的に追加されます。
   * オブジェクトの名前の入力を開始し、リストに名前が表示されたらクリックします。オブジェクトは自動的に追加されます。

   >[!TIP]
   >
   >ビューからレコードのページを開き、リンクされたレコードフィールドをダブルクリックするか、フィールドの **接続** をクリックして、接続されたオブジェクトタイプからオブジェクトを追加できます。

1. （オプション）接続するオブジェクトが見つからず、追加する場合は、「**+追加」をクリックして** 新しいプロジェクトまたはポートフォリオを作成して追加します。

   プロジェクトを計画レコードに接続する際に追加できるのは、テンプレートまたはポートフォリオを持たないプロジェクトのみです。 新しいプログラム、ユーザー、または会社を追加することはできません。

1. （オプション）「**すべて表示**」をクリックすると、少なくとも表示権限を持つすべてのオブジェクトが表示されます。

1. （条件付き）前の手順で「**すべて表示**」をクリックした場合、「**オブジェクトを接続**」ボックスが表示されます。

   ![](assets/connect-objects-box-to-select-projects.png)

1. 検索ボックスに Workfront オブジェクトの名前の入力を開始し、リストに名前が表示されたら選択します。

   または

   ボックス内の 1 つまたは複数のオブジェクトの名前を選択し、**オブジェクトを接続** をクリックします。

   >[!IMPORTANT]
   >
   >* 表示のアクセス権限のある Workfront オブジェクトのみを追加できます。
   >
   >* Workfront オブジェクトを追加すると、ワークスペースに対する表示権限以上の権限を持つすべてのユーザーは、Workfront での権限やアクセス権に関係なく、Workfront オブジェクトとそのフィールド情報を表示できるようになります。

   次のものが追加されます。

   * 選択した Workfront オブジェクトが、リンクされたレコードフィールドに追加されます。
   * レコードタイプを Workfront に接続するときにこれらを追加した場合、Workfront オブジェクトのリンクされたフィールド（またはルックアップフィールド）には、Workfront からの情報が自動的に入力されます。

   レコードタイプと別のアプリケーションのオブジェクトの接続について詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

1. （オプション）テーブルビューのリンクされたフィールド、またはレコードページのリンクされたフィールドで、Workfront Planning レコードに接続されている Workfront オブジェクトの名前をクリックします。

   少なくともオブジェクトに対する表示権限がある場合、これによりWorkfrontにWorkfront オブジェクトが開きます。

   >[!TIP]
   >
   >* レコードタイプを接続するときに複数のレコードを接続することを選択した場合、ルックアップフィールドの値は、コンマで区切って表示されるか、選択したアグリゲータに従って集計されます。
   >
   >* Workfront のリンクされた Workfront オブジェクトに対して、リンクされたレコードフィールドは作成されません。

1. （オプション）レコードタイプのテーブルビューで、リンクされた Workfront オブジェクトの列ヘッダーにポインタを合わせ、ドロップダウンメニューをクリックして、「**ルックアップフィールドを編集**」をクリックします。

1. **選択されていないフィールド**&#x200B;エリアから Workfront オブジェクトフィールドを追加します。

   または

   **選択されたフィールド**&#x200B;エリアから、Workfront オブジェクトフィールドを削除します。

   これにより、リンクされたフィールドが Workfront Planning レコードに追加または削除されます。削除されたフィールドに関連付けられた情報は Workfront に残ります。


### テーブル表示またはレコードページの「詳細」タブから、Workfrontの計画レコードをAdobe Experience Manager オブジェクトに接続します

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>Workfront Planning レコードを Adobe Experience Manager Assets に接続するには、Adobe Experience Manager Assets ライセンスが必要であり、組織の Workfront インスタンスが Adobe Business Platform または Adobe Admin Console にオンボーディングされている必要があります。
>
>Adobe Admin Console のオンボーディングについて質問がある場合は、[Adobe Unified Experience の FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md) を参照してください。

レコードタイプと Adobe Experience Manager Assets 間の接続を作成した後、個別のレコードを Experience Manager Assets に接続できます。接続の作成時に Experience Manager Assets から接続したアセットフィールドは、リンク元のレコードタイプで自動的に入力されます。

>[!NOTE]
>
>Planning レコードとそのフィールドには、Experience Manager AssetsとAdobe Experience Manager Assets間の統合を通じてWorkfront管理者がメタデータ・マッピングを構成する際に、Workfrontからアクセスできます。 詳しくは、[Adobe WorkfrontとExperience Manager Assets間のアセットメタデータのマッピングの設定 ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=ja) を参照してください。

レコードをAEM assets に接続するには：

{{step1-to-planning}}

1. レコードを接続するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプが表示されます。
1. レコードタイプのカードをクリックして、レコードタイプのページを開きます。
1. レコードタイプページの右上隅にある&#x200B;**ビュー**&#x200B;ドロップダウンメニューから、**テーブル**&#x200B;ビューを選択します。

1. （オプション）「**新規レコード**」をクリックして、選択したレコードタイプに新規レコードを追加します。詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
1. （条件付き）選択したレコードタイプを Experience Manager Assets に接続した後、リンクされたオブジェクト列に移動し、Experience Manager の他のオブジェクトとリンクするレコードに対応するセルにポインタを合わせて、**+** アイコンをクリックします。

   >[!TIP]
   >
   >  レコードページのリンクされたオブジェクトフィールドにある **+** アイコンをクリックして、アセットをレコードに接続できます。

   「**アセットを選択**」ボックスが表示されます。<!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. 次のタイプのアセットのいくつかをクリックして選択します。

   * 画像
   * フォルダー

   複数のアセットを選択できます。

   >[!IMPORTANT]
   >
   > 接続できるのは、Experience Manager で表示するアクセス権のあるアセットのみです。接続すると、すべての Workfront Planning ユーザーは、Experience Manager Assets へのアクセス権に関係なく、Workfront Planning でアセットを表示できます。

1. 「**選択**」をクリックします。<!-- we might change this to Connect-->

   次のものが追加されます。

   * 選択した Experience Manager Assets が、リンクされたレコードフィールドに追加されます。
   * リンクされたフィールド（またはルックアップフィールド）には、Experience Manager に接続されたアセットからの情報が入力されます。

     Experience Manager Assets のフィールドからのすべての既存の情報は、リンクされたフィールドまたはルックアップフィールドに自動的に表示されます。

     >[!TIP]
     >
     >* レコードタイプを接続するときに複数のレコードを接続することを選択した場合、複数のオブジェクトの値がコンマで区切られているか、選択したアグリゲータに従って集計されて表示されます。
     >
     >* Workfront Planning にリンクされたレコードへのリンクされたレコードフィールドは、Experience Manager Assets アプリケーションのリンクされた Experience Manager アセットに対しては作成されません。

1. （オプション）Experience Manager Assets にリンクしたレコードタイプに移動し、リンクされたレコードフィールド内のアセットの名前をクリックします。Experience Managerのアセット詳細がポップアップウィンドウに表示されます。

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   画像ファイルには、次のフィールドが表示されます。

   * 画像のサムネール
   * 画像ファイル名
   * 寸法
   * サイズ
   * 説明
   * Experience Manager のファイルパス
   * アセットタイプ
   * 作成日
   * 変更日時

1. （オプション）Experience ManagerアセットのレコードページをExperience Managerで開くには、リンク元のレコードのレコードタイプページに移動し、「リンクされたレコード」フィールドでアセットの名前をクリックしてポップアップウィンドウを開き、「**AEMで開く**」アイコンをクリックしてアセットを開き ![](assets/open-asset-icon.png) す。

   これにより、Adobe Experience Manager Assets で Experience Manager のアセットが開きます。

1. （オプション）レコードタイプのテーブルビューで、リンクされた Experience Manager のアセットの列ヘッダーにポインタを合わせ、ドロップダウンメニューをクリックし、「**ルックアップフィールドを編集**」を選択します。

1. **選択されていないフィールド**&#x200B;エリアから、Experience Manager Assets オブジェクトフィールドを追加します。

   または

   **選択されたフィールド**&#x200B;エリアから、Workfront オブジェクトフィールドを削除します。

   これにより、リンクされたフィールドがレコードに追加または削除されます。削除されたフィールドに関連付けられた情報は、Adobe Experience Assets に残ります。

### レコードページの「接続」タブから、Workfront Planning レコードと他のレコードまたはオブジェクトを接続します

1. 他の Planning レコード・タイプまたは他のアプリケーションのオブジェクト・タイプに接続されているレコード・タイプの任意のビューに移動します。
1. 他のレコードまたはオブジェクトと接続するレコードをビューで検索するには、前のサブセクションで説明した手順に従います。
1. レコードの名前をクリックします。

   プレビューページが開きます。
1. （オプション） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) をクリックして、レコードのページを開きます。
1. レコードのプレビューまたはページで、「**接続**」タブをクリックします。

   ![](assets/connections-tab-on-record-in-workfront-planning.png)

   選択したレコードタイプにリンクされているすべてのレコードタイプまたはオブジェクトタイプがセクションとして表示されます。 接続されたレコードまたはオブジェクトは、カード上のレコードまたはオブジェクトタイプの名前の下に表示されます。

   >[!TIP]
   >
   >    デフォルトでは、個々のレコードが接続されている接続レコードのみが表示されます。

1. （省略可能） [**すべての接続を表示**] をクリックすると、接続されたすべてのレコードの種類（接続されていないレコードを含む）が表示されます。

1. （オプション）セクションを折りたたむには、セクションの左側にある下向き矢印をクリックします。

1. （条件付き）同じタイプのレコードまたはオブジェクトをさらに追加するには、「**接続**」をクリックします。
1. 前の節で説明した手順に従って、Workfront Planning のレコードまたはWorkfrontやExperience Manager Assetsのオブジェクトを接続します。
レコードとオブジェクトが直ちに追加されます。
1. （オプション）レコードまたはオブジェクトの接続されたカードにポインタを合わせ、「**レコードを切断**」アイコンを **-** でクリックして、選択したレコードから切断します。

   ![](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

   レコードは、Workfront Planning のすべての領域、または接続済みと表示される可能性のある他のアプリケーションから直ちに切断されます。 参照フィールドの値も削除されます。

## Workfront オブジェクトからのレコードの接続

Workfront オブジェクトからWorkfront計画レコードを接続するには、次のものが必要です。

* Workfront Planning で確立されたレコード・タイプとWorkfrontオブジェクト・タイプ間の関連付け。
* Workfront管理者またはグループ管理者が、Planning セクションをレイアウトテンプレートのWorkfront プロジェクト、ポートフォリオおよびプログラムに追加する必要があります。

詳しくは、[Adobe Workfront オブジェクトの計画セクションでのレコードの管理 ](/help/quicksilver/planning/records/manage-records-in-planning-section.md) を参照してください。
