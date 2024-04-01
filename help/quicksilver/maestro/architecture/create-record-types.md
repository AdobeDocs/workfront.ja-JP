---
title: レコードタイプの作成
description: レコード・タイプは、Adobe Workfront Planning のオブジェクト・タイプです。 Workfront Planning では、組織のライフサイクルに必要な作業項目を示すカスタムレコードタイプを作成できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: eaf1cd4142b83a42d068e2d02fe673fa4dd25769
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 3%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# レコードタイプの作成

{{maestro-important-intro}}

レコード・タイプは、Adobe Workfront Planning のオブジェクト・タイプです。 Workfront Planning では、組織のライフサイクルに必要な作業関連項目を示すカスタムレコードタイプを作成できます。
レコードの種類は、次のいずれかになります。

レコードの種類の詳細については、「 [レコードタイプの概要](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <td> Adobe Workfront
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Adobe Workfront Planning クローズ済みベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <p>現在：プラン</p>
   または
   <p>新規：標準 </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Workfront Planning には、アクセスレベルの制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに計画領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## レコードタイプの作成に関する考慮事項

* レコードタイプは、次の方法でワークスペースに作成できます。

   * 自動：
      * テンプレートを使用してワークスペースを作成する場合。

        詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

      * Excel または CSV ファイルを使用してインポートする場合。

        >[!IMPORTANT]
        >
        >この機能は、2024 年 3 月 21 日以降、一時的に無効になっています。 後日有効になります。

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/maestro/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/maestro/records/connect-records.md). -->
   * 手動：

      * 最初から。

        この記事では、レコードの種類を最初から作成する方法について説明します。

* レコードタイプは、セクション内で移動したり、ワークスペースのセクション間で移動したりできます。 あるワークスペースから別のワークスペースにレコードタイプを移動することはできません。

## ワークスペーステンプレートを使用してレコードタイプを作成する

Workfront Planning テンプレートを使用してワークスペースを作成する際に、レコードタイプを自動的に作成できます。 各テンプレートには、サンプルレコードタイプが含まれています。

テンプレートからワークスペースを作成する場合、レコードタイプは次のセクションにグループ化されます。

* オペレーショナルレコードのタイプ
* 分類

「オペレーショナル・レコード・タイプ」セクションと「分類」セクションの両方で、レコード・タイプを手動で追加できます。

ワークスペースの作成について詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

各テンプレートに含まれるレコードの種類について詳しくは、 [Workspace テンプレートのリスト](../architecture/workspace-templates.md).

## レコードタイプを最初から作成する

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを作成するワークスペースを選択します。
1. （オプション）「 **セクションを追加** をクリックして、新しいセクションをワークスペースに追加します。
1. クリック **レコードタイプを追加**.
1. （条件付き）Excel または CSV ファイルのインポートによるレコードタイプの作成が有効な場合、 **ゼロから**. それ以外の場合は、 **レコードタイプを追加** ボックスが開きます。

   ![](assets/add-record-type-box-with-appearance-options.png)

1. 次の情報を更新します。

   * **レコードタイプ名**:「無題のオペレーショナルレコードタイプ」を、今後のレコードタイプの名前に置き換えます。
   * **外観**：レコードタイプに関連付けられるアイコンの色と形状を定義します。 次の操作を実行します。
      * 新しいレコードタイプを識別する色を選択します。 これは、レコードタイプアイコンの色です。 デフォルトでは「グレー」が選択されています。
      * リストからアイコンを選択するか、アイコンの名前を入力して内容を説明し、表示されたときに選択します。 これは、レコードタイプのアイコンです。 デフォルトでは、ファイルアイコンが選択されています。

1. の外側をクリック **レコードタイプを追加** ボックスを使用してレコードタイプを保存します。

   レコードタイプカードが、選択したセクションとワークスペースに追加されます。
レコードタイプに含まれるフィールドの数がカードに表示されます。
1. （オプション）レコードタイプカードをクリックして、レコードタイプのページを開きます。

   ![](assets/operational-record-type-blank.png)

   デフォルトでは、レコードタイプのページがテーブルビューに表示されます。 テーブルの列は、新しいレコードタイプに関連付けられたフィールドです。 各行は、追加する必要がある一意のレコードです。

   >[!TIP]
   >
   >    Excel または CSV ファイルからレコードタイプをインポートする場合、レコードもインポートされます。

   デフォルトでは、次のフィールドは、オペレーショナルレコードタイプのテーブル表示列に表示されます。

   * 名前
   * 説明
   * 開始日
   * 終了日
   * ステータス

