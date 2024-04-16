---
title: レコードビューの管理
description: Adobe Workfront Planning を使用する場合、レコードをテーブル、タイムラインまたはカレンダ・ビューで表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: b11ab1dd0fdcc22cf2a99751d0aa4979556ec3fc
workflow-type: tm+mt
source-wordcount: '1085'
ht-degree: 19%

---

# レコードビューの管理

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Adobe Workfront計画エリアでレコードタイプを選択すると、そのタイプのすべてのレコードを次のビューに表示できます。

* テーブル

  詳しくは、[テーブルビューの管理](../views/manage-the-table-view.md)を参照してください。

* タイムライン

  詳しくは、[タイムラインビューの管理](../views/manage-the-timeline-view.md)を参照してください。

* カレンダー

  詳しくは、を参照してください [カレンダー表示の管理](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

## アクセス要件

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Adobe Workfront Planning クローズドベータ版プログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
   <p>システム管理者は、自分が作成したビューまたは共有されているビューにのみアクセスできます。 </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">アクセスレベルの設定</td>
   <td> <p>Workfront Planning には、アクセス レベルの制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ビューに対する権限の管理</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者が、レイアウトテンプレートに計画エリアを追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>
 </tbody>
</table>

## レコードビューを使用する場合の考慮事項

* Workfront Planning のビューは、レコードタイプに固有です。 2 つの異なるレコードタイプに同じビューを適用することはできません。
* 作成したビューは、自分と、ビューを共有するユーザーにのみ表示されます。
* ビューを変更または削除すると、そのビューに対する権限を持つすべてのユーザーに対して、ビューが変更および削除されます。
<!--* Each user can create a maximum of 100 views. -->
* 次の要素は、各レコードビューに固有です。

   * フィルター
   * グループ化
   * 並べ替え

  <!-- some of these are not available in all of the views - edit above-->

  例えば、テーブルビューでフィルターを作成した場合、フィルター結果は、選択したビューにのみ表示され、レコードタイプに関連付けられたすべてのビューには表示されません。

  >[!NOTE]
  >
  > Adobe Workfront Planning は現在ベータ版なので、一部のビュー要素は、すべてのビューで使用できるとは限りません。

この記事では、レコードビューに関する次の情報について説明します。

* [ビューの作成と編集](#create-or-edit-record-views)
* [ビューの削除](#delete-views)
* [ビューの複製](#duplicate-views)
* [ビューの共有](#share-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

## レコードビューの類似点と相違点

次の表に、テーブルビュー、タイムラインビューおよびカレンダービューの類似点と相違点を示します。

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 機能 | テーブル表示 | タイムライン表示 | カレンダー表示 |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| リストまたはテーブル内のレコードの表示 | ✓ |              | |
| デフォルトでは、すべてのフィールドをテーブルの列として表示します | ✓ |              |    |
| フィールド（または列）の表示と非表示を切り替える | ✓ |               |    |
| 各レコードのフィールド値の編集 | ✓ |               |             |
| ビューにレコードを新しい行として追加 | ✓ |               |        |
| フィールドを新しい列としてビューに追加する | ✓ |               |         |
| 外部リストから行をコピーしてテーブルに貼り付ける | ✓ |               |          |
| タイムラインでのレコードの表示 |            | ✓ |             |
| レコードをフィルタリング | ✓ | ✓ | ✓ |
| カレンダーにレコードを表示 |           |              | ✓ |
| レコードのグループ化 | ✓ | ✓ |
| レコードの並べ替え | ✓ |              |
| カラーコードレコード |           | ✓ | ✓ |
| カラーコードグループ化 |           | ✓ |
| 特定のレコードの検索 | ✓ | ✓ |
| ビューを共有 | ✓ | ✓ | ✓ |
| ビューからレコードのページを開く | ✓ | ✓ |    |


## ビューの作成または編集 {#create-or-edit-views}

{{step1-to-maestro}}


最後にアクセスしたワークスペースがデフォルトで開きます。ワークスペースの作成については、[ワークスペースの作成](../architecture/create-workspaces.md)を参照してください。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](../architecture/create-record-types.md)を参照してください。

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. クリック **+表示** 新規ビューを追加します。
1. 次のビューのタイプから選択します。

   * テーブル
   * タイムライン
   * カレンダー

   選択したビューで新しいタブが作成されます。

   画面の幅によっては、に追加のビューが表示される場合があります。 **詳細** メニュー ![](assets/more-menu.png).


>[!TIP]
>
>レコードタイプを作成する場合、テーブル表示もデフォルトで作成されます。
>
>タイムライン表示またはカレンダー表示を作成するには、ビューを作成するレコードタイプに少なくとも 2 つの日付フィールドが必要です。 それ以外の場合は、「タイムライン」および「カレンダー」オプションはグレー表示になります。
>

![](assets/view-types-drop-down-from-record-type-list.png)

>[!NOTE]
>
>    タイムライン表示またはカレンダー表示を作成するには、ビューを作成するレコードタイプに少なくとも 2 つの日付フィールドが必要です。 それ以外の場合は、[ タイムライン ] または [ カレンダー ] オプションは淡色表示になります。

1. （条件付き）クリック **次**&#x200B;を選択します（タイムラインビューまたはカレンダービューの作成時）。

   デフォルトでは、Workfrontはビューに次のいずれかの名前を付けます。

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   数値は、自動的に生成される増分です。

1. （条件付き）を選択します **開始** および **終了日** （タイムラインビューまたはカレンダービューに表示されるレコードの場合）
1. 「**作成**」をクリックします。

   ビューは新しいタブとして表示されます。 ビューは、作成時または共有時から時系列で表示されます。
1. （任意） **詳細** メニュー ![](assets/more-caret-down-icon-views.png) 最後のビューの横：選択したレコードタイプのすべてのビューが表示されます。

   追加のビューは、の下に表示されます **詳細** 最後の「表示」タブの後のメニュー 「」の横の数字 **詳細** メニューには、追加のビュー数が表示されます。
1. （オプション）作成後にビューの名前を変更するには、「ビュー」ドロップダウンメニューをクリックし、 **詳細** メニュー ![](assets/more-menu.png) > **名前を変更** ビュー名を更新するには

   または

   ビュー名をダブルクリックし、新しい名前の入力を開始します。  <!--ensure there is not another saving step here?!-->

1. （オプション）特定のタイプのビューを管理するには、以下の記事を参照してください。

   * [テーブルビューの管理](../views/manage-the-table-view.md)
   * [タイムラインビューの管理](../views/manage-the-timeline-view.md)
   * [カレンダー表示の管理](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## ビューの削除

{{step1-to-maestro}}

最後にアクセスしたワークスペースがデフォルトで開きます。ワークスペースの作成については、[ワークスペースの作成](../architecture/create-workspaces.md)を参照してください。

1. レコードタイプのカードをクリックします。

   レコードタイプの作成については、[レコードタイプの作成](../architecture/create-record-types.md)を参照してください。

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. 「表示」タブのビュー名の 1 つにポインタを合わせ、 **詳細** ![](assets/more-menu.png) ビュー名の左側にある「」をクリックします **削除**.
最初に、 **詳細** 最後のタブの左側で、削除するビューを探します。

1. クリック **削除** を確認します。 <!--ensure there is not another saving step here?!-->

   レコード エリアにアクセスできるすべてのユーザーに対してビューが削除され、復元できなくなります。

## ビューを共有

ビューの共有については、を参照してください。 [ビューの共有](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## ビューの複製

ビューの複数のバージョンを保持し、バージョン間でわずかな変更を行う場合は、ビューを複製できます。

ビューを複製すると、既存のビューと同一のコピーが作成されます。

元のビューの共有権限は、複製されたビューに転送されません。

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。

ワークスペースの作成については、[ワークスペースの作成](../architecture/create-workspaces.md)を参照してください。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](../architecture/create-record-types.md)を参照してください。

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. 複製するビューのタブにポインタを合わせて、 **詳細** メニュー ![](assets/more-menu.png) ビュー名の右側で、 **複製**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   ビューが複製され、新しいビューの名前が次のパターンに従います。 `Original view's name (Copy)`. 新しいビュータブは、すべてのビュータブの最後に表示されます。

