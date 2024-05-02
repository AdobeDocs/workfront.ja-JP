---
title: レコードの作成
description: Adobe Workfront Planning を使用する場合、レコードはレコードタイプのインスタンスです。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 59%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# レコードの作成

{{maestro-important-intro}}

Adobe Workfront Planning では、レコードはレコードタイプのインスタンスです。

次のいずれかの操作を行って、レコードを作成できます。

* レコードタイプ用に手動で作成する
* 外部リストから情報をコピー＆ペーストして、レコードを作成します。

この記事では、レコードの作成方法について説明します。 テーブルビューまたはタイムラインビューでのレコードの管理については、次の記事を参照してください。

* [テーブルビューの管理](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [タイムラインビューの管理](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning にはアクセス制御はありません </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する参加以上の権限</a> </p>  
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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## レコードタイプにレコードを手動で追加してレコードを作成 <!--in a record type table (I don't think you can create them elsewhere right now)-->

レコードタイプのページのテーブルビューでレコードを作成できます。

レコード情報の編集については、[レコードの編集](/help/quicksilver/maestro/records/edit-records.md)を参照してください。

{#step1-to-maestro}

最後にアクセスしたワークスペースがデフォルトで開きます。ワークスペースの作成については、[ワークスペースの作成](../architecture/create-workspaces.md)を参照してください。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](../architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトで、レコードタイプのページがテーブルビューで開きます。
選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. （条件付き）レコードタイプページがテーブルビューで開かない場合は、テーブルビューのタブをクリックするか、をクリックします **+表示** テーブル表示を作成します。

1. 新しいレコードを追加するには、テーブルの最後の行の「**新しいレコード**」をクリックします。

   または

   テーブルの任意の列または行から、キーボードの **Shift + Enter** キーをクリックします。この場合は、空の行が追加されます。

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. 新しいレコードに関する情報を新しい行に入力します。

   >[!NOTE]
   >
   >  * レコードに必須のフィールドはありません。ただし、レコードを相互にリンクする際にレコードを識別するのに役立つので、レコードには名前を追加することをお勧めします。
   >
   >  * 他のレコードタイプまたは計算フィールドを参照するフィールドは、読み取り専用フィールドです。

1. 各行の情報の追加を続行し、キーボードの **Enter** キーをクリックして、変更を保存します。

   または

   新しいレコードの名前または **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) レコード名の左側。 レコードの詳細情報を含むプレビューがテーブルに表示されます。

   >[!TIP]
   >
   >にアクセスできます **詳細を開く** 名前フィールドがプライマリフィールドの場合に、レコードの名前フィールドからのみ表示されるアイコン。

1. レコードのプレビューでレコードの情報の編集を開始します。 Workfrontによって変更内容が自動保存されます。
1. （任意） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) レコードのプレビューの右上隅で、レコードのページを新しいタブで開きます。 レコードページでレコードの編集を続行します。


1. （オプション）新規レコードの追加を取り消すまたはやり直すには、次のキーボードショートカットを使用できます。

   * Ctrl + Z（Mac の場合は ⌘ + z）で、変更を取り消します
   * Ctrl + Shift + Z（Mac の場合は ⌘ + Shift + Z）で、変更を元に戻します

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

## 外部リストから情報をコピー＆ペーストしてレコードを作成する

1. 「」セクションの説明に従って、テーブルビューでレコードの作成を開始します [レコードタイプに手動で追加してレコードを作成](#create-records-by-manually-adding-them-to-a-record-type) この記事の内容です。

   新しいレコード情報を入力する列（またはフィールド）がテーブルビューにあることを確認します。

1. テーブルの最後の行の&#x200B;**新規 &lt; レコードタイプ名 >**&#x200B;をクリックして、新しいレコードを追加する数だけ新しい行をテーブルに追加します。

   例えば、別のアプリケーションから 10 件の新しいレコードの情報を貼り付ける場合は、10 行をテーブルビューに追加します。

1. 別のアプリケーションで、インポートするレコードのリストを作成します。

   例えば、Excel スプレッドシートを使用してリストを作成できます。

   リストには、情報が表形式で含まれている必要があります。

   >[!TIP]
   >
   > リストの列には、Workfront内の既存のフィールドに関する情報が含まれている必要があります。
   >
   > 目的のフィールドがWorkfrontに作成済みであること、およびシート内の情報がWorkfrontの各フィールドと一致する正しいフォーマットで表示されていることを確認します。

1. 別のアプリケーションから、複数の行と列を選択し、最初の新しいレコードから始まるレコードタイプのテーブルビューに情報を貼り付けます。

   Workfrontの計画エリアに、次の情報が読み込まれます。

   * 行には新しいレコードが含まれています
   * 列には、レコードのフィールドに関する情報が入力されます。
