---
title: レコードのページレイアウトの管理
description: Adobe Workfront Planning でレコードのプレビューとページのレイアウトを編集できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '1872'
ht-degree: 9%

---


# レコードページレイアウトの管理

<span class="preview"> このページでハイライト表示されている情報は、まだ一般公開されていない機能を指しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning でレコードのプレビューとページのレイアウトを編集できます。

レコードのプレビューは、レコードタイプのビューに表示される、レコードページの小さいビューです。

レコードのプレビューおよびページのレイアウトを変更すると、同じ種類のすべてのレコードのプレビューボックスおよび詳細ページに変更が反映されます。

ここでは、レコードのプレビューボックスまたはレコード ページのレイアウトと外観を変更する方法について説明します。 レコードの編集方法については、「[ レコードの編集 ](/help/quicksilver/planning/records/edit-records.md)」を参照してください。

レコードページの編集を開始する前に、レコードタイプとレコードを作成する必要があります。

詳しくは、次の記事を参照してください。

* [レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)

* [レコードの作成](/help/quicksilver/planning/records/create-records.md)

## アクセス要件

+++ 展開してアクセス要件を表示します…

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
<p>任意</p>
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
   <td>
   <p>標準</p>
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
   <td>
   <p>ワークスペース <span class="preview"> およびレコードタイプ </span> に対する投稿以上の権限 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューの計画領域と、プロジェクト、ポートフォリオおよびプログラムの計画領域を含むレイアウトテンプレートを割り当てる必要があります。 </p> 詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">Adobe計画アクセスの概要 </a> を参照してください。 </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レコードページの編集に関する考慮事項

* デフォルトでは、レコードの詳細ページとプレビューページには、レコードに関連付けられているすべてのフィールドが表示されます。

* プレビューまたは詳細ページでは、レコードに新しいフィールドを追加することはできません。 プレビューページと詳細ページに表示するには、テーブル表示で新しいフィールドを追加する必要があります。

* レコードのプレビューまたは詳細ページにセクションを追加して、共通の条件で情報を整理し、見つけやすくすることができます。

* 次の変更は、同じタイプのすべてのレコードに影響し、それらのレコードにアクセスするすべてのユーザーに表示されます。

   * フィールドの並べ替え
   * セクションの追加または削除

* レコードのプレビューで行った表示の変更は、レコードの詳細ページにすぐに表示されます。 レコードページで加えた変更は、レコードプレビューボックスにも表示されます。

* レコードにカバー画像またはサムネールを追加することが、レコードのプレビューまたはページの全体的なレイアウトの一部ではない。 各レコードに一意のカバー画像またはサムネールを追加できます。 詳しくは、[ レコードへのカバー画像の追加 ](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) および [ レコードへのサムネールの追加 ](/help/quicksilver/planning/records/add-thumbnails-to-records.md) を参照してください。

## レコードのプレビューまたはページへのセクションの追加

レコードページにセクションを追加する場合は、次の点を考慮してください。

