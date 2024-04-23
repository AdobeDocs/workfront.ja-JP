---
title: レコードへのサムネールの追加
description: Adobe Workfront Planning でレコード情報を編集し、各レコードを個々のサムネールに関連付けて、識別しやすくすることができます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 14%

---

<!--update the metadata with real information-->

# レコードへのサムネールの追加

{{maestro-important-intro}}

レコードをAdobe Workfront Planning 内の固有のサムネールに関連付けて、簡単に認識できるようにすることができます。

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

## レコードのサムネールに関する考慮事項

テーブル表示でレコードを視覚的に区別するために、各レコードに一意のサムネール画像を関連付けることができます。

次の点に注意してください。

* サムネールとして追加できるのは画像ファイルのみです。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* テーブル表示の個々のレコードにサムネール画像を追加できます。
* サムネールはレコード情報に属し、レコードが表示されるビューに表示されます。 例えば、次の領域では、レコード情報の横にサムネールが表示されます。

   * テーブル ビューのレコードの主フィールド
   * タイムライン ビューのレコード バー
* レコードのページまたは別の種類のビューからレコードのサムネールを追加することはできません。
* サムネールがレコードのページに表示されません。

## レコードへのサムネールの追加

{{step1-to-maestro}}

1. サムネールを追加するレコードのワークスペースを選択し、レコードタイプ カードをクリックします。

   これにより、レコードタイプ ページが開きます。
1. 「」からテーブル表示を選択します **表示** ドロップダウンメニュー。 選択したタイプのすべてのレコードがテーブルに表示されます。
1. プライマリフィールド情報の上にマウスポインターを置き、 **詳細** メニュー ![](assets/more-menu.png)を選択し、 **サムネール**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   プライマリフィールドとは、テーブルビューの最初の列に表示されるフィールドです。 プライマリフィールドは常にフリーズされ、非表示や再配置はできません。

   この **サムネールを記録** ボックスが開きます。

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. が含まれる **Upload** タブで、サムネールとして追加するファイルをドラッグ&amp;ドロップするか、 **選択してアップロード**&#x200B;を選択してから、追加する画像ファイルを探します。 ファイルはコンピューターに保存する必要があります。
1. （オプション）サイズ変更ツールを使用して、画像の切り抜きやサイズ変更を行います。
1. クリック **画像を使用** 画像をサムネールとして追加します。
これにより、が閉じます **サムネールを記録** ボックス。
1. （条件付き）テーブルビューへの投稿権限が少なくとも存在する場合は、 **フィールド** テーブルビューの右上隅
1. 「」を選択します **サムネール** サムネールを表示に切り替えます。 デフォルトでは、このオプションは選択されていません。

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   サムネールがプライマリフィールド値の左側に表示されます。
1. （オプションおよび条件付き）ビューに対する投稿以上の権限がない場合は、から新しいビューを選択します **表示** ドロップダウンメニューを使用するか、ビューを作成します。
1. （オプション）サムネールを削除するには、プライマリフィールドにカーソルを合わせて「 **詳細** メニュー ![](assets/more-menu.png)> **サムネール** > **削除** アイコン ![](assets/remove-image-icon.png)を選択し、 **変更を保存**.
