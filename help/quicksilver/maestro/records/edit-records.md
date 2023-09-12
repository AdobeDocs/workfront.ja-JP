---
title: レコードを編集
description: レコード情報は、AdobeMaestro で編集できます。 レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# レコードを編集

>[!IMPORTANT]
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなクローズドベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

レコード情報は、AdobeMaestro で編集できます。 レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。
詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

&lt;! — ここで、詳細ビューのフィールドはテーブルビューのフィールドと同じであると言います。この記事は、この情報を参照するために、レコードビューの管理からリンクされています —>

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe産物</p> </td>
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
   <td role="rowheader">アクセスレベル</td>
   <td> <p>任意</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/grant-access.md">AdobeMaestro へのアクセスを許可</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## レコードの編集に関する考慮事項

* 自分または別のユーザーが作成したレコードを編集できます。 <!--will change with access levels-->
* 編集したレコードが他のレコードにリンクされている場合、編集中のレコードの新しい情報は、リンクされたレコードに反映されます。
* レコードを一括で編集することはできません。 <!--this will probably change-->

## レコードを編集

次の領域でレコードを編集できます。

* [レコードの詳細ページから](#edit-a-record-from-the-records-details-page)
* [レコードタイプのテーブルビューから](#edit-a-record-from-the-record-type-table-view)

### レコードの詳細ページからレコードを編集する

1. 次をクリック： **メインメニュー** ![](assets/main-menu-workfront.png) を右上に配置するか、 **メインメニュー** ![](assets/main-menu-shell.png) 左上隅にある場合は、[ マエストロ ] をクリックします。

   最後にアクセスしたワークスペースが開きます。
1. 次のいずれかの操作を行います。

   * テーブルビューで、レコードの名前をクリックします。
   * テーブルビューで、レコード名の上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png)を選択し、次に **表示**

     ![](assets/contextual-menu-for-record-row.png)
   * タイムラインビューで、レコードバーをクリックします。

   レコード **詳細** ページが開きます。

1. 次をクリック： **その他** メニュー ![](assets/more-menu.png) をクリックし、 **編集**

   または

   詳細ページの編集可能なフィールド内をクリックして、情報を編集します。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

   >[!NOTE]
   >
   >    計算を含む、またはシステムで生成される、リンクされたフィールドやフィールドは編集できません。


1. クリック **変更を保存**. <!--logged a bug for this - this needs to be "Save"-->

### レコードタイプのテーブルビューからレコードを編集する

1. 次をクリック： **メインメニュー** ![](assets/main-menu-workfront.png) 右上隅に <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> 次に、「 **マエストロ** ![](assets/maestro-icon.png).

   最後にアクセスしたワークスペースが開きます。
1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。
1. （条件付き） **表示** テーブルの右上隅にあるドロップダウンメニューから、テーブルビューを選択します。 最後にアクセスしたときにタイムラインビューでレコードタイプを表示した場合を除き、これがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。
1. レコードの行内をクリックして、レコードのインライン情報の編集を開始し、 **入力** をクリックして、変更を保存します。 変更内容は自動的に保存されます。

   >[!TIP]
   >
   >リンクされたフィールドは編集できません。 これらのフィールドの情報は、リンクされたレコードから自動的に入力されます。 詳しくは、 [レコードタイプを接続](../architecture-and-fields/connect-record-types.md).



