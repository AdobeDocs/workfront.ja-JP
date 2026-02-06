---
title: 接続されたレコードページのレコードへの追加
description: 接続されたレコード ページのタブをレコードに追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。 これにより、テーブル表示の接続されたレコードがタブに追加されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5e0be9d9-efa5-4b16-bd56-f9c85bc57ced
source-git-commit: b2f1bbfbbec23a5400552eb0f989e0a0dc58413c
workflow-type: tm+mt
source-wordcount: '1843'
ht-degree: 3%

---

# 接続されたレコード ページをレコードに追加する

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Adobe Workfront Planning のレコードに「接続されたレコード」ページのタブを追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。 これにより、テーブル表示の接続されたレコードがタブに追加されます。

「接続済みレコード」ページをレコードに追加する場合は、次の点を考慮してください。

* テーブル ビューからレコード タイプにレコードまたはオブジェクト タイプを接続した後で、[ 接続済みレコード ] ページをレコードに追加できます。

* レコードのプレビュー領域またはレコードのページから、「接続済みレコード」ページを追加できます。

* 特定のレコードタイプに対して、接続できるレコードページは 1 つだけです。

  例えば、キャンペーンに接続されたレコードページを作成し、その接続されたペルソナを表示したい場合、ペルソナ用に接続されたレコードページを 1 つだけ持つことができます。

* 接続されたレコード ページには、1 つのオブジェクトまたはレコード タイプからの接続されたオブジェクトまたはレコードのみが表示されます。 ページには、そのタイプのすべてのレコードが表示されるわけではありません。

* 接続されたレコード ページに表示するオブジェクトまたはレコードの種類に応じて、次のビューを使用して表示できます。

   * 接続された Planning レコードは、次のタイプのビューで表示できます。
      * テーブル
      * タイムライン
      * カレンダー
   * 接続されたWorkfront プロジェクトはリスト表示で表示できます。

* 以下の接続されたレコードまたはオブジェクト タイプに対して、接続されたレコード ページを追加できます。

   * Workfront計画レコードタイプ
   * Workfront プロジェクト

     Workfrontでアクセスする権限がない場合でも、Connected Workfront プロジェクトを表示できます。

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
<p>任意のWorkfrontと任意の Planning パッケージ</p>
<p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
<tr>
<td> 
   <p> その他の製品</p> </td> 
   <td> 
   <p> 以下のアプリケーションのオブジェクトに接続済みレコードページを追加する場合は、Adobe Workfrontに加えて、以下が必要です。</p>
   <ul><li><p>Adobe Experience Manager Assets ライセンス、およびAEM Assets を Planning レコードタイプと統合するためのAEM AssetsとWorkfrontの統合。</p>
   <p>詳しくは、<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials：記事インデックス </a> を参照してください。 </p></li>
   <li><p> レコードタイプとGenStudio ブランドを接続するためのAdobe GenStudio for Performance Marketing ライセンス</p>
   <p>詳しくは、<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketingの基本を学ぶ </a> を参照してください。</p></li></ul>
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
   <p>ワークスペースおよびレコードタイプへの投稿以上の権限 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> 
  </td>
  </tr>   
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   

## 接続されたレコード ページをレコードに追加する

レコードに接続レコードページを追加する前に、まずレコードタイプを他のレコードタイプまたはWorkfront プロジェクトに接続する必要があります。

