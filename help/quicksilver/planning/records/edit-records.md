---
title: レコードの編集
description: レコードの情報は、Adobe Workfront Planning で編集できます。レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 567fa8c960f7db47279d6cde1f5e90dc7f38ae79
workflow-type: tm+mt
source-wordcount: '2192'
ht-degree: 44%

---


# レコードの編集

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

レコードに関連付けられたフィールドの値を編集することで、Adobe Workfront Planning 内のレコード情報を編集できます。

レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。

詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

レコードの作成について詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

&lt;!-- ここでは、詳細ビューのフィールドがテーブルビューのフィールドと同じであることに言及しています。この記事は、この情報を参照するためのレコードを管理ビューからリンクされています-->

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
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> <p>標準</p> 
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
   <td>  <p>ワークスペースおよびレコードタイプ </a> への投稿以上の権限 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>

</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## レコードの編集に関する考慮事項

* ワークスペースへの権限がある場合は、自分が作成したレコードや他のユーザーが作成したレコードを編集できます。
* 次のエリアからレコードフィールドを編集できます。

   * レコード ビューでのレコードのプレビュー
   * レコードの詳細ページ
   * テーブルビューでのインライン。

* ユーザーがビューでレコードを編集すると、変更はすべてのビューで直ちに表示され、レコードページは他のすべてのユーザーに表示されます。

* 次のタイプのフィールドは自動的に更新され、手動で値を編集することはできません。
   * 他のレコードからリンクされたフィールド
   * 数式タイプのフィールド
   * システムフィールド（作成者、作成日、最終変更者、最終変更日）
* 表示しているレコードが他のレコードにリンクされている場合、編集中のレコードの新しい情報がリンクされたレコードに反映されます。
* レコードを一括で編集することはできません。<!--this will probably change-->
* URL は、http://、https://、ftp:// または www で始まる場合にのみ、1 行テキストフィールドタイプのリンクとして認識されます。
* 各レコードにカバー画像を追加できます。 画像はレコードごとに一意であり、同じ時間のすべてのレコードには適用されません。
* レコードページのフィールドの順序を編集し、レコードのカバー画像を追加できます。詳しくは、[ レコードページレイアウトの管理 ](/help/quicksilver/planning/records/manage-the-record-page.md) を参照してください。

## レコードの編集

次のエリアからレコードを編集できます。

