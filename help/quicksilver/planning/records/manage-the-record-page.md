---
title: レコードのページレイアウトの管理
description: Adobe Workfront Planning でレコードのプレビューとページのレイアウトを編集できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '2395'
ht-degree: 5%

---


# レコードページレイアウトの管理

<span class="preview"> このページでハイライト表示されている情報は、まだ一般公開されていない機能を指しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

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
<ul> 
<li><p>任意のWorkfrontと任意の Planning パッケージ</p></li>
または
<li><p>任意のワークフローおよび任意の計画パッケージ</p></li></ul>
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

接続されたレコード ページのタブをレコードに追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。

接続されたレコードの情報は、テーブルビューで編集できます。 別のアプリケーションから接続されたオブジェクトの情報は、テーブルビューでは編集できません。

「接続済みレコード」ページをレコードに追加する場合は、次の点を考慮してください。

* レコード タイプのテーブル ビューからレコード タイプにレコード タイプまたはオブジェクト タイプを接続した後に、[ 接続されたレコード ] ページをレコードに追加できます。

* 実稼動環境では、レコードのプレビューから「接続されたレコード」ページを追加することはできません。

  <span class="preview"> プレビュー環境のレコードのプレビューから、「接続されたレコード」ページを追加できます。</span>

* 接続されたレコード・ページには、接続されたオブジェクトまたは 1 つのオブジェクトまたはレコード・タイプのレコードのみがテーブル・ビューに表示されます。 テーブルビューでは、そのタイプのすべてのレコードがページに表示されるわけではありません。

* 使用する環境によっては、次の点に注意してください。

   * 実稼動環境では、接続済みレコード ページをレコードに追加すると、レコードのプレビュー領域に「ページ」タブが表示されますが、空です。 接続されたレコードのテーブル表示を確認するには、完全ページに移動する必要があります。
   * <span class="preview"> プレビュー環境では、接続されたレコード ページが、レコードのプレビュー領域とブラウザータブの両方から表示されます。</span>

* 以下の接続されたレコードまたはオブジェクト タイプに対して、接続されたレコード ページを追加できます。

   * Workfront計画レコードタイプ
   * Workfront プロジェクト、プログラム、ポートフォリオ、グループまたは会社。 Connected Workfront オブジェクトは、Workfrontでアクセスする権限を持っていない場合でも表示できます。

  >[!NOTE]
  >
  >   接続されたAEM Assets レコードに対して、「接続されたレコード」ページを追加することはできません。

接続レコード ページを追加するには：

1. レコードの名前をクリックして開きます。
1. 次のいずれかの領域で **ページを追加** をクリックします。

   * <span class="preview"> レコードのプレビューウィンドウ </span>
   * レコードの詳細ページ。プレビューページの右上隅にある **新しいタブで開く** アイコン ![&#x200B; 新しいタブで詳細を開くアイコン &#x200B;](assets/open-details-in-a-new-tab-icon.png) をクリックします。

   **ページを作成** ボックスが開きます。

   ![&#x200B; 接続されたレコードを追加ページモーダル &#x200B;](assets/add-connection-view-page-modal.png)

1. **ページ名** を追加し、「**接続されたレコードページ**」をクリックしてから、「**作成**」をクリックします。

   レコードのページに新しいタブが追加されます。
1. リスト内の接続済みレコードまたはオブジェクト タイプの名前を検索またはクリックします。
選択したレコードタイプのテーブルビューが新しいページに表示され、接続されたレコードがテーブルビューに表示されます。
接続されたレコードのすべてのフィールドは、接続されたレコードのタブのテーブル表示に表示されます。

   接続されたレコードテーブルの最初の 5 つのフィールドは、デフォルトで表示されます。 デフォルトでは、参照フィールドは表示されません。

   ![&#x200B; キャンペーンの詳細のオーディエンスに接続されたテーブル表示 &#x200B;](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （オプション）接続されたレコードのテーブル表示で、次のいずれかの操作を行います。

   * レコードの名前をクリックします。 レコードのページが新しいタブで開きます。

     これにより、レコードのプレビューページが開きます。 右上隅の **新しいタブで開く** アイコン ![&#x200B; 新しいタブで開くアイコン &#x200B;](assets/open-details-in-a-new-tab-icon.png) をクリックして、接続されたレコードのページを開きます。

   * **接続** をクリックしてさらにレコードを接続し、接続ボックスの外側をクリックして接続ボックスを閉じます。 新しいレコードが自動的にテーブルに追加されます。
   * テーブルビュー内で接続されたレコードの情報を編集します。

   * 接続されているレコードの名前にポインタを合わせ、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、次のいずれかのオプションをクリックします。
      * 表示
      * リンクをコピー
      * サムネールを編集
      * 複製
      * 上または下にレコードを挿入
      * 削除
   * レコードの 1 つを選択し、画面の下部にある青いバーで次のいずれかのオプションをクリックします。
      * 表示
      * リンクをコピー
      * サムネールを編集
      * 複製
      * 削除。 複数のレコードを選択する場合は、「削除」オプションのみを使用できます。

     テーブルビューでのレコードの編集については、[&#x200B; レコードの編集 &#x200B;](/help/quicksilver/planning/records/edit-records.md) を参照してください。

   * 接続されたレコード ページのテーブル内の任意のレコードをインライン編集します。

     実稼動環境では、すべてのWorkfront オブジェクトが読み取り専用のテーブルビューに表示され、編集できません。

     <span class="preview"> プレビュー環境では、接続されたレコードページでプロジェクトをインライン編集できます。</span>

1. <span class="preview"> （条件付き）接続されたプロジェクトのリストを表示する場合、次のいずれかの操作をおこないます。</span>

   * <span class="preview"> 接続されたレコードページの右上隅にある **レコードを接続** をクリックして、既存のプロジェクトを接続します。</span>
   * <span class="preview"> テーブル内のインライン編集プロジェクト情報。</span>
   * <span class="preview">**新規行** をクリックして、テンプレートを使用せずにプロジェクトを作成します。 新しいプロジェクトは、現在のレコードにすぐに接続されます。</span>

     詳しくは、[&#x200B; レコードに関連付ける際に、Workfront Planning からWorkfront オブジェクトを作成する &#x200B;](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) を参照してください。
   * <span class="preview"> プロジェクトの上にマウスポインターを置いて **詳細** メニュー [&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックし、次のいずれかをクリックします。</span>
      * <span class="preview">**削除**：プロジェクトを削除します。 プロジェクトを削除すると、レコードから切断され、Workfrontのごみ箱に移動されます。</span>
      * <span class="preview">**切断**：レコードからプロジェクトを切断します。 プロジェクトの接続を解除すると、プロジェクトとその参照フィールドのすべての値が現在のレコードから削除されます。</span>

1. （オプション）「接続されたレコード」ページタブの名前をダブルクリックします

   または

   タブの名前にポインタを合わせて、**その他** ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**名前を変更** をクリックして、新しい [ 接続されたビュー ] タブに名前を変更します。
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

1. （条件付き）より多くのレコードまたはオブジェクトを接続するには、次のいずれかの操作を行います。

   * テーブルの下部にある「**接続**」をクリックして、レコードやWorkfront オブジェクト <span class="preview"> プロジェクトを除く </span> を追加または削除します。
   * <span class="preview"> プレビュー環境で、接続されたレコードページの右上隅にある **レコードを接続** をクリックして既存のプロジェクトを接続するか、テーブルの下部にある **新しい行** をクリックしてプロジェクトを作成し、自動的に現在のレコードに接続します。</span>

   詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
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



