---
title: 接続されたレコードページのレコードへの追加
description: 接続されたレコード ページのタブをレコードに追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。 これにより、テーブル表示の接続されたレコードがタブに追加されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '1776'
ht-degree: 5%

---


# 接続されたレコード ページをレコードに追加する

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

Adobe Workfront Planning のレコードに「接続されたレコード」ページのタブを追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。 これにより、テーブル表示の接続されたレコードがタブに追加されます。

「接続済みレコード」ページをレコードに追加する場合は、次の点を考慮してください。

* レコード タイプのテーブル ビューからレコード タイプにレコード タイプまたはオブジェクト タイプを接続した後に、[ 接続されたレコード ] ページをレコードに追加できます。

* レコードのプレビュー領域またはレコードのページから、「接続済みレコード」ページを追加できます。

* 接続されたレコード ページには、1 つのオブジェクトまたはレコード タイプからの接続されたオブジェクトまたはレコードのみが表示されます。 ページには、そのタイプのすべてのレコードが表示されるわけではありません。

* テーブル ビューでは、接続されたレコード ページのオブジェクトを表示できます。

<!--replace the above bullet with this: 

* You can display the objects in a connected records page in the following types of views:

   * Table
   * <span class="preview">Timeline</span>
   * <span class="preview">Calendar</span>

* <span class="preview">You can create one page per one object or record type. For example, you cannot create two connected record pages for connected projects or tactics.</span>

-->

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
   <p>詳しくは、<a href="https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketingの基本を学ぶ </a> を参照してください。</p></li></ul>
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

