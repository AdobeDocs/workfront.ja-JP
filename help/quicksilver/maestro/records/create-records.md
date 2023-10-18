---
title: レコードを作成
description: AdobeMaestro では、レコードはレコードタイプのインスタンスです。 個々のレコードを作成する前に、レコードタイプを作成する必要があります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '938'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# レコードを作成

>[!IMPORTANT]
>
>この記事の情報は、Adobe・マエストロに関して、Adobeからの新しいオファーです。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

AdobeMaestro では、レコードはレコードタイプのインスタンスです。

次のタイプのレコードを持つことができます。

* **業務記録**：作業関連のオブジェクトを表します。 例えば、「キャンペーン」というオペレーショナルレコードの場合、「月刊ニュースレター」や「夏物セール」などの名前の付いたレコードを使用できます。
* **分類レコード**：操作レコードに関連付けることができる属性を表します。 例えば、「チャネル」という分類レコードタイプの場合、「電子メール」、「ソーシャルメディア」、「広告」などの分類に名前を付けることができます。

運用レコードの作成は、分類レコード（分類）の作成と同じです。

次のいずれかの操作を行って、Maestro でレコードを作成できます。

* Maestro レコードタイプ用に手動で作成する
* これらを、サードパーティのアプリケーションから Maestro レコードに接続します。

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

## レコードタイプに手動でレコードを追加してレコードを作成する <!--in a record type table (I don't think you can create them elsewhere right now)-->

レコードタイプのページのテーブルビューでレコードを作成できます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-workfront.png) 右上隅に <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->を選択し、次に **マエストロ** ![](assets/maestro-icon.png).
最後にアクセスしたワークスペースは、デフォルトで開きます。 ワークスペースの作成について詳しくは、 [ワークスペースの作成](../architecture-and-fields/create-workspaces.md).
1. レコードタイプのカードをクリックします。 レコードタイプの作成について詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

   最後にアクセスしたビューで、レコードタイプのページが開きます。 デフォルトでは、レコードタイプのページがテーブルビューで開きます。
選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. （条件付き）レコードタイプのページがテーブルビューで開かない場合、 **表示** ドロップダウンメニューで、既存の **テーブル表示** ![](assets/table-view-icon.png) または、 **ビューを作成/テーブル** をクリックして、テーブルビューを作成します。

1. クリック **新規 &lt; レコードタイプ名 >** テーブルの最後の行で、テーブルに新しい行を追加します。

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. 新しいレコードに関する情報を新しい行に入力します。

   >[!NOTE]
   >
   >  * 「名前」フィールドは必須フィールドではありません。 ただし、レコードを相互にリンクする際にレコードを識別するのに役立つので、レコードには名前を付けることをお勧めします。
   >
   >  * 他のレコードタイプまたは計算フィールドを参照するフィールドは、読み取り専用フィールドです。

1. 各行の情報の追加を続行し、「 **入力** をクリックして、変更を保存します。

## 別のアプリケーションからレコードを接続してレコードを作成する

レコードを Maestro のリンクされたレコードにリンクすることで、他のアプリケーションからレコードを読み込むことができます。

1. Maestro レコードタイプを作成します ( [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

1. 前の手順で作成したレコードタイプの Maestro レコードを作成します。 詳しくは、 [レコードタイプに手動でレコードを追加してレコードを作成する](#create-records-by-manually-adding-them-to-a-record-type) 」を参照してください。

1. 作成した Maestro レコードタイプ用のサードパーティアプリケーションから、オブジェクトタイプへの接続を作成します。 詳しくは、 [レコードタイプを接続](../architecture-and-fields/connect-record-types.md).

1. 前の手順で作成したリンクされたレコードフィールドを使用して、サードパーティアプリケーションのレコードを上で作成した Maestro レコードに追加します。 詳しくは、 [レコードを接続](../records/connect-records.md).

   次のアイテムが Maestro で作成されます。

   * [ 接続されたレコード ] フィールドでリンクしたサードパーティのレコードの種類を参照する、読み取り専用の Maestro レコードの種類です。

     たとえば、Maestro レコードタイプをWorkfrontプロジェクトに接続する場合、同じワークスペースに「Workfrontプロジェクト」という読み取り専用のレコードタイプが作成されます。
   * サードパーティのレコードタイプページの読み取り専用レコード。 サードパーティアプリケーションから読み込まれたレコードは読み取り専用のままで、元のアプリケーションでのみ更新できます。


## 外部リストから情報をコピー&amp;ペーストしてレコードを作成する

1. Maestro で、「 」セクションの説明に従って、テーブルビューでレコードの作成を開始します。 [レコードタイプに手動でレコードを追加してレコードを作成する](#create-records-by-manually-adding-them-to-a-record-type) 」を参照してください。

   新しいレコード情報を入力する列（またはフィールド）が Maestro テーブルビューに含まれていることを確認します。

1. クリック **新規 &lt; レコードタイプ名 >** をテーブルの最後の行に追加し、新しいレコードを追加する数だけ新しい行を追加します。

   例えば、別のアプリケーションから 10 件の新しいレコードの情報を貼り付ける場合は、10 行をテーブルビューに追加します。

1. 別のアプリケーションで、Maestro にインポートするレコードのリストを作成します。

   例えば、Excel スプレッドシートを使用してリストを作成できます。

   リストには、情報が表形式で含まれている必要があります。

   >[!TIP]
   >
   > リストの列には、Maestro 内の既存のフィールドに関する情報を含める必要があります。
   >
   > 目的のフィールドが Maestro で既に作成され、シート内の情報が Maestro の各フィールドと一致する正しい形式で表示されていることを確認します。

1. サードパーティアプリケーションから、複数の行と列を選択し、最初の新しいレコードから始まるレコードタイプのテーブルビューに情報を貼り付けます。

   次の情報が Maestro に読み込まれます。

   * 行に新しいレコードが含まれます
   * 列には、レコードのフィールドに関する情報が入力されます。