* ページ上に配置できるセクションの数に制限はありません。
* 空のセクションを指定することはできません。 セクションに少なくとも 1 つのフィールドが必要です。
* あるセクションから別のセクションにフィールドをドラッグ&amp;ドロップできます。 詳しくは、この記事の「レコードのプレビューまたは詳細ページのフィールドを並べ替える [ を参照し ](#rearrange-fields-in-the-record-preview-or-details-page) ください。
* セクションからすべてのフィールドを削除すると、そのセクションは自動的に削除され、元に戻すことはできません。

レコードのプレビューまたはページにセクションを追加するには：

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意のタイプのビューで、レコードの名前をクリックします

   または

   テーブルビューで、最初の列の **詳細を開く** アイコン ![ テーブル名フィールドで詳細を開くアイコン ](assets/open-details-icon-in-table-name-field.png) をクリックします。

   レコードのプレビューがビューで開きます。

   ![ 詳細ボックス ](assets/details-box.png)

1. （オプション）レコードプレビューの右上隅にある **新しいタブで開く** アイコン ![ 新しいタブで詳細を開くアイコン ](assets/open-details-in-a-new-tab-icon.png) 新しいタブでレコードのページを開く）をクリックします。

   レコードページが開きます。 「詳細」タブがデフォルトで開きます。

   ![ 詳細ページ ](assets/details-page.png)

1. レコードのプレビューまたはページの「**詳細**」タブで、フィールドの左側の空白にマウスポインターを置き、「**セクションを追加** アイコン ![ セクションを追加アイコン ](assets/add-section-icon.png) をクリックして、セクションを追加します。
1. セクション名の内側をクリックして **名称未設定セクション** を名前に置き換え、Enter キーを押します。 セクションの下に表示されるフィールドは、自動的に新しいセクションの一部になります。
1. この記事の「レコードのプレビューまたは詳細ページのフィールドの並べ替え [ の節で説明しているように、新しいセクションへのフィールドのドラッグ&amp;ドロップを開始し ](#rearrange-fields-in-the-record-preview-or-details-page) す。

1. （オプション）セクションの名前の上にマウスポインターを置いて、**詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックします。

   ![ レコードページのセクションのその他のメニューオプション ](assets/more-menu-options-for-section-on-record-page.png)
1. （オプション）次のいずれかの操作を行って、セクションを編集します。

   * **名前変更** をクリックして、セクションの名前を変更します

     >[!TIP]
     >
     > 名前をクリックすると、セクションの名前をインラインで変更できます。

   * **上へ移動** をクリックして、セクションを 1 つ上の位置に移動します

     または

     **下に移動** をクリックして、セクションを 1 つ下の位置に移動します。
セクション内のすべてのフィールドは、セクションと共に移動します。

   * **削除** をクリックして、セクションを削除します。 セクションは削除され、復元できません。 このタイプのレコードにアクセスするすべてのユーザーに、削除されたセクションが表示されなくなります。

1. セクション名の左側にある下向き矢印をクリックして折りたたむか、右向き矢印をクリックして展開します。
デフォルトでは、すべてのセクションが展開されます。

1. （オプション）セクション名の左側にある **グラブ** アイコン ![ グラブアイコン ](assets/grab-icon.png) をクリックし、目的の場所にドラッグ&amp;ドロップします。

   レコードを表示するすべてのユーザーに対して、同じタイプのすべてのレコードのプレビューとページの両方で、セクションの新しい位置が更新されます。

   セクションとフィールドの順序に対するすべての変更は、自動的に保存されます。

1. （オプション） **エクスポート** メニュー ![ レコードの詳細ページのエクスポートアイコン ](assets/export-icon-in-record-details-page.png) をクリックして、「詳細」タブを Word またはPDF ファイルにエクスポートします。 詳しくは、[ レコードの詳細のエクスポート ](/help/quicksilver/planning/records/export-the-record-page.md) を参照してください。

1. （オプション）「**詳細**」タブの横にある「**接続**」タブをクリックします。 場合によっては、[**接続**] タブをクリックする前に **詳細** をクリックする必要があります。

   選択したレコードに接続されているすべてのレコードまたはオブジェクトが、レコードタイプの名前または属するアプリケーションの名前の下に表示されます。

   ![Workfront Planning のレコードの「接続」タブ ](assets/connections-tab-on-record-in-workfront-planning.png)

1. （オプション）「接続」タブの右上隅にある「**すべてのレコードを表示**」設定を選択します。 接続されているレコードがまだないレコードも含め、すべての接続されているレコードタイプが表示されます。 デフォルトでは、切替スイッチは選択解除されており、接続されたレコードのないレコードタイプは非表示になっています。

1. （任意）接続されたレコードタイプにさらにレコードを追加するには、「**接続**」をクリックします。 詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

1. （オプション）レコードカードの上にマウスポインターを置き、「レコードを切断」アイコン（**-**）をクリックしてから「**切断**」をクリックします。 <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
次のことが発生します。
   * レコードがWorkfront オブジェクトに接続されなくなりました。
   * Workfront オブジェクトも、Workfront Planning からレコードの接続されたフィールドから削除されます。
   * 計画レコードに接続されているWorkfront参照フィールドの値も削除されます。

## レコードの「詳細」タブでフィールドを並べ替える

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意のタイプのビューで、レコードの名前をクリックします

   または

   テーブルビューで、最初の列の **詳細を開く** アイコン ![ テーブル名フィールドで詳細を開くアイコン ](assets/open-details-icon-in-table-name-field.png) をクリックします。

   レコードのプレビューがビューで開きます。

   ![ 詳細ボックス ](assets/details-box.png)

1. （オプション）レコードプレビューの右上隅にある **新しいタブで開く** アイコン ![ 新しいタブアイコンで詳細ボックスを開く ](assets/open-details-in-a-new-tab-icon.png)<!--check the icon; they are changing it--> をクリックして、レコードのページを新しいタブで開きます。

   レコードの **詳細** タブは、デフォルトで開きます。

   ![ 詳細ページ ](assets/details-page.png)

1. レコード **詳細** タブで、フィールド名の左側にある **グラブ** アイコン ![ グラブアイコン ](assets/grab-icon.png) をクリックしてから、目的の場所にドラッグ&amp;ドロップします。

   >[!TIP]
   >
   >フィールドは、別のセクションにドラッグ&amp;ドロップできます。
   >セクションに少なくとも 1 つのフィールドが必要です。
   >

   レコードを表示しているすべてのユーザーについて、同じタイプのすべてのレコードのプレビューとページの両方でフィールドの新しい位置が更新されます。

   レコードのプレビューまたはページのレイアウトに対するすべての変更が、自動的に保存されます。

## レコードのページに接続表示ページを追加する

<!--suggested a new name for this type of page: "Connected records details" - check to see if this changed-->

接続表示をレコードのページに追加する場合は、次の点に注意してください。

* 接続表示ページは、レコードのページに追加できます。

* レコードのプレビュー領域に接続表示ページを追加することはできません。

* 接続ビューページには、接続されている 1 つのレコードタイプのページがテーブルビューに表示されます。

* 接続表示ページをレコードのページに追加すると、レコードのプレビュー領域にページタブが表示されます。 接続されたレコードのテーブル表示を確認するには、完全ページに移動する必要があります。<!--this might have changed? check and take disclaimer out-->

接続表示ページを追加するには：

1. レコードページビューで、レコード名をクリックして開き、プレビューページの右上隅にある **新しいタブで開く** アイコン ![ 新しいタブで詳細を開くアイコン ](assets/open-details-in-a-new-tab-icon.png) をクリックします。
1. **ページを追加**/**接続表示** をクリックします。

   ![ 接続表示ページを追加モーダル ](assets/add-connection-view-page-modal.png)
1. **ページ名** を追加し、「**接続ビュー**」をクリックしてから、「**作成**」をクリックします。

   レコードのページに新しいタブが追加されます。
1. リスト内の接続済みレコードまたはオブジェクト タイプの名前を検索またはクリックします。
選択したレコードタイプのテーブルビューが表示され、接続されたレコードがテーブルビューに表示されます。
接続されたレコードのすべてのフィールドは、接続されたレコードのタブのテーブル表示に表示されます。

   接続されたレコードテーブルの最初の 5 つのフィールドは、デフォルトで表示されます。 デフォルトでは、参照フィールドは表示されません。

   テーブル表示は読み取り専用です。

   <!--replace screen shot below when additional capabilities come to the table view - Fields, etc-->

   ![ キャンペーンの詳細のオーディエンスに接続されたテーブル表示 ](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （オプション）タブの名前をダブルクリックします

   または

   タブの名前にポインタを合わせて、**その他** ![ その他メニュー ](assets/more-menu.png) をクリックしてから、**名前を変更** をクリックして、新しい [ 接続されたビュー ] タブに名前を変更します。
1. （オプション）ツールバーの次のビュー要素のいずれかを使用して、テーブルビューを管理します。

   * フィルター
   * 並べ替え
   * グループ化
   * フィールド（フィールドの表示、非表示、並べ替えを行う）

   詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

   >[!NOTE]
   >
   >   接続されたレコードのタブのテーブル表示のフィールドを作成、編集、削除することはできません。
   >

1. レコードを追加または削除するには、「**接続**」をクリックします。 詳しくは、「レコードの接続 [ を参照してください ](/help/quicksilver/planning/records/connect-records.md)
1. （オプション）「接続ビュー」タブの名前の上にマウスポインターを置き、**詳細**![ 詳細メニュー ](assets/more-menu.png) をクリックしてから **削除** をクリックして、新しい「接続ビュー」タブを削除します。




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



