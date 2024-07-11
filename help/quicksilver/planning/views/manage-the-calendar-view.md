---
title: カレンダービューの管理
description: レコードとそのフィールドをカレンダーに表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 30%

---

# カレンダービューの管理

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

レコードタイプページから、レコードとそのフィールドをカレンダー表示で表示できます。

Adobe Workfrontのプランニング・ビューとその管理方法については、を参照してください。 [レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md).

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

*詳細については、を参照してください [Workfrontのドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## カレンダー表示の管理 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

次の点に注意してください。

* カレンダー表示を作成できるのは、1 つのレコードタイプに 2 つ以上の日付フィールドが関連付けられている場合のみです。 レコードタイプに日付フィールドが関連付けられている場合は、「カレンダー」表示オプションがグレー表示になります。

  レコードの日付フィールドから選択することも、接続されたレコードまたはオブジェクトタイプから日付フィールドを参照することもできます。
* 次のシナリオが存在します。

   * 開始日と終了日の両方に値がない場合、レコードはカレンダーに表示されません
   * 開始日または終了日に値がない場合、レコードは 1 日のイベントとして表示されます
   * 開始日が終了日より後の場合、レコードはカレンダーに表示されません。

カレンダー表示を管理するには：

1. カレンダーを表示するレコードタイプ ページに移動します。
1. 記事の説明に従って、カレンダービューを作成します [レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   選択したレコードタイプに関連付けられているレコードは、カレンダーにバーとして表示されます。 バーの色は、レコードアイコンの色と一致します。

1. カレンダー内を移動するには、次のいずれかの操作を行います。

   * 左右のアイコンをクリックするか、水平スクロールを使用してカレンダー内を前後に移動します。
   * クリック **今日** カレンダーを今日の日付に中央揃えにします。
   * 時間枠ドロップダウンメニューから次のいずれかのオプションを選択して、時間間隔を更新します。

      * 月
1. 以下のサブセクションで説明するように、次のビュー要素を更新します。
   * [フィルター](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### フィルターを追加

フィルターを使用すると、画面に表示される情報の量を減らすことができます。

カレンダー表示でフィルターを使用する場合は、次の点に注意してください。

<!-- this list is almost identical to the one for the table view - update both-->

* カレンダー表示に対して作成するフィルターは、同じレコードタイプに適用される他の表示のフィルターとは独立して機能します。

* フィルターは、選択したビューに固有です。同じレコードタイプの 2 つのカレンダービューに異なるフィルターを適用できます。

* 2 人のユーザーが同じカレンダー表示を見ると、現在適用されているのと同じフィルターが表示されます。

* 作成したカレンダー表示のフィルターに名前を付けることはできません。

* フィルターを削除すると、自分と同じレコードタイプにアクセスし、同じビューを表示している人から、フィルターが削除されます。

* カレンダービューにフィルターを追加する方法は、テーブルビューにフィルターを追加する方法と同じです。

  詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)の記事の「フィルターの追加」の節を参照してください。

* 接続されたレコードフィールドまたはルックアップフィールドでフィルタリングできます。

* 複数の値を表示する参照フィールドでフィルタリングできます。
