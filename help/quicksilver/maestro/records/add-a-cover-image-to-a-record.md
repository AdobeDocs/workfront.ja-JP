---
title: レコードへのカバー画像の追加
description: レコードの編集時に、Adobe Workfront Planning のレコード・ページに表紙を追加することで、レコードをパーソナライズできます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 36%

---


<!--update the metadata with real information-->

# レコードへのカバー画像の追加

{{planning-important-intro}}

レコードの編集時に、Adobe Workfront Planning のレコード・ページに表紙を追加することで、レコードをパーソナライズできます。

レコードの編集方法については、を参照してください [レコードを編集](/help/quicksilver/maestro/records/edit-records.md).

レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。

詳しくは、[リクエストタイプの作成](../architecture/create-record-types.md)を参照してください。

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
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
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
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Workfront Planning に対するアクセス制御はありません </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する参加以上の権限 </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td>  <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、<a href="/help/quicksilver/maestro/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

## レコードページの表紙画像に関する考慮事項

表紙画像を追加して、レコードのページをパーソナライズできます。

次の点に注意してください。

* カバー画像は、1 つのレコードに固有で、同じタイプのすべてのレコードには適用されません。
* カバー画像として追加できるのは画像ファイルのみです。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 任意のビューのレコードプレビューまたはレコードページから、カバー画像を個々のレコードに追加できます。
* どのレコードビューからもカバー画像をインラインで追加することはできません。

## レコードへのカバー画像の追加

レコードのプレビューまたはページの上部にカバー画像を追加して、レコードをパーソナライズできます。

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. （オプション）ワークスペース名の右側にある下向き矢印をクリックして、レコードを更新するワークスペースを選択します。

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

1. レコードのプレビューまたはページで、 **カバーを追加**. <!--check the casing here; I logged a bug for this-->
この **レコードカバー** ボックスが開きます。

1. クリック **選択してアップロード** コンピュータ上の画像を参照して選択し、追加してから、 **画像を使用**.

   画像はレコードのプレビューまたはページの上部にアップロードされ、変更は自動的に保存されます。

   ![](assets/record-page-with-cover-image.png)

1. （オプション）画像の上にマウスポインターを置き、 **詳細** メニュー ![](assets/more-menu.png) カバー画像の右下隅で、次のいずれかの操作を行います。

   * クリック **Upload** カバー画像を交換する場合は、手順 6 を繰り返して、新しい画像をアップロードして保存します。
   * クリック **再配置**&#x200B;を使用する必要があります **再配置** ツール ![](assets/reposition-tool-icon.png) カバー画像を中央に配置するには、をクリックします **保存** 完了した場合。
   * クリック **削除** カバー画像を取り外します。

   Workfront では、変更を自動的に保存します。