1. （オプションおよび条件付き）ページを作成するレコード タイプまたはオブジェクト タイプの接続されたフィールドが複数表示される場合は、[ 接続されたレコード ] ページに表示するレコードまたはオブジェクトのフィールドを **参照フィールドを選択** リストからクリックします。

   ![&#x200B; 参照フィールドの選択リスト &#x200B;](assets/select-reference-field-list-on-connected-records-page.png)

   接続されたレコード ページに、次のいずれかのページが追加されます。

   * レコードタイプのテーブル表示
   * プロジェクトオブジェクトタイプのリスト表示

   現在のレコードに接続されているレコードまたはプロジェクトがテーブル表示またはリスト表示に表示されます。

   >[!TIP]
   >
   >接続レコード ページに表示するには、レコードのテーブル領域または詳細領域に接続レコードを追加する必要があります。 それ以外の場合、テーブルまたはリストは空になります。

   接続されたレコードの最初の 5 つのフィールドは、デフォルトで表示されます。<!--No lookup fields display by default.-->

   ![&#x200B; キャンペーンの詳細のオーディエンスに接続されたテーブル表示 &#x200B;](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （条件付き）接続されたレコード ページに表示するレコードの種類に応じて、次のいずれかの操作を行います。

   * レコードのテーブル表示の管理
詳しくは、この記事の [&#x200B; 接続されたレコード ページのレコード テーブル ビューを管理する &#x200B;](#manage-the-record-table-view-in-the-connected-records-page) の節を参照してください。
   * プロジェクトのリスト表示の管理
詳しくは、この記事の「[&#x200B; 接続されたレコードのページでプロジェクトのリスト表示を管理 &#x200B;](#manage-the-project-list-view-in-the-connected-records-page) を参照してください。

1. （オプション）「**接続されたレコード」ページ** タブの名前をダブルクリックします

   または

   タブの名前にポインタを合わせ、**その他** ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**名前を変更** をクリックして、新しく接続されたレコードページタブに名前を変更します。


   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. （オプション）接続されたレコードページのタブの名前にポインタを合わせ、**詳細** ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**削除** をクリックしてタブを削除します。

### 接続されたレコードページでのレコードテーブルビューの管理

接続された Planning レコード用の「接続されたレコード」ページを作成する場合、次の操作を行います。<!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. レコードタイプのページに移動し、レコードの名前をクリックします。 これにより、レコードのプレビューページが開きます。
1. Planning レコードを表示する接続されたレコード・ページのタブをクリックします。
選択したレコードに接続されているレコードがテーブルビューに表示されます。
1. テーブル ビューの下部にある [**接続**] をクリックして既存のレコードを接続し、接続ボックスから選択します。次に、ボックスの外側をクリックして閉じます。 レコードがテーブルに自動的に追加され、選択したレコードに接続されます。 追加するには、レコードが存在している必要があります。

   詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。
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
      >[!TIP]
      >
      >You can select more than one record or object to disconnect them.
      -->

### 接続されたレコードページでのプロジェクトリスト表示の管理

接続されたWorkfront プロジェクトの「接続されたレコード」ページを作成する場合、次の操作を行います。

1. レコードタイプのページに移動し、レコードの名前をクリックします。 これにより、レコードのプレビューページが開きます。
1. Workfront プロジェクトを表示する接続済みレコードページのタブをクリックします。
選択したレコードに接続されているプロジェクトがリスト表示に表示されます。
1. 接続されたレコードページの右上隅にある「**レコードを接続**」をクリックして、既存のプロジェクトを接続します。

   詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
1. テーブル内のインライン編集プロジェクト情報。
1. **新しい行** をクリックして、テンプレートを使用せずにプロジェクトを作成します。 新しいプロジェクトは、現在のレコードに自動的に接続されます。

   詳しくは、[&#x200B; レコードに関連付ける際に、Workfront Planning からWorkfront オブジェクトを作成する &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) を参照してください。
1. リストのプロジェクト名にポインタを合わせて、「**詳細**」メニュー [&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックします。

   または

   1 つ以上のプロジェクトを選択し、リストの下部にある青いバーに注目して、次のいずれかをクリックします。

   * **削除**：プロジェクトを削除します。 プロジェクトを削除すると、レコードから切断され、Workfrontのごみ箱に移動されます。 Workfront管理者は、削除されたプロジェクトを、削除されてから最大 30 日後まで復元できます。
   * **切断**：レコードからプロジェクトを切断します。 プロジェクトの接続を解除すると、プロジェクトとその参照フィールドのすべての値が現在のレコードから削除されます。

   >[!TIP]
   >
   >複数のプロジェクトを選択して切断したり、削除することができます。
1. ビューのドロップダウンメニューをクリックし、**新規ビュー** をクリックしてページの新しいビューを追加するには、次の手順を実行します。
   1. **ビュー名** を追加します。
   1. **ビュータイプ** エリアから **リスト** を選択します。
   1. 「**作成**」をクリックします。
新しいリスト表示が表示ドロップダウンメニューに追加されます。
   1. （オプション）作成したビューの名前にポインタを合わせ、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、次のいずれかのオプションをクリックします。
      * **名前を変更**：ビューに新しい名前を追加します。
      * <span class="preview">**共有**</span>

        詳しくは、[ビューの共有](/help/quicksilver/planning/access/share-views.md)を参照してください。

        >[!NOTE]
        >
        >Workfrontで作成されたデフォルトのビューは共有できません。

      * **削除**
詳しくは、[&#x200B; レコードビューの削除 &#x200B;](/help/quicksilver/planning/views/delete-record-views.md) を参照してください。


        ![](assets/view-more-menu-projects-connected-records-page.png)
   1. **フィルター** アイコン ![&#x200B; フィルターアイコン &#x200B;](assets/filter-icon.png) をクリックし、フィルターを使用して特定のプロジェクトを表示します。

      >[!TIP]
      >
      ><span class="preview">**所有者**、**スポンサー** などの人物タイプのフィールドの場合、ワイルドカードを使用して、ログインしたユーザーがこれらの役割に割り当てられているプロジェクトを表示できます。</span>
      >
      >![&#x200B; プロジェクトに接続されたレコードページのユーザーワイルドカードを使用してフィルター &#x200B;](assets/filter-with-user-wildcard-project-connected-records-page.png)
      >
   1. **列** アイコン ![&#x200B; 列アイコン &#x200B;](assets/columns-icon.png) をクリックして、リストの列の表示と非表示を切り替えます。
   1. テーブルに既存のフィールドを追加するには、テーブル表示の右上隅にある「**+**」アイコンをクリックします。 フィールドは、追加する前に存在する必要があります。

      **列マネージャー** ボックスが開きます。 次の操作を実行します。

      1. 「**利用可能**」列で既存のオブジェクトフィールドを検索し、フィールド名の右側にある **+** をクリックして、「**選択済み**」列に追加します。

         選択したフィールドは、接続されたレコード ページのテーブル ビューに追加されます。
      1. **選択済み** 列のフィールドの右側にある **-** をクリックして、テーブル表示から削除します。
      1. **保存** をクリックして、接続されたレコードページのテーブルビューを保存します。


<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage multiple view types from the connected records page of a record. 

The views you create in the Connected records page of a record type are available everywhere in Workfront Planning where that record type page displays. Views created for the same record type anywhere else in Workfront Planning are also accessible in all connected records pages of that record type. 

To manage multiple views from the connected records page: 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->