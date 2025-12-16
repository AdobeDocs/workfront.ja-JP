---
title: 接続されたレコードページのレコードへの追加
description: 接続されたレコード ページのタブをレコードに追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。 これにより、テーブル表示の接続されたレコードがタブに追加されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '1513'
ht-degree: 4%

---


# 接続されたレコード ページをレコードに追加する

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

接続されたレコード ページのタブをレコードに追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。 これにより、テーブル表示の接続されたレコードがタブに追加されます。

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
-->

* 以下の接続されたレコードまたはオブジェクト タイプに対して、接続されたレコード ページを追加できます。

   * Workfront計画レコードタイプ
   * Workfront プロジェクト、プログラム、ポートフォリオ、グループまたは会社。 Connected Workfront オブジェクトは、Workfrontでアクセスする権限を持っていない場合でも表示できます。

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

レコードの種類を他のレコードまたはオブジェクトの種類に接続してから、レコードの接続ページをレコードに追加する必要があります。

1. レコード名をクリックすると、レコードタイプページの任意のビューからレコードが開きます。
1. 次のいずれかの領域で **ページを追加** をクリックします。

   * レコードのプレビューウィンドウ
   * レコードの詳細ページ。プレビューページの右上隅にある **新しいタブで開く** アイコン ![&#x200B; 新しいタブで詳細を開くアイコン &#x200B;](assets/open-details-in-a-new-tab-icon.png) をクリックします。

   **ページを作成** ボックスが開きます。

   ![&#x200B; 接続されたレコードを追加ページモーダル &#x200B;](assets/add-connection-view-page-modal.png)

1. **ページ名** を追加し、「**接続されたレコードページ**」をクリックしてから、「**作成**」をクリックします。

   新しく接続されたレコードページが、新しいタブとしてレコードのページに追加されます。

   現在のレコードに接続されているレコードがテーブルビューに表示されます。

   >[!TIP]
   >
   >接続レコード ページに表示するには、レコードのテーブル領域または詳細領域に接続レコードを追加する必要があります。

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   接続されたレコードの最初の 5 つのフィールドは、デフォルトで表示されます。<!--No lookup fields display by default.-->

   ![&#x200B; キャンペーンの詳細のオーディエンスに接続されたテーブル表示 &#x200B;](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （オプション）接続されたレコードの名前またはオブジェクト タイプをリスト内でクリックするか、検索してから、リストに表示されたらクリックします。

1. （オプションおよび条件付き）レコードのテーブル ビューまたは詳細ページに表示される複数のフィールドが接続されている場合は、接続されているレコード ページにレコードを表示するフィールドをクリックします。

   選択した接続済みレコードタイプのテーブル表示が、接続済みレコードページに追加されます。

1. （オプションおよび条件付き）接続された Planning レコード用の接続されたレコード・ページを作成する場合は、次のいずれかの操作を行います。<!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * レコードの名前をクリックします。 レコードのページが新しいタブで開きます。
   * テーブル ビューの下部にある [**接続**] をクリックして既存のレコードを接続し、接続ボックスから選択します。次に、ボックスの外側をクリックして閉じます。 レコードがテーブルに自動的に追加されます。 追加するには、レコードが存在している必要があります。

   詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。
   * テーブル表示で、接続されたレコードからの情報をインラインで編集します。

   * 接続されているレコードの名前にポインタを合わせ、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックします

     または

     レコードの 1 つを選択し、リストの下部にある青いバーで次のいずれかのオプションをクリックします。

      * **表示**：レコードページを新しいタブで開きます
      * **リンクをコピー** レコードページへのリンクをコピーする
      * **サムネールを編集** して「サムネールを記録 **ボックスを開き、レコードのサムネール画像を編集します**
      * **複製**：接続されたレコードを複製します。 複製されたレコードは、現在のレコードにも接続されます。
      * 接続されたレコードタイプに新しいレコードを追加するには、**上または下にレコードを挿入** します。 ここに追加された新しいレコードも、現在のレコードに接続されます。 このオプションは、テーブルでレコードを選択する際に青いバーでは使用できません。
      * **削除**：レコードを削除します。 接続されたレコードを削除すると、そのレコードの種類と、レコードが接続されているすべての場所からレコードが削除されます。

        テーブルビューでのレコードの編集については、[&#x200B; レコードの編集 &#x200B;](/help/quicksilver/planning/records/edit-records.md) を参照してください。

        >[!TIP]
        >
        >複数のレコードまたはオブジェクトを選択して削除できます。

   * 接続されたレコード ページのテーブル内の任意の Planning レコードをインライン編集します。

1. （オプションおよび条件付き）以下のWorkfront オブジェクトタイプの接続されたレコードページを作成する場合：

   * ポートフォリオ
   * プログラム
   * グループ
   * 会社

   接続されたレコードページのテーブル表示で、次のいずれかの操作を行います。

   * オブジェクトの名前をクリックします。 オブジェクトのページが新しいタブで開きます。
   * テーブル ビューの下部にある [**接続**] をクリックして既存のオブジェクトを接続し、接続ボックスからオブジェクトを選択します。次に、ボックスの外側をクリックしてオブジェクトを閉じます。 オブジェクトがテーブルに自動的に追加されます。 オブジェクトは、追加する前に存在する必要があります。

   詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

   * テーブル表示でオブジェクトの 1 つを選択し、リストの下部にある青いバーで次のいずれかのオプションをクリックします。

   * **表示**：レコードページを新しいタブで開きます
   * **リンクをコピー** レコードページへのリンクをコピーする
   * **接続解除**：表示しているレコードからオブジェクトを接続解除します。

   >[!TIP]
   >
   >複数のレコードまたはオブジェクトを選択して切断できます。

1. （オプションおよび条件付き）接続されたWorkfront プロジェクト用に接続されたレコードページを作成する場合：

   * 接続されたレコードページの右上隅にある「**レコードを接続**」をクリックして、既存のプロジェクトを接続します。

   詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
   * テーブル内のインライン編集プロジェクト情報。
   * **新しい行** をクリックして、テンプレートを使用せずにプロジェクトを作成します。 新しいプロジェクトは、現在のレコードにすぐに接続されます。

     詳しくは、[&#x200B; レコードに関連付ける際に、Workfront Planning からWorkfront オブジェクトを作成する &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) を参照してください。
   * プロジェクトの上にマウスポインターを置き、**詳細** メニュー [&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてください

     または

     1 つ以上のプロジェクトを選択し、リストの下部にある青いバーに注目して、次のいずれかをクリックします。

      * **削除**：プロジェクトを削除します。 プロジェクトを削除すると、レコードから切断され、Workfrontのごみ箱に移動されます。
      * **切断**：レコードからプロジェクトを切断します。 プロジェクトの接続を解除すると、プロジェクトとその参照フィールドのすべての値が現在のレコードから削除されます。

     >[!TIP]
     >
     >複数のプロジェクトを選択して切断したり、削除することができます。
   * テーブルに既存のフィールドを追加するには、テーブル表示の右上隅にある「**+**」アイコンをクリックします。 フィールドは、追加する前に存在する必要があります。

     **列マネージャー** ボックスが開きます。 次の操作を実行します。

      1. 「**利用可能**」列で既存のオブジェクトフィールドを検索し、フィールド名の右側にある **+** をクリックして、「**選択済み**」列に追加します。

         選択したフィールドは、接続されたレコード ページのテーブル ビューに追加されます。
      1. **選択済み** 列のフィールドの右側にある **-** をクリックして、テーブル表示から削除します。
      1. **保存** をクリックして、接続されたレコードページのテーブルビューを保存します。

1. （オプション）「**接続されたレコード」ページ** タブの名前をダブルクリックします

   または

   タブの名前にポインタを合わせて、**その他** ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**名前を変更** をクリックして、新しい [ 接続されたビュー ] タブに名前を変更します。
1. （オプション）接続されたレコードページのツールバーで次のビュー要素のいずれかを使用して、テーブルビューを管理します。

   * フィルター
   * 並べ替え。 プロジェクトでは使用できません。
   * グループ化。 プロジェクトでは使用できません。
   * フィールドの表示、非表示または並べ替えを行う列
   * 行の高さ。 プロジェクトでは使用できません。
   * 検索

   詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

   >[!NOTE]
   >
   >接続されたレコードのタブのテーブル表示のフィールドを作成、編集、削除することはできません。

   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. （オプション）接続されたレコードページのタブの名前にポインタを合わせ、「**詳細**![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、「**削除**」をクリックしてタブを削除します。

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