1. レコード名をクリックすると、レコードタイプページの任意のビューからレコードが開きます。
1. 次のいずれかの領域で **ページを追加** をクリックします。

   * レコードのプレビューウィンドウ
   * レコードの詳細ページ。プレビューページの右上隅にある **新しいタブで開く** アイコン ![&#x200B; 新しいタブで詳細を開くアイコン &#x200B;](assets/open-details-in-a-new-tab-icon.png) をクリックします。

   **ページを作成** ボックスが開きます。

   ![&#x200B; 接続されたレコードを追加ページモーダル &#x200B;](assets/add-connection-view-page-modal.png)

1. **ページ名** を追加し、**ページタイプ** の **接続されたレコードページ** をクリックして、**作成** をクリックします。
1. （省略可能） リスト内で接続されているレコードまたはオブジェクト タイプの名前をクリックするか、そのレコードまたはオブジェクト タイプを検索し、リストに表示されたらクリックして、そのレコードまたはオブジェクト タイプのページを作成します。

   >[!TIP]
   >
   >レコードタイプごとに、接続されたレコードページを 1 つ作成できます。 接続されたレコードタイプに既にページがある場合、オプションとして表示されなくなります。
   >

1. （オプションおよび条件付き）ページを作成するレコード タイプまたはオブジェクト タイプの接続されたフィールドが複数表示される場合は、[ 接続されたレコード ] ページに表示するレコードまたはオブジェクトのフィールドを **参照フィールドを選択** リストからクリックします。

   ![&#x200B; 参照フィールドの選択リスト &#x200B;](assets/select-reference-field-list-on-connected-records-page.png)

   接続されたレコード ページに、次のいずれかのページが追加されます。

   * レコードタイプのテーブル表示
   * プロジェクトオブジェクトタイプのリスト表示

   現在のレコードに接続されているレコードまたはプロジェクトがテーブル表示またはリスト表示に表示されます。

   >[!TIP]
   >
   >接続レコード ページに表示するには、レコードのテーブル領域または詳細領域に接続レコードを追加する必要があります。 それ以外の場合、テーブルまたはリストは空になります。

   接続されたレコードの最初の 5 つのフィールドは、デフォルトで表示されます。 デフォルトでは、参照フィールドは表示されません。

   ![&#x200B; キャンペーンの詳細のオーディエンスに接続されたテーブル表示 &#x200B;](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （条件付き）接続されたレコード ページに表示するレコードの種類に応じて、次のいずれかの操作を行います。

   * 計画レコードの管理
詳しくは、この記事の [Planning レコードの接続されたレコードの管理ページ &#x200B;](#manage-the-connected-records-page-for-planning-records) の節を参照してください。
   * Workfront プロジェクトの管理
詳しくは、この記事の [Workfront プロジェクトの接続されたレコードのページの管理 &#x200B;](#manage-the-connected-records-page-for-workfront-projects) を参照してください。

1. （オプション）「**接続されたレコード」ページ** タブの名前をダブルクリックします

   または

   タブの名前にポインタを合わせ、**その他** ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**名前を変更** をクリックして、新しく接続されたレコードページタブに名前を変更します。

1. （オプション）接続されたレコードページのタブの名前にポインタを合わせ、**詳細** ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**削除** をクリックしてタブを削除します。

### Planning レコードの接続されたレコード ページの管理

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

1. レコードタイプのページに移動し、レコードの名前をクリックします。 これにより、レコードのプレビューページが開きます。
1. Planning レコードを表示する接続されたレコード・ページのタブをクリックします。
選択したレコードに接続されているレコードがテーブルビューに表示されます。
1. 接続されたレコード ページの右上隅にある [**レコードの接続**] をクリックして既存のレコードを接続し、接続ボックスから選択します。次に、ボックスの外側をクリックして閉じます。 レコードが自動的にテーブルに追加され、選択したレコードに接続されます。 追加するには、レコードが存在している必要があります。

   詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

1. テーブルの下部にある「**新しい行**」をクリックして、新しいレコードを追加します。 新しいレコードは、選択したレコードに自動的に接続されます。
1. テーブル表示で、接続されたレコードからの情報をインラインで編集します。
1. 接続されているレコードの名前にポインタを合わせ、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックします

   または

   レコードの 1 つを選択し、リストの下部にある青いバーで次のいずれかのオプションをクリックします。

   * **表示**：レコードページを新しいタブで開きます
   * **リンクをコピー** レコードページへのリンクをコピーする
   * **サムネールを編集** して「サムネールを記録 **ボックスを開き、レコードのサムネール画像を編集します**
   * **複製**：接続されたレコードを複製します。 複製されたレコードは、現在のレコードにも接続されます。
   * 接続されたレコードタイプに新しいレコードを追加するには、**上または下にレコードを挿入** します。 ここに追加された新しいレコードも、現在のレコードに接続されます。 このオプションは、テーブルでレコードを選択する際に青いバーでは使用できません。
   * **削除**：レコードを削除します。 接続されたレコードを削除すると、そのレコードの種類と、レコードが接続されているすべての場所からレコードが削除されます。 削除されたレコードは、レコードタイプの **最近削除された項目** ビンに移動します。

     テーブルビューでのレコードの編集については、[&#x200B; レコードの編集 &#x200B;](/help/quicksilver/planning/records/edit-records.md) を参照してください。

     >[!TIP]
     >
     >複数のレコードまたはオブジェクトを選択して削除できます。

1. 接続されたレコード ページのテーブル内の任意のレコードをインライン編集します。
1. 接続されたレコードページのツールバーで次のビュー要素のいずれかを使用して、テーブルビューを管理します。

   * **フィルター**
   * **並べ替え**
   * **グループ化**
   * **フィールド**：フィールドの表示、非表示または並べ替えを行います
   * **行の高さ**
   * **検索**

   詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

   >[!NOTE]
   >
   >接続されたレコードのタブのテーブル表示のフィールドを作成、編集、削除することはできません。
   >

1. [ 接続されたレコード ] ページの右上隅にある [ ビュー ] ドロップダウン メニューをクリックし、[**新規ビュー**] をクリックしてページに新しいビューを追加し、次の操作を行います。

   1. **ビュー名** を追加します。
   1. **ビュータイプ** 領域から、次のいずれかのタイプのビューを選択します。

      * テーブル
詳しくは、[&#x200B; テーブル表示の管理 &#x200B;](/help/quicksilver/planning/views/manage-the-table-view.md) を参照してください。
      * タイムライン
詳しくは、[&#x200B; タイムライン表示の管理 &#x200B;](/help/quicksilver/planning/views/manage-the-timeline-view.md) を参照してください。
      * カレンダー
詳しくは、[&#x200B; カレンダー表示の管理 &#x200B;](/help/quicksilver/planning/views/manage-the-calendar-view.md) を参照してください。

        詳しくは、この記事の [&#x200B; 接続されたレコードのページから複数のビューを管理する &#x200B;](#manage-multiple-views-from-the-connected-records-page) の節を参照してください。

   1. 「**作成**」をクリックします。
新しいビューが「ビュー」ドロップダウンメニューに追加されます。

   1. （オプション）作成したビューの名前にポインタを合わせ、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、次のいずれかのオプションをクリックします。

      * **名前を変更**：ビューに新しい名前を追加します。
      * **共有**

        詳しくは、[ビューの共有](/help/quicksilver/planning/access/share-views.md)を参照してください。
      * **書き出し**

      * **削除**
詳しくは、[&#x200B; レコードビューの削除 &#x200B;](/help/quicksilver/planning/views/delete-record-views.md) を参照してください。

        ![&#x200B; プロジェクトの接続されたレコード ページの「詳細を表示」メニュー &#x200B;](assets/view-more-menu-projects-connected-records-page.png)

        >[!NOTE]
        >
        >Workfrontで作成されたシステムビューは削除できません。

### Workfront プロジェクトの「接続されたレコード」ページを管理します

接続されたWorkfront プロジェクトに「接続されたレコード」ページを作成する場合、次の手順を実行してページを管理します。

1. レコードタイプのページに移動し、レコードの名前をクリックします。 これにより、レコードのプレビューページが開きます。
1. Workfront プロジェクトを表示する [ 接続されたレコード ] ページのタブをクリックします。
選択したレコードに接続されているプロジェクトがリスト表示に表示されます。
1. 接続されたレコードページの右上隅にある「**レコードを接続**」をクリックして、既存のプロジェクトを接続します。

   詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
1. リスト表示のセル内をダブルクリックして、プロジェクトのフィールドを編集します。 読み取り専用のフィールドがあります。
1. リスト表示を編集するには、次のいずれかの操作を行います。

   * **新しい行** をクリックして、テンプレートを使用せずにプロジェクトを作成します。 新しいプロジェクトは、現在のレコードに自動的に接続されます。

     詳しくは、[&#x200B; レコードに関連付ける際に、Workfront Planning からWorkfront オブジェクトを作成する &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) を参照してください。
   * 既存のプロジェクトを追加するには、ビューの右上隅にある「**レコードを作成**」をクリックします。 プロジェクトは、選択したレコードに直ちに接続されます。

   * リストのプロジェクト名にポインタを合わせ、**詳細** メニュー [&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**表示** をクリックすると、別のタブでプロジェクトが開きます

     または

     1 つ以上のプロジェクトを選択し、リストの下部にあるアクションバーから **削除** または **切断** をクリックして、リストから項目を削除します。


   * ビューのドロップダウン メニューをクリックし、[**新しいビュー**] をクリックしてページに新しいビューを追加し、次の操作を行うか、または新しい名前の右側にある **詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックして、ビューの **名前を変更**、**共有**、または **削除** をクリックします。

     管理権限のないシステムビューやビューの名前変更、共有、削除はできません。

     ![&#x200B; プロジェクトの接続されたレコード ページの「詳細を表示」メニュー &#x200B;](assets/view-more-menu-projects-connected-records-page.png)

   * 次のいずれかをクリックして、ビューの要素を更新します。

      * **フィルター** でリスト内の情報量を制限
      * **列** 列の非表示や順序の変更
      * テーブル表示の右上隅にある「**+**」アイコンを使用して、既存のフィールドをリストに追加します。 フィールドは、追加する前に存在する必要があります。

   リスト表示でのオブジェクトの管理の詳細については、「[&#x200B; リスト表示の管理 &#x200B;](/help/quicksilver/planning/views/manage-the-list-view.md)」を参照してください。

<!-- this is repetitive from an earlier section above: 

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

   <!--not possible right now: * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).
      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. -->


<!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
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
