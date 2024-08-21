---
title: タイムラインビューの管理
description: Adobe Workfront計画レコードタイプページのタイムラインビューでレコードにアクセスして編集します。 フィルター、グループ化、設定を使用してタイムラインをカスタマイズします。 分類機能を使用して、接続されたレコードを表示します。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '1941'
ht-degree: 81%

---

# タイムラインビューの管理

<!--
title: Manage the timeline view 
description: You can display records in a timeline view, when accessing the record type page in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Adobe Workfront Planning でレコードタイプのページにアクセスする際、レコードをタイムラインビューで表示できます。

レコードビューについて詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

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
   <p>ビュー設定を一時的に変更するためのビューへのアクセス許可を表示します</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p> 
</td>
  </tr>
 </tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。


<!--EDIT PERMISSIONS AND ACCESS AND REPLACE THE table above with the following table at Planning GA release: 
## Access requirements

You must have the following to be able to access Workfront Planning: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following new Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning plan*</p></td>
   <td>
<p>Any of the following Workfront Planning plans:</p>
<ul><li>Planning</li>
<li>Planning Plus</li>
</ul>
<p>For more information about what is included in each Workfront Planning plan, see <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront pricing and packaging</a>. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <ul><li><p>Any, to view Workfront Planning information</p></li>
   <li><p>Standard, to create workspaces</p></li></ul>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a> and and <a href="../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md">Assign users to a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  

*********ensure that the link ^^^^^^^^above^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************

-->


## タイムラインビューの管理 {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

タイムラインビューを作成すると、選択したレコードタイプのすべてのレコードが時系列で表示されます。

次の点に注意してください。

* タイムラインビューを作成できるのは、レコードタイプに関連付けられた日付フィールドが 2 つ以上ある場合のみです。レコードタイプに関連付けられた日付フィールドが 1 つのみ、またはまったくない場合は、タイムライン表示のオプションは淡色表示になります。

  タイムラインビューを作成する際に、次の日付フィールドから選択できます。

   * レコード日付
   * レコードのシステム生成フィールド：作成日、最終変更日
   * 接続されたレコードまたはオブジェクトタイプから日付を参照します。
* 以下のシナリオのように、レコードに関連付けられた日付によっては、一部のレコードがタイムラインビューに表示されないことがあります。

   * 開始日と終了日に値がない場合
   * 開始日または終了日のどちらかに値がない場合
   * 開始日が終了日より後の場合

タイムラインビューを管理するには：

1. タイムラインを表示するレコードタイプページに移動します。
1. タイムラインビューを作成します。詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   ![](assets/timeline-view-example.png)

   選択したレコードタイプに関連付けられたレコードは、タイムラインにバーとして表示され、デフォルトでは開始日の時系列で並べ替えられます。

   >[!TIP]
   >
   >    タイムラインのレコードの並べ替えは、コンパクト表示には表示されません。

1. （オプションおよび条件付き）レコード名が切り詰められている場合は、レコードバーにマウスポインターを置くと、レコードのフルネームと追加情報が表示されます。

1. タイムラインを移動するには、次のいずれかを行います。

   * 左右のアイコンをクリックするか、水平スクロールを使用してタイムラインを前後に移動します。 ページを更新すると、選択した時間枠が保持されます。
   * 「**今日**」をクリックして、今日の日付をタイムラインの中心に置きます。
   * 時間枠ドロップダウンメニューから次のいずれかのオプションを選択して、時間間隔を更新します。

      * 年
      * 四半期
      * 月
1. **標準ビューに切り替え**&#x200B;をクリックして、別々の行にレコードを表示します。<!--check to see if they updated the name of the setting here-->

   または

   **コンパクトビューに切り替え**&#x200B;をクリックして、日付が同じ行で交わらないレコードを表示します。<!--check to see if they updated the name of the setting here-->

   デフォルトでは、レコードはコンパクトビューで表示されます。

1. キーワードに一致するレコードをすばやく検索するには、次の手順を実行します。

   1. **検索**&#x200B;アイコン ![](assets/search-icon.png) をクリックして、画面に表示されるレコードの任意のフィールドに関連付けられたキーワードを入力し始めます。正しい一致の数が検索項目の横に表示され、正しい一致のレコードがハイライト表示されます。

      ![](assets/search-box-and-results-timeline-view.png)

      画面に表示される任意の単語や特殊文字を使用できます。

      タイムラインビューに表示されないフィールドに関連付けられたキーワードは使用できません。

   1. キーボードの Enter キーを押して、次に見つかったフィールドに移動します。
   1. （オプション）複数の一致がある場合は、検索キーワードの右にある上下の矢印をクリックすると、表内のすべての一致を確認できます。
   1. 検索ボックスの **x** アイコンをクリックすると、検索キーワードをクリアできます。

