---
title: レコードの作成
description: Adobe Workfront Planning を使用する場合、レコードはレコードタイプのインスタンスです。 Workfront Planning で各レコード・タイプに一意のレコードを作成するには、レコードを手動でテーブル・ビューに追加するか、リストからインポートするか、複製するか、または他のレコードに接続する際に作成します。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 61cad7dc76ba04ea84ff0bd5052182f040f7b4d9
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 38%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# レコードの作成

{{planning-important-intro}}

Adobe Workfront Planning では、レコードはレコードタイプのインスタンスです。

次のいずれかを行うことで、レコードを作成できます。

* テーブル表示のレコードタイプページから追加
* 外部リストからのレコードのリストのコピー&amp;ペースト
* 複製
* 他のレコードから接続する場合と同様に作成します

この記事では、レコードの作成方法について説明します。

テーブルビューまたはタイムラインビューでのレコードの管理については、次の記事を参照してください。

* [テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)
* [タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## アクセス要件

<!--Updated for GA-->

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

Workfront Planning にアクセスするには、次のものが必要です：

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront計画*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容の詳細については、<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfrontの価格とパッケージ </a> を参照してください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 標準
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p> 
   <p>レコードをレコードに関連付ける際に、作成するオブジェクトタイプ（プロジェクトとポートフォリオ）のWorkfrontでのアクセス権を編集します。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>レコードの追加先となるワークスペースに対する権限を管理します。 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
   <p>子オブジェクト（プロジェクト）を追加するためのWorkfront オブジェクト（ポートフォリオ）への権限を管理します。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューに計画エリアを含むレイアウトテンプレートを割り当てる必要があります </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

<!--OLD info: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p>  
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## レコードタイプ <!--in a record type table (I don't think you can create them elsewhere right now)--> に追加してレコードを作成

レコードタイプのページのテーブルビューでレコードを作成できます。

レコード情報の編集については、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトで、レコードタイプのページがテーブルビューで開きます。
選択したタイプのすべてのレコードがビューに表示されます。

1. （条件付き）表示するビューに応じて、次のいずれかの操作を行います。

   * テーブル表示で、次の操作を行います。

      * テーブルの最後の行にある「**新規レコード**」をクリックします

      * テーブルの任意の列または行から、キーボードの **Shift + Enter** キーをクリックします。これにより、開始レコードの下に空の行が追加されます。
      * レコードの主フィールドにポインタを合わせ、フィールドの右側にある **詳細** メニュー ![](assets/more-menu.png) をクリックして、「**上にレコードを挿入**」または **下にレコードを挿入** をクリックします。

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * 任意のビューから：

      * ページの右上隅にある「**新規レコード**」をクリックします。 レコードのプレビューボックスが開きます。

     Workfrontは、新しい各レコードにサムネールとカバー画像を自動アップロードします。 これらの画像は、後で変更できます。 詳しくは、次の記事を参照してください。

      * [レコードへのカバー画像の追加](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [レコードにサムネールを追加する](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. プレビューボックスに表示されるフィールドに、新しいレコードに関する情報を入力します。

   >[!NOTE]
   >
   >  * レコードに必須のフィールドはありません。ただし、レコードを相互にリンクするときにレコードを識別すると便利なので、レコードの主フィールドの情報を追加することをお勧めします。 主フィールドについて詳しくは、[ テーブル表示の管理 ](/help/quicksilver/planning/views/manage-the-table-view.md) および [プライマリフィールドの概要 ](/help/quicksilver/planning/fields/primary-field-overview.md) を参照してください。
   >
   >  * 他のレコードタイプまたは計算フィールドを参照するフィールドは、読み取り専用フィールドです。

1. （条件付き）テーブルにレコードを追加する場合は、引き続き各行に情報を追加し、キーボードの **Enter** をクリックして変更を保存します。

   または

   新しいレコードの名前か、レコード名の左側にある&#x200B;**詳細を開く**&#x200B;アイコン ![](assets/open-details-icon-in-table-name-field.png) をクリックします。レコードの詳細情報を含むプレビューがテーブルに表示されます。

   >[!TIP]
   >
   >**詳細を開く** アイコンにアクセスできるのは、レコードの名前フィールド（名前フィールドがプライマリフィールドの場合）のみです。

1. レコードのプレビューでレコードの情報の編集を開始します。 Workfront では、変更を自動的に保存します。
1. （オプション）レコードのプレビューの右上隅に ![](assets/open-details-in-a-new-tab-icon.png) る **新しいタブで開く** アイコンをクリックして、レコードのページを新しいタブで開きます。 レコードページでレコードの編集を続行します。 詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

1. （オプション）テーブル表示で新しいレコードやその情報を追加する際に、それらの追加の取り消しまたはやり直しを行うには、次のキーボードショートカットを使用します。

   * Ctrl + Z（Mac の場合は ⌘ + z）で、変更を取り消します
   * Ctrl + Shift + Z（Mac の場合は  ⌘ + Shift + Z）で、変更を元に戻します

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## 外部リストからレコードをコピー&amp;ペーストして作成

1. この記事の[レコードタイプにレコードを手動で追加してレコードを作成](#create-records-by-manually-adding-them-to-a-record-type)の節の説明に従って、テーブルビューでレコードの作成を開始します。

   新しいレコード情報を入力する列（またはフィールド）がテーブルビューに含まれていることを確認します。

1. テーブルの最後の行の&#x200B;**新規 &lt; レコードタイプ名 >**&#x200B;をクリックして、新しいレコードを追加する数だけ新しい行をテーブルに追加します。

   例えば、別のアプリケーションから 10 件の新しいレコードの情報を貼り付ける場合は、10 行をテーブルビューに追加します。

1. 別のアプリケーションで、読み込むレコードのリストを作成します。

   例えば、Excel スプレッドシートを使用してリストを作成できます。

   リストには、情報が表形式で含まれている必要があります。

   >[!TIP]
   >
   > リストの列には、Workfront 内の既存のフィールドに関する情報を含める必要があります。
   >
   > 目的のフィールドが Workfront で既に作成され、シート内の情報が Workfront の各フィールドと一致する正しい形式で表示されていることを確認します。

1. 別のアプリケーションから、複数の行と列を選択し、最初の新しいレコードから始まるレコードタイプのテーブルビューに情報を貼り付けます。

   次の情報が Workfront Planning エリアに読み込まれます。

   * 行には新しいレコードが含まれています
   * 列には、レコードのフィールドに関する情報が入力されます。

## レコードを複製して作成

レコードの複製について詳しくは、「[ レコードの複製 ](/help/quicksilver/planning/records/copy-or-duplicate-records.md)」を参照してください。

## 接続するレコードの作成

他のレコードから関連付ける際に、レコードまたはWorkfront オブジェクトを作成できます。

既存のレコードから新しいレコードまたはWorkfront オブジェクトを接続して追加するには、次のものが必要です。

* 接続されたレコードタイプ。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* 接続されたレコード。 詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
* この記事の [ アクセス要件 ](#access-requirements) の節で説明しているように、Workfront Planning およびWorkfrontでの正しいアクセス権と権限。

>[!NOTE]
>
>Workfront プロジェクトおよびポートフォリオをWorkfront Planning レコードに関連付けて作成することは、Planning レコードを他のレコードから関連付けて作成することと似ています。

他のレコードとの接続時にレコードを作成するには、次の手順に従います。

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、Workfront Planning レコードの接続を開始します。
1. （条件付き）別のレコードの「接続済みレコード」フィールドから追加しようとしてレコードが見つからない場合は、レコードを検索して、「**+追加**」をクリックします。 「**+追加**」ボタンの後に、接続元のレコードタイプの名前が続きます。

   ![](assets/add-button-to-create-records-in-context-highlighted.png)

   レコードが作成され、接続されたレコードフィールドに追加されます。
1. （オプション）作成したレコードを持つレコードタイプのテーブル表示に移動します。 新しいレコードがビューの最後の行に表示されます。
1. （オプション）テーブル表示で新しいレコードの情報の追加を開始します
または
名前をクリックして詳細ページを開き、情報を追加します。