* [レコードタイプのテーブル表示](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [ビューでのレコードのプレビュー](#edit-a-record-from-the-records-preview-in-a-view)
* [レコードのページ](#edit-a-record-from-the-records-page)
* [計画セクションのWorkfrontオブジェクト](#edit-a-record-from-a-workfront-object-in-the-planning-section)

### レコードタイプのテーブルビューでレコードをインラインで編集

テーブルビューからレコードを編集すると、レコードの表示時に他のユーザーによって編集されているフィールドが示されます。

詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

グループ化またはサブグループ化の最後のレコードの後に新しいレコードを追加すると、Workfrontでは新しいレコードのグループ化に含まれるフィールドが自動的に更新されます。 必要に応じてこれらのフィールドを手動で編集でき、レコードがグループから削除される可能性があります。

詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

{{step1-to-planning}}

1. レコードを編集するワークスペースをクリックします

   ワークスペースが開き、レコードタイプがカードとして表示されます。
1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。
1. （条件付き）テーブルビューのタブをクリックするか、「**+ 表示**」をクリックして、テーブルビューを作成します。最後にアクセスしたときに別のタイプのビューでレコードタイプを表示した場合を除き、テーブルビューがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。
1. レコードの行内をクリックして、レコードに関する情報の編集をインラインで開始します。

   ![ 書式設定テーブルビューでレコードの段落フィールドを編集 ](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  次のフィールドは読み取り専用で、Workfront によって自動的に更新されるので、情報を編集できません。
   >  
   >  * レコードタイプを接続して作成されるリンクフィールド。詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
   >  * 次のタイプのフィールド：作成者、作成日、最終変更者、最終変更日、数式フィールド。

1. （オプションおよび条件付き）段落タイプのフィールドを編集する場合、次の&#x200B;**リッチテキスト**&#x200B;書式オプションを使用します：

   * 太字
   * 斜体
   * 下線
   * リンクを追加
   * 箇条書きリストを追加
   * 番号付きリストを追加

   ![ 段落フィールドのリッチテキストツールバー ](assets/rich-text-toolbar-on-paragraph-field.png)

1. （オプション）接続されたレコードフィールドをダブルクリックして、接続済みレコードやオブジェクトを別のレコードに追加します。詳しくは、[レコーのを接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。
1. キーボードの **Enter** キーを押すか、行の外側をクリックして変更を保存します。変更点は自動的に保存されます。テーブルビューの右上隅に&#x200B;**保存済み**&#x200B;インジケータが短時間表示され、変更が保存されたことを示します。


1. （オプション）あるフィールドから別のフィールドに情報をコピー＆ペーストするには、次のいずれかの操作を行います。

   * 1 つのフィールドの 1 つ以上の既存の値をコピーして、別のレコードの同じタイプのフィールドに貼り付けます
   * 列の列ヘッダーをクリックして選択、コピーし、別の列の列見出しをクリックして、コピーした列の内容をペーストします。列には、類似したフィールドタイプが含まれている必要があります。
   * Shift キーを押したまま、表内の複数の行をクリックして選択し、選択した行の情報をコピーしてから、別の行をクリックして、選択した情報を新しい行とその後の行にペーストします。
   * 1 つのセルから情報をコピーして、複数のセルを選択し、同じ情報を複数のセルに貼り付けます。 複数のセルを選択して、隣接する行と列の複数のセルに同じ情報を貼り付けることができます。
   * コピーする情報が含まれている既存のセルの右下隅を選択し、同じ情報を貼り付ける隣接するセル間でドラッグ アンド ドロップします。 すべてのセルに同じ種類の情報を含める必要があります。

     ![ テーブル表示でのコピー貼り付けに使用する、ドラッグ可能な右下隅 ](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)


   * 外部ソース （Excel ファイルなど）から 1 つまたは複数のセルをコピーし、次のいずれかのフィールド型に貼り付けます。

      * Workfront Planning 接続フィールド。
      * 人物フィールド。 1 つの値を持つフィールドのみがサポートされます。

     外部ソースから情報をコピーして、WorkfrontやAEM Assetsの接続フィールドなど、他のフィールドタイプに貼り付けることはできません。

   >[!NOTE]
   >
   >次の点に注意してください。
   >
   >* 次のキーボードショートカットを使用して、情報をコピー＆ペーストします。
   >   * コピー：Ctrl + C （Macの場合は ⌘ + C）
   >   * 貼り付け：Ctrl + V （Macの場合は ⌘ + V）
   >
   >* レコードページにフィールド値をコピー＆ペーストすることはできません。この機能は、レコードタイプのテーブルビューでのみサポートされます。
   >* 次のフィールドタイプのフィールド値をコピーして貼り付けることはできません。
   >
   >    * レコードタイプを接続する際に作成されるルックアップフィールド。 リンクされたレコードフィールドをコピー＆ペーストできます。詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
   >    * 次のタイプのフィールド：作成者、作成日、最終変更者、最終変更日

1. （オプション）次のキーボードショートカットを使用すると、レコードの情報の編集またはコピー＆ペーストの取り消しまたはやり直しを実行できます。

   * CTRL + Z （Macの場合は ⌘ + Z）
   * Ctrl + Shift + Z （Macの場合は ⌘ + Shift + Z）

   >[!TIP]
   >
   >    キーボードショートカットを複数回連続して使用して、複数の変更を元に戻すことができます。

1. （オプション）レコードにサムネールを追加します。詳しくは、[レコードへのサムネールの追加](/help/quicksilver/planning/records/add-thumbnails-to-records.md)を参照してください。

### ビューでのレコードのプレビューからのレコードの編集

{{step1-to-planning}}

1. レコードを編集するワークスペースをクリックします

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意のタイプのビューで、レコードをクリックします

   または

   テーブル表示で、最初の列の **詳細を開く** アイコン ![ テーブル名フィールドで詳細を開くアイコン ](assets/open-details-icon-in-table-name-field.png) をクリックします。 レコードのプレビューがビューで開きます。

   ![ 詳細ボックス ](assets/details-box.png)

1. （オプション）レコードのタイトルの右側にある **詳細** メニューをクリックし、「名前を変更 **をクリックし** す。 これにより、レコードのタイトルとして表示されるフィールドが更新されます。

   レコードのタイトルは、テーブル表示で表示された場合、レコードのプライマリフィールドになります。 詳しくは、[プライマリフィールドの概要 ](/help/quicksilver/planning/fields/primary-field-overview.md) を参照してください。

1. レコードのプレビューのフィールド情報の編集を開始します。

   >[!TIP]
   >
   >  次のフィールドは読み取り専用で、Workfront によって自動的に更新されるので、情報を編集できません。
   >  
   >  * レコードタイプを接続して作成された他のレコードのルックアップフィールド。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
   >  * 次のタイプのフィールド：作成者、作成日、最終変更者、最終変更日、数式フィールド。

1. （任意） **カバーを追加** をクリックして、カバー画像をレコードに追加します。 詳細については、[ レコードにカバー画像を追加する ](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) を参照してください。

1. （オプション）サムネールアイコンの上にマウスポインターを置き、**詳細** メニュー ![ ](assets/more-menu.png)>**サムネールを編集** をクリックしてサムネール画像を追加します。 詳しくは、[レコードへのサムネールの追加](/help/quicksilver/planning/records/add-thumbnails-to-records.md)を参照してください。

   Workfront では、変更を自動的に保存します。

1. （任意）レコードのプレビューボックスの右上隅にある **リアルタイムインジケーター**![ リアルタイムインジケーターアイコン ](assets/real-time-indicator-icon.png) をクリックし、「**共同作業者を表示**」設定を有効にして、他のユーザーがリアルタイムで編集しているフィールドをハイライト表示します。

   レコードに同時にアクセスするすべてのユーザーの名前とアバターがこの領域に表示されます。

   この設定を無効にすると、アバターと名前はリアルタイムインジケーター領域にリストされ、編集中のフィールドはハイライト表示されません。

   ![ 時間インジケーターの展開されたレコードのプレビューボックス ](assets/real-time-indicator-expanded-record-preview-box.png)

1. （任意） **エクスポート** メニュー ![ レコードの詳細ページのエクスポートアイコン ](assets/export-icon-in-record-details-page.png) をクリックして、レコードの詳細をエクスポートします。 詳しくは、[ レコードの詳細の書き出し ](/help/quicksilver/planning/records/export-the-record-page.md) を参照してください。

1. （オプション）レコードのプレビューの右上隅にある **新しいタブで開く** アイコン ![ 新しいタブで詳細を開く ](assets/open-details-in-a-new-tab-icon.png) アイコン <!--check the icon; they are changing it--> 新しいタブでレコードのページを開く）をクリックします。 この記事の[レコードのページからレコードを編集](#edit-a-record-from-the-records-page)の節の説明に従って、レコードを引き続き編集します。

### レコードのページからレコードを編集

{{step1-to-planning}}

1. レコードを編集するワークスペースをクリックします

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 次のいずれかの操作を行います。

   * この記事の「[ レコードのプレビューからレコードを編集する ](#edit-a-record-from-the-records-preview-in-a-view)」の説明に従って、任意の表示からレコードのプレビューにアクセスし、レコードプレビューの右上隅にある **新しいタブで開く** アイコン ![ 新しいタブで詳細を開く ](assets/open-details-in-a-new-tab-icon.png) アイコン <!--check the icon; they are changing it--> をクリックして、レコードのページを新しいタブで開きます。

   * **テーブル** ビューで、レコードの名前にポインタを合わせ、**詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、**表示** をクリックします

     ![ レコード行のコンテキストメニュー ](assets/contextual-menu-for-record-row.png)

     レコードページが開きます。

     ![ 詳細ページ ](assets/details-page.png)

1. （オプション）レコードのタイトルの右側にある **詳細** メニューをクリックし、「名前を変更 **をクリックし** す。 これにより、レコードのタイトルとして表示されるフィールドが更新されます。

   レコードのタイトルは、テーブル表示で表示された場合、レコードのプライマリフィールドになります。 詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

1. レコードページの編集可能なフィールドをクリックして編集します。

   >[!TIP]
   >
   >  次のフィールドは読み取り専用で、Workfront によって自動的に更新されるので、情報を編集できません。
   >  
   >  * レコードタイプを接続して作成されるリンクフィールド。詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
   >  * 次のタイプのフィールド：作成者、作成日、最終変更者、最終変更日、数式フィールド。

1. （オプション）表示されるフィールドの右側にある情報アイコンをクリックして、フィールドの説明を表示します。
1. （任意）「**表紙を追加**」をクリックして、表紙画像をレコードに追加します

   または

   既存のカバー画像にポインタを合わせ、**その他** メニュー ![ その他メニュー ](assets/more-menu.png)/**アップロード** をクリックして、レコードの新しいカバー画像を追加します。

   詳細については、[ レコードにカバー画像を追加する ](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) を参照してください。

1. （オプション）既存のサムネールまたは **サムネールアイコン**![ 詳細ページでサムネールアイコンを記録 ](assets/record-thumbnail-icon-on-details-page.png) にポインタを合わせ、**詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png)/**サムネールを編集** をクリックして、レコードのサムネールを追加します。

   詳しくは、[ レコードへのサムネールの追加 ](/help/quicksilver/planning/records/add-thumbnails-to-records.md) を参照してください。

   Workfront では、変更を自動的に保存します。

1. （任意）レコードのページの右上隅にある **リアルタイムインジケーター**![ リアルタイムインジケーターアイコン ](assets/real-time-indicator-icon.png) をクリックし、「**共同作業者を表示**」設定を有効にして、他のユーザーがリアルタイムで編集しているフィールドをハイライト表示します。

   レコードに同時にアクセスするすべてのユーザーの名前とアバターがこの領域に表示されます。

   この設定を無効にすると、アバターと名前はリアルタイムインジケーター領域にリストされ、編集中のフィールドはハイライト表示されません。

   ![ リアルタイムインジケーターの展開されたレコードのプレビューボックス ](assets/real-time-indicator-expanded-record-preview-box.png)

1. （任意） **エクスポート** メニュー ![ レコードの詳細ページのエクスポートアイコン ](assets/export-icon-in-record-details-page.png) をクリックして、レコードの詳細をエクスポートします。 詳しくは、[ レコードの詳細の書き出し ](/help/quicksilver/planning/records/export-the-record-page.md) を参照してください。


## 計画セクションのWorkfrontオブジェクトからレコードを編集する

レコードをWorkfront オブジェクトに関連付けた後、オブジェクトの「計画」セクションから、Workfront内のWorkfront計画レコードを編集できます。

詳しくは、[Workfront オブジェクトからのレコード接続の管理 ](/help/quicksilver/planning/records/manage-records-in-planning-section.md) を参照してください。


<!--

<div class="preview">

## Add new choices to an existing select field when editing records in the table view

You can add new choices to an existing single- or multi-select field when editing records in the table view. 

>[!IMPORTANT]
>
>The functionality described in this section is available only in the table view. It is not available in any other areas where single- or multi-select fields display.


**EXAMPLE**

You might have a single-select field called Status that has the choices New and Closed, and you want to add a choice for an In progress status. You can add the choice by doing one of the following things:

* Editing the field. For information, see [Edit fields](/help/quicksilver/planning/fields/edit-fields.md)
* Adding a new option while editing the record in the table view, as described below. 


To add a new choice to an existing select field when editing a record: 

1. Go to a record type page and open the table view. 
1. Add the single- or multi-select field that you would like to add a choice to in the table view as a new column. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md). 
1. Start editing the field inline by double-clicking the cell for the field. 
1. Type the name of the choice you want to add, then click **Add choice**.

    ![Add choice in single-select field in table view](assets/add-choice-in-table-view-for-single-select-field.png)

    The new choice is added immediately to the single-select field. 

</div>

-->