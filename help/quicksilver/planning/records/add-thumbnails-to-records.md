---
title: レコードにサムネールを追加する
description: Adobe Workfront Planning でレコード情報を編集し、各レコードを個々のサムネールに関連付けて、容易に認識できるようにします。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: f5430d81f1914a3717130de3af54b4b84e0e2d06
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 39%

---

<!--update the metadata with real information-->

# レコードにサムネールを追加する

{{planning-important-intro}}

レコードを Adobe Workfront Planning 内の一意のサムネールに関連付けて、容易に認識できるようにします。

レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。
詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

## アクセス要件

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <p>現在：プラン</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Workfront Planning に対するアクセス制御はありません </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限の管理 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td>  <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

*詳細については、を参照してください [Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
1. プライマリフィールドの情報にポインタを合わせて、**その他**&#x200B;メニュー![](assets/more-menu.png)、**サムネール**&#x200B;の順にクリックします。

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   プライマリフィールドは、テーブルビューの最初の列に表示されるフィールドです。プライマリフィールドは常にフリーズされ、非表示や再配置はできません。 プライマリフィールドが式フィールドの場合、「詳細」メニューで「サムネール」オプションを使用できません。

   この **Upload** デフォルトでは、タブは次で開きます **サムネールを記録** ボックス。

   サムネールのアップロードについて詳しくは、「」を参照してください [詳細ページからのレコードへのサムネールの追加](#add-a-thumbnail-to-a-record-from-the-details-page) この記事では、手順 6 から開始します。 <!--see if this is accurate-->

<!--
   ![](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**. -->

### 詳細ページからのレコードへのサムネールの追加

{{step1-to-planning}}

1. サムネールを追加するレコードのワークスペースをクリックし、レコードタイプ カードをクリックします。

   レコードタイプページが開きます。
1. 任意のビューで、レコードをクリックして開きます。

   詳細プレビューボックスが表示されます。
1. （任意） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) 右上隅

   レコードの詳細ページが開きます。
1. サムネール画像またはアイコンにポインタを合わせる ![](assets/record-thumbnail-icon-on-details-page.png)を選択し、 **詳細** メニュー ![](assets/more-menu.png) > **サムネールを編集**.

   この **Upload** デフォルトでは、タブは次で開きます **サムネールを記録** ボックス。

   ![](assets/record-thumbnail-box-for-upload.png)

1. ファイルをドラッグ&amp;ドロップして、サムネールとして追加

   または

   クリック **画像の参照**&#x200B;を選択してから、追加する画像ファイルを探します。 ファイルはお使いのコンピューターに保存しておく必要があります。

1. （任意）に画像をアップロードした後 **サムネールを記録** ボックスで、サイジングツールを使用して画像を切り抜き、サイズを変更します。
1. （任意） **新しい画像をアップロード** アイコン ![](assets/upload-new-image-icon.png) 別の画像をアップロードします。
1. （任意） **ギャラリー** タブをクリックしてから、画像をクリックします。 画像ギャラリーは変更できません。

   ![](assets/record-thumbnail-box-for-gallery.png)

1. （オプション）サムネールを保存する前に削除するには、をクリックします **削除** アイコン ![](assets/remove-image-icon.png) 画像の右側。

1. 「**画像を使用**」をクリックして、画像をサムネールとして追加します。
これにより、が閉じます **サムネールを記録** ボックス。
サムネールは、レコードが表示されるWorkfront Planning の領域に表示されます。

   >[!TIP]
   >
   >   このビューにサムネールを表示するには、テーブル表示でサムネール フィールドを有効にする必要があります。 この機能は、デフォルトでは無効になっています。

1. （オプション）保存後にサムネールを削除するには、任意のビューのレコードをクリックして詳細ページを開き、サムネール画像の上にマウスポインターを置いて「 **詳細** メニュー ![](assets/more-menu.png)> **削除** アイコン ![](assets/remove-image-icon.png). サムネール画像が削除されます。




<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->