1. （オプション）ページのヘッダーでレコードタイプ名を更新する

   または

   次をクリック： **その他** アイコン ![](assets/more-menu.png) をクリックして、レコードタイプ名の右に移動し、 **名前を変更** をクリックして、名前を変更します。

1. （オプション）「 **+新しいレコード** 選択したレコードタイプのレコードを追加します。 詳しくは、 [レコードを作成](../records/create-records.md).
1. （オプション） **+** レコードタイプにフィールドを追加するには、テーブルの右上隅にあるアイコンを使用します。

   フィールドの作成について詳しくは、 [フィールドの作成](../fields/create-fields.md).

1. （オプション）ヘッダーで、レコードタイプ名の左側にある左向き矢印をクリックして、選択したワークスペースに戻ります。

   レコードタイプカードには、レコードタイプに含まれるフィールドと接続の数が表示されます。

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   レコードの追加、レコードの種類の削除、編集、またはレコードの種類のページでのビューの更新に関する詳細は、次の記事を参照してください。

   * [レコードを作成](../records/create-records.md)
   * [レコードタイプを削除](../architecture/delete-record-types.md)
   * [レコードタイプを編集](../architecture/edit-record-types.md)
   * [レコードビューの管理](../views/manage-record-views.md)

1. （オプション）ワークスペースでレコードタイプカードをクリックしたまま押し続け、レコードタイプを目的の場所にドラッグ&amp;ドロップしたり、別のセクションに移動したりします。

   変更内容は自動的に保存されます。

## Excel または CSV ファイルをインポートしてレコードタイプを作成する

>[!IMPORTANT]
>
>この機能は、2024 年 3 月 21 日以降、一時的に無効になっています。 後日有効になります。

Excel または CSV ファイルを使用してレコードタイプをインポートする際は、次の点を考慮してください。

* Excel ファイルの各シートがレコードタイプになります。
* 各シートの列は、各レコードタイプに関連付けられたフィールドになります。
* フィールドは、それぞれのレコードタイプに対して一意です。
* 各シートの各行は、それぞれのレコードタイプに関連付けられた一意のレコードになります。
* Excel ファイルの各シートは、次のシートを超えてはなりません。
   * 50,000 行
   * 500 列
* Excel ファイルのサイズは 5 MB 以下にする必要があります。
* 空のシートはサポートされていません。

Excel ファイルを使用してレコードタイプをインポートするには、次の手順に従います。

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを作成するワークスペースを選択します。
1. クリック **レコードタイプを追加**.
1. クリック **Excel/CSV**.
1. お使いのコンピューターに以前に保存した Excel または CSV ファイルをドラッグ&amp;ドロップするか、 **CSV または Excel ファイルを選択** をクリックして 1 つを参照します。
1. クリック **データの確認**.

   「プレビューと編集」(Preview and edit) ボックスには、次の情報が表示されます。

   * 左側のパネルに、シートまたは将来のレコードタイプの名前が表示されます。 Workfront Planning では、新しいレコードタイプごとにアイコンと色がデフォルトで選択されます。
   * 最初のシートまたはレコードの種類が選択され、それに関連するフィールドの名前が列ヘッダーとして表示されます。 各フィールドのタイプは、デフォルトで選択されています。
   * 各行は新しいレコードを表します。 「プレビューと編集」ボックスには、最初の 10 件のレコードのみが表示されます。

   ![](assets/preview-and-edit-box.png)

1. （オプション）左パネルの各シートの名前をクリックして、シートに含まれる情報を確認します。

   >[!NOTE]
   >
   >    空のシートはサポートされず、淡色表示になります。


1. （オプション） **読み込むシートを選択** ドロップダウンメニューを開き、読み込まないシートの選択を解除します。

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   選択を解除したシートは、グレーの背景で表示されます。

1. クリック **インポート** ファイルをインポートする準備が整ったら、次の手順に従います。

   次の情報は、Workfront Planning にインポートされます。

   * 新しいレコードタイプ
   * 各レコードタイプに関連付けられた新しいフィールド
   * 各レコードタイプに関連付けられた新しいレコード

   レコードタイプページのフィールドとレコードの管理を開始できます。

   Workfront Planning にアクセスできるすべてのユーザーが、インポートされたレコードのタイプとその情報を表示および編集できるようになりました。 <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront Planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront Planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront Planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](../architecture/connect-record-types.md). 
-->