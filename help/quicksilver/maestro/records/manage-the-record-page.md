---
title: レコードページの管理
description: Adobe Workfront計画では、レコードボックスとページのレイアウトを編集して管理できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 25%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# レコードページの管理

{{maestro-important-intro}}

Adobe Workfront計画では、レコードボックスとページのレイアウトを編集して管理できます。 レコード ビューにレコード ボックスを表示できます。

レコードボックスは、レコードタイプのビューに表示されるレコードページの小さいビューです。

レコード ボックスとページのレイアウトを変更すると、同じ種類のすべてのレコードのボックスとページが変更されます。

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

* レコードボックスまたはページ内のフィールドを並べ替えると、そのタイプのすべてのレコードとそのレコードにアクセスするすべてのユーザーのフィールドが並べ替えられます。
* カバー画像をレコードに追加することは、レコードボックスまたはページの全体的なレイアウトの一部ではありません。 各レコードに一意のカバー画像を追加できます。 詳しくは、を参照してください [レコードへのカバー画像の追加](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

## レコードボックスまたはページ内のフィールドの並べ替え

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

1. レコードボックスまたはページで、グラブアイコンをクリックします ![](assets/grab-icon.png) フィールド名の左側で、目的の場所にドラッグ&amp;ドロップします。

   レコードを表示するすべてのユーザーについて、同じタイプのすべてのレコードのボックスとページの両方で、フィールドの新しい位置が更新されます。

   レコードボックスまたはページのレイアウトに対するすべての変更は、自動的に保存されます。

