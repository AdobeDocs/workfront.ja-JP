---
title: レコードページの管理
description: Adobe Workfront Planning でレコードのプレビューとページのレイアウトを編集できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 20%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# レコードページの管理

{{planning-important-intro}}

Adobe Workfront Planning でレコードのプレビューとページのレイアウトを編集できます。

レコードのプレビューは、レコードタイプのビューに表示される、レコードページの小さいビューです。

レコードのプレビューおよびページのレイアウトを変更すると、同じ種類のすべてのレコードのプレビューボックスおよび詳細ページに変更が反映されます。

ここでは、レコードのプレビューボックスまたはレコード ページのレイアウトと外観を変更する方法について説明します。 レコードの編集方法については、を参照してください [レコードを編集](/help/quicksilver/planning/records/edit-records.md).

レコードページの編集を開始する前に、レコードタイプとレコードを作成する必要があります。

詳しくは、次の記事を参照してください。

* [レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)

* [レコードの作成](/help/quicksilver/planning/records/create-records.md)

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
   <p>新規：ライト以上</p>
   または
   <p>現在：ワーク以上</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning に対するアクセス制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する管理以上の権限</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者やグループ管理者は、レイアウトテンプレートに Planning エリアを追加する必要があります。詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## レコードページの編集に関する考慮事項

* デフォルトでは、レコードの詳細ページとプレビューページには、レコードに関連付けられているすべてのフィールドが表示されます。

* プレビューまたは詳細ページでは、レコードに新しいフィールドを追加することはできません。 プレビューページと詳細ページに表示するには、テーブル表示で新しいフィールドを追加する必要があります。

* レコードのプレビューまたは詳細ページにセクションを追加して、共通の条件で情報を整理し、見つけやすくすることができます。

* 次の変更は、同じタイプのすべてのレコードに影響し、それらのレコードにアクセスするすべてのユーザーに表示されます。

   * フィールドの並べ替え
   * セクションの追加または削除

* レコードのプレビューで行った表示の変更は、レコードの詳細ページにすぐに表示されます。 レコードページで加えた変更は、レコードプレビューボックスにも表示されます。

* レコードにカバー画像を追加することが、レコードのプレビューまたはページの全体的なレイアウトの一部ではない。 各レコードに一意のカバー画像を追加できます。 詳しくは、を参照してください [レコードへのカバー画像の追加](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

## レコードのプレビューまたはページへのセクションの追加

レコードページにセクションを追加する場合は、次の点を考慮してください。

* ページ上に配置できるセクションの数に制限はありません。
* 空のセクションを指定することはできません。 セクションに少なくとも 1 つのフィールドが必要です。
* あるセクションから別のセクションにフィールドをドラッグ&amp;ドロップできます。 詳しくは、セクションを参照してください [レコードのプレビューまたは詳細ページでのフィールドの並べ替え](#rearrange-fields-in-the-record-preview-or-details-page) この記事の内容です。
* セクションからすべてのフィールドを削除すると、そのセクションは自動的に削除され、元に戻すことはできません。

レコードのプレビューまたはページにセクションを追加するには：

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意のタイプのビューで、レコードの名前をクリックします

   または

   テーブル テーブル表示で、 **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) レコード名の左側。

   レコードのプレビューがビューで開きます。

   ![](assets/details-box.png)

   >[!TIP]
   >
   >「名前」フィールドがプライマリフィールドである場合にのみ、テーブルビューでレコードの「名前」フィールドの左側に&#x200B;**詳細を開く**&#x200B;アイコンを表示できます。

1. （任意） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) レコードのプレビューの右上隅で、レコードのページを新しいタブで開きます。

   レコードページが開きます。

   ![](assets/details-page.png)

1. レコードのプレビューまたはページで、フィールドの左側の空白にポインタを合わせて、 **セクションを追加** アイコン ![](assets/add-section-icon.png) セクションを追加します。
1. セクションの名前の内側をクリックして置換 **無題のセクション** 名前を指定して、「Enter」をクリックします。 セクションの下に表示されるフィールドは、自動的に新しいセクションの一部になります。
1. 「」の説明に従って、フィールドの新しいセクションへのドラッグ&amp;ドロップを開始します [レコードのプレビューまたは詳細ページでのフィールドの並べ替え](#rearrange-fields-in-the-record-preview-or-details-page) この記事の内容です。

1. （オプション）セクションの名前の上にマウスポインターを置いて、 **詳細** メニュー ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. （オプション）次のいずれかの操作を行って、セクションを編集します。

   * クリック **名前を変更** セクションの名前を変更するには

     >[!TIP]
     >
     > 名前をクリックすると、セクションの名前をインラインで変更できます。

   * クリック **上に移動** 断面を 1 つ上の位置に移動するには

     または

     クリック **下に移動** をクリックして、断面を 1 つ下の位置に移動します。
セクション内のすべてのフィールドは、セクションと共に移動します。

   * クリック **削除** セクションを削除します。 セクションは削除され、復元できません。 このタイプのレコードにアクセスするすべてのユーザーに、削除されたセクションが表示されなくなります。

1. セクション名の左側にある下向き矢印をクリックして折りたたむか、右向き矢印をクリックして展開します。
デフォルトでは、すべてのセクションが展開されます。

1. （任意） **グラブ** アイコン ![](assets/grab-icon.png) セクション名の左側で、目的の場所にドラッグ&amp;ドロップします。

   レコードを表示するすべてのユーザーに対して、同じタイプのすべてのレコードのプレビューとページの両方で、セクションの新しい位置が更新されます。

   セクションとフィールドの順序に対するすべての変更は、自動的に保存されます。

## レコードのプレビューまたは詳細ページでのフィールドの並べ替え

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意のタイプのビューで、レコードの名前をクリックします

   または

   テーブル テーブル表示で、 **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) レコード名の左側。

   レコードのプレビューがビューで開きます。

   ![](assets/details-box.png)

   >[!TIP]
   >
   >「名前」フィールドがプライマリフィールドである場合にのみ、テーブルビューでレコードの「名前」フィールドの左側に&#x200B;**詳細を開く**&#x200B;アイコンを表示できます。

1. （任意） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> レコードのプレビューの右上隅で、レコードのページを新しいタブで開きます。

   レコードページが開きます。

   ![](assets/details-page.png)

1. レコードのプレビューまたはページで、 **グラブ** アイコン ![](assets/grab-icon.png) フィールド名の左側で、目的の場所にドラッグ&amp;ドロップします。 <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   レコードを表示しているすべてのユーザーについて、同じタイプのすべてのレコードのプレビューとページの両方でフィールドの新しい位置が更新されます。

   レコードのプレビューまたはページのレイアウトに対するすべての変更が、自動的に保存されます。

