---
title: レコードへのカバー画像の追加
description: Adobe Workfront計画でレコード情報を編集し、各レコードを表紙画像に関連付けて、レコードのページをパーソナライズできます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 20%

---

<!--update the metadata with real information-->

# レコードへのカバー画像の追加

{{maestro-important-intro}}

Adobe Workfront計画でレコード情報を編集し、各レコードを表紙画像に関連付けて、レコードのページをパーソナライズできます。

レコードの作成と編集を開始するには、レコードタイプを作成する必要があります。
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
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Workfront Planning にはアクセス制御はありません </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースへの投稿以上の権限 </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td>  <p>Workfront管理者を含むすべてのユーザーには、メインメニューに計画エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、<a href="/help/quicksilver/maestro/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

## レコードページの表紙画像に関する考慮事項

表紙画像を追加して、レコードのページをパーソナライズできます。 画像は各レコードに固有で、同じタイプのすべてのレコードには適用されません。

次の点に注意してください。

* カバー画像として追加できるのは画像ファイルのみです。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* カバー画像は、任意のビューのレコード ボックスまたはレコード ページから個々のレコードに追加できます。
* テーブル表示からカバー画像をインラインで追加することはできません。

## レコードへのカバー画像の追加

レコードをパーソナライズするには、レコードボックスまたはページの上部にカバー画像を追加します。

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. （オプション）ワークスペース名の右側にある下向き矢印をクリックして、レコードを更新するワークスペースを選択します。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意の種類のビューで、レコードの名前をクリックします

   または

   テーブル テーブル表示で、 **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) レコード名の左側。

   レコードのボックスがビューで開きます。

   ![](assets/details-box.png)

   >[!TIP]
   >
   >を表示できます **詳細を開く** テーブル ビューで、[ 名前 ] フィールドがプライマリ フィールドの場合のみ、[ 名前 ] フィールドの左側にあるアイコンです。

1. （任意） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> レコード ボックスの右上隅で、レコードのページを新しいタブで開きます。

   レコードページが開きます。

   ![](assets/details-page.png)

1. レコード ボックスまたはレコード ページで、 **カバーを追加**. <!--check the casing here; I logged a bug for this-->
この **レコードカバー** ボックスが開きます。

1. クリック **選択してアップロード** コンピュータ上の画像を参照して選択し、追加してから、 **画像を使用**.

   画像はレコードボックスまたはページの上部にアップロードされ、変更は自動的に保存されます。

   ![](assets/record-page-with-cover-image.png)

1. （オプション）画像の上にマウスポインターを置き、 **詳細** メニュー ![](assets/more-menu.png) カバー画像の右下隅で、次のいずれかの操作を行います。

   * クリック **Upload** カバー画像を交換する場合は、手順 6 を繰り返して、新しい画像をアップロードして保存します。
   * クリック **再配置**&#x200B;を使用する必要があります **再配置** ツール ![](assets/reposition-tool-icon.png) カバー画像を中央に配置するには、をクリックします **保存** 完了した場合。
   * クリック **削除** カバー画像を取り外します。

   Workfrontによって変更内容が自動保存されます。