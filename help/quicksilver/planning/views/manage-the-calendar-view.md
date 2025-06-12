---
title: カレンダービューの管理
description: レコードとそのフィールドをカレンダーに表示できます。 この記事では、カレンダービューを作成し、既存のカレンダービューを編集または削除する方法について説明します。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 24%

---

# カレンダービューの管理

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードタイプページから、レコードとそのフィールドをカレンダー表示で表示できます。

Adobe Workfrontのプランニングビューとその管理方法について詳しくは、[ レコードビューの管理 ](/help/quicksilver/planning/views/manage-record-views.md) を参照してください。

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
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
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
<p><span class="preview">プレビュー環境では、標準ユーザーとシステム管理者は、デフォルトで計画を有効にしています。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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
1. 「レコードビューの管理 [ の記事の説明に従って、カレンダービューを作成 ](/help/quicksilver/planning/views/manage-record-views.md) ます。

   ![ カレンダー表示の例 ](assets/calendar-view-example.png)

   選択したレコードタイプに関連付けられているレコードは、カレンダーにバーとして表示されます。 バーの色は、レコードアイコンの色と一致します。

1. カレンダー内を移動するには、次のいずれかの操作を行います。

   * 左右のアイコンをクリックするか、水平スクロールを使用してカレンダー内を前後に移動します。
   * カレンダーを今日の日付の中央に配置するには、[**今日**] をクリックします。
   * 時間枠ドロップダウンメニューから次のいずれかのオプションを選択して、時間間隔を更新します。

      * **月**：レコードは月別カレンダーに表示されます。


      * **週**：レコードは次の領域に表示されます。

         * 複数日にまたがるレコードは、カレンダーの上部に表示されます。
         * 1 日以下のレコードは、カレンダー表示の下半分に表示されます。 開始日と終了日の時間を表示するように選択した場合、レコードは該当する日の適切な時間に表示されます。


1. 以下のサブセクションで説明するように、次のビュー要素を更新します。
   * [フィルター](#add-filters)
   * [設定](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
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

### カレンダー表示設定の編集

カレンダー表示設定の編集は、タイムラインビューの設定の編集と似ています。

詳しくは、「タイムライン表示の管理」の記事の「タイムライン表示設定の編集 [ の節を参照し ](/help/quicksilver/planning/views/manage-the-timeline-view.md) ください。
