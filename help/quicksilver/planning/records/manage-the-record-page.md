---
title: レコードのページレイアウトの管理
description: Adobe Workfront Planning でレコードのプレビューとページのレイアウトを編集できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '2262'
ht-degree: 4%

---


# レコードページレイアウトの管理

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning でレコードのプレビューとページのレイアウトを編集できます。

レコードのプレビューは、レコードタイプのビューに表示される、レコードページの小さいビューです。

レコードのプレビューおよびページのレイアウトを変更すると、同じ種類のすべてのレコードのプレビューボックスおよび詳細ページに変更が反映されます。

ここでは、レコードのプレビューボックスまたはレコード ページのレイアウトと外観を変更する方法について説明します。 レコードの編集方法については、「[&#x200B; レコードの編集 &#x200B;](/help/quicksilver/planning/records/edit-records.md)」を参照してください。

レコードページの編集を開始する前に、レコードタイプとレコードを作成する必要があります。

詳しくは、次の記事を参照してください。

* [レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)

* [レコードの作成](/help/quicksilver/planning/records/create-records.md)

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontと任意の Planning パッケージ</p>
<p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <p>ワークスペースおよびレコードタイプへの投稿以上の権限 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> 
  </td>
  </tr>   
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   


<!--Old:
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td>
   <td>
<p>Any</p>
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->

## レコードページの編集に関する考慮事項

* デフォルトでは、レコードの詳細ページとプレビューページには、レコードに関連付けられているすべてのフィールドが表示されます。

* プレビューまたは詳細ページでは、レコードに新しいフィールドを追加することはできません。 プレビューページと詳細ページに表示するには、テーブル表示で新しいフィールドを追加する必要があります。

* レコードのプレビューまたは詳細ページにセクションを追加して、共通の条件で情報を整理し、見つけやすくすることができます。

* 次の変更は、同じタイプのすべてのレコードに影響し、それらのレコードにアクセスするすべてのユーザーに表示されます。

   * フィールドの並べ替え
   * セクションの追加または削除

* レコードのプレビューで行った表示の変更は、レコードの詳細ページにすぐに表示されます。 レコードページで加えた変更は、レコードプレビューボックスにも表示されます。

* レコードにカバー画像またはサムネールを追加することが、レコードのプレビューまたはページの全体的なレイアウトの一部ではない。 各レコードに一意のカバー画像またはサムネールを追加できます。 詳しくは、[&#x200B; レコードへのカバー画像の追加 &#x200B;](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) および [&#x200B; レコードへのサムネールの追加 &#x200B;](/help/quicksilver/planning/records/add-thumbnails-to-records.md) を参照してください。

## レコードのプレビューまたはページへのセクションの追加

レコードページにセクションを追加する場合は、次の点を考慮してください。

* ページ上に配置できるセクションの数に制限はありません。
* 空のセクションを指定することはできません。 セクションに少なくとも 1 つのフィールドが必要です。
* あるセクションから別のセクションにフィールドをドラッグ&amp;ドロップできます。 詳しくは、この記事の「レコードのプレビューまたは詳細ページのフィールドを並べ替える [&#x200B; を参照し &#x200B;](#rearrange-fields-in-the-record-preview-or-details-page) ください。
* セクションからすべてのフィールドを削除すると、そのセクションは自動的に削除され、元に戻すことはできません。

レコードのプレビューまたはページにセクションを追加するには：

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意のタイプのビューで、レコードの名前をクリックします

   または

   テーブルビューで、最初の列の **詳細を開く** アイコン ![&#x200B; テーブル名フィールドで詳細を開くアイコン &#x200B;](assets/open-details-icon-in-table-name-field.png) をクリックします。

   レコードのプレビューがビューで開きます。

   ![&#x200B; 詳細ボックス &#x200B;](assets/details-box.png)

1. （オプション）レコードプレビューの右上隅にある **新しいタブで開く** アイコン ![&#x200B; 新しいタブで詳細を開くアイコン &#x200B;](assets/open-details-in-a-new-tab-icon.png) 新しいタブでレコードのページを開く）をクリックします。

   レコードページが開きます。 「詳細」タブがデフォルトで開きます。

   ![&#x200B; 詳細ページ &#x200B;](assets/details-page.png)

1. レコードのプレビューまたはページの「**詳細**」タブで、フィールドの左側の空白にマウスポインターを置き、「**セクションを追加** アイコン ![&#x200B; セクションを追加アイコン &#x200B;](assets/add-section-icon.png) をクリックして、セクションを追加します。
1. セクション名の内側をクリックして **名称未設定セクション** を名前に置き換え、Enter キーを押します。 セクションの下に表示されるフィールドは、自動的に新しいセクションの一部になります。
1. この記事の「レコードのプレビューまたは詳細ページのフィールドの並べ替え [&#x200B; の節で説明しているように、新しいセクションへのフィールドのドラッグ&amp;ドロップを開始し &#x200B;](#rearrange-fields-in-the-record-preview-or-details-page) す。

1. （オプション）セクションの名前の上にマウスポインターを置いて、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックします。

   ![&#x200B; レコードページのセクションのその他のメニューオプション &#x200B;](assets/more-menu-options-for-section-on-record-page.png)
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

1. （オプション）セクション名の左側にある **グラブ** アイコン ![&#x200B; グラブアイコン &#x200B;](assets/grab-icon.png) をクリックし、目的の場所にドラッグ&amp;ドロップします。

   レコードを表示するすべてのユーザーに対して、同じタイプのすべてのレコードのプレビューとページの両方で、セクションの新しい位置が更新されます。

   セクションとフィールドの順序に対するすべての変更は、自動的に保存されます。

1. （オプション） **エクスポート** メニュー ![&#x200B; レコードの詳細ページのエクスポートアイコン &#x200B;](assets/export-icon-in-record-details-page.png) をクリックして、「詳細」タブを Word またはPDF ファイルにエクスポートします。 詳しくは、[&#x200B; レコードの詳細のエクスポート &#x200B;](/help/quicksilver/planning/records/export-the-record-page.md) を参照してください。

1. （オプション）「**詳細**」タブの横にある「**接続**」タブをクリックします。 場合によっては、[**接続**] タブをクリックする前に **詳細** をクリックする必要があります。

   選択したレコードに接続されているすべてのレコードまたはオブジェクトが、レコードタイプの名前または属するアプリケーションの名前の下に表示されます。

   ![Workfront Planning のレコードの「接続」タブ &#x200B;](assets/connections-tab-on-record-in-workfront-planning.png)

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

   テーブルビューで、最初の列の **詳細を開く** アイコン ![&#x200B; テーブル名フィールドで詳細を開くアイコン &#x200B;](assets/open-details-icon-in-table-name-field.png) をクリックします。

   レコードのプレビューがビューで開きます。

   ![&#x200B; 詳細ボックス &#x200B;](assets/details-box.png)

1. （オプション）レコードプレビューの右上隅にある **新しいタブで開く** アイコン ![&#x200B; 新しいタブアイコンで詳細ボックスを開く &#x200B;](assets/open-details-in-a-new-tab-icon.png)<!--check the icon; they are changing it--> をクリックして、レコードのページを新しいタブで開きます。

   レコードの **詳細** タブは、デフォルトで開きます。

   ![&#x200B; 詳細ページ &#x200B;](assets/details-page.png)

1. レコード **詳細** タブで、フィールド名の左側にある **グラブ** アイコン ![&#x200B; グラブアイコン &#x200B;](assets/grab-icon.png) をクリックしてから、目的の場所にドラッグ&amp;ドロップします。

   >[!TIP]
   >
   >フィールドは、別のセクションにドラッグ&amp;ドロップできます。
   >セクションに少なくとも 1 つのフィールドが必要です。
   >

   レコードを表示しているすべてのユーザーについて、同じタイプのすべてのレコードのプレビューとページの両方でフィールドの新しい位置が更新されます。

   レコードのプレビューまたはページのレイアウトに対するすべての変更が、自動的に保存されます。

## 接続されたレコード ページをレコードに追加する

接続されたレコード ページのタブをレコードに追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。 これにより、テーブル表示の接続されたレコードがタブに追加されます。

「接続済みレコード」ページをレコードに追加する場合は、次の点を考慮してください。

* レコード タイプのテーブル ビューからレコード タイプにレコード タイプまたはオブジェクト タイプを接続した後に、[ 接続されたレコード ] ページをレコードに追加できます。

* レコードのプレビュー領域またはレコードのページから、「接続済みレコード」ページを追加できます。

* 接続されたレコード・ページには、接続されたオブジェクトまたは 1 つのオブジェクトまたはレコード・タイプのレコードのみがテーブル・ビューに表示されます。 ページには、そのタイプのすべてのレコードが表示されるわけではありません。

* 以下の接続されたレコードまたはオブジェクト タイプに対して、接続されたレコード ページを追加できます。

   * Workfront計画レコードタイプ
   * Workfront プロジェクト、プログラム、ポートフォリオ、グループまたは会社。 Connected Workfront オブジェクトは、Workfrontでアクセスする権限を持っていない場合でも表示できます。

  >[!NOTE]
  >
  > 接続されたAEM Assets レコードに対して、「接続されたレコード」ページを追加することはできません。

接続レコード ページを追加するには：

1. レコード名をクリックすると、レコードタイプページの任意のビューからレコードが開きます。
1. 次のいずれかの領域で **ページを追加** をクリックします。

   * レコードのプレビューウィンドウ
   * レコードの詳細ページ。プレビューページの右上隅にある **新しいタブで開く** アイコン ![&#x200B; 新しいタブで詳細を開くアイコン &#x200B;](assets/open-details-in-a-new-tab-icon.png) をクリックします。

   **ページを作成** ボックスが開きます。

   ![&#x200B; 接続されたレコードを追加ページモーダル &#x200B;](assets/add-connection-view-page-modal.png)

1. **ページ名** を追加し、「**接続されたレコードページ**」をクリックしてから、「**作成**」をクリックします。

   新しく接続されたレコードページが、新しいタブとしてレコードのページに追加されます。

   現在のレコードに接続されているレコードがテーブルビューに表示されます。

   >[!TIP]
   >
   >接続レコード ページに表示するには、レコードのテーブル領域または詳細領域に接続レコードを追加する必要があります。

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   接続されたレコードの最初の 5 つのフィールドは、デフォルトで表示されます。<!--No lookup fields display by default.-->

   ![&#x200B; キャンペーンの詳細のオーディエンスに接続されたテーブル表示 &#x200B;](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （オプション）リスト内の接続されたレコードまたはオブジェクトタイプの名前を検索またはクリックします。

1. （オプションおよび条件付き）接続された Planning レコードまたはプロジェクト以外のWorkfrontオブジェクトを表示する場合は、接続されたレコード・ページのテーブル・ビューで、次のいずれかの操作を行います。<!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * レコードの名前をクリックします。 レコードのページが新しいタブで開きます。

   * テーブル ビューの下部にある [**接続**] をクリックしてさらにレコードを接続し、接続ボックスの外側をクリックしてレコードを閉じます。 新しいレコードが自動的にテーブルに追加されます。

     詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
   * テーブル表示で、接続されたレコードからの情報をインラインで編集します。

   * 接続されているレコードの名前にポインタを合わせ、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックします

     または

     レコードの 1 つを選択し、リストの下部にある青いバーで次のいずれかのオプションをクリックします。

      * **表示**：レコードページを新しいタブで開きます
      * **リンクをコピー** レコードページへのリンクをコピーする
      * **サムネールを編集** して「サムネールを記録 **ボックスを開き、レコードのサムネール画像を編集します**
      * **複製**：接続されたレコードを複製します。 複製されたレコードは、現在のレコードにも接続されます。
      * 接続されたレコードタイプに新しいレコードを追加するには、**上または下にレコードを挿入** します。 ここに追加された新しいレコードも、現在のレコードに接続されます。 このオプションは、テーブルでレコードを選択する際に青いバーでは使用できません。
      * **削除**：レコードを削除します。 接続されたレコードを削除すると、そのレコードの種類と、レコードが接続されているすべての場所からレコードが削除されます。

     テーブルビューでのレコードの編集については、[&#x200B; レコードの編集 &#x200B;](/help/quicksilver/planning/records/edit-records.md) を参照してください。

         >[!TIP]
         >
         > 複数のレコードまたはオブジェクトを選択して削除できます。
     
   * 接続されたレコード ページのテーブル内の任意の Planning レコードをインライン編集します。

     その他のWorkfront オブジェクトは、読み取り専用のテーブルビューで表示され、編集することはできません。

1. （オプションおよび条件付き）接続されたレコードページのテーブルビューで、接続されたWorkfront プロジェクトを表示する際に、次のいずれかの操作を行います。

   * 接続されたレコードページの右上隅にある「**レコードを接続**」をクリックして、既存のプロジェクトを接続します。

   詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
   * テーブル内のインライン編集プロジェクト情報。
   * **新しい行** をクリックして、テンプレートを使用せずにプロジェクトを作成します。 新しいプロジェクトは、現在のレコードにすぐに接続されます。

     詳しくは、[&#x200B; レコードに関連付ける際に、Workfront Planning からWorkfront オブジェクトを作成する &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) を参照してください。
   * プロジェクトの上にマウスポインターを置き、**詳細** メニュー [&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてください

     または

     1 つ以上のプロジェクトを選択し、リストの下部にある青いバーに注目して、次のいずれかをクリックします。

      * **削除**：プロジェクトを削除します。 プロジェクトを削除すると、レコードから切断され、Workfrontのごみ箱に移動されます。
      * **切断**：レコードからプロジェクトを切断します。 プロジェクトの接続を解除すると、プロジェクトとその参照フィールドのすべての値が現在のレコードから削除されます。

1. （オプション）「**接続されたレコード」ページ** タブの名前をダブルクリックします

   または

   タブの名前にポインタを合わせて、**その他** ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**名前を変更** をクリックして、新しい [ 接続されたビュー ] タブに名前を変更します。
1. （オプション）接続されたレコードページのツールバーで次のビュー要素のいずれかを使用して、テーブルビューを管理します。

   * フィルター
   * 並べ替え
   * グループ化
   * フィールド（フィールドの表示、非表示、並べ替えを行う）
   * 行の高さ
   * 検索

   詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

   >[!NOTE]
   >
   >接続されたレコードのタブのテーブル表示のフィールドを作成、編集、削除することはできません。

1. （オプション）接続されたレコードページのタブの名前にポインタを合わせ、「**詳細**![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、「**削除**」をクリックしてタブを削除します。

<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



