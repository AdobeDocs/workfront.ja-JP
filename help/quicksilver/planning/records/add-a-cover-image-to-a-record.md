---
title: レコードへのカバー画像の追加
description: レコードの編集時に、Adobe Workfront Planning のレコード・ページに表紙を追加することで、レコードをパーソナライズできます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 23%

---


<!--update the metadata with real information-->

# レコードへのカバー画像の追加

{{planning-important-intro}}

レコードの編集時に、Adobe Workfront Planning のレコード・ページに表紙を追加することで、レコードをパーソナライズできます。

レコードの編集方法については、を参照してください [レコードを編集](/help/quicksilver/planning/records/edit-records.md).

レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。

詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

## アクセス要件

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding cover images-->

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
   <p>現在：ワーク以上</p>
   <p>新規：標準</p>  
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

## レコードページの表紙画像に関する考慮事項

表紙画像を追加して、レコードのページをパーソナライズできます。

次の点に注意してください。

* カバー画像は、1 つのレコードに固有で、同じタイプのすべてのレコードには適用されません。
* カバー画像として追加できるのは画像ファイルのみです。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 任意のビューのレコードプレビューまたはレコードページから、カバー画像を個々のレコードに追加できます。
* レコード ビューからカバー画像を追加することはできません。
* Workfrontは、レコードを作成するたびに、カバー画像を自動的にアップロードします。 この画像は後で変更できます。

## レコードへのカバー画像の追加

レコードのプレビューまたはページの上部にカバー画像を追加して、レコードをパーソナライズできます。

{{step1-to-planning}}

1. レコードをパーソナライズするワークスペースをクリックします。

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開し、レコードをパーソナライズするワークスペースを選択します。

   ワークスペースが開き、レコードタイプが表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意の種類のビューから、レコードをクリックします

   または

   テーブル テーブル表示で、 **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) レコード名の左側。

   レコードのプレビューがビューで開きます。

   ![](assets/details-box.png)

1. （任意） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> レコードのプレビューの右上隅で、レコードのページを新しいタブで開きます。

   レコードページが開きます。

   ![](assets/details-page.png)

1. レコードのプレビューまたはページで、 **カバーを追加**


   または

   既存のカバー画像にポインタを合わせ、 **詳細** メニュー ![](assets/more-menu.png) を選択し、 **Upload**. <!--check the casing here; I logged a bug for this-->
この **レコードカバー** でボックスが開きます **Upload** タブ。

   ![](assets/record-cover-box-for-upload.png)

1. クリック **画像の参照** コンピュータ上の画像を参照して選択し、追加します。

1. （オプション）画像を保存する前に削除するには、 **新しい画像をアップロード** アイコン ![](assets/upload-new-image-icon.png) をクリックし、新しい画像をアップロードします。

1. （任意） **ギャラリー** タブをクリックしてから、画像ギャラリー内の画像をクリックします。 画像ギャラリーは変更できません。

   ![](assets/record-cover-box-for-gallery.png)

1. クリック **画像を使用**.

   画像はレコードのプレビューまたはページの上部にアップロードされ、変更は自動的に保存されます。

   ![](assets/record-page-with-cover-image.png)

1. （オプション）画像の上にマウスポインターを置き、 **詳細** メニュー ![](assets/more-menu.png) カバー画像の右下隅で、次のいずれかの操作を行います。

   * クリック **Upload** カバー画像を交換する場合は、手順 6 を繰り返して、新しい画像をアップロードして保存します。
   * クリック **再配置**&#x200B;を使用する必要があります **再配置** ツール ![](assets/reposition-tool-icon.png) カバー画像を中央に配置するには、をクリックします **保存** 完了した場合。
   * クリック **削除** カバー画像を取り外します。

   Workfront では、変更を自動的に保存します。
