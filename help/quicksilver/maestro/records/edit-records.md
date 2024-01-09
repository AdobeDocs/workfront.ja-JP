---
title: レコードを編集
description: レコード情報は、AdobeMaestro で編集できます。 レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 1%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# レコードを編集

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro 機能を使用するには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

レコード情報は、AdobeMaestro で編集できます。 レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。
詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).

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
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


## レコードの編集に関する考慮事項

* 自分または別のユーザーが作成したレコードを編集できます。 <!--will change with access levels-->
* 計算を含む他のレコードやフィールドからリンクされたフィールドは編集できません。
* 表示したレコードが他のレコードにリンクされている場合、編集中のレコードの新しい情報は、リンクされたレコードに反映されます。
* レコードを一括で編集することはできません。 <!--this will probably change-->
* URL は、http://、https://、ftp://、www のいずれかで始まる場合にのみ、1 行のテキストフィールドタイプのリンクとして認識されます。.
* 段落タイプのフィールドの編集時に、次のリッチテキスト書式設定オプションを使用できます。

   * 太字
   * 斜体
   * 下線
   * リンクを追加
   * 箇条書きリストを追加
   * 番号付きリストを追加

## レコードを編集

次の領域でレコードを編集できます。

* [レコードの詳細ページから](#edit-a-record-from-the-records-details-page)
* [レコードタイプのテーブルビューから](#edit-a-record-from-the-record-type-table-view)

### レコードの詳細ページからレコードを編集する

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. （オプション）ワークスペース名の右側にある下向き矢印をクリックして、レコードを更新するワークスペースを選択します。
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

1. クリック **変更を保存**. <!--logged a bug for this - this needs to be "Save"-->

### レコードタイプのテーブルビューからレコードを編集する

{#step1-to-maestro}

最後にアクセスしたワークスペースが開きます。

1. （オプション）ワークスペース名の右側にある下向き矢印をクリックして、レコードを更新するワークスペースを選択します。
1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。
1. （条件付き） **表示** テーブルの右上隅にあるドロップダウンメニューで、 **テーブル** 表示。 最後にアクセスしたときにタイムラインビューでレコードタイプを表示した場合を除き、これがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。
1. レコードの行内をクリックして、レコードに関する情報の編集をインラインで開始します。

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. 押す **入力** キーボードでクリックするか、行の外側をクリックして変更を保存します。 変更内容は自動的に保存されます。 保存済みのインジケータが、テーブルビューの右上隅に短く表示され、変更が保存されたことが示されます。

   >[!NOTE]
   >
   >  次のフィールドの情報は読み取り専用で、Workfrontによって自動的に更新されるので、編集できません。
   >  
   >  * レコードタイプを接続して作成した、リンクされたフィールド。 詳しくは、 [レコードタイプを接続](../architecture/connect-record-types.md).
   >  * 次のタイプのフィールド：作成者、作成日、最終変更者、最終変更日


1. （オプション）フィールドの 1 つ以上の既存の値をコピーし、別のレコードの同じタイプのフィールドに貼り付けて、 **入力** をクリックして、変更を保存します。

   >[!NOTE]
   >
   >次の点に注意してください。
   >
   >* 情報を貼り付けるフィールドと同じタイプの Maestro フィールド以外の別のソースから情報をコピーすることはできません。
   >
   >* レコードの「詳細」領域にフィールド値をコピーして貼り付けることはできません。 この機能は、レコードタイプのテーブルビューでのみサポートされます。
   >* 次のフィールドタイプのフィールド値をコピーして貼り付けることはできません。
   >
   >
   >    * レコードタイプを接続して作成した、リンクされたフィールド。 リンクされたレコードフィールドをコピーして貼り付けることができます。 詳しくは、 [レコードタイプを接続](../architecture/connect-record-types.md).
   >    * 次のタイプのフィールド：作成者、作成日、最終変更者、最終変更日

<!--1. (Optional) Use the following keyboard shortcuts to undo or redo editing or copying and pasting record information: 

    * **Undo**: CTRL/CMD + Z
    * **Redo**: CTRL/CMD + Shift + Z-->