1. 以下のサブセクションで説明するように、次のビュー要素を更新します。
   * [フィルター](#add-filters)
   * [グループ化](#add-grouping)
   * [設定](#edit-the-timeline-view-settings)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->

### フィルターを追加

フィルターを使用すると、画面に表示される情報の量を減らすことができます。

タイムラインビューでフィルターを使用する際は、次の点を考慮してください。

<!-- this list is almost identical to the one for the table view - update both-->

* タイムラインビュー用に作成したフィルターは、同じレコードタイプに適用される他のビューのフィルターとは独立して機能します。

* フィルターは、選択したビューに固有です。同じレコードタイプの 2 つのタイムラインビューに、異なるフィルターを適用できます。

* 同じタイムラインビューを表示する 2 人のユーザーには、現在適用されている同じフィルターが表示されます。

* タイムラインビュー用に作成したフィルターには名前を付けることはできません。

* フィルターを削除すると、自分と同じレコードタイプにアクセスし、同じビューを表示している人から、フィルターが削除されます。

* タイムラインビューでのフィルターの追加方法は、テーブルビューでのフィルターの追加方法と同じです。

  詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)の記事の「フィルターの追加」の節を参照してください。

* 接続されたレコードフィールドまたはルックアップフィールドでフィルタリングできます。
* 複数の値を表示する参照フィールドでフィルタリングできます。


### グループ化を追加

<!-- groupings are almost identical between this view and table  but they display a little differently, so I kept the steps for both; update in both places if they make changes to groupings-->

ビューにグループ化を適用する際に、類似の情報でレコードをグループ化できます。

タイムラインビューでグループ化を追加する操作は、テーブルビューでグループ化を追加する操作と似ています。

タイムラインビューでグループ化を操作する際は、次の点を考慮してください。

* テーブルビューとタイムラインビューの両方でグループ化を適用できます。テーブルビューのグループ化は、同じレコードタイプのタイムラインビューのグループ化とは独立しています。
* ビューでは、3 つのレベルのグループ化を適用できます。レコードは、選択したグループ化の順にグループ化されます。
&lt;!--* API を使用すると、最大 4 レベルのグループ化を適用できます。--現在これを確認中-->
* グループは、選択したビューに固有です。同じレコードタイプの 2 つのテーブルビューに、異なるグループ化を適用することができます。同じテーブルビューを見ている 2 人のユーザーには、現在適用されているのと同じグループ化が表示されます。
* テーブルビュー用に作成したグループ化に名前を付けることはできません。
* グループ化を削除すると、自分と同じレコードタイプにアクセスし、同じビューを表示している人から、グループ化が削除されます。
* グループ化の下に一覧表示されたレコードは編集できます。
* 接続されているレコードフィールドまたはルックアップフィールドでグループ化できます。
* アグリゲータによって集計されていない複数の値を持つルックアップ フィールドでグループ化する場合、レコードはフィールド値の一意の組み合わせごとにグループ化されます。
* 現在のレコードタイプから最大 4 レベル離れたフィールドを参照できます。 例えば、アクティビティレコードタイプのグループを作成し、そのアクティビティが、Workfront プロジェクトに接続されたキャンペーンレコードタイプに接続された製品レコードタイプに接続されている場合、アクティビティレコードタイプに作成しているグループでプロジェクトのステータスを参照できます。
<!--checking into this: * You can apply up to 4 levels of grouping when using the API. -->
<!-- checking also into this: * You cannot group by a Paragraph-type field.-->

タイムラインビューでグループ化を追加するには：

1. レコードタイプのタイムラインビューを作成します。詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。
1. タイムラインビューの右上隅にある&#x200B;**グループ化**&#x200B;をクリックします。

   ![](assets/grouping-ui-timeline-view-with-linked-fields.png)

1. 推奨フィールドの 1 つをクリックするか、「**別のフィールドを選択**」で別のフィールドを検索して、リストに表示されたらクリックします。

   グループ化はタイムラインに自動的に適用され、レコードがグループ化ボックス内に表示されます。

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. （オプション）上記の手順を繰り返して、最大 3 つのグループ化を追加できます。

   グループ化用に選択したフィールドの数がグループ化アイコンの横に表示されます。

   <!-- update screen shot with view redesign-->

   ![](assets/grouping-applied-in-timeline-view.png)

1. （オプション）「**以下でレコードをグループ化**」ボックスで、グループ化用に選択したフィールドの右側にある **x** アイコンをクリックすると、グループ化を削除できます。

   または

   **すべてクリア**&#x200B;をクリックすると、すべてのフィールドを削除できます。

1. 「**以下でレコードをグループ化**」ボックスの外側をクリックして閉じます。
1. （オプション）「**設定**」、「**カラー**」の順にクリックすると、グループ化をカラーコーディングできます。詳しくは、この記事の[タイムラインビュー設定の編集](#edit-the-timeline-view-settings)の節を参照してください。
   <!--1. (Optional) Click **Breakdown** to display connected records on the timeline. For information, see the section [Use the Breakdown feature to display connected records in the timeline view](#break-down-connected-records-in-the-timeline-view)-->

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### タイムラインビュー設定の編集 {#edit-the-timeline-view-settings}

タイムラインビュー設定を変更すると、ビューのタイムラインセクションに表示される情報と表示のされ方を指定できます。

1. レコードタイプのタイムラインビューを作成します。詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。
1. 「**設定**」をクリックします。
1. 左パネルの&#x200B;**日付および時刻**&#x200B;をクリックし、**開始日**&#x200B;と&#x200B;**終了日**&#x200B;を選択してタイムラインで表示します。デフォルトの開始日と終了日を選択するか、使用可能な任意の日付フィールドを選択できます。レコードを表すバーは、開始日に指定した日付で始まり、終了日に指定した日付で終わります。

   >[!NOTE]
   >
   >開始日または終了日の値がないレコード、または開始日が終了日より後のレコードは、タイムラインビューに表示されません。

1. 左パネルで「**バーのスタイル**」をクリックし、レコードバーに表示するフィールドを指定します。

   レコードのテーブルビューで定義されたレコードのプライマリフィールド（またはタイトル）は、デフォルトで選択されています。<!--adjust this when the primary field is released??-->

1. （オプションおよび条件付き）レコードにサムネールを追加した場合、「サムネール」オプションを選択すると、レコードに関連付けられた画像がレコードバーに表示されます。

   >[!NOTE]
   >
   >    タイムラインビューにサムネールを表示するには、まずテーブルビューにサムネールを追加する必要があります。詳しくは、[ レコードへのサムネールの追加 ](/help/quicksilver/planning/records/add-thumbnails-to-records.md) を参照してください。

1. **フィールドを追加**&#x200B;をクリックすると、レコードバーに最大 4 つのフィールドを追加できます。
1. **フィールドを検索**&#x200B;ボックスの内側をクリックし、追加するフィールドをクリックします。

   >[!TIP]
   >
   >   * レコードバーにフィールドを追加する前に、フィールドを作成する必要があります。
   > 
   >   * 1 つ以上のフィールドを選択する必要があります。**名前**&#x200B;はデフォルトで選択されています。

   タイムライン上でバーがどのように表示されるかを示すプレビューが右側に表示されます。

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. 左パネルの&#x200B;**カラー**&#x200B;をクリックすると、タイムラインのレコードとグループ化の色をカスタマイズできます。

   ![](assets/color-tab-timeline-view.png)

1. （条件付きおよびオプション）タイムラインビューにグループ化を追加した場合、グループ化の色を設定するには、「**グループ化の色を設定**」セクションで次のオプションから選択します。

   * **デフォルト（グレー）**：グループ化の色をグレーに設定します。これがデフォルトです。
   * **フィールド値**：グループ化の色は、グループ化に使用するフィールドの色と一致します。

     >[!NOTE]
     >
     >    * カラーは、色分けされたオプションを含むフィールドにのみ一致させることができます。 例えば、カラーをステータスフィールドに一致させたり、カラーに関連付けられたオプションを含むフィールドに一致させることができます。
     >    
     >    * リンクされたレコードまたはオブジェクト タイプのルックアップ フィールドの色を一致させることはできません。


   例えば、複数選択フィールドや単一選択フィールドには、色分けされたオプションを含めることができます。

   色分けされたオプションを使用しないフィールドでグループ化した場合、グループ化の色はグレーのままになります。

   >[!TIP]
   >
   >タイムラインビューにグループ化を追加しなかった場合、このセクションは表示されません。

1. レコードの色を設定するには、「**レコードの色を設定**」セクションで次のオプションから選択します。

   * **レコードタイプ**：レコードの色を、選択したレコードタイプの色と一致させます。これはデフォルトのオプションです。
   * **フィールド値**：レコードの色を、指定したフィールドの色と一致させます。手順 10 に進みます。<!--ensure this stays accurate-->
   * **グループ化**：レコードの色を、グループ化で指定した色と一致させます。タイムラインビューにグループ化が適用されていない場合、このオプションは淡色表示になります。
   * **なし**：レコードは白いバーで表示されます。

1. （条件付き）レコードの色に&#x200B;**フィールド値**&#x200B;を選択した場合、**レコードの色を次と一致させる**&#x200B;ドロップダウンメニューからフィールドを選択します。

   ![](assets/field-selector-drop-down-menu-timeline-view.png)

   ドロップダウンメニューには、色分けされたオプションを持つフィールドのみが表示されます。

   例えば、複数選択フィールドや単一選択フィールドには、色分けされたオプションを含めることができます。

   選択したレコードタイプに対して色分けされたオプションを含むフィールドがない場合、このオプションは淡色表示になります。

1. 「**保存**」をクリックします。

   選択した設定でレコードがタイムラインビューに表示されます。

<!--
### Use the Breakdown feature to display connected records in the timeline view

You can display connected records in a record's timeline view by using the Breakdown feature. Breaking down records by their connections allows you to view the timelines of other connected records and understand how they might affect the performance and deadlines of your records. 

#### Considerations when using the Breakdown feature

* You can display connected records or objects under the records of the selected record type in the timeline view. 
* You can display the following in the timeline view, using the Breakdown feature:
    * Workfront Planning records connected to the selected record type. 
    * Workfront (*************or AEM Assets*************)  object types connected to the selected record type.
    * Workfront Planning records or objects from other application that are connected to records connected to the selected record type. 
    
        For example, you might connect campaigns to portfolios. In addition, you might connect  another record type, products, with projects, as well as with campaigns. When you build the campaign timeline view, you can break down the campaigns by portfolios, products, and projects. 

* You cannot display object types that are connected only to Workfront objects in Workfront, but are not connected to a Workfront Planning record type. You can only display object or record types that are connected in Workfront Planning. 

    For example, tasks, are connected to projects in Workfront. Using the Breakdown feature, you can display projects that are connected to campaigns in Planning, but not tasks connected to projects in Workfront. 

    If you want to display both portfolios and projects in the timeline view of a Workfront Planning record type, both the portfolios and the projects must be connected to the Planning record or to a record connected to the Planning record whose timeline view you are managing.
* You can only display record types that are associated with at least two date fields. 
* The date fields for the record types you want to display in the timeline view must be visible in the table view of the selected record type, as lookup fields. 
* The Start and End dates of the record types you want to display in the timeline view must by in chronological order. For example, if a record has a Start date of January 31 and an End date of January 1, it does not display in the timeline view. For more information, see the section [Manage a timeline view](#manage-a-timeline-view) in this article. 
* There is a limit of 5 record types that you can include in a record's breakdown. 


#### Break down connected records in the timeline view

1. Create a timeline view for a record type, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 
1. Click **Breakdown**.
1. Expand the **Select a linked record type** box and select a connected record type. (**************add new screen shot***************)

    ![](assets/breakdown-picker-and-button-on-timeline.png)

    >[!TIP]
    >
    >    If you do not have any connected records, or if the connected records do not have at least two date fields, the **Select a linked record type** box is not available.

1. Choose a **Start date** and an **End date field**.

    >[!TIP]
    >
    >    The Start and End dates must be sequential. If the End date is before the Start date, no records will display in the timeline. 

    A right-pointing arrow displays on the selected record's bar in the timeline, if they they are connected with other records. 

    ![](assets/campaigns-broken-down-by-programs-in-timeline-highlighted.png)    


1. (Optional) Repeat the steps above to add more connected records. 

    >[!TIP]
    >
    >    You can add up to 5 connected records in a timeline using the Breakdown feature. 


-->