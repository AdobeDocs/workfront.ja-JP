---
title: テーブル表示の管理
description: Maestro でレコードタイプページにアクセスする際に、テーブルビューでレコードとそのフィールドをAdobeで表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 5%

---


# テーブル表示の管理

<!--
title: Manage the table view
description: You can display records in a table view when using Adobe Maestro. 
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

Maestro でレコードタイプページにアクセスする際に、テーブルビューでレコードとそのフィールドをAdobeで表示できます。

Maestro ビューとその管理方法については、 [レコードビューの管理](../views/manage-record-views.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe産物</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">アクセスレベル</td>
   <td> <p>任意</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/grant-access.md">AdobeMaestro へのアクセスを許可</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## テーブルビューの管理 {#manage-a-table-view}

<!--insert screen shot of table view-->

テーブルビューを作成すると、選択したタイプのすべてのレコードがテーブルに表示されます。 各行は一意のレコードで、各列はレコードフィールドです。 デフォルトでは、すべてのフィールドとすべてのレコードが表示されます。

テーブル・ビューを管理する手順は、次のとおりです。

1. 「 」を参照して、テーブルビューを作成します。 [レコードビューの管理](../views/manage-record-views.md).

   ![](assets/table-view-example.png)

1. 以下のサブセクションで説明するように、次のビュー要素を更新します。
   * [列（またはフィールド）](#add-columns-or-fields)
   * [行（またはレコード）](#add-rows-or-records)
   * [フィルター](#add-filters)
   * [グループ化](#add-groupings)
   * [並べ替え](#sort-information)


### 列（またはフィールド）を追加 {#add-columns}

Maestro テーブルビューの列ヘッダーには、ビュー内のレコードに関連付けられたフィールドが表示されます。 テーブルビューに表示されるのと同じフィールドは、Maestro レコードの [ 詳細 ] セクションにも表示されます。 詳しくは、 [レコードを編集](../records/edit-records.md).

<!-- this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default. -->

ビューに列を追加する操作は、レコードタイプにフィールドを追加する操作と同じです。

テーブルビューでは、最大 500 個のフィールド（または列）を追加できます。

1. レコードタイプのページに移動し、 **テーブル** ビューを選択します。
1. 記事の説明に従って、フィールド（または列）の追加を開始します。 [フィールドの作成](../architecture-and-fields/create-fields.md).

   追加した列は、レコードタイプにアクセスするすべてのユーザーに対して表示され、選択したレコードタイプのレコードの [ 詳細 ] ページに新しいフィールドとして追加されます。

1. テーブル内の列を並べ替えるには、次のいずれかの操作を行います。

   * 列ヘッダーをつかんで、目的の位置にドラッグ&amp;ドロップします。 移動した列は、テーブルを調整するまで、青い背景で短く表示されます。

   * クリック **フィールド** テーブルのツールバーで、目的の順序でフィールドをドラッグ&amp;ドロップし、 **フィールドの表示と順序ボックス** をクローズします。

     ![](assets/fields-setting-table-view-toolbar-expanded.png)

   >[!TIP]
   >
   >* 「名前」フィールドは、常にテーブル表示の最初のフィールドです。
   >
   >* [ 名前 ] フィールドを別の位置に移動することはできません。
   >
   >* 「名前」フィールドを非表示にすることはできません。
   >
   >* 「名前」フィールドは固定され、水平スクロールの一部ではありません。

1. 列の幅を広げるには、列の区切り線をクリックしてドラッグし、目的の場所にドロップします。

   >[!TIP]
   >
   >列の幅と順序に対して行った変更は、永続的に適用され、レコードタイプにアクセスするすべてのユーザーに表示されます。

1. 列を非表示にするには、列見出しの上にマウスポインターを置き、下向き矢印をクリックして、 **フィールドを非表示**

   または

   クリック **フィールド** をクリックし、非表示にするフィールドに関連付けられた切り替えを無効にします。

   >[!TIP]
   >
   >非表示のフィールドの数は、ツールバーのフィールドアイコンの左側に表示されます。


1. 次から： **フィールド** 設定で、テーブルの列に表示するフィールドに関連付けられた切り替えを有効にします。 デフォルトでは、すべてのフィールドが表示されます。

### 行（またはレコード）を追加 {#add-rows}

Maestro テーブルビューの行には、選択したレコードタイプの個々のレコードが表示されます。

Maestro では、1 つのレコードタイプに対して最大 10,000 個のレコード（または行）を指定できます。

Maestro テーブルビューに行を追加する操作は、テーブルでレコードを作成する操作と同じです。

詳しくは、 [レコードを作成](../records/create-records.md).

<!-- this is not possible right now:

1. To reorder the rows, click the row header, drag and drop it in the desired location. 

    The changes you make to the row order are permanent and visible to all users who access the record type
-->

### フィルターを追加 {#add-filters}

<!-- this section links from the timeline view; consider splitting them if they become different-->

フィルターを使用すると、画面に表示される情報の量を減らすことができます。

テーブルビューでフィルタを使用する際は、次の点に注意してください。
<!-- this list is almost identical to the one for the table view - update both-->

* 同じレコードタイプに適用された場合、テーブル表示用に作成したフィルタは、タイムライン表示のフィルタとは独立して機能します。

* フィルターは、選択したビューに固有です。 同じレコードタイプの 2 つのテーブルビューに、異なるフィルタを適用できます。 同じテーブル表示を見ている 2 人のユーザーには、現在適用されているのと同じフィルターが表示されます。

* 作成してテーブルビューに適用したフィルターに名前を付けることはできません。

* フィルターを削除すると、自分と同じレコードタイプにアクセスするすべてのユーザーからフィルターが削除され、使用したのと同じビューが使用されます。

* テーブル表示にフィルターを追加する方法は、タイムライン表示にフィルターを追加する方法と同じです。

テーブルビューにフィルターを追加するには、次の手順に従います。

1. 記事の説明に従って、レコードタイプのページのテーブルビューを作成します。 [レコードビューの管理](../views/manage-record-views.md).
1. テーブルビューを選択し、「 **フィルター** をクリックします。
1. クリック **条件を追加** 次の情報を追加します。

   * フィルターに使用するフィールドを選択します <!-- the tip below might change-->

   * オプション（またはフィルター修飾子）を選択して、フィールドが満たす必要のある条件の種類を定義します

     次の表に、フィールドの各タイプで使用可能な修飾子を示します。

     >[!TIP]
     >
     > リンクされたフィールドは選択できません。 詳しくは、 [フィールドの作成](../architecture-and-fields/create-fields.md).

     <table>
        <thead>
        <tr>
            <th><b>フィールドタイプ</b></th>
            <th><b>修飾子</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>1 行、段落 </td>
            <td><p>が次を含む</p>
            <p>が次を含まない</p>
            <p>が次に等しい</p>
            <p>が次に等しくない</p>
            <p>が空である</p>
            <p>が空ではない</p></td>
        </tr>
        <tr><td>単一選択</td>
            <td><p>が次に等しい</p>
            <p>が次に等しくない</p>
            <p>が次のいずれかである</p>
            <p>が次のいずれでもない</p>
            <p>が空である</p>
            <p>が空ではない</p></td>
        </tr>
        <tr>
            <td>複数選択</td>
            <td><p>が次のいずれかを含む</p>
            <p>が次のすべてを含む</p>
            <p>が次に完全に等しい</p>
            <p>が次のいずれも含まない</p>
            <p>が空である</p>
            <p>が空ではない</p></td>
        </tr>
        <tr>
            <td>数値、割合、通貨</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>が空である</p>
            <p>が空ではない</p></td>
        </tr>
        <tr>
            <td>日付</td>
            <td><p>が次に等しい</p>
            <p>が次に等しくない</p>
            <p>が次の後にある</p>
            <p>が次の前にある</p>
            <p>が次の範囲である</p><p>が次の範囲ではない :</p>
            <p>が空である</p><p>が空ではない</p></td>
        </tr>

     <tr>
            <td>チェックボックス</td>
            <td><p>が次に等しい</p>
        </tr>
        </tbody>
        </table>

   * 選択したフィールドの値を選択します。

   ![](assets/filter-ui-table-view.png)

   追加できるフィルター条件の数に制限はありません。

1. （オプション）「 **条件を追加** 別のフィルターオプションを追加するには、上記の手順を繰り返します。 適用されたフィルターの数がフィルターアイコンの左側に表示されます。
1. 次の演算子をクリックして、フィルター条件の結合方法と適用方法を指定します。

   * **および**：指定したすべての条件を満たす必要があります。
   * **または**：指定した条件のいずれかを満たす必要があります。 これはデフォルトのオプションです。

   レコードのリストは自動的にフィルタリングされます。  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. （オプション）「 **フィルター**」、「 **x** アイコンをクリックして、フィルターを削除します。 <!--right now you cannot "clear all" for filters, but this might come later-->

<!-- this is not available yet

### Add groupings {#add-groupings}

*******************this section might link in the future from the timeline view; right now it's only documented there; also, check the steps below because this was not released to the table when they were written*****************

You can group records by similar information when applying  a grouping to a view.

You can apply groupings both in the table and timeline views. The groupings of the table view are independent from those in the timeline view of the same record type. 

Consider the following:

* You can apply 3 levels of grouping in a Maestro view. The records are grouped in the order of groupings that you select. (***************check on this; this might be true for timeline, but not for table??? One dev said in a demo that there are unlimited groupings in a table - check *********************)
* You can apply up to 4 levels of grouping when using the API. 

To add a grouping:

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. (Conditional) To apply a grouping in the table view, do the following:
    
    1. ***************start adding steps for building a grouping - see if there it a global setting or just per column; also, see if the steps are different for a table vs a timeline view?!**********************
1. (Conditional) To apply a grouping in the timeline view, do the following:

    1. Go to a timeline view, then click **Group**. ************************did they rename this to "Grouping"?!****************************
        ******************insert screen shot***********
    1. Click one of the 5 suggested fields, or click **Choose a different field** to display all fields, then click one when it displays in the list. 
    
        >[!TIP]
        >
        > You cannot select linked fields. For information, see [Create fields](../architecture-and-fields/create-fields.md).  
    The grouping is applied automatically to the timeline and records display inside the grouping box.    <********************ensure this is correct functionality here*************
    
    1. (Optional) Click **Add grouping** to add up to 3 groupings. 

        The number of groupings applied displays to the left of the Grouping icon in the upper-right corner of the toolbar. **********ensure this says "grouping" and not "group"*****************
    
    1. (Optional) Click **Clear all** to remove all groupings.  

-->

### 並べ替えの追加 {#sort-information}

並べ替えを適用すると、情報を指定された順序で整理できます。

次の情報を並べ替えることができます。

* テーブルビュー内のすべてのレコード。 <!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

テーブルビューでレコードを並べ替える際は、次の点に注意してください。

<!-- if this is available for the timeline view, update both when you update one-->

* 並べ替えは、選択したビューに固有です。 同じレコードタイプの 2 つのテーブルビューに異なる並べ替え基準を適用することができます。 同じテーブル表示を見ている 2 人のユーザーには、現在適用されているのと同じ並べ替えが表示されます。

* 作成してテーブルビューに適用した並べ替えに名前を付けることはできません。

* 作成した並べ替えは、移動しても保持されます。

* レコードタイプのテーブルビューに表示されている数だけフィールドを並べ替えることができます。

* 並べ替え基準を削除すると、自分と同じレコードタイプにアクセスするすべてのユーザーから削除され、使用したのと同じビューが使用されます。

並べ替えるには <!--ungrouped (add this when sorting for groupings will be available--> レコードを作成するには、以下の手順を実行します。

1. 「 」を参照して、テーブルビューを作成します。 [レコードビューの管理](../views/manage-record-views.md).
1. 次をクリック： **並べ替え** アイコン ![](assets/sort-icon.png) テーブルの右上隅に

   または

   テーブル表示で列の名前の上にマウスポインターを置き、列ヘッダー名の右にある下向き矢印をクリックして、 **このフィールドで並べ替え**. このフィールドは、テーブル表示の右上隅にある並べ替えアイコンで並べ替え選択として追加されます。
1. Adobe Analytics の **レコードの並べ替え基準** ボックスをクリックするか、推奨フィールドの 1 つをクリックするか、 **別のフィールドを選択** 別のフィールドを検索し、リストに表示されたらクリックします。

   並べ替えはテーブルビューに自動的に適用され、選択した条件で並べ替えられたレコードが表示されます。

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. （オプション）上記の手順を繰り返して、追加のフィールドで並べ替えます。

   並べ替えるフィールドの数は、ツールバーの右上隅にある並べ替えアイコンの左側に表示されます。 選択できるフィールドは、テーブル表示の列に表示されるフィールドのみです。

   >[!TIP]
   >
   > リンクされたフィールドは選択できません。 詳しくは、 [フィールドの作成](../architecture-and-fields/create-fields.md).

1. （オプション） **レコードの並べ替え基準** ボックスで、 **x** 並べ替えを削除するための並べ替えフィールドの右側のアイコン

   または

   クリック **すべてクリア** をクリックして、並べ替えからすべてのフィールドを削除します。

1. の外側をクリック **レコードの並べ替え基準** ボックスを使用して閉じます。

   テーブルに表示される情報は、選択した条件に従って並べ替えられます。

   並べ替え用に選択されたフィールドには、並べ替えアイコンに続いて、並べ替えが適用される順序を示す数字が表示されます。

   ![](assets/sorting-in-table-view.png)


<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->