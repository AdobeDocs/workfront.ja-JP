---
title: レコードを作成
description: Adobe Workfront Planning を使用する場合、レコードはレコードタイプのインスタンスです。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 3%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# レコードを作成

{{maestro-important-intro}}

Adobe Workfront Planning では、レコードはレコードタイプのインスタンスです。

次のいずれかの操作を行って、レコードを作成できます。

* レコードタイプ用に手動で作成する
* 外部リストから情報をコピー&amp;ペーストして、レコードを作成します。

この記事では、レコードを作成する方法について説明します。 テーブルまたはタイムラインビューのレコードの管理について詳しくは、次の記事を参照してください。

* [テーブル表示の管理](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [タイムライン表示を管理](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning のアクセス制御はありません </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに権限を付与する（またはそれ以上の場合）</a> </p>  
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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## レコードタイプに手動でレコードを追加してレコードを作成する <!--in a record type table (I don't think you can create them elsewhere right now)-->

レコードタイプのページのテーブルビューでレコードを作成できます。

レコード情報の編集について詳しくは、 [レコードを編集](/help/quicksilver/maestro/records/edit-records.md).

{#step1-to-maestro}

最後にアクセスしたワークスペースは、デフォルトで開きます。 ワークスペースの作成について詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

1. レコードタイプのカードをクリックします。 レコードタイプの作成について詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).

   最後にアクセスしたビューで、レコードタイプのページが開きます。 デフォルトでは、レコードタイプのページがテーブルビューで開きます。
選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. （条件付き）レコードタイプのページがテーブルビューで開かない場合は、テーブルビューのタブをクリックするか、 **+表示** をクリックして、テーブルビューを作成します。

1. 新しいレコードを追加するには、 **新しいレコード** テーブルの最後の行

   または

   クリック **Shift + Enter** キーボードで、テーブルの任意の列または行を選択します。 この場合は、空の行が表示されます。

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. 新しいレコードに関する情報を新しい行に入力します。

   >[!NOTE]
   >
   >  * レコードに必須のフィールドはありません。 ただし、レコードを相互にリンクする際にレコードを識別するのに役立つので、レコードには名前を追加することをお勧めします。
   >
   >  * 他のレコードタイプまたは計算フィールドを参照するフィールドは、読み取り専用フィールドです。

1. 各行の情報の追加を続行し、「 **入力** をクリックして、変更を保存します。

   または

   新しいレコードの名前または **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) をレコード名の左にドラッグします。 レコードの詳細情報を含むボックスがテーブルで開きます。

   >[!TIP]
   >
   >[ 詳細 ] ボックスにアクセスできるのは、[ 名前 ] フィールドが主フィールドの場合のレコードの名前フィールドだけです。

1. レコードのボックス内のレコードの情報の編集を開始します。 Workfrontは変更を自動的に保存します。
1. （オプション） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) をクリックし、レコードのページを新しいタブで開きます。 レコードページ上のレコードの編集を続けます。


1. （オプション）次のキーボードショートカットを使用して、新しいレコードの追加の取り消しまたはやり直しをおこないます。

   * Ctrl + Z( Macの場合は⌘ + Z)：変更を元に戻します。
   * Ctrl + Shift + Z(Macの場合は⌘ + Shift + Z)：変更をやり直します。

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## 外部リストから情報をコピー&amp;ペーストしてレコードを作成する

1. 「 」セクションの説明に従って、テーブルビューでレコードの作成を開始します。 [レコードタイプに手動でレコードを追加してレコードを作成する](#create-records-by-manually-adding-them-to-a-record-type) 」を参照してください。

   新しいレコード情報を入力する列（またはフィールド）がテーブルビューに含まれていることを確認します。

1. クリック **新規 &lt; レコードタイプ名 >** をテーブルの最後の行に追加し、新しいレコードを追加する数だけ新しい行を追加します。

   例えば、別のアプリケーションから 10 件の新しいレコードの情報を貼り付ける場合は、10 行をテーブルビューに追加します。

1. 別のアプリケーションで、インポートするレコードのリストを作成します。

   例えば、Excel スプレッドシートを使用してリストを作成できます。

   リストには、情報が表形式で含まれている必要があります。

   >[!TIP]
   >
   > リストの列には、Workfrontにある既存のフィールドに関する情報が含まれている必要があります。
   >
   > 目的のフィールドがWorkfrontで既に作成されていて、シート内の情報がWorkfrontの各フィールドと一致する正しい形式で表示されていることを確認します。

1. 別のアプリケーションから、複数の行と列を選択し、最初の新しいレコードから始まるレコードタイプのテーブルビューに情報を貼り付けます。

   次の情報がWorkfront Planning 領域にインポートされます。

   * 行に新しいレコードが含まれます
   * 列には、レコードのフィールドに関する情報が入力されます。
