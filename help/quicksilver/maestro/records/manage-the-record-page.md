---
title: レコードページを管理
description: Adobe Workfront Planning で、レコードボックスとページのレイアウトを編集できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 7d3778d52f9a3afa12a7bdf348f7400693f8f7ab
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 4%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# レコードページを管理

{{maestro-important-intro}}

Adobe Workfront Planning で、レコードボックスとページのレイアウトを編集できます。 レコードビューにレコードボックスを表示できます。

レコードボックスは、レコードタイプのビューに表示されるレコードページの小さなビューです。

レコードボックスとページのレイアウトを変更すると、同じ種類のすべてのレコードのボックスとページが変更されます。

レコードページの編集を開始する前に、レコードの種類とレコードを作成する必要があります。

詳しくは、次の記事を参照してください。

* [レコードタイプの作成](../architecture/create-record-types.md)

* [レコードを作成](/help/quicksilver/maestro/records/create-records.md)

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
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織がAdobe Workfront Planning ベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <p>新規：明るいかそれ以上</p>
   または
   <p>現在：作業以上</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning のアクセス制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに計画領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## レコードページの編集に関する考慮事項

* レコードボックスまたはページ内のフィールドを並べ替えると、そのタイプのすべてのレコードと、それらのレコードにアクセスするすべてのユーザーのフィールドが並べ替えられます。
* レコードに表紙画像を追加することは、レコードボックスやページの全体的なレイアウトには含まれません。 各レコードに一意のカバー画像を追加できます。

## レコードボックスまたはページのフィールドを並べ替える

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. （オプション）ワークスペース名の右側にある下向き矢印をクリックして、レコードを更新するワークスペースを選択します。
1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意のタイプのビューで、レコードの名前をクリックします。

   または

   テーブルビューで、 **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) をレコード名の左側に追加します。

   レコードのボックスがビューに開きます。

   ![](assets/details-box.png)

   >[!TIP]
   >
   >次の項目を表示すると、 **詳細を開く** テーブルビューのレコードの [ 名前 ] フィールドの左側にあるアイコンは、[ 名前 ] フィールドが主フィールドの場合にのみ表示されます。

1. （オプション） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> をクリックし、レコードのページを新しいタブで開きます。

   レコードページが開きます。

   ![](assets/details-page.png)

1. レコードボックスまたはページで、「取得」アイコンをクリックします。 ![](assets/grab-icon.png) フィールド名の左側にドラッグ&amp;ドロップし、目的の場所に移動します。

   フィールドの新しい位置は、レコードを表示しているすべてのユーザーの、同じタイプのすべてのレコードのボックスとページの両方で更新されます。

   レコードボックスまたはページのレイアウトに対するすべての変更は、自動的に保存されます。


## レコードボックスまたはページに表紙画像を追加する

レコードボックスまたはページの上部に表紙画像を追加して、レコードをパーソナライズできます。

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. （オプション）ワークスペース名の右側にある下向き矢印をクリックして、レコードを更新するワークスペースを選択します。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意のタイプのビューで、レコードの名前をクリックします。

   または

   テーブルビューで、 **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) をレコード名の左側に追加します。

   レコードのボックスがビューに開きます。

   ![](assets/details-box.png)

   >[!TIP]
   >
   >次の項目を表示すると、 **詳細を開く** テーブルビューのレコードの [ 名前 ] フィールドの左側にあるアイコンは、[ 名前 ] フィールドが主フィールドの場合にのみ表示されます。

1. （オプション） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> をクリックし、レコードのページを新しいタブで開きます。

   レコードページが開きます。

   ![](assets/details-page.png)

1. レコードボックスまたはページで、 **カバーを追加**. <!--check the casing here; I logged a bug for this-->
The **レコードのカバー** ボックスが開きます。

1. クリック **アップロードを選択** コンピュータ上の画像を参照して選択し、追加し、クリックします。 **画像を使用**.

   画像がレコードボックスまたはページの上部にアップロードされ、変更内容が自動的に保存されます。

   ![](assets/record-page-with-cover-image.png)

1. （オプション）画像の上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png) カバー画像の右下隅で、次のいずれかの操作を行います。

   * クリック **アップロード** カバー画像を置き換える場合は、手順 6 を繰り返して新しい画像をアップロードし、保存します。
   * クリック **再配置**&#x200B;をクリックし、 **再配置** ツール ![](assets/reposition-tool-icon.png) カバー画像を中央に配置するには、 **保存** 完了したら、
   * クリック **削除** をクリックして、カバー画像を削除します。

   すべての変更が直ちに有効になります。

