---
title: レコードページの管理
description: Adobe Workfront Planning でレコードのプレビューとページのレイアウトを編集できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 24%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# レコードページの管理

{{maestro-important-intro}}

Adobe Workfront Planning でレコードのプレビューとページのレイアウトを編集できます。

レコードのプレビューは、レコードタイプのビューに表示される、レコードページの小さいビューです。

レコードのプレビューとページのレイアウトを変更すると、同じ種類のすべてのレコードのボックスとページに変更が反映されます。

レコードページの編集を開始する前に、レコードタイプとレコードを作成する必要があります。

詳しくは、次の記事を参照してください。

* [レコードタイプの作成](../architecture/create-record-types.md)

* [レコードの作成](/help/quicksilver/maestro/records/create-records.md)

## アクセス要件

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
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Adobe Workfront Planning ベータ版プログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス*</p></td>
   <td>
   <p>新規：ライト以上</p>
   または
   <p>現在：ワーク以上</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning にはアクセス制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する管理以上の権限</a> </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者またはグループ管理者が、レイアウトテンプレートにプランニング エリアを追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## レコードページの編集に関する考慮事項

* レコードのプレビューまたはページのフィールドを並べ替えると、そのタイプのすべてのレコードと、それらのレコードにアクセスするすべてのユーザーのフィールドが並べ替えられます。

* レコードのプレビューで行った表示の変更は、レコードの詳細ページにすぐに表示されます。 レコードページで加えた変更は、レコードプレビューボックスにも表示されます。

<!--Replace the first bullet with this when we add sections:

* The following changes affect all the records of the same type and are visible to all users accessing those records: 

   * Rearranging fields
   * Adding or removing sections
-->

* レコードにカバー画像を追加することが、レコードのプレビューまたはページの全体的なレイアウトの一部ではない。 各レコードに一意のカバー画像を追加できます。 詳しくは、を参照してください [レコードへのカバー画像の追加](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

<!--

## Add sections to a record preview or page

You can add sections to a record preview or page, to organize the information by common criteria and make it easier to find. 

Consider the following when adding sections to a record page:

* There is no limit to how many sections you can have on a page (***************IS THIS TRUE???***********)
* You cannot have an empty section. You must have at least one field in a section. 
* You can drag and drop fields from one section to another. 
* When you remove all the fields from a section, the section is automatically deleted and cannot be recovered. 

To add a section to a record preview or page: 

{{step1-to-maestro}}

The workspace that you access last opens. 

1. (Optional) Click the downward-pointing arrow to the right of the workspace name to select the workspace whose records you want to update. 
1. Click a record type card. 

    The record type page opens. 

1. From a view of any type, click the name of a record 

    Or 
    
    From the table table view, click the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of a record name. 
    
    The record's preview opens in the view.

    ![](assets/details-box.png) 

    >[!TIP]
    >
    >You can view the **Open details** icon to the left of the Name field of a record in a table view only when the Name field is a primary field. 

1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) (****************check the icon; they are changing it**********)  in the upper-right corner of the record preview  to open the record's page in a new tab. 

    The record page opens. 

    ![](assets/details-page.png)

1. In the record preview or page, hover over the white space to the left of the fields, then click the **Add section** icon ![](assets/add-section-icon.png) to add a section. 
1. Click inside the section's name and replace **Untitled** with a name, then click Enter. (************has this changed to Untitled section???**********)
1. Start dragging and dropping fields to the new section, as described in the section [Rearrange fields in the record preview or page](#rearrange-fields-in-the-record-preview-or-page) in this article. 

1. (Optional) Hover over the name of a section and click the **More** menu ![](assets/more-menu.png). 

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Optional) Do one of the following to edit the section: 

   * Click **Rename** to rename the section

      >[!TIP]
      >
      > You can rename a section inline, by clicking the name.
   
   * Click **Move up** to move the section up one position 

      Or 
      
      Click **Move down** to move the section down one position.
      All fields in the section move with the section. 

   * Click **Delete** to delete the section. The section is deleted and it cannot be recovered. All users accessing the records of this type will no longer view the deleted section. 

1. Click the downward-pointing arrow to the left of a section name to collapse it, or the right-pointing arrow  to expand it. 
   All sections are expanded by default. 

1. (Optional) Click the **grab** icon ![](assets/grab-icon.png) to the left of a section name, then drag and drop it in a desired spot. 

    The new position of the section updates in both the preview and the page of all records of the same type for all users viewing the records. 

    All changes to sections and field order are saved automatically. 

-->

## レコードのプレビューまたはページ内のフィールドの並べ替え

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. （オプション）ワークスペース名の右側にある下向き矢印をクリックして、レコードを更新するワークスペースを選択します。
1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意の種類のビューで、レコードの名前をクリックします

   または

   テーブル テーブル表示で、 **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) レコード名の左側。

   レコードのプレビューがビューで開きます。

   ![](assets/details-box.png)

   >[!TIP]
   >
   >を表示できます **詳細を開く** テーブル ビューで、[ 名前 ] フィールドがプライマリ フィールドの場合のみ、[ 名前 ] フィールドの左側にあるアイコンです。

1. （任意） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> レコードのプレビューの右上隅で、レコードのページを新しいタブで開きます。

   レコードページが開きます。

   ![](assets/details-page.png)

1. レコードのプレビューまたはページで、 **グラブ** アイコン ![](assets/grab-icon.png) フィールド名の左側で、目的の場所にドラッグ&amp;ドロップします。 <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   レコードを表示しているすべてのユーザーについて、同じタイプのすべてのレコードのプレビューとページの両方でフィールドの新しい位置が更新されます。

   レコードのプレビューまたはページのレイアウトに対するすべての変更が、自動的に保存されます。

