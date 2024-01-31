---
title: レコードにサムネールを追加
description: AdobeMaestro でレコード情報を編集し、各レコードを個々のサムネールに関連付けて、簡単に認識できるようにすることができます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

<!--update the metadata with real information-->

# レコードにサムネールを追加

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro 機能を使用するには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

レコードをAdobeMaestro 内の一意のサムネールに関連付けて、簡単に認識できるようにすることができます。

レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。
詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).

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
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Maestro のアクセス制御はありません </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに権限を付与する（またはそれ以上の場合） </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td>  <p>Workfrontの管理者を含むすべてのユーザーには、メインメニューの Maestro 領域を含むレイアウトテンプレートを割り当てる必要があります。 </p> <p>詳しくは、 <a href="/help/quicksilver/maestro/access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## サムネールの記録に関する考慮事項

テーブルビュー内のレコードを視覚的に区別するために、レコードごとに一意のサムネール画像を関連付けることができます。

次の点に注意してください。

* サムネールとして追加できるのは、画像ファイルのみです。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* テーブルビューで個々のレコードにサムネール画像を追加できます。
* サムネールはレコード情報に属し、レコードが表示されるビューに表示されます。 例えば、次の領域では、レコード情報と共にサムネールが表示されます。

   * テーブルビューのレコードの主フィールド
   * タイムライン表示のレコードバー。
* レコードの詳細ページやタイムラインビューからは、レコードのサムネールを追加できません。
* レコードの詳細ページにサムネールは表示されません。

## レコードにサムネールを追加する

{{step1-to-maestro}}

1. レコードにサムネールを追加するワークスペースを選択し、レコードタイプカードをクリックします。

   レコードタイプのページが開きます。
1. 以下からテーブルビューを選択します。 **表示** ドロップダウンメニュー。 選択したタイプのすべてのレコードがテーブルに表示されます。
1. 主フィールドの情報にカーソルを合わせ、 **その他** メニュー ![](assets/more-menu.png)を選択し、次に **サムネール**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   主フィールドは、テーブルビューの最初の列に表示されるフィールドです。 主フィールドは常にフリーズし、隠したり再配置することはできません。

   The **サムネールを記録** ボックスが開きます。

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. Adobe Analytics の **アップロード** タブをクリックし、ファイルをドラッグ&amp;ドロップしてサムネールとして追加するか、 **アップロードを選択**&#x200B;をクリックし、追加する画像ファイルを参照します。 ファイルはお使いのコンピューターに保存する必要があります。
1. （オプション）サイズ調整ツールを使用して、画像の切り抜きとサイズ変更をおこないます。
1. クリック **画像を使用** をクリックして、画像をサムネールとして追加します。
これにより、 **サムネールを記録** ボックス。
1. （条件付き）少なくともテーブルビューに対する Contribute 権限を持っている場合は、 **フィールド** をクリックします。
1. を選択します。 **サムネール** サムネールの表示/非表示を切り替えます。 デフォルトでは、このオプションは選択されていません。

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   サムネールは、プライマリフィールド値の左側に表示されます。
1. （オプションおよび条件付き）Contribute またはそれ以上の権限を持っていない場合は、 **表示** ドロップダウンメニューを使用するか、ビューを作成します。
1. （オプション）サムネールを削除するには、プライマリフィールドの上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png)> **サムネール** > **削除** アイコン ![](assets/remove-image-icon.png)を選択し、次に **変更を保存**.
