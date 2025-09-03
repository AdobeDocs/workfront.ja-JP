---
title: カレンダービューの管理
description: レコードとそのフィールドをカレンダーに表示できます。 この記事では、カレンダービューを作成し、既存のカレンダービューを編集または削除する方法について説明します。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 29%

---

# カレンダービューの管理

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードタイプページから、レコードとそのフィールドをカレンダー表示で表示できます。

Adobe Workfrontのプランニングビューとその管理方法について詳しくは、[ レコードビューの管理 ](/help/quicksilver/planning/views/manage-record-views.md) を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。 

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
    <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> ビューを作成および削除するための標準</p>
   <p>ビュー要素を更新する投稿者以上</p>
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
   <td> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、Planning を含むレイアウト テンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p></div></li></ul>
</td>
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

<!--
<div class="preview">

* You can create and edit records in the calendar view. For information, see [Create records](/help/quicksilver/planning/records/create-records.md).

</div>
-->

<!--move this bullet under the same div as above OR add a span or another div tag?? ??

* You can resize the records' bars in the calendar monthly view by clicking, then dragging and dropping their margins in a new position. Resizing the records' bars updates their start and end dates immediately. For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

-->

カレンダー表示を管理するには：

1. カレンダーを表示するレコードタイプ ページに移動します。
1. 「レコードビューの管理 [ の記事の説明に従って、カレンダービューを作成 ](/help/quicksilver/planning/views/manage-record-views.md) ます。

   ![ カレンダー表示の例 ](assets/calendar-view-example.png)

   選択したレコードタイプに関連付けられているレコードは、カレンダーにバーとして表示されます。 バーの色は、既定ではレコード アイコンの色と一致します。

1. カレンダー内を移動するには、次のいずれかの操作を行います。

   * カレンダーの左上隅にある左右のアイコンをクリックするか、水平スクロールを使用してカレンダーを前後に移動します。
   * 右上隅にある **今日** をクリックして、カレンダーを今日の日付の中央に配置します。
   * 時間枠ドロップダウンメニューから次のいずれかのオプションを選択して、時間間隔を更新します。

      * **月**：レコードは月別カレンダーに表示されます。

      * **週**：レコードは次の領域に表示されます。

         * 複数日にまたがるレコードは、カレンダーの上部に表示されます。
         * 1 日以下のレコードは、カレンダー表示の下半分に表示されます。 開始日と終了日の時間を表示するように選択した場合、レコードは該当する日の適切な時間に表示されます。

1. <span class="preview"> （オプション） **フルスクリーン** アイコン ![ フルスクリーンアイコンを開く ](assets/open-full-screen-icon.png) をクリックしてフルスクリーンでビューを開き、**フルスクリーンを終了** アイコン ![ フルスクリーンアイコンを終了 ](assets/exit-full-screen-icon.png) またはキーボードの Esc キーをクリックしてフルスクリーンを終了します。 </span>

