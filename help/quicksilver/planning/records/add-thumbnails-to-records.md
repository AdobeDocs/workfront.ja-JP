---
title: レコードへのサムネールの追加
description: Adobe Workfront Planning でレコード情報を編集し、各レコードを個々のサムネールに関連付けて、容易に認識できるようにします。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 27%

---


# レコードにサムネールを追加する

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

レコードを Adobe Workfront Planning 内の一意のサムネールに関連付けて、容易に認識できるようにします。

レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。
詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

## アクセス要件

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td>   <p>ワークスペースおよびレコードタイプへの投稿以上の権限  </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
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
<p>Any </p> 
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
   <td><p> Standard </p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->


## レコードのサムネールに関する考慮事項

テーブルビュー内のレコードを視覚的に区別するために、各レコードに一意のサムネール画像を関連付けることができます。

次の点に注意してください。

* サムネールは 1 つのレコードに固有で、同じタイプのすべてのレコードには適用されません。
* サムネールとして追加できるのは、画像ファイルのみです。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* サムネール画像は、テーブル表示の個々のレコード、またはレコードのページやプレビューボックスから追加できます。
* Workfrontでは、レコードを作成するたびに、サムネール画像を自動的にアップロードします。 この画像は後で変更できます。
* サムネールはレコード情報に属し、レコードが表示される領域に表示されます。 例えば、次のエリアでは、レコード情報と共にサムネールが表示されます。

   * テーブルビューのレコードのプライマリフィールド
   * タイムライン表示上のレコードバー。
   * レコードの詳細プレビューとページ。

## レコードにサムネールを追加する

サムネールは次の方法で追加できます。

* [テーブル表示からのレコードへのサムネールの追加](#add-a-thumbnail-to-a-record-from-the-table-view)
* [詳細ページからのレコードへのサムネールの追加](#add-a-thumbnail-to-a-record-from-the-details-page)

### テーブル表示からのレコードへのサムネールの追加

{{step1-to-planning}}

1. サムネールを追加するレコードのワークスペースをクリックし、レコードタイプ カードをクリックします。

   レコードタイプページが開きます。
1. **表示**&#x200B;ドロップダウンメニューからテーブルビューを選択します。選択したタイプのすべてのレコードがテーブルに表示されます。
1. プライマリフィールド情報の上にマウスポインターを置き、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**サムネール** をクリックしてください。

   ![&#x200B; さらに記録メニューが展開されました &#x200B;](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   プライマリフィールドは、テーブルビューの最初の列に表示されるフィールドです。プライマリフィールドは常にフリーズされ、非表示や再配置はできません。 プライマリフィールドが式フィールドの場合、「詳細」メニューで「サムネール」オプションを使用できません。

   「**サムネールを記録** ボックスにデフォルトで **アップロード** タブが開きます。

   サムネールのアップロードについて詳しくは、この記事の [&#x200B; 詳細ページからレコードにサムネールを追加する &#x200B;](#add-a-thumbnail-to-a-record-from-the-details-page) の手順 6 から始まる節を参照してください。<!--see if this is accurate-->

<!--
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![Upload new image icon](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![Remove image icon](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![Record thumbnail box for gallery](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![More menu](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![Remove image icon](assets/remove-image-icon.png), then click **Save changes**. -->

### 詳細ページからのレコードへのサムネールの追加

{{step1-to-planning}}

1. サムネールを追加するレコードのワークスペースをクリックし、レコードタイプ カードをクリックします。

   レコードタイプページが開きます。
1. 任意のビューで、レコードをクリックして開きます。

   詳細プレビューボックスが表示されます。
1. （オプション）右上隅にある **新しいタブで開く** アイコン ![&#x200B; 詳細を新しいタブアイコンで開く &#x200B;](assets/open-details-in-a-new-tab-icon.png) をクリックします。

   レコードの詳細ページが開きます。

1. （条件付き）レコードのプレビューまたは詳細ページで、サムネール画像またはアイコン ![&#x200B; 詳細ページのサムネールアイコンを記録 &#x200B;](assets/record-thumbnail-icon-on-details-page.png) にカーソルを置き、レコード名の上のスペースにカーソルを置いて **サムネールを追加** または **サムネールを編集** をクリックします。

   「**サムネールを記録** ボックスにデフォルトで **アップロード** タブが開きます。

   ![&#x200B; アップロード用にサムネールボックスを記録する &#x200B;](assets/record-thumbnail-box-for-upload.png)

1. ファイルをドラッグ&amp;ドロップして、サムネールとして追加

   または

   **画像を参照**」をクリックして、追加する画像ファイルを参照します。 ファイルはお使いのコンピューターに保存しておく必要があります。

1. （任意）「サムネールを記録 **ボックスに画像をアップロードした後**、サイジングツールを使用して画像を切り抜き、サイズを変更します。
1. （オプション） **新しい画像をアップロード** アイコン ![&#x200B; 新しい画像をアップロード &#x200B;](assets/upload-new-image-icon.png) アイコンをクリックして、別の画像をアップロードします。
1. （オプション）「**ギャラリー**」タブをクリックして、画像をクリックします。 画像ギャラリーは変更できません。

   ![&#x200B; ギャラリーのサムネイル ボックスを記録する &#x200B;](assets/record-thumbnail-box-for-gallery.png)

1. （オプション）サムネールを保存前に削除するには、画像の右側にある **削除** アイコン ![&#x200B; 画像を削除アイコン &#x200B;](assets/remove-image-icon.png) をクリックします。

1. 「**画像を使用**」をクリックして、画像をサムネールとして追加します。
これにより、「サムネールを記録 **ボックスが閉じ** す。
サムネールは、レコードが表示されるWorkfront Planning の領域に表示されます。

   >[!TIP]
   >
   >   このビューにサムネールを表示するには、テーブル表示でサムネール フィールドを有効にする必要があります。 この機能は、デフォルトでは無効になっています。

1. （オプション）保存後にサムネールを削除するには、任意のビューのレコードをクリックして詳細ページを開き、サムネール画像にカーソルを置いて **詳細** メニュー ![&#x200B; 詳細メニューアイコン &#x200B;](assets/more-menu.png)>**削除** アイコン ![&#x200B; 削除アイコン &#x200B;](assets/remove-image-icon.png) をクリックします。 サムネール画像が削除されます。


<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![More menu](assets/more-menu.png), then click **Thumbnail**. 

   ![Record more menu expanded](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->
