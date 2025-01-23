---
title: テーブル表示の管理
description: Adobe Workfront Planning の「レコードタイプ」ページにアクセスすると、レコードとそのフィールドをテーブル・ビューに表示できます。 この記事では、テーブルビューを作成し、既存のテーブルビューを編集または削除する方法について説明します。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0dd723b5-d674-4626-8fc2-7da41f3b7f35
source-git-commit: 9db8ea3f26dd7e8b4c8aa52fb9902832db7a6a5c
workflow-type: tm+mt
source-wordcount: '2879'
ht-degree: 68%

---

# テーブルビューの管理

<span class="preview"> このページでハイライト表示されている情報は、まだ一般公開されていない機能を指しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning のレコードタイプのページにアクセスすると、レコードとそのフィールドをテーブルビューで表示できます。

レコードビューとその管理方法について詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
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
   <td><p> 標準 </p>
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
   <td>   <p>ビューに対する権限を管理</p>  
   <p>ビュー設定を一時的に変更するためのビューへのアクセス許可を表示します</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


<!--
OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
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
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

## テーブル表示を使用したレコードの編集

レコード情報は、テーブル表示でのみ編集できます。

テーブル ビューでレコードを編集する方法の詳細については、「[ レコードの編集 ](/help/quicksilver/planning/records/edit-records.md)」を参照してください。

## テーブルビューの管理 {#manage-a-table-view}

<!--insert screen shot of table view-->

テーブルビューを作成すると、選択したタイプのすべてのレコードがテーブルに表示されます。各行は一意のレコードであり、各列はレコードフィールドです。デフォルトでは、すべてのフィールドとすべてのレコードが表示されます。

テーブルビューを管理するには：

1. [レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)の記事の説明に従って、テーブルビューを作成します。

   ![](assets/table-view-example.png)

1. （オプション）「**行の高さ**」をクリックし、次のオプションから選択して、テーブルの行の高さを変更します。
   * 低い
   * 中
   * 高い