1. 以下のサブセクションで説明するように、次のビュー要素を更新します。
   * [フィルター](#add-filters)
     <!--<span class="preview">[Row height](#modify-row-height)</span>-->
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

* 接続されたレコードフィールドまたはルックアップフィールドでフィルタリングできます。

* 複数の値を表示する参照フィールドでフィルタリングできます。

カレンダー表示にフィルターを追加するには：

1. 「レコードビューの管理 [ の記事の説明に従って、レコードタイプのページのカレンダービューを作成 ](/help/quicksilver/planning/views/manage-record-views.md) ます。
1. カレンダー表示を選択し、カレンダーのツールバーの **フィルター** をクリックします。
1. 「**条件を追加**」をクリックして、次の情報を追加します。

   * **でフィルターする** フィールドを選択 <!-- the tip below might change-->

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

   ![ フィルター UI テーブル表示 ](assets/filter-ui-table-view.png)

   追加できるフィルタリング条件の数に制限はありません。

1. （オプション）「**条件を追加**」をクリックして、別のフィルタリングオプションを追加し、上記の手順を繰り返します。適用されたフィルターの数が、フィルターアイコンの左側に表示されます。
1. 次の演算子をクリックして、フィルター条件の結合方法と適用方法を指定します。

   * **AND**：指定されたすべての条件が満たされている必要があります。
   * **OR**：指定された条件のいずれかが満たされている必要があります。 これはデフォルトのオプションです。

   1. （任意）複数の条件グループの間に、追加の **AND** または **OR** 演算子を追加します。

      ![ ビューの多層化フィルター ](assets/multi-tiered-filters-in-views.png)

   レコードのリストは自動的にフィルタリングされます。<!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. （任意）「**x**」アイコンをクリックして、フィルター条件を削除します。
1. （任意）「**フィルター**」をクリックして、「フィルター」ボックスを閉じます。<!--right now you cannot "clear all" for filters, but this might come later-->

<!--
<span class="preview">

### Modify row height

You can modify the row height of a calendar cell to increase or decrease the number of record bars you display in each cell. 

The number of records displayed in the calendar varies depending on how many fields you display on the records' bars. 

>[!TIP]
>
>This setting is available only when viewing the calendar by month. 


1. Create a calendar view for a record type page, as described in the article [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 
1. (Conditional) Display the calendar view by month, then click **Row height** in the calendar's toolbar.    
1. Choose from the following options: 

<table>
<thead>
<tr>
    <th><b>Row height option</b></th>
    <th><b>Number of records</b></th>
</tr>
</thead>
<tbody>
<tr>
    <td>Short</td>
    <td><p>Contains:</p>

<ul><li>2 records displaying 1 field</li>
<li>1 record displaying more than 1 field</li></ul>
    </td>
</tr>
<tr><td>Standard</td>
    <td><p>Contains:</p>

<ul><li>4 records displaying 1 field</li>
<li>2 record displaying more than 1 field</li></ul>
    </td>
</tr>
<tr>
    <td>Medium</td>
    <td><p>Contains:</p>

<ul><li>8 records displaying 1 field</li>
<li>4 record displaying more than 1 field</li></ul>
    </td>
</tr>
<tr>
    <td>Tall</td>
    <td><p>Contains:</p>

<ul><li>12 records displaying 1 field</li>
<li>6 record displaying more than 1 field</li></ul>
    </td>
</tr>
<tr>
    <td>Fit to content</td>
    <td><p>All records are visible, up to 500 records</p></td>
</tr>
</tbody>
</table> 

1. (Optional) Click **Show more** if there are records that are not visible in the calendar. 

    >[!TIP]
    >
    >The **Show more** option displays when you choose Fit to content and there are are more than 500 records in one time frame.


</span>

-->

### カレンダー表示設定の編集

カレンダー表示設定を更新して、ビューに表示する情報と方法を指定します。

1. 「レコードビューの管理 [ の記事の説明に従って、レコードタイプのカレンダービューを作成 ](/help/quicksilver/planning/views/manage-record-views.md) ます。
1. 「**設定**」をクリックします。
1. 左側のパネルで **日時** をクリックし、**開始日** と **終了日** を選択してカレンダーに表示します。 デフォルトの開始日と終了日を選択することも、使用可能な任意の日付フィールドを選択することもできます。

   レコードを表すバーは、開始日に指定した日付で始まり、終了日に指定した日付で終わります。

   >[!NOTE]
   >
   >* 開始日または終了日の値がないレコード、または開始日が終了日よりも後のレコードは、カレンダー表示に表示されません。
   >
   >* 「分類」オプションを使用して追加のレコードを表示する場合、開始日と終了日はメインレコードの日付です。 この領域で接続されているレコードの開始日と終了日を選択することはできません。

1. 左側のパネルで **バースタイル** をクリックし、レコードバーに表示する情報を指定します。

   レコードのテーブルビューで定義されたレコードのプライマリフィールド（またはタイトル）は、デフォルトで選択されています。
   <!--adjust this when the primary field is released??-->

1. （オプションおよび条件付き）レコードにサムネールを追加した場合、「**サムネール**」オプションを選択すると、レコードに関連付けられている画像がレコードバーに表示されます。

   >[!NOTE]
   >
   >    カレンダー表示にサムネイルを表示するには、まずテーブル ビューにサムネイルを追加する必要があります。 詳しくは、[ レコードへのサムネールの追加 ](/help/quicksilver/planning/records/add-thumbnails-to-records.md) を参照してください。

1. **フィールドを追加** をクリックして、**フィールドを検索** ボックス内をクリックし、追加するフィールドをクリックします。

   >[!TIP]
   >
   >   * レコードバーにフィールドを追加する前に、フィールドを作成する必要があります。
   > 
   >   * 1 つ以上のフィールドを選択する必要があります。**名前**&#x200B;はデフォルトで選択されています。
   >
   >   * 最大 5 個のフィールドを追加できます。

   カレンダー上でバーがどのように表示されるかを示すプレビューが右側に表示されます。

   ![ カレンダー表示設定のバーのスタイルセクション ](assets/bar-style-section-in-calendar-view-settings-with-preview.png)

1. 左側のパネルで **カラー** をクリックして、カレンダー上のレコードの色をカスタマイズします。

   ![ カレンダー表示設定のカラーパネル ](assets/color-panel-on-calendar-view-settings.png)

1. **レコードの色を設定** セクションで、次のオプションからレコードの色を設定します。

   * **レコードタイプ**：カレンダーのレコードバーの色は、選択したレコードタイプの色と一致します。 これはデフォルトのオプションです。
   * **フィールド値**：レコードの色は、指定したフィールドの色と一致します。
   * **なし**：レコードは白いバーで表示されます。

1. （条件付き）レコードの色に&#x200B;**フィールド値**&#x200B;を選択した場合、**レコードの色を次と一致させる**&#x200B;ドロップダウンメニューからフィールドを選択します。

   ![ カレンダー表示のフィールドセレクタードロップダウンメニュー ](assets/field-selector-drop-down-menu-calendar-view.png)

   ドロップダウンメニューには、色分けされたオプションを持つフィールドのみが表示されます。

   例えば、複数選択フィールドや単一選択フィールドには、色分けされたオプションを含めることができます。

   選択したレコードタイプに対して色分けされたオプションを含むフィールドがない場合、このオプションは淡色表示になります。


1. 「**保存**」をクリックします。

   レコードは、選択した仕様でカレンダー表示に表示されます。