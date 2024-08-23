---
title: レコードビューの管理
description: Adobe Workfront Planning を使用する際に、テーブル、タイムラインまたはカレンダービューでレコードを表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 61cad7dc76ba04ea84ff0bd5052182f040f7b4d9
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 75%

---

# レコードビューの管理

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Adobe Workfront Planning でレコードタイプを選択すると、そのタイプのすべてのレコードを次のビューに表示できます。

* テーブル

  詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

* タイムライン

  詳しくは、[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)を参照してください。

* カレンダー

  詳しくは、[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-calendar-view.md)を参照してください。

この記事では、レコードビューに関する次の情報について説明します。

* [ビューの作成と編集](#create-or-edit-record-views)
* [ビューの削除](#delete-views)
* [ ビューの複製 ](#duplicate-views)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## アクセス要件

<!--Updated for GA-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <td> <ul><li><p>すべて（Workfront計画情報を表示する場合）</p></li>
   <li><p>標準、ワークスペースを作成するには</p></li></ul>
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
   <p>ビュー設定を一時的に変更するためのビューまたはそれ以上のアクセス許可</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--old: 

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

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->


## レコードビューを使用する際の考慮事項

* Workfront Planning のビューは、レコードタイプに固有です。同じビューを 2 つの異なるレコードタイプに適用することはできません。
* 作成したビューは、自分と、そのビューを共有しているユーザーにのみ表示されます。
* ビューを変更または削除すると、そのビューに対する権限を持つすべてのユーザーに対して、ビューが変更および削除されます。
* 各ユーザーは、最大 100 のビューを作成できます。 1 つのレコードタイプに対して 100 を超えるビューを表示できますが、1 人のユーザーが作成できるビューは 100 のみです。
* 作成したビューは他のユーザーと共有できます。 詳しくは、[ ビューの共有 ](/help/quicksilver/planning/access/share-views.md) を参照してください。
* 次の要素は、レコードビューごとに固有です。

   * フィルター
   * グループ化
   * 並べ替え
   * バーの外観（タイムライン表示）

  <!-- some of these are not available in all of the views - edit above-->

  例えば、テーブルビューでフィルターを作成した場合、フィルター結果は、選択したビューにのみ表示され、レコードタイプに関連付けられているすべてのビューに表示されるわけではありません。

  >[!NOTE]
  >
  > 一部のビュー要素は、すべてのビューで使用できるわけではありません。


## レコードビューの類似点と相違点

テーブルビュー、タイムラインビューおよびカレンダービューの類似点と相違点を次の表に示します。

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 機能 | テーブルビュー | タイムラインビュー | カレンダービュー |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| 一覧または表でレコードを表示します | ✓ |              | |
| すべてのフィールドをテーブル内の列として表示します（デフォルト） | ✓ |              |    |
| フィールド（または列）の表示／非表示を切り替える | ✓ |               |    |
| 各レコードのフィールド値を編集 | ✓ |               |             |
| ビューにレコードを新しい行として追加 | ✓ |               |        |
| ビューにフィールドを新しい列として追加 | ✓ |               |         |
| 外部リストから行をコピーしてテーブルに貼り付ける | ✓ |               |          |
| タイムラインでレコードを表示 |            | ✓ |             |
| レコードのフィルタリング | ✓ | ✓ | ✓ |
| カレンダーにレコードを表示 |           |              | ✓ |
| レコードをグループ化 | ✓ | ✓ |
| レコードの並べ替え | ✓ |              |
| カラーコードのレコード |           | ✓ | ✓ |
| カラーコードのグループ化 |           | ✓ |
| 特定のレコードを検索 | ✓ | ✓ |
| 他のユーザーとのビューの共有 | ✓ | ✓ | ✓ |
| ビューからレコードのページを開く | ✓ | ✓ |    |


## ビューを作成または編集 {#create-or-edit-views}

{{step1-to-planning}}


1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. 「**+ ビュー**」をクリックして、新しいビューを追加します。
1. 次のタイプのビューから選択します。

   * テーブル
   * タイムライン
   * カレンダー

   選択したビューで新しいタブが作成されます。

   画面の幅によっては、**その他**&#x200B;メニュー ![](assets/more-menu.png) に追加のビューが表示される場合があります。


>[!TIP]
>
>レコードタイプを作成すると、テーブルビューもデフォルトで作成されます。
>
>タイムライン表示またはカレンダー表示を作成するには、ビューを作成するレコードタイプに少なくとも 2 つの日付フィールドが必要です。
>
>それ以外の場合は、「タイムライン」および「カレンダー」オプションは淡色表示になります。
>

![](assets/view-types-drop-down-from-record-type-list.png)

1. （条件付き）タイムラインビューまたはカレンダービューを作成する際は、「**次へ**」をクリックします。

   デフォルトでは、ビューに次のいずれかの名前が付けられます。

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   この数字は自動的に 1 ずつ増えて生成されます。

1. （条件付き）タイムラインビューまたはカレンダービューに表示されるレコードの場合は、「**開始日**」と「**終了日**」を選択します。

   >[!TIP]
   >
   >    レコードの日付フィールドから選択することも、接続されたレコードまたはオブジェクトタイプから日付フィールドを参照することもできます。 タイムライン表示およびカレンダー表示の開始日および終了日として参照フィールドを選択する場合、日付フィールド （MAXまたは最小）にアグリゲータを使用する必要があります。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

1. 「**作成**」をクリックします。

   ビューは新しいタブとして表示されます。ビューは、作成時または共有時からの時間順で表示されます。
1. （オプション）最後のビューの横にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-caret-down-icon-views.png) をクリックすると、選択したレコードタイプのすべてのビューが表示されます。

   最後のビュータブの後の&#x200B;**その他**&#x200B;メニューに、追加のビューが表示されます。**その他**&#x200B;メニューの横の数字は、追加のビューの数を示します。
1. （オプション）ビューの作成後に名前を変更するには、ビューのドロップダウンメニューをクリックし、**その他**&#x200B;メニュー ![](assets/more-menu.png)／**名前を変更**&#x200B;をクリックして、ビュー名を更新します。

   または

   ビュー名をダブルクリックし、新しい名前を入力していきます。<!--ensure there is not another saving step here?!-->

1. （オプション）特定のタイプのビューを管理するには、次の記事を参照してください。

   * [テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [カレンダービューの管理](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## ビューの削除

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. ビュータブのビュー名の 1 つにポインタを合わせ、ビュー名の左側にある&#x200B;**その他** ![](assets/more-menu.png) をクリックしたあと、「**削除**」をクリックします。
まず、最後のタブの左側にある**その他**&#x200B;をクリックして、削除するビューを探します。

1. 「**削除**」をクリックして確定します。<!--ensure there is not another saving step here?!-->

   ビューは、レコードエリアにアクセスできるすべてのユーザーに対して削除され、復元できません。

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## ビューの複製

ビューの複数のバージョンを保持し、バージョン間でわずかな変更を行う場合は、ビューを複製できます。

ビューを複製すると、既存のビューと同一のコピーが作成されます。

元のビューの共有権限は、複製されたビューには移行されません。

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプ ページが開きます。
デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. 複製するビューのタブにポインタを合わせて、ビュー名の右側にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックして、「**複製**」をクリックします。

   ![](assets/view-more-menu-with-duplicate-option.png)


   ビューが複製され、新しいビューの名前が次のパターンに従います。`Original view's name (Copy)`新しいビュータブは、すべてのビュータブの最後に表示されます。