1. 以下のサブセクションで説明するように、次のビュー要素を更新します。
   * [列（またはフィールド）](#add-columns-or-fields)
   * [行（またはレコード）](#add-rows-or-records)
   * [フィルター](#add-filters)
   * [グループ化](#add-groupings)
   * [並べ替え](#add-a-sort)
   * [リアルタイムプレゼンスインジケーターの有効化](#enable-the-real-time-presence-indicator)


### 列（またはフィールド）の追加 {#add-columns}

テーブルビューの列ヘッダーには、ビュー内のレコードに関連付けられたフィールドが表示されます。テーブルビューに表示される同じフィールドが、レコードの「詳細」セクションにも表示されます。詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

<!--this is not available yet:You can display record fields (or columns) in both a table and a timeline view. However, the number of columns displayed in the table of the timeline view is limited and you cannot add columns in addition to those selected by default.-->

ビューへの列の追加は、レコードタイプへのフィールドの追加と同じです。

テーブルビューには最大 500 個のフィールド（または列）を追加できます。

1. レコードタイプページに移動してテーブルビュータブをクリックするか、**+ ビュー** をクリックして新しいビューを追加してから、**テーブル** を選択します。

1. [フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)の記事の説明に従って、フィールド（または列）の追加を開始します。

   追加した列は、レコードタイプにアクセスするすべてのユーザーに表示され、レコードのページに新しいフィールドとして追加されます。

1. テーブルの列を並べ替えるには、次のいずれかの操作を行います。

   * 列ヘッダーをつかみ、目的の位置にドラッグ＆ドロップします。移動した列は、テーブルに他の調整を行うまで、青色の背景で短時間表示されます。

   * テーブルのツールバーで&#x200B;**フィールド**&#x200B;をクリックし、フィールドを目的の順序でドラッグ＆ドロップし、「**フィールドの表示と順序**」ボックスの外側をクリックしてボックスを閉じます。

     ![](assets/fields-setting-table-view-toolbar-expanded.png)


     >[!TIP]
     >
     >* デフォルトでは、「名前」フィールドが常にテーブルビューの最初のフィールドです。これは、プライマリフィールドと見なされます。
     >
     >* 別のフィールドをプライマリフィールドとして指定しない限り、「名前」フィールドを別の位置に移動することはできません。詳しくは、手順 4 に進んでください。<!--accurate?-->
     >
     >

   * 最初の列のフィールドを別のフィールドに置き換えるには、プライマリフィールドを変更します。詳しくは、手順 4 に進んでください。<!--accurate?-->

1. （オプション）テーブルの最初の列に表示されないフィールドの列ヘッダーにあるフィールド名の上にポインタを合わせ、フィールド名の右側にある下向き矢印をクリックして、「**プライマリフィールドとして設定**」をクリックします。

   ![](assets/set-as-primary-field-option-table-view.png)

1. 「**フィールドを設定**」をクリックして確認します。

   フィールドは、テーブルビューの最初の列として表示されるプライマリフィールドになります。前のプライマリフィールドは、2 番目の列に移動します。

   プライマリフィールドはレコードのタイトルになり、レコードのページのヘッダー領域およびレコードが表示されるすべての場所に表示されます。 例えば、レコードのタイトルは、接続されたフィールドとすべてのビューに表示されます。 主フィールドについて詳しくは、[プライマリフィールドの概要 ](/help/quicksilver/planning/fields/primary-field-overview.md) を参照してください。

1. 列の区切り線をクリックしてドラッグし、目的の場所にドロップして、列の幅を広げます。

   >[!TIP]
   >
   >列の幅と順序に対して行った変更は永続的に適用され、レコードタイプにアクセスするすべてのユーザーに表示されます。

1. 列ヘッダー上にポインタを合わせ、下向き矢印をクリックして、「**フィールドを非表示**」をクリックします。

   または

   テーブルツールバーの「**フィールド**」をクリックし、非表示にするフィールド（または列）に関連付けられた切替スイッチを無効にします。**フィールドの表示と順序**&#x200B;ボックスが表示されます。

   >[!TIP]
   >
   >非表示のフィールドの数は、ツールバーのフィールドアイコンの左側に表示されます。


1. **フィールド**&#x200B;アイコンをクリックし、テーブルの列に表示するフィールドに関連付けられた切替スイッチを有効にします。デフォルトでは、すべてのフィールドが表示されます。

1. キーワードに一致するレコードをすばやく検索するには、次の手順を実行します。

   1. **検索**&#x200B;アイコン ![](assets/search-icon.png) をクリックして、画面に表示されるレコードの任意のフィールドに関連付けられたキーワードの入力を開始します。正しい一致の数が検索項目の横に表示され、正しく一致するフィールドがハイライト表示されます。

      ![](assets/search-box-with-results-blue-outline-table-view.png)

      画面に表示される任意の単語や特殊文字を使用できます。

      テーブルビューで非表示になっているフィールドに関連付けられたキーワードは使用できません。

   1. キーボードの **Enter** キーを押して、次に見つかったフィールドに移動します。

   1. （オプション）複数の一致がある場合は、検索キーワードの右にある上下の矢印をクリックすると、表内のすべての一致を確認できます。

   1. 検索ボックスの **x** アイコンをクリックして、検索キーワードをクリアします。


### 行（またはレコード）の追加 {#add-rows}

テーブルビューの行には、選択したレコードタイプの個別のレコードが表示されます。

1 つのレコードタイプに対して最大 50,000 個のレコード（または行）を指定できます。

1. レコードタイプページに移動してテーブルビュータブをクリックするか、**+ ビュー** をクリックして新しいビューを追加してから、**テーブル** を選択します。

1. [レコードの作成](/help/quicksilver/planning/records/create-records.md)の記事の説明に従って、レコード（または行）の追加を開始します。

   テーブルビューで追加したレコードはすぐに保存され、ワークスペースに対する表示以上の権限を持つすべてのユーザーに表示されます。

1. （オプション）それぞれのレコードにサムネールを追加し、テーブルの右上隅にある「**フィールド**」をクリックし、「**サムネール**」フィールドの切替スイッチを選択して、プライマリフィールドの左側に表示します。デフォルトでは選択解除されています。

   詳しくは、[レコードへのサムネールの追加](/help/quicksilver/planning/records/add-thumbnails-to-records.md)を参照してください。

1. （オプション）行内の 1 つまたは複数のレコードを選択し、レコードの左側にある **ハンドル** アイコン ![](assets/handle-icon.png) をドラッグ&amp;ドロップして、行を並べ替えます。

   >[!NOTE]
   >
   >テーブルビューに少なくとも 1 つの並べ替えが適用されていると、行の並べ替えを行うことができません。
   >
   >行順序に加えた変更は、レコードタイプにアクセスするすべてのユーザーに表示されます

<!-- this section below links from the timeline view; consider splitting them if they become different-->

### フィルターを追加 {#add-filters}

フィルターを使用すると、画面に表示される情報の量を減らすことができます。

テーブル表示でフィルターを使用する場合は、次の点に注意してください。

<!-- this list is almost identical to the one for the table view - update both-->

* テーブルビュー用に作成したフィルターは、同じレコードタイプに適用された場合、タイムラインビューのフィルターとは独立して機能します。

* フィルターは、選択したビューに固有です。同じレコードタイプの 2 つのテーブルビューには、異なるフィルターを適用できます。同じテーブルビューを見ている 2 人のユーザーには、現在適用されている同じフィルターが表示されます。

* 作成したフィルターに名前を付けて、テーブルビューに適用することはできません。

* フィルターを削除すると、自分と同じレコードタイプにアクセスするすべてのユーザーからフィルターが削除され、自分が使用している同じビューが使用されます。

* テーブルビューへのフィルターの追加は、タイムラインビューへのフィルターの追加と同じです。

* 接続されたレコードフィールドまたはルックアップフィールドでフィルタリングできます。

* 複数の値を表示する参照フィールドでフィルタリングできます。

* 現在のレコードタイプから最大 4 レベル離れたフィールドを参照できます。 例えば、アクティビティレコードタイプのフィルターを作成し、アクティビティが、Workfront プロジェクトに接続されたキャンペーンレコードタイプに接続された製品レコードタイプに接続されている場合、アクティビティ レコードタイプに作成しているフィルターでプロジェクトの予算を参照できます。

テーブルビューにフィルターを追加するには：

1. [レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)の記事の説明に従って、レコードタイプのページのテーブルビューを作成します。
1. テーブルビューを選択し、テーブルの右上隅にある&#x200B;**フィルター**&#x200B;をクリックします。
1. 「**条件を追加**」をクリックして、次の情報を追加します。

   * <!-- the tip below might change--> でフィルターする **フィールドを選択**

   * **オプションを選択** （またはフィルター修飾子）して、フィールドが満たす必要がある条件の種類を定義します

     次の表に、各タイプのフィールドで使用可能な修飾子を示します。

     <table>
        <thead>
        <tr>
            <th><b>フィールドタイプ</b></th>
            <th><b>修飾子</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>1 行、段落、式 </td>
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
            <td>複数選択、人物</td>
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
            <p>が次の範囲である</p><p>が次の範囲ではない</p>
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

   追加できるフィルタリング条件の数に制限はありません。

1. （オプション）「**条件を追加**」をクリックして、別のフィルタリングオプションを追加し、上記の手順を繰り返します。適用されたフィルターの数が、フィルターアイコンの左側に表示されます。
1. 次の演算子をクリックして、フィルター条件の結合方法と適用方法を指定します。

   * **AND**：指定されたすべての条件が満たされている必要があります。
   * **OR**：指定された条件のいずれかが満たされている必要があります。 これはデフォルトのオプションです。

   <div class="preview">

   1. （任意）複数の条件グループの間に、追加の **AND** または **OR** 演算子を追加します。

      ![](assets/multi-tiered-filters-in-views.png)

   </div>

   レコードのリストは自動的にフィルタリングされます。<!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. （任意）「**x**」アイコンをクリックして、フィルター条件を削除します。
1. （任意）「**フィルター**」をクリックして、「フィルター」ボックスを閉じます。<!--right now you cannot "clear all" for filters, but this might come later-->

### グループ化の追加 {#add-groupings}

<!--this section exists in the timeline view too, but the display is slightly different, so I kept both steps; consider updating both sections if any updates to groupings are introduced-->

ビューにグループ化を適用する際に、類似の情報でレコードをグループ化できます。

テーブルビューへのグループ化の追加は、タイムラインビューへのグループ化の追加と似ています。

次の点に注意してください。

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

グループ化を追加するには：

1. [レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)の記事の説明に従って、レコードタイプのタイムラインビューを作成します。
1. テーブルビューの右上隅にある「**グループ化**」をクリックします。

   ![](assets/grouping-ui-table-view-with-linked-fields.png)

1. フィールド候補の 1 つをクリックするか、「**別のフィールドを選択**」をクリックして別のフィールドを検索し、リストに表示されたらクリックします。

   グループ化はテーブルに自動的に適用され、レコードがグループ化の区切り線の下に表示されます。

1. （任意）「**条件を追加**」をクリックし、上記の手順を繰り返して、最大 3 つのグループを追加します。

   グループ化用に選択したフィールドの数がグループ化アイコンの横に表示されます。

   ![](assets/grouping-applied-in-table-view.png)

1. （オプション）「**以下でレコードをグループ化**」ボックスで、グループ化用に選択したフィールドの右側にある **x** アイコンをクリックすると、グループ化を削除できます。

   または

   **すべてクリア**&#x200B;をクリックすると、すべてのフィールドを削除できます。

1. 「**以下でレコードをグループ化**」ボックスの外側をクリックして閉じます。
1. （オプション）任意のグループ化の最後にある「**+新規レコード**」をクリックして新しいレコードを追加し、ページを更新して新しいレコードを適切なグループ化に追加します。<!--this might need to be changed when they add the Refresh button on the toolbar of the table view-->

### 並べ替えの追加 {#sort-information}

並べ替えを適用すると、情報を特定の順序で整理できます。

次の情報を並べ替えることができます。

* テーブルビュー内のすべてのレコード。<!--or timeline view. ***********verify this is the case for the timeline view*********************-->
  <!--* All groupings. - this is not available yet-->

テーブルビューでレコードを並べ替える際は、次の点を考慮してください。

<!-- if this is available for the timeline view, update both when you update one-->

* 並べ替えは、選択したビューに一意です。同じレコードタイプの 2 つのテーブルビューには、異なる並べ替え基準を適用できます。同じテーブルビューを見ている 2 人のユーザーには、現在適用されている同じ並べ替えが表示されます。

* 作成した並べ替えに名前を付けて、テーブルビューに適用することはできません。

* 作成した並べ替えは、別の場所に移動しても保持されます。

* レコードタイプのテーブルビューに表示されるフィールドの数だけ並べ替えることができます。

* 接続されたレコードフィールドで並べ替えることはできませんが、接続されたレコードタイプの参照フィールドで並べ替えることはできます。

* （アグリゲータによって要約されていない）複数の値がある参照フィールドで並べ替える場合、最初の値が並べ替えに使用されます。

* 並べ替え基準を削除すると、自分と同じレコードタイプにアクセスするすべてのユーザーから並べ替え基準が削除され、自分が使用している同じビューが使用されます。

* 現在のレコードタイプから最大 4 レベル離れたフィールドを参照できます。 例えば、アクティビティレコードタイプの並べ替えを作成し、アクティビティが、Workfront プロジェクトに接続されたキャンペーンレコードタイプに接続された製品レコードタイプに接続されている場合、アクティビティ レコードタイプに対して作成している並べ替えで、プロジェクトのステータスを参照できます。

<!--ungrouped (add this when sorting for groupings will be available--> レコードを並べ替えるには、次の操作を行います。

1. [レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)の記事の説明に従って、テーブルビューを作成します。
1. テーブルの右上隅にある&#x200B;**並べ替え**&#x200B;アイコン ![](assets/sort-icon.png) をクリックします。

   または

   テーブルビューの列の名前の上にポインタを合わせ、列ヘッダー名の右側にある下向き矢印をクリックして、「**このフィールドで並べ替え**」をクリックします。このフィールドは、テーブルビューの右上隅にある、並べ替えアイコンの並べ替え選択として追加されます。

1. （条件付き） [**レコードの並べ替え基準**] ボックスで、フィールド候補の 1 つをクリックするか、**別のフィールドを選択** をクリックして別のフィールドを検索し、リストに表示されたらクリックします。

   並べ替えはテーブルビューに自動的に適用され、レコードは選択した条件に従って並べ替えられて表示されます。

   <!-- add a step that you can rearrange the sorting fields here, when this will be possible-->

1. （オプション）「**条件を追加**」をクリックし、上記の手順を繰り返して追加のフィールドで並べ替えます。

   並べ替えるフィールドの数が、ツールバーの右上隅にある並べ替えアイコンの左側に表示されます。テーブルビューの列に表示されるフィールドのみを選択できます。

1. （オプション）「**レコードの並べ替え基準**」ボックスで、並べ替えフィールドの右側にある **x** アイコンをクリックして並べ替えを削除します

   または

   「**すべてクリア**」をクリックして、並べ替えからすべてのフィールドを削除します。

1. 「**レコードの並べ替え基準**」ボックスの外側をクリックしてボックスを閉じます。

   ![](assets/sorting-in-table-view.png)

   テーブルに表示される情報は、選択した条件に従って並べ替えられます。

   並べ替え用に選択されたフィールドには、並べ替えアイコンと、その後に並べ替えが適用される順序を示す数字が表示されます。

<!-- this is not available yet: 

To sort grouped records: 

1. Create a view, as described in [Create or edit record views](#create-or-edit-record-views). 
1. ************************* add steps here for sorting grouped records****************

-->

### リアルタイムプレゼンスインジケーターの有効化

デフォルトでは、すべてのレコードビューの右上隅に表示される、レコード情報を同時に編集している他のユーザーのアバターです。

テーブルビューを表示すると、レコードの表示中に別のユーザーが編集しているフィールドを表示することもできます。

詳しくは、「レコードの表示の管理 [ の「リアルタイムプレゼンスインジケーターの有効化」の節を参照し ](/help/quicksilver/planning/views/manage-record-views.md) ください。