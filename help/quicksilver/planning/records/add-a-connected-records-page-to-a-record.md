---
title: レコードへの接続レコードページの追加
description: 接続されたレコード ページのタブをレコードに追加することで、接続されたレコードまたはオブジェクトからの情報を表示できます。 これにより、テーブルビュー内の接続されたレコードがタブに追加されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5e0be9d9-efa5-4b16-bd56-f9c85bc57ced
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: a6f2c9eda2045093c8d77243ed6843a1472d36c6
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 4%

---

# レコードへの接続されたレコードページの追加

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Adobe Workfront Planningのレコードに接続レコードページのタブを追加することで、接続されたレコードまたはオブジェクトからの情報を表示できます。 これにより、テーブルビュー内の接続されたレコードがタブに追加されます。

接続されたレコードページをレコードに追加する場合は、次の点を考慮してください。

* レコードまたはオブジェクトタイプをテーブルビューからレコードタイプに接続した後、接続レコードページをレコードに追加できます。

* レコードのプレビュー領域またはレコードのページから、接続されたレコードページを追加できます。

* 特定のレコードタイプに対して接続されたレコードページは1つだけです。

  例えば、キャンペーンに接続されたレコードページを作成し、その接続されたペルソナを表示する場合、ペルソナに対して1つの接続されたレコードページのみを持つことができます。

* 接続されたレコードページには、接続されたオブジェクトまたは1つのオブジェクトまたはレコードタイプのレコードのみが表示されます。 このページには、そのタイプのすべてのレコードが表示されるわけではありません。

* 接続されたレコード ページに表示するオブジェクトまたはレコードタイプに応じて、次のビューを使用して表示できます。

   * 接続されたPlanning レコードは、次のタイプのビューで表示できます。
      * テーブル
      * タイムライン
      * カレンダー
   * 接続されたWorkfront プロジェクトは、リストビューで表示できます。

* 次の接続レコードまたはオブジェクトタイプに対して、接続レコードページを追加できます。

   * Workfront計画のレコードタイプ
   * Workfront プロジェクト

     Workfrontでアクセスするための権限がない場合でも、接続されたWorkfront プロジェクトを表示できます。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontおよびプランニングパッケージ</p>
<p>任意のワークフローとプランニングパッケージ</p>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p> 
   </td> 
<tr>
<td> 
   <p> その他の製品</p> </td> 
   <td> 
   <p> 次のアプリケーションからオブジェクトの接続レコードページを追加する場合は、Adobe Workfrontに加えて、次の機能が必要です。</p>
   <ul><li><p>Adobe Experience Manager ライセンスと、Adobe Experience ManagerとWorkfront間の統合により、AEM オブジェクトをプランニングレコードタイプに接続できます。</p>
   <p>詳しくは、<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Experience Manager AssetsおよびAssets Essentials向けAdobe Workfront：記事インデックス </a>を参照してください。 </p></li>
   <li><p> レコードタイプとGenStudio Brandsを連携させるAdobe GenStudio for Performance Marketingライセンス</p>
   <p>詳しくは、<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketingの基本を学ぶ</a>を参照してください。</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <p>ワークスペースおよびレコードタイプに対する権限の貢献度を上げます </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> 
  </td>
  </tr>   
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++   

## レコードへの接続されたレコードページの追加

最初に、接続されたレコードページをレコードに追加する前に、レコードタイプを他のレコードタイプまたはWorkfront プロジェクトに接続する必要があります。

1. レコードの名前をクリックして、レコードタイプページの任意のビューからレコードを開きます。
1. 次のいずれかの領域から「**ページを追加**」をクリックします。

   * レコードのプレビューウィンドウ
   * プレビューページの右上隅にある&#x200B;**新しいタブで開く** アイコン ![新しいタブアイコンで詳細を開く](assets/open-details-in-a-new-tab-icon.png)をクリックした後、レコードの詳細ページ。

   「**ページを作成**」ボックスが開きます。

   ![接続レコードの追加ページモーダル ](assets/add-connection-view-page-modal.png)

