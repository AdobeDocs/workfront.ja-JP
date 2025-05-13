---
title: レコード表示の管理
description: Adobe Workfront Planning を使用する場合、レコードをテーブル、タイムラインまたはカレンダ・ビューで表示できます。 この記事では、ビューを作成し、既存のビューを編集または削除する方法について説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 0d968a3f398c2e7dc4154cd5a16acf35ca7c86f5
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 51%

---


# レコードビューの管理

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


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
* [ビューの複製](#duplicate-a-view)
* [ ビューでリアルタイムプレゼンス指標を有効にする ](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
   <p>ビュー設定を一時的に変更したり、複製したりするためのビューへのアクセス許可を表示します</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>実稼動環境では、システム管理者を含むすべてのユーザーを、Planning を含むレイアウト・テンプレートに割り当てる必要があります。</p>
<p><span class="preview">プレビュー環境では、標準ユーザーとシステム管理者は、デフォルトで計画を有効にしています。</span></p></td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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
| レコードを年および四半期別に表示 |           | ✓ |    |
| 月別にレコードを表示 |           | ✓ | ✓ |
| レコードを週別に表示 |           |               | ✓ |


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

   画面の幅に応じて、追加のビューが **その他** メニュー ![ その他メニュー ](assets/more-menu.png) に表示される場合があります。


>[!TIP]
>
>レコードタイプを作成すると、テーブルビューもデフォルトで作成されます。
>
>タイムライン表示またはカレンダー表示を作成するには、ビューを作成するレコードタイプに少なくとも 2 つの日付フィールドが必要です。
>
>それ以外の場合は、「タイムライン」および「カレンダー」オプションは淡色表示になります。
>

![ レコードタイプリストからの表示タイプドロップダウン ](assets/view-types-drop-down-from-record-type-list.png)

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
1. （オプション）選択したレコードタイプのすべてのビューを表示するには、最後のビューの横にある **その他** メニュー ![ その他のキャレットダウンアイコンビュー ](assets/more-caret-down-icon-views.png) をクリックします。

   最後のビュータブの後の&#x200B;**その他**&#x200B;メニューに、追加のビューが表示されます。**その他**&#x200B;メニューの横の数字は、追加のビューの数を示します。
1. （オプション）作成後にビューの名前を変更するには、ビューのドロップダウンメニューをクリックし、**詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png)>**名前を変更** をクリックしてビュー名を更新します

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

1. ビュータブ内のビュー名の 1 つにポインタを合わせ、ビュー名の左側にある **その他**![ その他メニュー ](assets/more-menu.png) をクリックしてから、**削除** をクリックします。
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

1. 複製するビューのタブにポインタを合わせ、ビュー名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックしてから、「**複製**」をクリックします。

   ![ 「複製」オプションを使用した詳細メニューの表示 ](assets/view-more-menu-with-duplicate-option.png)


   ビューが複製され、新しいビューの名前が次のパターンに従います。`Original view's name (Copy)`新しいビュータブは、すべてのビュータブの最後に表示されます。

## ビューでリアルタイムプレゼンスインジケーターを有効にする

デフォルトでは、すべてのレコードビューの右上隅に表示される、レコード情報を同時に編集している他のユーザーのアバターです。

テーブルビューを表示すると、レコードの表示中に別のユーザーが編集しているフィールドを表示することもできます。

1. レコードタイプのページに移動し、任意のビューを開きます。
1. （条件付き）選択したタイプのレコードを同時に編集する他のユーザーがいる場合、そのアバターはビューの右上隅に表示されます。
1. アバターの横にあるドロップダウンメニューをクリックし、「**共同作業者を表示**」切替スイッチを選択します。 この切り替えはデフォルトで選択されています。

   ![ 「共同作業者を表示」切替スイッチが選択されている ](assets/show-collaborators-toggle-selected.png)

1. （条件付き）テーブルビューを開くと、他のユーザーがアクティブに編集しているフィールドが、テーブルビューでのアバターの概要に対応する色でハイライト表示されます。

   アバターのハイライト色がグレーの場合、ユーザーは 30 秒以上前にレコードのアクティブな編集を停止しました。

   ![ リアルタイムインジケーターテーブルフィールドとアバター接続 ](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >任意の表示から「**共同作業者を表示**」切り替えスイッチを選択できます。 他のユーザーが現在編集しているフィールドの輪郭は、テーブルビューでのみ表示されます。