1. **ページ名**&#x200B;を追加し、**ページタイプ**&#x200B;の&#x200B;**接続レコードページ**&#x200B;をクリックしてから、**作成**&#x200B;をクリックします。
1. （オプション）リスト内の接続されたレコードまたはオブジェクトタイプの名前をクリックするか、検索し、リストに表示されたときにクリックして、そのレコードまたはオブジェクトタイプのページを作成します。

   >[!TIP]
   >
   >レコードタイプごとに1つの接続レコードページを作成できます。 接続されたレコードタイプに既にページがある場合、そのレコードタイプはオプションとして表示されなくなります。
   >

1. （オプションおよび条件付き）表示用のページを作成するレコードまたはオブジェクトタイプの複数の接続フィールドの場合は、**参照フィールドを選択** リストから、接続されたレコードページに表示するレコードまたはオブジェクトのフィールドをクリックします。

   ![参照フィールドリストを選択](assets/select-reference-field-list-on-connected-records-page.png)

   次のいずれかのページが、接続されたレコード ページに追加されます。

   * レコードタイプのテーブルビュー
   * プロジェクトオブジェクトタイプのリストビュー

   現在のレコードに接続されているレコードまたはプロジェクトは、テーブルまたはリストビューに表示されます。

   >[!TIP]
   >
   >接続されたレコード ページに表示する前に、レコードのテーブルまたは詳細領域に接続されたレコードを追加する必要があります。 それ以外の場合、テーブルまたはリストは空です。

   接続されたレコードの最初の5つのフィールドは、デフォルトで表示されます。 デフォルトではルックアップフィールドは表示されません。

   ![ キャンペーンの詳細の下のオーディエンス接続テーブルビュー](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （条件付き）接続されたレコードページに表示するレコードのタイプに応じて、次のいずれかの操作を行います。

   * プランニングレコードの管理
詳しくは、この記事の「[ プランニングレコードの接続レコードの管理](#manage-the-connected-records-page-for-planning-records)」の節を参照してください。
   * Workfront プロジェクトの管理
詳しくは、この記事の「[Workfront プロジェクトの接続されたレコードの管理](#manage-the-connected-records-page-for-workfront-projects)」の節を参照してください。

1. （オプション）「**接続されたレコード」ページ**」タブの名前をダブルクリックします

   または

   タブの名前にカーソルを合わせ、**詳細** ![詳細メニュー](assets/more-menu.png)をクリックし、**名前変更**&#x200B;をクリックして、新しい接続されたレコードページのタブに名前変更します。

1. （オプション）接続されたレコードページの名前にカーソルを合わせ、**詳細** ![詳細メニュー](assets/more-menu.png)をクリックし、**削除**&#x200B;をクリックしてタブを削除します。

### プランニングレコードの接続レコードページの管理

<!--

#### Manage the connected records page for Planning records in the Production environment

When you create a connected records page for  connected Planning records in the Production environment, do the following: (****or AEM Assets - AEM is not available yet?? see note below********)

1. Go to a record type page and click the name of a record. This opens the record's preview page.
1. Click the tab for a connected records page that display Planning records.
   The records connected to the record you selected display in the table view. 
1. Click **Connect** at the bottom of the table view to connect existing records, select them from the connection box, then click outside the box to close it. The records are automatically added to the table and connected to the record you selected. The records must exist before you can add them.

   For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).

1. Edit any information from the connected records inline in the table view. 
1. Hover over a connected record's name, then click the **More** menu ![More menu](assets/more-menu.png)

   Or 
   
   Select one of the records, then click one of the following options in the blue bar at the bottom of the list: 

   * **View** to open the record page in a new tab
   * **Copy link** to copy a link to the record page
   * **Edit thumbnail** to open the **Record thumbnail** box and edit the record's thumbnail image
   * **Duplicate** to duplicate the connected record. The duplicated record is also connected to the current record.
   * **Insert record above or below** to add new records to the connected record type. New records added here are also connected to the current record. This option is not available in the blue bar when selecting a record in the table.
   * **Delete** to delete the record. Deleting a connected record deletes it from its record type and from everywhere where the record is connected. The deleted records move to the **Recently deleted** bin of their record type.

      For information about editing records in the table view, see [Edit records](/help/quicksilver/planning/records/edit-records.md). 

      >[!TIP]
      >
      >You can select more than one record or object to delete them.
      >

1. Inline edit any of the records in the table on the connected records page.
1. Use any of the following view elements in the toolbar of a connected record page to manage the table view:

   * **Filters**
   * **Sort**
   * **Grouping**
   * **Fields**, to display, hide, or rearrange fields
   * **Row height**
   * **Search**

   For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 

   >[!NOTE]
   >
   >You cannot create, edit, or delete fields in the table view of a connected record's tab.
   >

#### Manage the connected records page for Planning records in the Preview environment

When you create a connected records page for connected Planning records in the Preview environment, do the following: (***********or AEM Assets -- AEM is not available yet?? see note below**********)

-->

1. レコードタイプページに移動し、レコードの名前をクリックします。 これにより、レコードのプレビューページが開きます。
1. プランニングレコードを表示する接続レコードページのタブをクリックします。
選択したレコードに接続されたレコードがテーブルビューに表示されます。
1. 接続されたレコードページの右上隅にある「**レコードを接続**」をクリックして、既存のレコードを接続し、接続ボックスから選択してから、ボックスの外側をクリックして閉じます。 レコードは自動的にテーブルに追加され、選択したレコードに接続されます。 レコードを追加する前に、レコードが存在している必要があります。

   詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

1. テーブルの下部にある&#x200B;**新しい行**&#x200B;をクリックして、新しいレコードを追加します。 新しいレコードは、選択したレコードに自動的に接続されます。
1. テーブルビューで、接続されたレコードの情報をインラインで編集します。
1. 接続されたレコードの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックします

   または

   レコードのいずれかを選択し、リストの下部にある青いバーで次のいずれかのオプションをクリックします。

   * **表示**&#x200B;して、新しいタブでレコード ページを開く
   * **リンクをコピー**&#x200B;して、レコードページにリンクをコピーします
   * **サムネール**&#x200B;を編集して&#x200B;**サムネールを記録** ボックスを開き、レコードのサムネール画像を編集します
   * **複製**&#x200B;して、接続されたレコードを複製します。 複製されたレコードは、現在のレコードにも接続されます。
   * **接続されたレコードタイプに新しいレコードを追加するには、**&#x200B;の上下にレコードを挿入します。 ここに追加された新しいレコードも、現在のレコードに接続されます。 このオプションは、テーブル内のレコードを選択する際に、青いバーでは使用できません。
   * **削除**&#x200B;してレコードを削除します。 接続されたレコードを削除すると、そのレコードのタイプと、レコードが接続されているすべての場所から削除されます。 削除されたレコードは、レコードタイプの&#x200B;**最近削除された** ビンに移動します。

     テーブルビューでのレコードの編集について詳しくは、[ レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

     >[!TIP]
     >
     >複数のレコードまたはオブジェクトを選択して削除できます。

1. 接続されたレコードページのテーブル内の任意のレコードをインラインで編集します。
1. 接続されたレコードページのツールバーで次のいずれかのビュー要素を使用して、テーブルビューを管理します。

   * **フィルター**
   * **並べ替え**
   * **グループ化**
   * フィールドを表示、非表示、または並べ替える&#x200B;**フィールド**
   * **行の高さ**
   * **検索**

   詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

   >[!NOTE]
   >
   >接続されたレコードのタブのテーブルビューでは、フィールドを作成、編集または削除できません。
   >

1. 接続されたレコードページの右上隅にある「ビュー」ドロップダウンメニューをクリックし、**新しいビュー**&#x200B;をクリックして、ページの新しいビューを追加してから、次の操作を行います。

   1. **ビュー名**&#x200B;を追加します。
   1. **表示タイプ**&#x200B;領域から、次のいずれかのタイプのビューを選択します。

      * テーブル
詳しくは、[ テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください
      * タイムライン
詳しくは、[ タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)を参照してください。
      * カレンダー
詳しくは、[ カレンダービューの管理](/help/quicksilver/planning/views/manage-the-calendar-view.md)を参照してください。

        詳しくは、この記事の「[接続されたレコードの複数のビューを管理する](#manage-multiple-views-from-the-connected-records-page)」の節を参照してください。

   1. 「**作成**」をクリックします。
ビューのドロップダウンメニューに新しいビューが追加されます。

   1. （オプション）作成したビューの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、次のいずれかのオプションをクリックします。

      * **ビューの新しい名前を追加するには、**&#x200B;の名前を変更します。
      * **共有**

        詳しくは、[ビューの共有](/help/quicksilver/planning/access/share-views.md)を参照してください。
      * **書き出し**

      * **削除**
詳しくは、[ レコードビューの削除](/help/quicksilver/planning/views/delete-record-views.md)を参照してください。

        ![ プロジェクト接続レコードページのその他のメニューを表示](assets/view-more-menu-projects-connected-records-page.png)

        >[!NOTE]
        >
        >Workfrontで作成したシステムビューは削除できません。

### Workfront プロジェクトの「接続されたレコード」ページの管理

接続されたWorkfront プロジェクト用に接続されたレコードページを作成する場合は、次の手順に従ってページを管理します。

1. レコードタイプページに移動し、レコードの名前をクリックします。 これにより、レコードのプレビューページが開きます。
1. Workfront プロジェクトを表示する接続レコードページのタブをクリックします。

   ![ プロジェクトがレコードを接続しました](assets/projects-connected-records-page-table.png)

   選択したレコードに接続されたプロジェクトがリストビューに表示されます。

   リスト表示でのオブジェクトの管理または編集について詳しくは、[ リスト表示の管理](/help/quicksilver/planning/views/manage-the-list-view.md)を参照してください。

<!-- 
removed this part, so we won't have to have duplicate information to keep up with for the list view in Planning: 
1. Click **Connect records** in the upper-right corner of the connected record page to connect existing projects.

   For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
1. Double-click inside a cell in the list view to edit a project's fields. Some fields are read-only. 
1. Do one of the following to edit the list view: 

   * Click **New row** to create a project without a template. The new project is automatically connected to the current record.

      For more information, see [Create Workfront objects from Workfront Planning as you connect them to records](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md).
   * Click **Create records **in the upper-right corner of the view to add existing projects. Projects are immediately connected to the selected record. 

   * Hover over a project name in the list and click the **More** menu [More menu](assets/more-menu.png) and click **View** to open the project in another tab
     
      Or

      Select one or more projects, and from the actions bar at the bottom of the list, click **Delete** or **Disconnect** to remove the item from the list.
      

   * Click the views dropdown menu, and click **New view** to add a new view for the page, then do the following, or click the **More** menu ![More menu](assets/more-menu.png) to the right of a new name, then **Rename**, **Share**, or **Delete** the view. 

      You cannot rename, share or delete System Views or views you do not have Manage permissions to.

      ![View more menu on Projects Connected records page](assets/view-more-menu-projects-connected-records-page.png)

   * Click one of the following to update the view's elements: 

      * **Filter** to limit the amount of information in the list
      * **Columns** to hide columns or change their order
      * The **+** icon in the upper-right corner of the table view to add existing fields to the list. Fields must exist before you can add them. 

   For more information about managing objects in a list view, see [Manage the list view](/help/quicksilver/planning/views/manage-the-list-view.md).
-->

<!--
 this is repetitive from an earlier section above: 

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. (Conditional) When displaying Planning records in the connected records page, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: 

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Delete**

   <!--
   not possible right now: * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).
      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types.
      -->


<!--
No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      TIP      
      You can select more than one record or object to disconnect them.
      -->
